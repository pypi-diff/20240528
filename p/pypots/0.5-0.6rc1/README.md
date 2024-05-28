# Comparing `tmp/pypots-0.5.tar.gz` & `tmp/pypots-0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypots-0.5.tar", last modified: Mon May  6 14:24:30 2024, max compression
+gzip compressed data, was "pypots-0.6rc1.tar", last modified: Tue May 28 16:45:09 2024, max compression
```

## Comparing `pypots-0.5.tar` & `pypots-0.6rc1.tar`

### file list

```diff
@@ -1,313 +1,389 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-06 14:22:32.000000 pypots-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 14:22:32.000000 pypots-0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28506 2024-05-06 14:24:30.542978 pypots-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26693 2024-05-06 14:22:32.000000 pypots-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.506978 pypots-0.5/pypots/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-06 14:22:32.000000 pypots-0.5/pypots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22480 2024-05-06 14:22:32.000000 pypots-0.5/pypots/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.506978 pypots-0.5/pypots/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.506978 pypots-0.5/pypots/classification/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/brits/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/brits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/classification/grud/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/grud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/grud/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/grud/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/grud/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/classification/raindrop/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/raindrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/raindrop/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/raindrop/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/raindrop/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/pypots_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/clustering/crli/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/crli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/crli/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/crli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18175 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/crli/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/clustering/vader/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/vader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/vader/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/vader/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20197 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/vader/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/checking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/data/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19043 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/dataset/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/generating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/load_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/load_specific_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/data/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/saving/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/saving/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/forecasting/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/forecasting/bttf/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/bttf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/bttf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/bttf/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/bttf/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/forecasting/csdi/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/csdi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/csdi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/csdi/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/csdi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/imputation/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/autoformer/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/autoformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/autoformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/autoformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/autoformer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17417 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/brits/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/brits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/crossformer/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/crossformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/crossformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/crossformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/crossformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/csdi/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/csdi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/csdi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/csdi/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/csdi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/dlinear/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/dlinear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/dlinear/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/dlinear/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/dlinear/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/etsformer/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/etsformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/etsformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/etsformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/etsformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/fedformer/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/fedformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/fedformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/fedformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/fedformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/film/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/film/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/film/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/film/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/film/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/frets/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/frets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/frets/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/frets/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/frets/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/gpvae/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/gpvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/gpvae/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/gpvae/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/gpvae/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/informer/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/informer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/informer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/informer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/itransformer/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/itransformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/itransformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/itransformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/itransformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/locf/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/locf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/locf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/locf/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/mean/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mean/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/median/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/median/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/median/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/mrnn/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mrnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mrnn/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mrnn/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mrnn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/patchtst/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/patchtst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/patchtst/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/patchtst/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/patchtst/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/saits/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/saits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/saits/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/saits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/saits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/timesnet/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/timesnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/timesnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/timesnet/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/timesnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/transformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/transformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/transformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/usgan/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/usgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/usgan/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/usgan/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17287 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/usgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/functional/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/autoformer/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/autoformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/autoformer/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/autoformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/brits/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/brits/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/crli/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crli/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crli/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/crossformer/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crossformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crossformer/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crossformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/csdi/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/csdi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/csdi/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/csdi/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/dlinear/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/dlinear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/dlinear/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/etsformer/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/etsformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/etsformer/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/etsformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/fedformer/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/fedformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/fedformer/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    32398 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/fedformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/film/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/film/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/film/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/film/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/frets/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/frets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/frets/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/gpvae/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/gpvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/gpvae/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/gpvae/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/grud/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/grud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/grud/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/grud/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/informer/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/informer/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/informer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/mrnn/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/mrnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/mrnn/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/mrnn/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/patchtst/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/patchtst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/patchtst/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/patchtst/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/raindrop/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/raindrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/raindrop/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/raindrop/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/saits/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/saits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/saits/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/saits/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/saits/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/nn/modules/timesnet/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/timesnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/timesnet/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/timesnet/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/nn/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/nn/modules/usgan/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/usgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/usgan/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/usgan/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/nn/modules/vader/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/vader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/vader/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/vader/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/pypots/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/constant_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/exponential_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/lambda_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/linear_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/multiplicative_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/multistep_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/step_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/pypots/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/pypots/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/metrics/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    13674 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/metrics/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/pypots/utils/visual/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/visual/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/visual/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.506978 pypots-0.5/pypots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28506 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 14:24:30.542978 pypots-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-06 14:22:32.000000 pypots-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.761210 pypots-0.6rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 16:43:10.000000 pypots-0.6rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 16:43:10.000000 pypots-0.6rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32081 2024-05-28 16:45:09.761210 pypots-0.6rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30260 2024-05-28 16:43:10.000000 pypots-0.6rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.717209 pypots-0.6rc1/pypots/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22480 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.721209 pypots-0.6rc1/pypots/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.721209 pypots-0.6rc1/pypots/classification/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/brits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/brits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.721209 pypots-0.6rc1/pypots/classification/grud/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/grud/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/grud/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/grud/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.721209 pypots-0.6rc1/pypots/classification/raindrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/raindrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/raindrop/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/raindrop/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/classification/raindrop/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.721209 pypots-0.6rc1/pypots/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/cli/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/cli/pypots_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/cli/tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.721209 pypots-0.6rc1/pypots/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.725209 pypots-0.6rc1/pypots/clustering/crli/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/crli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/crli/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/crli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18422 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/crli/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.725209 pypots-0.6rc1/pypots/clustering/vader/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/vader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/vader/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/vader/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/clustering/vader/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.725209 pypots-0.6rc1/pypots/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.725209 pypots-0.6rc1/pypots/data/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19043 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/dataset/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/generating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/load_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/load_specific_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.725209 pypots-0.6rc1/pypots/data/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/saving/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/saving/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.725209 pypots-0.6rc1/pypots/forecasting/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17701 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.725209 pypots-0.6rc1/pypots/forecasting/bttf/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/bttf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/bttf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/bttf/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/bttf/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.729210 pypots-0.6rc1/pypots/forecasting/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/csdi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/csdi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17875 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/forecasting/csdi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.729210 pypots-0.6rc1/pypots/imputation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.729210 pypots-0.6rc1/pypots/imputation/autoformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/autoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/autoformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/autoformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/autoformer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17664 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.729210 pypots-0.6rc1/pypots/imputation/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/brits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/brits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.729210 pypots-0.6rc1/pypots/imputation/crossformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/crossformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/crossformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/crossformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/crossformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.729210 pypots-0.6rc1/pypots/imputation/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/csdi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/csdi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17017 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/csdi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.729210 pypots-0.6rc1/pypots/imputation/dlinear/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/dlinear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/dlinear/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/dlinear/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/dlinear/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.729210 pypots-0.6rc1/pypots/imputation/etsformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/etsformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/etsformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/etsformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/etsformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.733209 pypots-0.6rc1/pypots/imputation/fedformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/fedformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/fedformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/fedformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/fedformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.733209 pypots-0.6rc1/pypots/imputation/film/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/film/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/film/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/film/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/film/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.733209 pypots-0.6rc1/pypots/imputation/frets/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/frets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/frets/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/frets/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/frets/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.733209 pypots-0.6rc1/pypots/imputation/gpvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/gpvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/gpvae/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/gpvae/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17667 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/gpvae/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.733209 pypots-0.6rc1/pypots/imputation/grud/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/grud/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/grud/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/grud/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.733209 pypots-0.6rc1/pypots/imputation/informer/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/informer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/informer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/informer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.733209 pypots-0.6rc1/pypots/imputation/itransformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/itransformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/itransformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/itransformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/itransformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.733209 pypots-0.6rc1/pypots/imputation/koopa/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/koopa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/koopa/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/koopa/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/koopa/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/locf/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/locf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/locf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/locf/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/mean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/mean/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/median/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/median/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/median/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/micn/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/micn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/micn/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/micn/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/micn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/mrnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/mrnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/mrnn/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/mrnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/mrnn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/nonstationary_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/nonstationary_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/nonstationary_transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/nonstationary_transformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/nonstationary_transformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/patchtst/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/patchtst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/patchtst/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/patchtst/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/patchtst/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/pyraformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/pyraformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/pyraformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/pyraformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/pyraformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.737209 pypots-0.6rc1/pypots/imputation/revinscinet/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/revinscinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/revinscinet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/revinscinet/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/revinscinet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/imputation/saits/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/saits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/saits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/saits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/saits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/imputation/scinet/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/scinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/scinet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/scinet/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/scinet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/imputation/stemgnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/stemgnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/stemgnn/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/stemgnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/stemgnn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/imputation/tide/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/tide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/tide/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/tide/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/tide/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/imputation/timesnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/timesnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/timesnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/timesnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/timesnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/imputation/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/transformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/transformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/imputation/usgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/usgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/usgan/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/usgan/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/imputation/usgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/functional/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.741209 pypots-0.6rc1/pypots/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/autoformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/autoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/autoformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/autoformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/brits/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/brits/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/crli/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/crli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/crli/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/crli/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/crossformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/crossformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/crossformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/crossformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/csdi/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/csdi/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/dlinear/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/dlinear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/dlinear/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/etsformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/etsformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/etsformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/etsformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/fedformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/fedformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/fedformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33256 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/fedformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.745210 pypots-0.6rc1/pypots/nn/modules/film/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/film/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/film/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/film/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/frets/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/frets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/frets/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/gpvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/gpvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/gpvae/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/gpvae/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/grud/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/grud/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/grud/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/informer/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/informer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/informer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/koopa/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/koopa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/koopa/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/koopa/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/micn/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/micn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/micn/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/micn/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/mrnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/mrnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/mrnn/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/mrnn/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/nonstationary_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/nonstationary_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/nonstationary_transformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/nonstationary_transformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.749210 pypots-0.6rc1/pypots/nn/modules/patchtst/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/patchtst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/patchtst/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/patchtst/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.753209 pypots-0.6rc1/pypots/nn/modules/pyraformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/pyraformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/pyraformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/pyraformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.753209 pypots-0.6rc1/pypots/nn/modules/raindrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/raindrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/raindrop/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/raindrop/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.753209 pypots-0.6rc1/pypots/nn/modules/revin/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/revin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/revin/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.753209 pypots-0.6rc1/pypots/nn/modules/saits/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/saits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/saits/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/saits/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/saits/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.753209 pypots-0.6rc1/pypots/nn/modules/scinet/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/scinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/scinet/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/scinet/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.753209 pypots-0.6rc1/pypots/nn/modules/stemgnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/stemgnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/stemgnn/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/stemgnn/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.753209 pypots-0.6rc1/pypots/nn/modules/tide/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/tide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/tide/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/tide/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.753209 pypots-0.6rc1/pypots/nn/modules/timesnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/timesnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/timesnet/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/timesnet/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.757209 pypots-0.6rc1/pypots/nn/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/transformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/transformer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/transformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.757209 pypots-0.6rc1/pypots/nn/modules/usgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/usgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/usgan/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/usgan/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.757209 pypots-0.6rc1/pypots/nn/modules/vader/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/vader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/vader/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/nn/modules/vader/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.757209 pypots-0.6rc1/pypots/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.757209 pypots-0.6rc1/pypots/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/constant_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/exponential_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/lambda_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/linear_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/multiplicative_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/multistep_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/lr_scheduler/step_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/optim/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.761210 pypots-0.6rc1/pypots/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.761210 pypots-0.6rc1/pypots/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/metrics/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13674 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/metrics/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.761210 pypots-0.6rc1/pypots/utils/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/visual/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-28 16:43:10.000000 pypots-0.6rc1/pypots/utils/visual/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:45:09.721209 pypots-0.6rc1/pypots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32081 2024-05-28 16:45:09.000000 pypots-0.6rc1/pypots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-05-28 16:45:09.000000 pypots-0.6rc1/pypots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:45:09.000000 pypots-0.6rc1/pypots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 16:45:09.000000 pypots-0.6rc1/pypots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-28 16:45:09.000000 pypots-0.6rc1/pypots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 16:45:09.000000 pypots-0.6rc1/pypots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-28 16:45:09.761210 pypots-0.6rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-28 16:43:10.000000 pypots-0.6rc1/setup.py
```

### Comparing `pypots-0.5/LICENSE` & `pypots-0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypots-0.5/PKG-INFO` & `pypots-0.6rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.5
-Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
+Version: 0.6rc1
+Summary: A Python Toolbox for Machine Learning on Partially-Observed Time Series
 Home-page: https://pypots.com/
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/
 Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
 Project-URL: Tracker, https://github.com/WenjieDu/PyPOTS/issues/
@@ -45,15 +45,15 @@
 <p align="center"><i>a Python toolbox for machine learning on Partially-Observed Time Series</i></p>
 
 <p align="center">
     <a href="https://docs.pypots.com/en/latest/install.html#reasons-of-version-limitations-on-dependencies">
        <img alt="Python version" src="https://img.shields.io/badge/Python-v3.7+-E97040?logo=python&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS">
-        <img alt="powered by Pytorch" src="https://img.shields.io/badge/PyTorch-❤️-F8C6B5?logo=pytorch&logoColor=white">
+        <img alt="powered by Pytorch" src="https://img.shields.io/badge/PyTorch-%E2%9D%A4%EF%B8%8F-F8C6B5?logo=pytorch&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/releases">
         <img alt="the latest release version" src="https://img.shields.io/github/v/release/wenjiedu/pypots?color=EE781F&include_prereleases&label=Release&logo=github&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/LICENSE">
         <img alt="BSD-3 license" src="https://img.shields.io/badge/License-BSD--3-E9BB41?logo=opensourceinitiative&logoColor=white">
     </a>
@@ -87,15 +87,18 @@
     <a href="https://pepy.tech/project/pypots">
         <img alt="PyPI downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pypots_downloads.json">
     </a>
     <a href="https://arxiv.org/abs/2305.18811">
         <img alt="arXiv DOI" src="https://img.shields.io/badge/DOI-10.48550/arXiv.2305.18811-F8F7F0">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README_zh.md">
-        <img alt="README in Chinese" src="https://img.shields.io/badge/README-🇨🇳中文版-FCEFE8">
+        <img alt="README in Chinese" src="https://pypots.com/figs/pypots_logos/readme/CN.svg">
+    </a>
+   <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README.md">
+        <img alt="README in English" src="https://pypots.com/figs/pypots_logos/readme/US.svg">
     </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error,
 and unexpected malfunction, missing values are common to see in time series from the real-world environment.
 This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced
 data analysis. Although this problem is important, the area of machine learning on POTS still lacks a dedicated toolkit.
@@ -120,63 +123,72 @@
 [**❖ Contribution**](#-contribution),
 [**❖ Community**](#-community).
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, forecasting, and anomaly detection tasks on multivariate partially-observed
 time series with missing values. The table below shows the availability of each algorithm (sorted by Year) in PyPOTS for different tasks.
-The symbol ✅ indicates the algorithm is available for the corresponding task (note that models will be continuously updated
+The symbol `✅` indicates the algorithm is available for the corresponding task (note that models will be continuously updated
 in the future to handle tasks that are not currently supported. Stay tuned❗️).
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to refer to our time-series
 imputation survey repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation) to see how to config and
 tune the hyperparameters.
 
-🔥 Note that Transformer, iTransformer, FreTS, Crossformer, PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer
-are not proposed as imputation methods in their original papers, and they cannot accept POTS as input.
-**To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
-the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+🔥 Note that all models whose name with `🧑‍🔧` in the table (e.g. Transformer, iTransformer, Informer etc.) are not originally
+proposed as algorithms for POTS data in their papers, and they cannot directly accept time series with missing values as input,
+let alone imputation. **To make them applicable to POTS data, we specifically apply the embedding strategy and
+training approach (ORT+MIT) the same as we did in [the SAITS paper](https://arxiv.org/pdf/2202.08516)[^1].**
 
 The task types are abbreviated as follows:
 **`IMPU`**: Imputation;
 **`FORE`**: Forecasting;
 **`CLAS`**: Classification;
 **`CLUS`**: Clustering;
 **`ANOD`**: Anomaly Detection.
 The paper references and links are all listed at the bottom of this file.
 
-| **Type**      | **Algo**                           | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** |
-|:--------------|:-----------------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-----------------|
-| Neural Net    | iTransformer[^24]                  |    ✅     |          |          |          |          | 2024 - ICLR      |
-| Neural Net    | FreTS[^23]                         |    ✅     |          |          |          |          | 2024 - NeurIPS   |
-| Neural Net    | SAITS[^1]                          |    ✅     |          |          |          |          | 2023 - ESWA      |
-| Neural Net    | Crossformer[^16]                   |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | TimesNet[^14]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | PatchTST[^18]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | ETSformer[^19]                     |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | DLinear[^17]                       |    ✅     |          |          |          |          | 2023 - AAAI      |
-| Neural Net    | FiLM[^22]                          |    ✅     |          |          |          |          | 2022 - NeurIPS   |
-| Neural Net    | Raindrop[^5]                       |          |          |    ✅     |          |          | 2022 - ICLR      |
-| Neural Net    | FEDformer[^20]                     |    ✅     |          |          |          |          | 2022 - ICML      |
-| Neural Net    | Autoformer[^15]                    |    ✅     |          |          |          |          | 2021 - NeurIPS   |
-| Neural Net    | CSDI[^12]                          |    ✅     |    ✅     |          |          |          | 2021 - NeurIPS   |
-| Neural Net    | Informer[^21]                      |    ✅     |          |          |          |          | 2021 - AAAI      |
-| Neural Net    | US-GAN[^10]                        |    ✅     |          |          |          |          | 2021 - AAAI      |
-| Neural Net    | CRLI[^6]                           |          |          |          |    ✅     |          | 2021 - AAAI      |
-| Probabilistic | BTTF[^8]                           |          |    ✅     |          |          |          | 2021 - TPAMI     |
-| Neural Net    | GP-VAE[^11]                        |    ✅     |          |          |          |          | 2020 - AISTATS   |
-| Neural Net    | VaDER[^7]                          |          |          |          |    ✅     |          | 2019 - GigaSci.  |
-| Neural Net    | M-RNN[^9]                          |    ✅     |          |          |          |          | 2019 - TBME      |
-| Neural Net    | BRITS[^3]                          |    ✅     |          |    ✅     |          |          | 2018 - NeurIPS   |
-| Neural Net    | GRU-D[^4]                          |    ✅     |          |    ✅     |          |          | 2018 - Sci. Rep. |
-| Neural Net    | Transformer[^2]                    |    ✅     |          |          |          |          | 2017 - NeurIPS   |
-| Naive         | LOCF/NOCB                          |    ✅     |          |          |          |          |                  |
-| Naive         | Mean                               |    ✅     |          |          |          |          |                  |
-| Naive         | Median                             |    ✅     |          |          |          |          |                  |
+| **Type**      | **Algo**                    | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue**   |
+|:--------------|:----------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-------------------|
+| Neural Net    | iTransformer🧑‍🔧[^24]      |    ✅     |          |          |          |          | `2024 - ICLR`      |
+| Neural Net    | SAITS[^1]                   |    ✅     |          |          |          |          | `2023 - ESWA`      |
+| Neural Net    | FreTS🧑‍🔧[^23]             |    ✅     |          |          |          |          | `2023 - NeurIPS`   |
+| Neural Net    | Koopa🧑‍🔧[^29]             |    ✅     |          |          |          |          | `2023 - NeurIPS`   |
+| Neural Net    | Crossformer🧑‍🔧[^16]       |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | TimesNet[^14]               |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | PatchTST🧑‍🔧[^18]          |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | ETSformer🧑‍🔧[^19]         |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | MICN🧑‍🔧[^27]              |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | DLinear🧑‍🔧[^17]           |    ✅     |          |          |          |          | `2023 - AAAI`      |
+| Neural Net    | TiDE🧑‍🔧[^28]              |    ✅     |          |          |          |          | `2023 - TMLR`      |
+| Neural Net    | SCINet🧑‍🔧[^30]            |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | Nonstationary Tr.🧑‍🔧[^25] |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | FiLM🧑‍🔧[^22]              |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | RevIN_SCINet🧑‍🔧[^31]      |    ✅     |          |          |          |          | `2022 - ICLR`      |
+| Neural Net    | Pyraformer🧑‍🔧[^26]        |    ✅     |          |          |          |          | `2022 - ICLR`      |
+| Neural Net    | Raindrop[^5]                |          |          |    ✅     |          |          | `2022 - ICLR`      |
+| Neural Net    | FEDformer🧑‍🔧[^20]         |    ✅     |          |          |          |          | `2022 - ICML`      |
+| Neural Net    | Autoformer🧑‍🔧[^15]        |    ✅     |          |          |          |          | `2021 - NeurIPS`   |
+| Neural Net    | CSDI[^12]                   |    ✅     |    ✅     |          |          |          | `2021 - NeurIPS`   |
+| Neural Net    | Informer🧑‍🔧[^21]          |    ✅     |          |          |          |          | `2021 - AAAI`      |
+| Neural Net    | US-GAN[^10]                 |    ✅     |          |          |          |          | `2021 - AAAI`      |
+| Neural Net    | CRLI[^6]                    |          |          |          |    ✅     |          | `2021 - AAAI`      |
+| Probabilistic | BTTF[^8]                    |          |    ✅     |          |          |          | `2021 - TPAMI`     |
+| Neural Net    | StemGNN🧑‍🔧[^33]           |    ✅     |          |          |          |          | `2020 - NeurIPS`   |
+| Neural Net    | Reformer🧑‍🔧[^32]          |    ✅     |          |          |          |          | `2020 - ICLR`      |
+| Neural Net    | GP-VAE[^11]                 |    ✅     |          |          |          |          | `2020 - AISTATS`   |
+| Neural Net    | VaDER[^7]                   |          |          |          |    ✅     |          | `2019 - GigaSci.`  |
+| Neural Net    | M-RNN[^9]                   |    ✅     |          |          |          |          | `2019 - TBME`      |
+| Neural Net    | BRITS[^3]                   |    ✅     |          |    ✅     |          |          | `2018 - NeurIPS`   |
+| Neural Net    | GRU-D[^4]                   |    ✅     |          |    ✅     |          |          | `2018 - Sci. Rep.` |
+| Neural Net    | Transformer🧑‍🔧[^2]        |    ✅     |          |          |          |          | `2017 - NeurIPS`   |
+| Naive         | LOCF/NOCB                   |    ✅     |          |          |          |          |                    |
+| Naive         | Mean                        |    ✅     |          |          |          |          |                    |
+| Naive         | Median                      |    ✅     |          |          |          |          |                    |
 
 
 ## ❖ PyPOTS Ecosystem
 At PyPOTS, things are related to coffee, which we're familiar with. Yes, this is a coffee universe!
 As you can see, there is a coffee pot in the PyPOTS logo.
 And what else? Please read on ;-)
 
@@ -384,17 +396,25 @@
 [^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
 [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
 [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
 [^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
 [^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
 [^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
 [^22]: Zhou, T., Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency improved Legendre Memory Model for Long-term Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
-[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2024*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2023). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2023*.
 [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H., Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are Effective for Time Series Forecasting](https://openreview.net/forum?id=JePfAI8fah). *ICLR 2024*.
-
+[^25]: Liu, Y., Wu, H., Wang, J., & Long, M. (2022). [Non-stationary Transformers: Exploring the Stationarity in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/4054556fcaa934b0bf76da52cf4f92cb-Abstract-Conference.html). *NeurIPS 2022*.
+[^26]: Liu, S., Yu, H., Liao, C., Li, J., Lin, W., Liu, A. X., & Dustdar, S. (2022). [Pyraformer: Low-Complexity Pyramidal Attention for Long-Range Time Series Modeling and Forecasting](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2022*.
+[^27]: Wang, H., Peng, J., Huang, F., Wang, J., Chen, J., & Xiao, Y. (2023). [MICN: Multi-scale Local and Global Context Modeling for Long-term Series Forecasting](https://openreview.net/forum?id=zt53IDUR1U). *ICLR 2023*.
+[^28]: Das, A., Kong, W., Leach, A., Mathur, S., Sen, R., & Yu, R. (2023). [Long-term Forecasting with TiDE: Time-series Dense Encoder](https://openreview.net/forum?id=pCbC3aQB5W). *TMLR 2023*.
+[^29]: Liu, Y., Li, C., Wang, J., & Long, M. (2023). [Koopa: Learning Non-stationary Time Series Dynamics with Koopman Predictors](https://proceedings.neurips.cc/paper_files/paper/2023/hash/28b3dc0970fa4624a63278a4268de997-Abstract-Conference.html). *NeurIPS 2023*.
+[^30]: Liu, M., Zeng, A., Chen, M., Xu, Z., Lai, Q., Ma, L., & Xu, Q. (2022). [SCINet: Time Series Modeling and Forecasting with Sample Convolution and Interaction](https://proceedings.neurips.cc/paper_files/paper/2022/hash/266983d0949aed78a16fa4782237dea7-Abstract-Conference.html). *NeurIPS 2022*.
+[^31]: Kim, T., Kim, J., Tae, Y., Park, C., Choi, J. H., & Choo, J. (2022). [Reversible Instance Normalization for Accurate Time-Series Forecasting against Distribution Shift](https://openreview.net/forum?id=cGDAkQo1C0p). *ICLR 2022*.
+[^32]: Kitaev, N., Kaiser, Ł., & Levskaya, A. (2020). [Reformer: The Efficient Transformer](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2020*.
+[^33]: Cao, D., Wang, Y., Duan, J., Zhang, C., Zhu, X., Huang, C., Tong, Y., Xu, B., Bai, J., Tong, J., & Zhang, Q. (2020). [Spectral Temporal Graph Neural Network for Multivariate Time-series Forecasting](https://proceedings.neurips.cc/paper/2020/hash/cdf6581cb7aca4b7e19ef136c6e601a5-Abstract.html). *NeurIPS 2020*.
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
 </a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.5 Summary: A Python Toolbox for
-Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
-Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
-Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
-https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
-WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
-PyPOTS/archive/main.zip Keywords: data science,data mining,neural
+Metadata-Version: 2.1 Name: pypots Version: 0.6rc1 Summary: A Python Toolbox
+for Machine Learning on Partially-Observed Time Series Home-page: https://
+pypots.com/ Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-
+Clause Project-URL: Documentation, https://docs.pypots.com/ Project-URL:
+Source, https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://
+github.com/WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/
+WenjieDu/PyPOTS/archive/main.zip Keywords: data science,data mining,neural
 networks,machine learning,deep learning,artificial intelligence,time-series
 analysis,time
 series,imputation,interpolation,classification,clustering,forecasting,partially
 observed,irregular sampled,partially-observed time series,incomplete time
 series,missing data,missing values Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
@@ -25,15 +25,16 @@
 Provides-Extra: test Provides-Extra: doc Provides-Extra: dev License-File:
 LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
                           ******** WWeellccoommee ttoo PPyyPPOOTTSS ********
     a Python toolbox for machine learning on Partially-Observed Time Series
 _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_p_o_w_e_r_e_d_ _b_y_ _P_y_t_o_r_c_h_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]
   _[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e
   _C_l_i_m_a_t_e_ _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _c_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_D_o_c_s_ _b_u_i_l_d_i_n_g_]
-        _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]
+   _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]_[_R_E_A_D_M_E_ _i_n
+                                   _E_n_g_l_i_s_h_]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of machine learning on POTS still lacks a dedicated
 toolkit. PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS
@@ -53,74 +54,87 @@
 available-algorithms), [**â PyPOTS Ecosystem**](#-pypots-ecosystem), [**â
 Installation**](#-installation), [**â Usage**](#-usage), [**â Citing
 PyPOTS**](#-citing-pypots), [**â Contribution**](#-contribution), [**â
 Community**](#-community). ## â Available Algorithms PyPOTS supports
 imputation, classification, clustering, forecasting, and anomaly detection
 tasks on multivariate partially-observed time series with missing values. The
 table below shows the availability of each algorithm (sorted by Year) in PyPOTS
-for different tasks. The symbol â indicates the algorithm is available for
+for different tasks. The symbol `â` indicates the algorithm is available for
 the corresponding task (note that models will be continuously updated in the
 future to handle tasks that are not currently supported. Stay tunedâï¸).
 ð Since **v0.2**, all neural-network models in PyPOTS has got
 hyperparameter-optimization support. This functionality is implemented with the
 [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to
 refer to our time-series imputation survey repo [Awesome_Imputation](https://
 github.com/WenjieDu/Awesome_Imputation) to see how to config and tune the
-hyperparameters. ð¥ Note that Transformer, iTransformer, FreTS, Crossformer,
-PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer are not
-proposed as imputation methods in their original papers, and they cannot accept
-POTS as input. **To make them applicable on POTS data, we apply the embedding
-strategy and training approach (ORT+MIT) the same as we did in [SAITS paper]
-(https://arxiv.org/pdf/2202.08516).** The task types are abbreviated as
-follows: **`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**:
-Classification; **`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The
-paper references and links are all listed at the bottom of this file. |
-**Type** | **Algo** | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** |
-**Year - Venue** | |:--------------|:-----------------------------------|:-----
----:|:--------:|:--------:|:--------:|:--------:|:-----------------| | Neural
-Net | iTransformer[^24] | â | | | | | 2024 - ICLR | | Neural Net | FreTS[^23]
-| â | | | | | 2024 - NeurIPS | | Neural Net | SAITS[^1] | â | | | | | 2023
-- ESWA | | Neural Net | Crossformer[^16] | â | | | | | 2023 - ICLR | | Neural
-Net | TimesNet[^14] | â | | | | | 2023 - ICLR | | Neural Net | PatchTST[^18]
-| â | | | | | 2023 - ICLR | | Neural Net | ETSformer[^19] | â | | | | |
-2023 - ICLR | | Neural Net | DLinear[^17] | â | | | | | 2023 - AAAI | |
-Neural Net | FiLM[^22] | â | | | | | 2022 - NeurIPS | | Neural Net | Raindrop
-[^5] | | | â | | | 2022 - ICLR | | Neural Net | FEDformer[^20] | â | | | |
-| 2022 - ICML | | Neural Net | Autoformer[^15] | â | | | | | 2021 - NeurIPS |
-| Neural Net | CSDI[^12] | â | â | | | | 2021 - NeurIPS | | Neural Net |
-Informer[^21] | â | | | | | 2021 - AAAI | | Neural Net | US-GAN[^10] | â |
-| | | | 2021 - AAAI | | Neural Net | CRLI[^6] | | | | â | | 2021 - AAAI | |
-Probabilistic | BTTF[^8] | | â | | | | 2021 - TPAMI | | Neural Net | GP-VAE
-[^11] | â | | | | | 2020 - AISTATS | | Neural Net | VaDER[^7] | | | | â | |
-2019 - GigaSci. | | Neural Net | M-RNN[^9] | â | | | | | 2019 - TBME | |
-Neural Net | BRITS[^3] | â | | â | | | 2018 - NeurIPS | | Neural Net | GRU-
-D[^4] | â | | â | | | 2018 - Sci. Rep. | | Neural Net | Transformer[^2] |
-â | | | | | 2017 - NeurIPS | | Naive | LOCF/NOCB | â | | | | | | | Naive |
-Mean | â | | | | | | | Naive | Median | â | | | | | | ## â PyPOTS
-Ecosystem At PyPOTS, things are related to coffee, which we're familiar with.
-Yes, this is a coffee universe! As you can see, there is a coffee pot in the
-PyPOTS logo. And what else? Please read on ;-) _[_T_S_D_B_ _l_o_g_o_]ð Time series
-datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete
-coffee beans with missing parts that have their own meanings. To make various
-public time-series datasets readily available to users, Time Series Data Beans
-(TSDB) is created to make loading time-series datasets super easy! Visit [TSDB]
-(https://github.com/WenjieDu/TSDB) right now to know more about this handy tool
-ð , and it now supports a total of 169 open-source datasets! _[_P_y_G_r_i_n_d_e_r
-_l_o_g_o_]ð To simulate the real-world data beans with missingness, the ecosystem
-library [PyGrinder](https://github.com/WenjieDu/PyGrinder), a toolkit helping
-grind your coffee beans into incomplete ones, is created. Missing patterns fall
-into three categories according to Robin's theory[^13]: MCAR (missing
-completely at random), MAR (missing at random), and MNAR (missing not at
-random). PyGrinder supports all of them and additional functionalities related
-to missingness. With PyGrinder, you can introduce synthetic missing values into
-your datasets with a single line of code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the
-beans, the grinder, and the pot, how to brew us a cup of coffee? Tutorials are
-necessary! Considering the future workload, PyPOTS tutorials are released in a
-single repo, and you can find them in [BrewPOTS](https://github.com/WenjieDu/
-BrewPOTS). Take a look at it now, and learn how to brew your POTS datasets!
+hyperparameters. ð¥ Note that all models whose name with `ð§âð§` in the
+table (e.g. Transformer, iTransformer, Informer etc.) are not originally
+proposed as algorithms for POTS data in their papers, and they cannot directly
+accept time series with missing values as input, let alone imputation. **To
+make them applicable to POTS data, we specifically apply the embedding strategy
+and training approach (ORT+MIT) the same as we did in [the SAITS paper](https:/
+/arxiv.org/pdf/2202.08516)[^1].** The task types are abbreviated as follows:
+**`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**: Classification;
+**`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The paper references and
+links are all listed at the bottom of this file. | **Type** | **Algo** |
+**IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** | |:---
+-----------|:----------------------------|:--------:|:--------:|:--------:|:---
+-----:|:--------:|:-------------------| | Neural Net | iTransformerð§âð§
+[^24] | â | | | | | `2024 - ICLR` | | Neural Net | SAITS[^1] | â | | | | |
+`2023 - ESWA` | | Neural Net | FreTSð§âð§[^23] | â | | | | | `2023 -
+NeurIPS` | | Neural Net | Koopað§âð§[^29] | â | | | | | `2023 -
+NeurIPS` | | Neural Net | Crossformerð§âð§[^16] | â | | | | | `2023 -
+ICLR` | | Neural Net | TimesNet[^14] | â | | | | | `2023 - ICLR` | | Neural
+Net | PatchTSTð§âð§[^18] | â | | | | | `2023 - ICLR` | | Neural Net |
+ETSformerð§âð§[^19] | â | | | | | `2023 - ICLR` | | Neural Net |
+MICNð§âð§[^27] | â | | | | | `2023 - ICLR` | | Neural Net |
+DLinearð§âð§[^17] | â | | | | | `2023 - AAAI` | | Neural Net |
+TiDEð§âð§[^28] | â | | | | | `2023 - TMLR` | | Neural Net |
+SCINetð§âð§[^30] | â | | | | | `2022 - NeurIPS` | | Neural Net |
+Nonstationary Tr.ð§âð§[^25] | â | | | | | `2022 - NeurIPS` | | Neural
+Net | FiLMð§âð§[^22] | â | | | | | `2022 - NeurIPS` | | Neural Net |
+RevIN_SCINetð§âð§[^31] | â | | | | | `2022 - ICLR` | | Neural Net |
+Pyraformerð§âð§[^26] | â | | | | | `2022 - ICLR` | | Neural Net |
+Raindrop[^5] | | | â | | | `2022 - ICLR` | | Neural Net |
+FEDformerð§âð§[^20] | â | | | | | `2022 - ICML` | | Neural Net |
+Autoformerð§âð§[^15] | â | | | | | `2021 - NeurIPS` | | Neural Net |
+CSDI[^12] | â | â | | | | `2021 - NeurIPS` | | Neural Net |
+Informerð§âð§[^21] | â | | | | | `2021 - AAAI` | | Neural Net | US-GAN
+[^10] | â | | | | | `2021 - AAAI` | | Neural Net | CRLI[^6] | | | | â | |
+`2021 - AAAI` | | Probabilistic | BTTF[^8] | | â | | | | `2021 - TPAMI` | |
+Neural Net | StemGNNð§âð§[^33] | â | | | | | `2020 - NeurIPS` | |
+Neural Net | Reformerð§âð§[^32] | â | | | | | `2020 - ICLR` | | Neural
+Net | GP-VAE[^11] | â | | | | | `2020 - AISTATS` | | Neural Net | VaDER[^7] |
+| | | â | | `2019 - GigaSci.` | | Neural Net | M-RNN[^9] | â | | | | |
+`2019 - TBME` | | Neural Net | BRITS[^3] | â | | â | | | `2018 - NeurIPS` |
+| Neural Net | GRU-D[^4] | â | | â | | | `2018 - Sci. Rep.` | | Neural Net
+| Transformerð§âð§[^2] | â | | | | | `2017 - NeurIPS` | | Naive | LOCF/
+NOCB | â | | | | | | | Naive | Mean | â | | | | | | | Naive | Median | â
+| | | | | | ## â PyPOTS Ecosystem At PyPOTS, things are related to coffee,
+which we're familiar with. Yes, this is a coffee universe! As you can see,
+there is a coffee pot in the PyPOTS logo. And what else? Please read on ;-)
+_[_T_S_D_B_ _l_o_g_o_]ð Time series datasets are taken as coffee beans at PyPOTS, and
+POTS datasets are incomplete coffee beans with missing parts that have their
+own meanings. To make various public time-series datasets readily available to
+users, Time Series Data Beans (TSDB) is created to make loading time-series
+datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB) right now
+to know more about this handy tool ð , and it now supports a total of 169
+open-source datasets! _[_P_y_G_r_i_n_d_e_r_ _l_o_g_o_]ð To simulate the real-world data
+beans with missingness, the ecosystem library [PyGrinder](https://github.com/
+WenjieDu/PyGrinder), a toolkit helping grind your coffee beans into incomplete
+ones, is created. Missing patterns fall into three categories according to
+Robin's theory[^13]: MCAR (missing completely at random), MAR (missing at
+random), and MNAR (missing not at random). PyGrinder supports all of them and
+additional functionalities related to missingness. With PyGrinder, you can
+introduce synthetic missing values into your datasets with a single line of
+code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the beans, the grinder, and the pot, how
+to brew us a cup of coffee? Tutorials are necessary! Considering the future
+workload, PyPOTS tutorials are released in a single repo, and you can find them
+in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and
+learn how to brew your POTS datasets!
 _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
 install PyPOTS like below as well as TSDB and PyGrinder: ``` bash # via pip pip
@@ -276,14 +290,43 @@
 Beyond efficient transformer for long sequence time-series forecasting](https:/
 /ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. [^22]: Zhou, T.,
 Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency
 improved Legendre Memory Model for Long-term Time Series Forecasting](https://
 proceedings.neurips.cc/paper_files/paper/2022/hash/
 524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
 [^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian,
-D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective
+D., Cao, L., & Niu, Z. (2023). [Frequency-domain MLPs are More Effective
 Learners in Time Series Forecasting](https://proceedings.neurips.cc/
 paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-
-Conference.html). *NeurIPS 2024*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
+Conference.html). *NeurIPS 2023*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
 Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are
 Effective for Time Series Forecasting](https://openreview.net/
-forum?id=JePfAI8fah). *ICLR 2024*. ð  Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+forum?id=JePfAI8fah). *ICLR 2024*. [^25]: Liu, Y., Wu, H., Wang, J., & Long, M.
+(2022). [Non-stationary Transformers: Exploring the Stationarity in Time Series
+Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/
+4054556fcaa934b0bf76da52cf4f92cb-Abstract-Conference.html). *NeurIPS 2022*.
+[^26]: Liu, S., Yu, H., Liao, C., Li, J., Lin, W., Liu, A. X., & Dustdar, S.
+(2022). [Pyraformer: Low-Complexity Pyramidal Attention for Long-Range Time
+Series Modeling and Forecasting](https://openreview.net/forum?id=0EXmFzUn5I).
+*ICLR 2022*. [^27]: Wang, H., Peng, J., Huang, F., Wang, J., Chen, J., & Xiao,
+Y. (2023). [MICN: Multi-scale Local and Global Context Modeling for Long-term
+Series Forecasting](https://openreview.net/forum?id=zt53IDUR1U). *ICLR 2023*.
+[^28]: Das, A., Kong, W., Leach, A., Mathur, S., Sen, R., & Yu, R. (2023).
+[Long-term Forecasting with TiDE: Time-series Dense Encoder](https://
+openreview.net/forum?id=pCbC3aQB5W). *TMLR 2023*. [^29]: Liu, Y., Li, C., Wang,
+J., & Long, M. (2023). [Koopa: Learning Non-stationary Time Series Dynamics
+with Koopman Predictors](https://proceedings.neurips.cc/paper_files/paper/2023/
+hash/28b3dc0970fa4624a63278a4268de997-Abstract-Conference.html). *NeurIPS
+2023*. [^30]: Liu, M., Zeng, A., Chen, M., Xu, Z., Lai, Q., Ma, L., & Xu, Q.
+(2022). [SCINet: Time Series Modeling and Forecasting with Sample Convolution
+and Interaction](https://proceedings.neurips.cc/paper_files/paper/2022/hash/
+266983d0949aed78a16fa4782237dea7-Abstract-Conference.html). *NeurIPS 2022*.
+[^31]: Kim, T., Kim, J., Tae, Y., Park, C., Choi, J. H., & Choo, J. (2022).
+[Reversible Instance Normalization for Accurate Time-Series Forecasting against
+Distribution Shift](https://openreview.net/forum?id=cGDAkQo1C0p). *ICLR 2022*.
+[^32]: Kitaev, N., Kaiser, Å., & Levskaya, A. (2020). [Reformer: The Efficient
+Transformer](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2020*. [^33]:
+Cao, D., Wang, Y., Duan, J., Zhang, C., Zhu, X., Huang, C., Tong, Y., Xu, B.,
+Bai, J., Tong, J., & Zhang, Q. (2020). [Spectral Temporal Graph Neural Network
+for Multivariate Time-series Forecasting](https://proceedings.neurips.cc/paper/
+2020/hash/cdf6581cb7aca4b7e19ef136c6e601a5-Abstract.html). *NeurIPS 2020*. ð 
+Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.5/README.md` & `pypots-0.6rc1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 <p align="center"><i>a Python toolbox for machine learning on Partially-Observed Time Series</i></p>
 
 <p align="center">
     <a href="https://docs.pypots.com/en/latest/install.html#reasons-of-version-limitations-on-dependencies">
        <img alt="Python version" src="https://img.shields.io/badge/Python-v3.7+-E97040?logo=python&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS">
-        <img alt="powered by Pytorch" src="https://img.shields.io/badge/PyTorch-❤️-F8C6B5?logo=pytorch&logoColor=white">
+        <img alt="powered by Pytorch" src="https://img.shields.io/badge/PyTorch-%E2%9D%A4%EF%B8%8F-F8C6B5?logo=pytorch&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/releases">
         <img alt="the latest release version" src="https://img.shields.io/github/v/release/wenjiedu/pypots?color=EE781F&include_prereleases&label=Release&logo=github&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/LICENSE">
         <img alt="BSD-3 license" src="https://img.shields.io/badge/License-BSD--3-E9BB41?logo=opensourceinitiative&logoColor=white">
     </a>
@@ -49,15 +49,18 @@
     <a href="https://pepy.tech/project/pypots">
         <img alt="PyPI downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pypots_downloads.json">
     </a>
     <a href="https://arxiv.org/abs/2305.18811">
         <img alt="arXiv DOI" src="https://img.shields.io/badge/DOI-10.48550/arXiv.2305.18811-F8F7F0">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README_zh.md">
-        <img alt="README in Chinese" src="https://img.shields.io/badge/README-🇨🇳中文版-FCEFE8">
+        <img alt="README in Chinese" src="https://pypots.com/figs/pypots_logos/readme/CN.svg">
+    </a>
+   <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README.md">
+        <img alt="README in English" src="https://pypots.com/figs/pypots_logos/readme/US.svg">
     </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error,
 and unexpected malfunction, missing values are common to see in time series from the real-world environment.
 This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced
 data analysis. Although this problem is important, the area of machine learning on POTS still lacks a dedicated toolkit.
@@ -82,63 +85,72 @@
 [**❖ Contribution**](#-contribution),
 [**❖ Community**](#-community).
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, forecasting, and anomaly detection tasks on multivariate partially-observed
 time series with missing values. The table below shows the availability of each algorithm (sorted by Year) in PyPOTS for different tasks.
-The symbol ✅ indicates the algorithm is available for the corresponding task (note that models will be continuously updated
+The symbol `✅` indicates the algorithm is available for the corresponding task (note that models will be continuously updated
 in the future to handle tasks that are not currently supported. Stay tuned❗️).
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to refer to our time-series
 imputation survey repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation) to see how to config and
 tune the hyperparameters.
 
-🔥 Note that Transformer, iTransformer, FreTS, Crossformer, PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer
-are not proposed as imputation methods in their original papers, and they cannot accept POTS as input.
-**To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
-the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+🔥 Note that all models whose name with `🧑‍🔧` in the table (e.g. Transformer, iTransformer, Informer etc.) are not originally
+proposed as algorithms for POTS data in their papers, and they cannot directly accept time series with missing values as input,
+let alone imputation. **To make them applicable to POTS data, we specifically apply the embedding strategy and
+training approach (ORT+MIT) the same as we did in [the SAITS paper](https://arxiv.org/pdf/2202.08516)[^1].**
 
 The task types are abbreviated as follows:
 **`IMPU`**: Imputation;
 **`FORE`**: Forecasting;
 **`CLAS`**: Classification;
 **`CLUS`**: Clustering;
 **`ANOD`**: Anomaly Detection.
 The paper references and links are all listed at the bottom of this file.
 
-| **Type**      | **Algo**                           | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** |
-|:--------------|:-----------------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-----------------|
-| Neural Net    | iTransformer[^24]                  |    ✅     |          |          |          |          | 2024 - ICLR      |
-| Neural Net    | FreTS[^23]                         |    ✅     |          |          |          |          | 2024 - NeurIPS   |
-| Neural Net    | SAITS[^1]                          |    ✅     |          |          |          |          | 2023 - ESWA      |
-| Neural Net    | Crossformer[^16]                   |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | TimesNet[^14]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | PatchTST[^18]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | ETSformer[^19]                     |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | DLinear[^17]                       |    ✅     |          |          |          |          | 2023 - AAAI      |
-| Neural Net    | FiLM[^22]                          |    ✅     |          |          |          |          | 2022 - NeurIPS   |
-| Neural Net    | Raindrop[^5]                       |          |          |    ✅     |          |          | 2022 - ICLR      |
-| Neural Net    | FEDformer[^20]                     |    ✅     |          |          |          |          | 2022 - ICML      |
-| Neural Net    | Autoformer[^15]                    |    ✅     |          |          |          |          | 2021 - NeurIPS   |
-| Neural Net    | CSDI[^12]                          |    ✅     |    ✅     |          |          |          | 2021 - NeurIPS   |
-| Neural Net    | Informer[^21]                      |    ✅     |          |          |          |          | 2021 - AAAI      |
-| Neural Net    | US-GAN[^10]                        |    ✅     |          |          |          |          | 2021 - AAAI      |
-| Neural Net    | CRLI[^6]                           |          |          |          |    ✅     |          | 2021 - AAAI      |
-| Probabilistic | BTTF[^8]                           |          |    ✅     |          |          |          | 2021 - TPAMI     |
-| Neural Net    | GP-VAE[^11]                        |    ✅     |          |          |          |          | 2020 - AISTATS   |
-| Neural Net    | VaDER[^7]                          |          |          |          |    ✅     |          | 2019 - GigaSci.  |
-| Neural Net    | M-RNN[^9]                          |    ✅     |          |          |          |          | 2019 - TBME      |
-| Neural Net    | BRITS[^3]                          |    ✅     |          |    ✅     |          |          | 2018 - NeurIPS   |
-| Neural Net    | GRU-D[^4]                          |    ✅     |          |    ✅     |          |          | 2018 - Sci. Rep. |
-| Neural Net    | Transformer[^2]                    |    ✅     |          |          |          |          | 2017 - NeurIPS   |
-| Naive         | LOCF/NOCB                          |    ✅     |          |          |          |          |                  |
-| Naive         | Mean                               |    ✅     |          |          |          |          |                  |
-| Naive         | Median                             |    ✅     |          |          |          |          |                  |
+| **Type**      | **Algo**                    | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue**   |
+|:--------------|:----------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-------------------|
+| Neural Net    | iTransformer🧑‍🔧[^24]      |    ✅     |          |          |          |          | `2024 - ICLR`      |
+| Neural Net    | SAITS[^1]                   |    ✅     |          |          |          |          | `2023 - ESWA`      |
+| Neural Net    | FreTS🧑‍🔧[^23]             |    ✅     |          |          |          |          | `2023 - NeurIPS`   |
+| Neural Net    | Koopa🧑‍🔧[^29]             |    ✅     |          |          |          |          | `2023 - NeurIPS`   |
+| Neural Net    | Crossformer🧑‍🔧[^16]       |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | TimesNet[^14]               |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | PatchTST🧑‍🔧[^18]          |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | ETSformer🧑‍🔧[^19]         |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | MICN🧑‍🔧[^27]              |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | DLinear🧑‍🔧[^17]           |    ✅     |          |          |          |          | `2023 - AAAI`      |
+| Neural Net    | TiDE🧑‍🔧[^28]              |    ✅     |          |          |          |          | `2023 - TMLR`      |
+| Neural Net    | SCINet🧑‍🔧[^30]            |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | Nonstationary Tr.🧑‍🔧[^25] |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | FiLM🧑‍🔧[^22]              |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | RevIN_SCINet🧑‍🔧[^31]      |    ✅     |          |          |          |          | `2022 - ICLR`      |
+| Neural Net    | Pyraformer🧑‍🔧[^26]        |    ✅     |          |          |          |          | `2022 - ICLR`      |
+| Neural Net    | Raindrop[^5]                |          |          |    ✅     |          |          | `2022 - ICLR`      |
+| Neural Net    | FEDformer🧑‍🔧[^20]         |    ✅     |          |          |          |          | `2022 - ICML`      |
+| Neural Net    | Autoformer🧑‍🔧[^15]        |    ✅     |          |          |          |          | `2021 - NeurIPS`   |
+| Neural Net    | CSDI[^12]                   |    ✅     |    ✅     |          |          |          | `2021 - NeurIPS`   |
+| Neural Net    | Informer🧑‍🔧[^21]          |    ✅     |          |          |          |          | `2021 - AAAI`      |
+| Neural Net    | US-GAN[^10]                 |    ✅     |          |          |          |          | `2021 - AAAI`      |
+| Neural Net    | CRLI[^6]                    |          |          |          |    ✅     |          | `2021 - AAAI`      |
+| Probabilistic | BTTF[^8]                    |          |    ✅     |          |          |          | `2021 - TPAMI`     |
+| Neural Net    | StemGNN🧑‍🔧[^33]           |    ✅     |          |          |          |          | `2020 - NeurIPS`   |
+| Neural Net    | Reformer🧑‍🔧[^32]          |    ✅     |          |          |          |          | `2020 - ICLR`      |
+| Neural Net    | GP-VAE[^11]                 |    ✅     |          |          |          |          | `2020 - AISTATS`   |
+| Neural Net    | VaDER[^7]                   |          |          |          |    ✅     |          | `2019 - GigaSci.`  |
+| Neural Net    | M-RNN[^9]                   |    ✅     |          |          |          |          | `2019 - TBME`      |
+| Neural Net    | BRITS[^3]                   |    ✅     |          |    ✅     |          |          | `2018 - NeurIPS`   |
+| Neural Net    | GRU-D[^4]                   |    ✅     |          |    ✅     |          |          | `2018 - Sci. Rep.` |
+| Neural Net    | Transformer🧑‍🔧[^2]        |    ✅     |          |          |          |          | `2017 - NeurIPS`   |
+| Naive         | LOCF/NOCB                   |    ✅     |          |          |          |          |                    |
+| Naive         | Mean                        |    ✅     |          |          |          |          |                    |
+| Naive         | Median                      |    ✅     |          |          |          |          |                    |
 
 
 ## ❖ PyPOTS Ecosystem
 At PyPOTS, things are related to coffee, which we're familiar with. Yes, this is a coffee universe!
 As you can see, there is a coffee pot in the PyPOTS logo.
 And what else? Please read on ;-)
 
@@ -346,17 +358,25 @@
 [^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
 [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
 [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
 [^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
 [^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
 [^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
 [^22]: Zhou, T., Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency improved Legendre Memory Model for Long-term Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
-[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2024*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2023). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2023*.
 [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H., Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are Effective for Time Series Forecasting](https://openreview.net/forum?id=JePfAI8fah). *ICLR 2024*.
-
+[^25]: Liu, Y., Wu, H., Wang, J., & Long, M. (2022). [Non-stationary Transformers: Exploring the Stationarity in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/4054556fcaa934b0bf76da52cf4f92cb-Abstract-Conference.html). *NeurIPS 2022*.
+[^26]: Liu, S., Yu, H., Liao, C., Li, J., Lin, W., Liu, A. X., & Dustdar, S. (2022). [Pyraformer: Low-Complexity Pyramidal Attention for Long-Range Time Series Modeling and Forecasting](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2022*.
+[^27]: Wang, H., Peng, J., Huang, F., Wang, J., Chen, J., & Xiao, Y. (2023). [MICN: Multi-scale Local and Global Context Modeling for Long-term Series Forecasting](https://openreview.net/forum?id=zt53IDUR1U). *ICLR 2023*.
+[^28]: Das, A., Kong, W., Leach, A., Mathur, S., Sen, R., & Yu, R. (2023). [Long-term Forecasting with TiDE: Time-series Dense Encoder](https://openreview.net/forum?id=pCbC3aQB5W). *TMLR 2023*.
+[^29]: Liu, Y., Li, C., Wang, J., & Long, M. (2023). [Koopa: Learning Non-stationary Time Series Dynamics with Koopman Predictors](https://proceedings.neurips.cc/paper_files/paper/2023/hash/28b3dc0970fa4624a63278a4268de997-Abstract-Conference.html). *NeurIPS 2023*.
+[^30]: Liu, M., Zeng, A., Chen, M., Xu, Z., Lai, Q., Ma, L., & Xu, Q. (2022). [SCINet: Time Series Modeling and Forecasting with Sample Convolution and Interaction](https://proceedings.neurips.cc/paper_files/paper/2022/hash/266983d0949aed78a16fa4782237dea7-Abstract-Conference.html). *NeurIPS 2022*.
+[^31]: Kim, T., Kim, J., Tae, Y., Park, C., Choi, J. H., & Choo, J. (2022). [Reversible Instance Normalization for Accurate Time-Series Forecasting against Distribution Shift](https://openreview.net/forum?id=cGDAkQo1C0p). *ICLR 2022*.
+[^32]: Kitaev, N., Kaiser, Ł., & Levskaya, A. (2020). [Reformer: The Efficient Transformer](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2020*.
+[^33]: Cao, D., Wang, Y., Duan, J., Zhang, C., Zhu, X., Huang, C., Tong, Y., Xu, B., Bai, J., Tong, J., & Zhang, Q. (2020). [Spectral Temporal Graph Neural Network for Multivariate Time-series Forecasting](https://proceedings.neurips.cc/paper/2020/hash/cdf6581cb7aca4b7e19ef136c6e601a5-Abstract.html). *NeurIPS 2020*.
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
 </a>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
                           ******** WWeellccoommee ttoo PPyyPPOOTTSS ********
     a Python toolbox for machine learning on Partially-Observed Time Series
 _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_p_o_w_e_r_e_d_ _b_y_ _P_y_t_o_r_c_h_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]
   _[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e
   _C_l_i_m_a_t_e_ _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _c_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_D_o_c_s_ _b_u_i_l_d_i_n_g_]
-        _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]
+   _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]_[_R_E_A_D_M_E_ _i_n
+                                   _E_n_g_l_i_s_h_]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of machine learning on POTS still lacks a dedicated
 toolkit. PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS
@@ -28,74 +29,87 @@
 available-algorithms), [**â PyPOTS Ecosystem**](#-pypots-ecosystem), [**â
 Installation**](#-installation), [**â Usage**](#-usage), [**â Citing
 PyPOTS**](#-citing-pypots), [**â Contribution**](#-contribution), [**â
 Community**](#-community). ## â Available Algorithms PyPOTS supports
 imputation, classification, clustering, forecasting, and anomaly detection
 tasks on multivariate partially-observed time series with missing values. The
 table below shows the availability of each algorithm (sorted by Year) in PyPOTS
-for different tasks. The symbol â indicates the algorithm is available for
+for different tasks. The symbol `â` indicates the algorithm is available for
 the corresponding task (note that models will be continuously updated in the
 future to handle tasks that are not currently supported. Stay tunedâï¸).
 ð Since **v0.2**, all neural-network models in PyPOTS has got
 hyperparameter-optimization support. This functionality is implemented with the
 [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to
 refer to our time-series imputation survey repo [Awesome_Imputation](https://
 github.com/WenjieDu/Awesome_Imputation) to see how to config and tune the
-hyperparameters. ð¥ Note that Transformer, iTransformer, FreTS, Crossformer,
-PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer are not
-proposed as imputation methods in their original papers, and they cannot accept
-POTS as input. **To make them applicable on POTS data, we apply the embedding
-strategy and training approach (ORT+MIT) the same as we did in [SAITS paper]
-(https://arxiv.org/pdf/2202.08516).** The task types are abbreviated as
-follows: **`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**:
-Classification; **`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The
-paper references and links are all listed at the bottom of this file. |
-**Type** | **Algo** | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** |
-**Year - Venue** | |:--------------|:-----------------------------------|:-----
----:|:--------:|:--------:|:--------:|:--------:|:-----------------| | Neural
-Net | iTransformer[^24] | â | | | | | 2024 - ICLR | | Neural Net | FreTS[^23]
-| â | | | | | 2024 - NeurIPS | | Neural Net | SAITS[^1] | â | | | | | 2023
-- ESWA | | Neural Net | Crossformer[^16] | â | | | | | 2023 - ICLR | | Neural
-Net | TimesNet[^14] | â | | | | | 2023 - ICLR | | Neural Net | PatchTST[^18]
-| â | | | | | 2023 - ICLR | | Neural Net | ETSformer[^19] | â | | | | |
-2023 - ICLR | | Neural Net | DLinear[^17] | â | | | | | 2023 - AAAI | |
-Neural Net | FiLM[^22] | â | | | | | 2022 - NeurIPS | | Neural Net | Raindrop
-[^5] | | | â | | | 2022 - ICLR | | Neural Net | FEDformer[^20] | â | | | |
-| 2022 - ICML | | Neural Net | Autoformer[^15] | â | | | | | 2021 - NeurIPS |
-| Neural Net | CSDI[^12] | â | â | | | | 2021 - NeurIPS | | Neural Net |
-Informer[^21] | â | | | | | 2021 - AAAI | | Neural Net | US-GAN[^10] | â |
-| | | | 2021 - AAAI | | Neural Net | CRLI[^6] | | | | â | | 2021 - AAAI | |
-Probabilistic | BTTF[^8] | | â | | | | 2021 - TPAMI | | Neural Net | GP-VAE
-[^11] | â | | | | | 2020 - AISTATS | | Neural Net | VaDER[^7] | | | | â | |
-2019 - GigaSci. | | Neural Net | M-RNN[^9] | â | | | | | 2019 - TBME | |
-Neural Net | BRITS[^3] | â | | â | | | 2018 - NeurIPS | | Neural Net | GRU-
-D[^4] | â | | â | | | 2018 - Sci. Rep. | | Neural Net | Transformer[^2] |
-â | | | | | 2017 - NeurIPS | | Naive | LOCF/NOCB | â | | | | | | | Naive |
-Mean | â | | | | | | | Naive | Median | â | | | | | | ## â PyPOTS
-Ecosystem At PyPOTS, things are related to coffee, which we're familiar with.
-Yes, this is a coffee universe! As you can see, there is a coffee pot in the
-PyPOTS logo. And what else? Please read on ;-) _[_T_S_D_B_ _l_o_g_o_]ð Time series
-datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete
-coffee beans with missing parts that have their own meanings. To make various
-public time-series datasets readily available to users, Time Series Data Beans
-(TSDB) is created to make loading time-series datasets super easy! Visit [TSDB]
-(https://github.com/WenjieDu/TSDB) right now to know more about this handy tool
-ð , and it now supports a total of 169 open-source datasets! _[_P_y_G_r_i_n_d_e_r
-_l_o_g_o_]ð To simulate the real-world data beans with missingness, the ecosystem
-library [PyGrinder](https://github.com/WenjieDu/PyGrinder), a toolkit helping
-grind your coffee beans into incomplete ones, is created. Missing patterns fall
-into three categories according to Robin's theory[^13]: MCAR (missing
-completely at random), MAR (missing at random), and MNAR (missing not at
-random). PyGrinder supports all of them and additional functionalities related
-to missingness. With PyGrinder, you can introduce synthetic missing values into
-your datasets with a single line of code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the
-beans, the grinder, and the pot, how to brew us a cup of coffee? Tutorials are
-necessary! Considering the future workload, PyPOTS tutorials are released in a
-single repo, and you can find them in [BrewPOTS](https://github.com/WenjieDu/
-BrewPOTS). Take a look at it now, and learn how to brew your POTS datasets!
+hyperparameters. ð¥ Note that all models whose name with `ð§âð§` in the
+table (e.g. Transformer, iTransformer, Informer etc.) are not originally
+proposed as algorithms for POTS data in their papers, and they cannot directly
+accept time series with missing values as input, let alone imputation. **To
+make them applicable to POTS data, we specifically apply the embedding strategy
+and training approach (ORT+MIT) the same as we did in [the SAITS paper](https:/
+/arxiv.org/pdf/2202.08516)[^1].** The task types are abbreviated as follows:
+**`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**: Classification;
+**`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The paper references and
+links are all listed at the bottom of this file. | **Type** | **Algo** |
+**IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** | |:---
+-----------|:----------------------------|:--------:|:--------:|:--------:|:---
+-----:|:--------:|:-------------------| | Neural Net | iTransformerð§âð§
+[^24] | â | | | | | `2024 - ICLR` | | Neural Net | SAITS[^1] | â | | | | |
+`2023 - ESWA` | | Neural Net | FreTSð§âð§[^23] | â | | | | | `2023 -
+NeurIPS` | | Neural Net | Koopað§âð§[^29] | â | | | | | `2023 -
+NeurIPS` | | Neural Net | Crossformerð§âð§[^16] | â | | | | | `2023 -
+ICLR` | | Neural Net | TimesNet[^14] | â | | | | | `2023 - ICLR` | | Neural
+Net | PatchTSTð§âð§[^18] | â | | | | | `2023 - ICLR` | | Neural Net |
+ETSformerð§âð§[^19] | â | | | | | `2023 - ICLR` | | Neural Net |
+MICNð§âð§[^27] | â | | | | | `2023 - ICLR` | | Neural Net |
+DLinearð§âð§[^17] | â | | | | | `2023 - AAAI` | | Neural Net |
+TiDEð§âð§[^28] | â | | | | | `2023 - TMLR` | | Neural Net |
+SCINetð§âð§[^30] | â | | | | | `2022 - NeurIPS` | | Neural Net |
+Nonstationary Tr.ð§âð§[^25] | â | | | | | `2022 - NeurIPS` | | Neural
+Net | FiLMð§âð§[^22] | â | | | | | `2022 - NeurIPS` | | Neural Net |
+RevIN_SCINetð§âð§[^31] | â | | | | | `2022 - ICLR` | | Neural Net |
+Pyraformerð§âð§[^26] | â | | | | | `2022 - ICLR` | | Neural Net |
+Raindrop[^5] | | | â | | | `2022 - ICLR` | | Neural Net |
+FEDformerð§âð§[^20] | â | | | | | `2022 - ICML` | | Neural Net |
+Autoformerð§âð§[^15] | â | | | | | `2021 - NeurIPS` | | Neural Net |
+CSDI[^12] | â | â | | | | `2021 - NeurIPS` | | Neural Net |
+Informerð§âð§[^21] | â | | | | | `2021 - AAAI` | | Neural Net | US-GAN
+[^10] | â | | | | | `2021 - AAAI` | | Neural Net | CRLI[^6] | | | | â | |
+`2021 - AAAI` | | Probabilistic | BTTF[^8] | | â | | | | `2021 - TPAMI` | |
+Neural Net | StemGNNð§âð§[^33] | â | | | | | `2020 - NeurIPS` | |
+Neural Net | Reformerð§âð§[^32] | â | | | | | `2020 - ICLR` | | Neural
+Net | GP-VAE[^11] | â | | | | | `2020 - AISTATS` | | Neural Net | VaDER[^7] |
+| | | â | | `2019 - GigaSci.` | | Neural Net | M-RNN[^9] | â | | | | |
+`2019 - TBME` | | Neural Net | BRITS[^3] | â | | â | | | `2018 - NeurIPS` |
+| Neural Net | GRU-D[^4] | â | | â | | | `2018 - Sci. Rep.` | | Neural Net
+| Transformerð§âð§[^2] | â | | | | | `2017 - NeurIPS` | | Naive | LOCF/
+NOCB | â | | | | | | | Naive | Mean | â | | | | | | | Naive | Median | â
+| | | | | | ## â PyPOTS Ecosystem At PyPOTS, things are related to coffee,
+which we're familiar with. Yes, this is a coffee universe! As you can see,
+there is a coffee pot in the PyPOTS logo. And what else? Please read on ;-)
+_[_T_S_D_B_ _l_o_g_o_]ð Time series datasets are taken as coffee beans at PyPOTS, and
+POTS datasets are incomplete coffee beans with missing parts that have their
+own meanings. To make various public time-series datasets readily available to
+users, Time Series Data Beans (TSDB) is created to make loading time-series
+datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB) right now
+to know more about this handy tool ð , and it now supports a total of 169
+open-source datasets! _[_P_y_G_r_i_n_d_e_r_ _l_o_g_o_]ð To simulate the real-world data
+beans with missingness, the ecosystem library [PyGrinder](https://github.com/
+WenjieDu/PyGrinder), a toolkit helping grind your coffee beans into incomplete
+ones, is created. Missing patterns fall into three categories according to
+Robin's theory[^13]: MCAR (missing completely at random), MAR (missing at
+random), and MNAR (missing not at random). PyGrinder supports all of them and
+additional functionalities related to missingness. With PyGrinder, you can
+introduce synthetic missing values into your datasets with a single line of
+code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the beans, the grinder, and the pot, how
+to brew us a cup of coffee? Tutorials are necessary! Considering the future
+workload, PyPOTS tutorials are released in a single repo, and you can find them
+in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and
+learn how to brew your POTS datasets!
 _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
 install PyPOTS like below as well as TSDB and PyGrinder: ``` bash # via pip pip
@@ -251,14 +265,43 @@
 Beyond efficient transformer for long sequence time-series forecasting](https:/
 /ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. [^22]: Zhou, T.,
 Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency
 improved Legendre Memory Model for Long-term Time Series Forecasting](https://
 proceedings.neurips.cc/paper_files/paper/2022/hash/
 524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
 [^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian,
-D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective
+D., Cao, L., & Niu, Z. (2023). [Frequency-domain MLPs are More Effective
 Learners in Time Series Forecasting](https://proceedings.neurips.cc/
 paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-
-Conference.html). *NeurIPS 2024*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
+Conference.html). *NeurIPS 2023*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
 Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are
 Effective for Time Series Forecasting](https://openreview.net/
-forum?id=JePfAI8fah). *ICLR 2024*. ð  Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+forum?id=JePfAI8fah). *ICLR 2024*. [^25]: Liu, Y., Wu, H., Wang, J., & Long, M.
+(2022). [Non-stationary Transformers: Exploring the Stationarity in Time Series
+Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/
+4054556fcaa934b0bf76da52cf4f92cb-Abstract-Conference.html). *NeurIPS 2022*.
+[^26]: Liu, S., Yu, H., Liao, C., Li, J., Lin, W., Liu, A. X., & Dustdar, S.
+(2022). [Pyraformer: Low-Complexity Pyramidal Attention for Long-Range Time
+Series Modeling and Forecasting](https://openreview.net/forum?id=0EXmFzUn5I).
+*ICLR 2022*. [^27]: Wang, H., Peng, J., Huang, F., Wang, J., Chen, J., & Xiao,
+Y. (2023). [MICN: Multi-scale Local and Global Context Modeling for Long-term
+Series Forecasting](https://openreview.net/forum?id=zt53IDUR1U). *ICLR 2023*.
+[^28]: Das, A., Kong, W., Leach, A., Mathur, S., Sen, R., & Yu, R. (2023).
+[Long-term Forecasting with TiDE: Time-series Dense Encoder](https://
+openreview.net/forum?id=pCbC3aQB5W). *TMLR 2023*. [^29]: Liu, Y., Li, C., Wang,
+J., & Long, M. (2023). [Koopa: Learning Non-stationary Time Series Dynamics
+with Koopman Predictors](https://proceedings.neurips.cc/paper_files/paper/2023/
+hash/28b3dc0970fa4624a63278a4268de997-Abstract-Conference.html). *NeurIPS
+2023*. [^30]: Liu, M., Zeng, A., Chen, M., Xu, Z., Lai, Q., Ma, L., & Xu, Q.
+(2022). [SCINet: Time Series Modeling and Forecasting with Sample Convolution
+and Interaction](https://proceedings.neurips.cc/paper_files/paper/2022/hash/
+266983d0949aed78a16fa4782237dea7-Abstract-Conference.html). *NeurIPS 2022*.
+[^31]: Kim, T., Kim, J., Tae, Y., Park, C., Choi, J. H., & Choo, J. (2022).
+[Reversible Instance Normalization for Accurate Time-Series Forecasting against
+Distribution Shift](https://openreview.net/forum?id=cGDAkQo1C0p). *ICLR 2022*.
+[^32]: Kitaev, N., Kaiser, Å., & Levskaya, A. (2020). [Reformer: The Efficient
+Transformer](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2020*. [^33]:
+Cao, D., Wang, Y., Duan, J., Zhang, C., Zhu, X., Huang, C., Tong, Y., Xu, B.,
+Bai, J., Tong, J., & Zhang, Q. (2020). [Spectral Temporal Graph Neural Network
+for Multivariate Time-series Forecasting](https://proceedings.neurips.cc/paper/
+2020/hash/cdf6581cb7aca4b7e19ef136c6e601a5-Abstract.html). *NeurIPS 2020*. ð 
+Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.5/pypots/__init__.py` & `pypots-0.6rc1/pypots/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # X.YaN # Alpha release
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-__version__ = "0.5"
+__version__ = "0.6rc1"
 
 
 from . import imputation, classification, clustering, forecasting, optim, data, utils
 
 __all__ = [
     "imputation",
     "classification",
```

### Comparing `pypots-0.5/pypots/base.py` & `pypots-0.6rc1/pypots/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/base.py` & `pypots-0.6rc1/pypots/classification/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,17 +356,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/classification/brits/__init__.py` & `pypots-0.6rc1/pypots/classification/brits/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/brits/core.py` & `pypots-0.6rc1/pypots/classification/brits/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/brits/data.py` & `pypots-0.6rc1/pypots/classification/brits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/brits/model.py` & `pypots-0.6rc1/pypots/classification/brits/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/grud/__init__.py` & `pypots-0.6rc1/pypots/classification/grud/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/grud/core.py` & `pypots-0.6rc1/pypots/classification/grud/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,38 +3,34 @@
 and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
-from typing import Union
-
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from ...nn.modules.grud import BackboneGRUD
 
 
 class _GRUD(nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         rnn_hidden_size: int,
         n_classes: int,
-        device: Union[str, torch.device],
     ):
         super().__init__()
         self.n_steps = n_steps
         self.n_features = n_features
         self.rnn_hidden_size = rnn_hidden_size
         self.n_classes = n_classes
-        self.device = device
 
         # create models
         self.model = BackboneGRUD(
             n_steps,
             n_features,
             rnn_hidden_size,
         )
```

### Comparing `pypots-0.5/pypots/classification/grud/data.py` & `pypots-0.6rc1/pypots/classification/grud/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/grud/model.py` & `pypots-0.6rc1/pypots/classification/grud/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 
         # set up the model
         self.model = _GRUD(
             self.n_steps,
             self.n_features,
             self.rnn_hidden_size,
             self.n_classes,
-            self.device,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.5/pypots/classification/raindrop/__init__.py` & `pypots-0.6rc1/pypots/classification/raindrop/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/raindrop/core.py` & `pypots-0.6rc1/pypots/classification/raindrop/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/raindrop/data.py` & `pypots-0.6rc1/pypots/classification/raindrop/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/classification/raindrop/model.py` & `pypots-0.6rc1/pypots/classification/raindrop/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/cli/base.py` & `pypots-0.6rc1/pypots/cli/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/cli/dev.py` & `pypots-0.6rc1/pypots/cli/dev.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/cli/doc.py` & `pypots-0.6rc1/pypots/cli/doc.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/cli/env.py` & `pypots-0.6rc1/pypots/cli/env.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/cli/pypots_cli.py` & `pypots-0.6rc1/pypots/cli/pypots_cli.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/cli/tuning.py` & `pypots-0.6rc1/pypots/cli/tuning.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,44 @@
 from argparse import ArgumentParser, Namespace
 
 import torch
 
 from .base import BaseCommand
 from .utils import load_package_from_path
 from ..classification import BRITS as BRITS_classification
-from ..classification import Raindrop, GRUD
+from ..classification import GRUD as GRUD_classification
+from ..classification import Raindrop
 from ..clustering import CRLI, VaDER
 from ..data.saving.h5 import load_dict_from_h5
-from ..imputation import SAITS, Transformer, CSDI, USGAN, GPVAE, MRNN, BRITS, TimesNet
+from ..imputation import (
+    SAITS,
+    FreTS,
+    Koopa,
+    iTransformer,
+    Crossformer,
+    TimesNet,
+    PatchTST,
+    ETSformer,
+    MICN,
+    DLinear,
+    SCINet,
+    NonstationaryTransformer,
+    FiLM,
+    Pyraformer,
+    Autoformer,
+    CSDI,
+    Informer,
+    USGAN,
+    StemGNN,
+    GPVAE,
+    MRNN,
+    BRITS,
+    GRUD,
+    Transformer,
+)
 from ..optim import Adam
 from ..utils.logging import logger
 from ..utils.random import set_random_seed
 
 try:
     import nni
 except ImportError:
@@ -29,23 +55,39 @@
         "❌ Hyperparameter tuning mode needs NNI (https://github.com/microsoft/nni) installed, "
         "but is missing in the current environment."
     )
 
 NN_MODELS = {
     # imputation models
     "pypots.imputation.SAITS": SAITS,
+    "pypots.imputation.iTransformer": iTransformer,
     "pypots.imputation.Transformer": Transformer,
+    "pypots.imputation.FreTS": FreTS,
+    "pypots.imputation.Koopa": Koopa,
+    "pypots.imputation.Crossformer": Crossformer,
+    "pypots.imputation.PatchTST": PatchTST,
+    "pypots.imputation.ETSformer": ETSformer,
+    "pypots.imputation.MICN": MICN,
+    "pypots.imputation.DLinear": DLinear,
+    "pypots.imputation.SCINet": SCINet,
+    "pypots.imputation.NonstationaryTransformer": NonstationaryTransformer,
+    "pypots.imputation.FiLM": FiLM,
+    "pypots.imputation.Pyraformer": Pyraformer,
+    "pypots.imputation.Autoformer": Autoformer,
+    "pypots.imputation.Informer": Informer,
+    "pypots.imputation.StemGNN": StemGNN,
     "pypots.imputation.TimesNet": TimesNet,
     "pypots.imputation.CSDI": CSDI,
     "pypots.imputation.USGAN": USGAN,
     "pypots.imputation.GPVAE": GPVAE,
     "pypots.imputation.BRITS": BRITS,
     "pypots.imputation.MRNN": MRNN,
+    "pypots.imputation.GRUD": GRUD,
     # classification models
-    "pypots.classification.GRUD": GRUD,
+    "pypots.classification.GRUD": GRUD_classification,
     "pypots.classification.BRITS": BRITS_classification,
     "pypots.classification.Raindrop": Raindrop,
     # clustering models
     "pypots.clustering.CRLI": CRLI,
     "pypots.clustering.VaDER": VaDER,
 }
 
@@ -204,15 +246,15 @@
                     model_arguments_set
                 )
                 mismatched = tuner_params_set.difference(
                     set(hyperparameter_intersection)
                 )
                 raise RuntimeError(
                     f"Hyperparameters do not match. Mismatched hyperparameters "
-                    f"(in the tuning configuration but not in the given model's arguments): {list(mismatched)}"
+                    f"(in the tuning configuration but not in {model_class.__name__}'s arguments): {list(mismatched)}"
                 )
 
             # initializing optimizer and model
             # if tuning a GAN model, we need two optimizers
             if "G_optimizer" in model_all_arguments:
                 # optimizer for the generator
                 tuner_params["G_optimizer"] = Adam(lr=lr)
```

### Comparing `pypots-0.5/pypots/cli/utils.py` & `pypots-0.6rc1/pypots/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/clustering/base.py` & `pypots-0.6rc1/pypots/clustering/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,17 +349,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/clustering/crli/__init__.py` & `pypots-0.6rc1/pypots/clustering/crli/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/clustering/crli/core.py` & `pypots-0.6rc1/pypots/clustering/crli/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/clustering/crli/data.py` & `pypots-0.6rc1/pypots/clustering/crli/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/clustering/crli/model.py` & `pypots-0.6rc1/pypots/clustering/crli/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,17 +311,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/clustering/vader/__init__.py` & `pypots-0.6rc1/pypots/clustering/vader/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/clustering/vader/core.py` & `pypots-0.6rc1/pypots/clustering/vader/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/clustering/vader/data.py` & `pypots-0.6rc1/pypots/clustering/vader/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/clustering/vader/model.py` & `pypots-0.6rc1/pypots/clustering/vader/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,17 +324,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/data/__init__.py` & `pypots-0.6rc1/pypots/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/data/checking.py` & `pypots-0.6rc1/pypots/data/checking.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/data/dataset/base.py` & `pypots-0.6rc1/pypots/data/dataset/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/data/generating.py` & `pypots-0.6rc1/pypots/data/generating.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/data/load_preprocessing.py` & `pypots-0.6rc1/pypots/data/load_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/data/load_specific_datasets.py` & `pypots-0.6rc1/pypots/data/load_specific_datasets.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/data/saving/h5.py` & `pypots-0.6rc1/pypots/data/saving/h5.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/data/saving/pickle.py` & `pypots-0.6rc1/pypots/data/saving/pickle.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/data/utils.py` & `pypots-0.6rc1/pypots/data/utils.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/forecasting/base.py` & `pypots-0.6rc1/pypots/forecasting/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,17 +351,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/forecasting/bttf/__init__.py` & `pypots-0.6rc1/pypots/forecasting/bttf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/forecasting/bttf/core.py` & `pypots-0.6rc1/pypots/forecasting/bttf/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/forecasting/bttf/model.py` & `pypots-0.6rc1/pypots/forecasting/bttf/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/forecasting/bttf/submodules.py` & `pypots-0.6rc1/pypots/forecasting/bttf/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/forecasting/csdi/__init__.py` & `pypots-0.6rc1/pypots/forecasting/csdi/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/forecasting/csdi/core.py` & `pypots-0.6rc1/pypots/forecasting/csdi/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/forecasting/csdi/data.py` & `pypots-0.6rc1/pypots/forecasting/csdi/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/forecasting/csdi/model.py` & `pypots-0.6rc1/pypots/forecasting/csdi/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,17 +320,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/imputation/__init__.py` & `pypots-0.6rc1/pypots/imputation/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,25 +9,34 @@
 from .brits import BRITS
 from .csdi import CSDI
 from .gpvae import GPVAE
 from .mrnn import MRNN
 from .saits import SAITS
 from .transformer import Transformer
 from .itransformer import iTransformer
+from .nonstationary_transformer import NonstationaryTransformer
+from .pyraformer import Pyraformer
 from .timesnet import TimesNet
 from .etsformer import ETSformer
 from .fedformer import FEDformer
 from .film import FiLM
 from .frets import FreTS
 from .crossformer import Crossformer
 from .informer import Informer
 from .autoformer import Autoformer
 from .dlinear import DLinear
 from .patchtst import PatchTST
 from .usgan import USGAN
+from .scinet import SCINet
+from .revinscinet import RevIN_SCINet
+from .koopa import Koopa
+from .micn import MICN
+from .tide import TiDE
+from .grud import GRUD
+from .stemgnn import StemGNN
 
 # naive imputation methods
 from .locf import LOCF
 from .mean import Mean
 from .median import Median
 
 __all__ = [
@@ -41,17 +50,26 @@
     "FreTS",
     "Crossformer",
     "TimesNet",
     "PatchTST",
     "DLinear",
     "Informer",
     "Autoformer",
+    "NonstationaryTransformer",
+    "Pyraformer",
     "BRITS",
     "MRNN",
     "GPVAE",
     "USGAN",
     "CSDI",
+    "SCINet",
+    "RevIN_SCINet",
+    "Koopa",
+    "MICN",
+    "TiDE",
+    "GRUD",
+    "StemGNN",
     # naive imputation methods
     "LOCF",
     "Mean",
     "Median",
 ]
```

### Comparing `pypots-0.5/pypots/imputation/autoformer/__init__.py` & `pypots-0.6rc1/pypots/imputation/autoformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/autoformer/core.py` & `pypots-0.6rc1/pypots/imputation/autoformer/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/autoformer/data.py` & `pypots-0.6rc1/pypots/imputation/autoformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/autoformer/model.py` & `pypots-0.6rc1/pypots/imputation/autoformer/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/base.py` & `pypots-0.6rc1/pypots/imputation/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,17 +353,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/imputation/brits/__init__.py` & `pypots-0.6rc1/pypots/imputation/brits/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/brits/core.py` & `pypots-0.6rc1/pypots/imputation/brits/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/brits/data.py` & `pypots-0.6rc1/pypots/imputation/brits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/brits/model.py` & `pypots-0.6rc1/pypots/imputation/brits/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/crossformer/__init__.py` & `pypots-0.6rc1/pypots/imputation/crossformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/crossformer/core.py` & `pypots-0.6rc1/pypots/imputation/crossformer/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/crossformer/data.py` & `pypots-0.6rc1/pypots/imputation/crossformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/crossformer/model.py` & `pypots-0.6rc1/pypots/imputation/crossformer/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/csdi/__init__.py` & `pypots-0.6rc1/pypots/imputation/csdi/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/csdi/core.py` & `pypots-0.6rc1/pypots/imputation/csdi/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/csdi/data.py` & `pypots-0.6rc1/pypots/imputation/csdi/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/csdi/model.py` & `pypots-0.6rc1/pypots/imputation/csdi/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,17 +300,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/imputation/dlinear/__init__.py` & `pypots-0.6rc1/pypots/imputation/dlinear/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/dlinear/core.py` & `pypots-0.6rc1/pypots/imputation/dlinear/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/dlinear/data.py` & `pypots-0.6rc1/pypots/imputation/dlinear/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/dlinear/model.py` & `pypots-0.6rc1/pypots/imputation/dlinear/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/etsformer/__init__.py` & `pypots-0.6rc1/pypots/imputation/etsformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/etsformer/core.py` & `pypots-0.6rc1/pypots/imputation/etsformer/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/etsformer/data.py` & `pypots-0.6rc1/pypots/imputation/etsformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/etsformer/model.py` & `pypots-0.6rc1/pypots/imputation/etsformer/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,22 +99,22 @@
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
     """
 
     def __init__(
         self,
-        n_steps,
-        n_features,
-        n_e_layers,
-        n_d_layers,
-        d_model,
-        n_heads,
-        d_ffn,
-        top_k,
+        n_steps: int,
+        n_features: int,
+        n_e_layers: int,
+        n_d_layers: int,
+        d_model: int,
+        n_heads: int,
+        d_ffn: int,
+        top_k: int,
         dropout: float = 0,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
```

### Comparing `pypots-0.5/pypots/imputation/fedformer/__init__.py` & `pypots-0.6rc1/pypots/imputation/fedformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/fedformer/core.py` & `pypots-0.6rc1/pypots/imputation/fedformer/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/fedformer/data.py` & `pypots-0.6rc1/pypots/imputation/fedformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/fedformer/model.py` & `pypots-0.6rc1/pypots/imputation/fedformer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,21 +107,21 @@
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
     """
 
     def __init__(
         self,
-        n_steps,
-        n_features,
-        n_layers,
-        d_model,
-        n_heads,
-        d_ffn,
-        moving_avg_window_size,
+        n_steps: int,
+        n_features: int,
+        n_layers: int,
+        d_model: int,
+        n_heads: int,
+        d_ffn: int,
+        moving_avg_window_size: int,
         dropout: float = 0,
         version="Fourier",
         modes=32,
         mode_select="random",
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         batch_size: int = 32,
```

### Comparing `pypots-0.5/pypots/imputation/film/__init__.py` & `pypots-0.6rc1/pypots/imputation/film/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/film/core.py` & `pypots-0.6rc1/pypots/imputation/film/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/film/data.py` & `pypots-0.6rc1/pypots/imputation/film/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/film/model.py` & `pypots-0.6rc1/pypots/imputation/film/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     window_size :
         A list including the window sizes for the HiPPO projection layers.
 
     multiscale :
         A list including the multiscale factors for the HiPPO projection layers.
 
-    ratio :
+    dropout :
         The dropout ratio for the HiPPO projection layers.
         It only works when mode_type == 1.
 
     mode_type :
         The mode type of the SpectralConv1d layers.
         It has to be one of [0, 1, 2].
 
@@ -99,16 +99,16 @@
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         window_size: list,
         multiscale: list,
-        modes1: int,
-        ratio: float = 0.5,
+        modes1: int = 32,
+        dropout: float = 0.5,
         mode_type: int = 0,
         d_model: int = 128,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
@@ -131,28 +131,28 @@
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
         self.window_size = window_size
         self.multiscale = multiscale
         self.modes1 = modes1
-        self.ratio = ratio
+        self.dropout = dropout
         self.mode_type = mode_type
         self.d_model = d_model
         self.ORT_weight = ORT_weight
         self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _FiLM(
             self.n_steps,
             self.n_features,
             self.window_size,
             self.multiscale,
             self.modes1,
-            self.ratio,
+            self.dropout,
             self.mode_type,
             self.d_model,
             self.ORT_weight,
             self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
```

### Comparing `pypots-0.5/pypots/imputation/frets/__init__.py` & `pypots-0.6rc1/pypots/imputation/frets/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/frets/core.py` & `pypots-0.6rc1/pypots/imputation/frets/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/frets/data.py` & `pypots-0.6rc1/pypots/imputation/frets/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/frets/model.py` & `pypots-0.6rc1/pypots/imputation/frets/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/gpvae/__init__.py` & `pypots-0.6rc1/pypots/imputation/gpvae/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/gpvae/core.py` & `pypots-0.6rc1/pypots/imputation/gpvae/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/gpvae/data.py` & `pypots-0.6rc1/pypots/imputation/gpvae/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/gpvae/model.py` & `pypots-0.6rc1/pypots/imputation/gpvae/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,17 +329,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/imputation/informer/__init__.py` & `pypots-0.6rc1/pypots/imputation/informer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/informer/core.py` & `pypots-0.6rc1/pypots/imputation/informer/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/informer/data.py` & `pypots-0.6rc1/pypots/imputation/informer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/informer/model.py` & `pypots-0.6rc1/pypots/imputation/informer/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/itransformer/__init__.py` & `pypots-0.6rc1/pypots/imputation/itransformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/itransformer/core.py` & `pypots-0.6rc1/pypots/imputation/itransformer/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/itransformer/model.py` & `pypots-0.6rc1/pypots/imputation/itransformer/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/locf/core.py` & `pypots-0.6rc1/pypots/imputation/locf/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/locf/model.py` & `pypots-0.6rc1/pypots/imputation/locf/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/mean/model.py` & `pypots-0.6rc1/pypots/imputation/mean/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/median/model.py` & `pypots-0.6rc1/pypots/imputation/median/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/mrnn/__init__.py` & `pypots-0.6rc1/pypots/imputation/mrnn/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/mrnn/core.py` & `pypots-0.6rc1/pypots/imputation/mrnn/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/mrnn/data.py` & `pypots-0.6rc1/pypots/imputation/mrnn/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/mrnn/model.py` & `pypots-0.6rc1/pypots/imputation/mrnn/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/patchtst/__init__.py` & `pypots-0.6rc1/pypots/imputation/patchtst/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/patchtst/core.py` & `pypots-0.6rc1/pypots/imputation/patchtst/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/patchtst/data.py` & `pypots-0.6rc1/pypots/imputation/patchtst/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/patchtst/model.py` & `pypots-0.6rc1/pypots/imputation/patchtst/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/saits/core.py` & `pypots-0.6rc1/pypots/imputation/saits/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/saits/data.py` & `pypots-0.6rc1/pypots/imputation/saits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/saits/model.py` & `pypots-0.6rc1/pypots/imputation/saits/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/timesnet/__init__.py` & `pypots-0.6rc1/pypots/imputation/timesnet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/timesnet/core.py` & `pypots-0.6rc1/pypots/imputation/timesnet/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/timesnet/data.py` & `pypots-0.6rc1/pypots/imputation/timesnet/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/timesnet/model.py` & `pypots-0.6rc1/pypots/imputation/timesnet/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/transformer/__init__.py` & `pypots-0.6rc1/pypots/imputation/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/transformer/core.py` & `pypots-0.6rc1/pypots/imputation/transformer/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/transformer/model.py` & `pypots-0.6rc1/pypots/imputation/transformer/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     d_ffn :
         The dimension of the layer in the Feed-Forward Networks (FFN).
 
     dropout :
         The dropout rate for all fully-connected layers in the model.
 
     attn_dropout :
-        The dropout rate for DMSA.
+        The dropout rate for the attention mechanism.
 
     ORT_weight :
         The weight for the ORT loss.
 
     MIT_weight :
         The weight for the MIT loss.
```

### Comparing `pypots-0.5/pypots/imputation/usgan/core.py` & `pypots-0.6rc1/pypots/imputation/usgan/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/usgan/data.py` & `pypots-0.6rc1/pypots/imputation/usgan/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/imputation/usgan/model.py` & `pypots-0.6rc1/pypots/imputation/usgan/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,17 +343,19 @@
 
                 if self.patience == 0:
                     logger.info(
                         "Exceeded the training patience. Terminating the training procedure..."
                     )
                     break
 
-        except Exception as e:
+        except KeyboardInterrupt:  # if keyboard interrupt, only warning
+            logger.warning("‼️ Training got interrupted by the user. Exist now ...")
+        except Exception as e:  # other kind of exception follows below processing
             logger.error(f"❌ Exception: {e}")
-            if self.best_model_dict is None:
+            if self.best_model_dict is None:  # if no best model, raise error
                 raise RuntimeError(
                     "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
                     "Training got interrupted. Please investigate the error printed above.\n"
                     "Model got trained and will load the best checkpoint so far for testing.\n"
```

### Comparing `pypots-0.5/pypots/nn/functional/normalization.py` & `pypots-0.6rc1/pypots/nn/functional/normalization.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/autoformer/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/autoformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/autoformer/autoencoder.py` & `pypots-0.6rc1/pypots/nn/modules/autoformer/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/autoformer/layers.py` & `pypots-0.6rc1/pypots/nn/modules/autoformer/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/brits/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/brits/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/brits/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/brits/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/brits/layers.py` & `pypots-0.6rc1/pypots/nn/modules/brits/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/crli/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/crli/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/crli/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/crli/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/crli/layers.py` & `pypots-0.6rc1/pypots/nn/modules/crli/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/crossformer/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/crossformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/crossformer/autoencoder.py` & `pypots-0.6rc1/pypots/nn/modules/crossformer/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/crossformer/layers.py` & `pypots-0.6rc1/pypots/nn/modules/crossformer/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/csdi/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/csdi/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/csdi/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/csdi/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/csdi/layers.py` & `pypots-0.6rc1/pypots/nn/modules/csdi/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/dlinear/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/dlinear/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/dlinear/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/dlinear/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/etsformer/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/etsformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/etsformer/autoencoder.py` & `pypots-0.6rc1/pypots/nn/modules/etsformer/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/etsformer/layers.py` & `pypots-0.6rc1/pypots/nn/modules/etsformer/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             x_freq = x_freq[:, self.low_freq : -1]
             f = fft.rfftfreq(t)[self.low_freq : -1]
         else:
             x_freq = x_freq[:, self.low_freq :]
             f = fft.rfftfreq(t)[self.low_freq :]
 
         x_freq, index_tuple = self.topk_freq(x_freq)
-        f = repeat(f, "f -> b f d", b=x_freq.size(0), d=x_freq.size(2))
+        f = repeat(f, "f -> b f d", b=x_freq.size(0), d=x_freq.size(2)).to(x_freq.device)
         f = rearrange(f[index_tuple], "b f d -> b f () d").to(x_freq.device)
 
         return self.extrapolate(x_freq, f, t)
 
     def extrapolate(self, x_freq, f, t):
         x_freq = torch.cat([x_freq, x_freq.conj()], dim=1)
         f = torch.cat([f, -f], dim=1)
```

### Comparing `pypots-0.5/pypots/nn/modules/fedformer/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/fedformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/fedformer/autoencoder.py` & `pypots-0.6rc1/pypots/nn/modules/fedformer/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/fedformer/layers.py` & `pypots-0.6rc1/pypots/nn/modules/fedformer/layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import torch
 import torch.nn.functional as F
 from scipy.special import eval_legendre
 from sympy import Poly, legendre, Symbol, chebyshevt
 from torch import Tensor
 from torch import nn
 
+from ..autoformer.layers import MovingAvgBlock
 from ..transformer.attention import AttentionOperator
 
 
 def legendreDer(k, x):
     def _legendre(k, x):
         return (2 * k + 1) * eval_legendre(k, x)
 
@@ -948,7 +949,32 @@
                 continue
             out_ft[:, :, :, j] = xqkvw[:, :, :, i]
         # Return to time domain
         out = torch.fft.irfft(
             out_ft / self.in_channels / self.out_channels, n=xq.size(-1)
         )
         return out, None
+
+
+class SeriesDecompositionMultiBlock(nn.Module):
+    """
+    Series decomposition block from FEDfromer,
+    i.e. series_decomp_multi from https://github.com/MAZiqing/FEDformer
+
+    """
+
+    def __init__(self, kernel_size):
+        super().__init__()
+        self.moving_avg = [MovingAvgBlock(kernel, stride=1) for kernel in kernel_size]
+        self.layer = torch.nn.Linear(1, len(kernel_size))
+
+    def forward(self, x):
+        moving_mean = []
+        for func in self.moving_avg:
+            moving_avg = func(x)
+            moving_mean.append(moving_avg.unsqueeze(-1))
+        moving_mean = torch.cat(moving_mean, dim=-1)
+        moving_mean = torch.sum(
+            moving_mean * nn.Softmax(-1)(self.layer(x.unsqueeze(-1))), dim=-1
+        )
+        res = x - moving_mean
+        return res, moving_mean
```

### Comparing `pypots-0.5/pypots/nn/modules/film/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/film/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/film/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/film/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/film/layers.py` & `pypots-0.6rc1/pypots/nn/modules/film/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/frets/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/frets/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/frets/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/frets/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/gpvae/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/gpvae/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/gpvae/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/gpvae/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/gpvae/layers.py` & `pypots-0.6rc1/pypots/nn/modules/gpvae/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/grud/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/grud/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/grud/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/grud/backbone.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         )
         self.temp_decay_x = TemporalDecay(
             input_size=self.n_features, output_size=self.n_features, diag=True
         )
 
     def forward(
         self, X, missing_mask, deltas, empirical_mean, X_filledLOCF
-    ) -> Tuple[list, torch.Tensor]:
+    ) -> Tuple[torch.Tensor, ...]:
         """Forward processing of GRU-D.
 
         Parameters
         ----------
         X:
 
         missing_mask:
@@ -78,8 +78,10 @@
             representation_collector.append(hidden_state)
 
             x_h = gamma_x * x_filledLOCF + (1 - gamma_x) * empirical_mean
             x_replaced = m * x + (1 - m) * x_h
             data_input = torch.cat([x_replaced, hidden_state, m], dim=1)
             hidden_state = self.rnn_cell(data_input, hidden_state)
 
+        representation_collector = torch.stack(representation_collector, dim=1)
+
         return representation_collector, hidden_state
```

### Comparing `pypots-0.5/pypots/nn/modules/grud/layers.py` & `pypots-0.6rc1/pypots/nn/modules/grud/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/informer/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/informer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/informer/autoencoder.py` & `pypots-0.6rc1/pypots/nn/modules/informer/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/informer/layers.py` & `pypots-0.6rc1/pypots/nn/modules/informer/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/mrnn/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/mrnn/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/mrnn/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/mrnn/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/mrnn/layers.py` & `pypots-0.6rc1/pypots/nn/modules/mrnn/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/patchtst/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/patchtst/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/patchtst/autoencoder.py` & `pypots-0.6rc1/pypots/nn/modules/patchtst/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/patchtst/layers.py` & `pypots-0.6rc1/pypots/nn/modules/patchtst/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/raindrop/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/raindrop/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/raindrop/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/raindrop/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/raindrop/layers.py` & `pypots-0.6rc1/pypots/nn/modules/raindrop/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/saits/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/saits/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/saits/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/saits/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/saits/embedding.py` & `pypots-0.6rc1/pypots/nn/modules/saits/embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 import torch.nn as nn
 
 from ..transformer import PositionalEncoding
 
 
 class SaitsEmbedding(nn.Module):
-    """The embedding method from the SAITS paper :cite:`du2023saits`.
+    """The embedding method from the SAITS paper :cite:`du2023SAITS`.
 
     Parameters
     ----------
     d_in :
         The input dimension.
 
     d_out :
```

### Comparing `pypots-0.5/pypots/nn/modules/saits/loss.py` & `pypots-0.6rc1/pypots/nn/modules/saits/loss.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/timesnet/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/timesnet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/timesnet/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/timesnet/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/timesnet/layers.py` & `pypots-0.6rc1/pypots/nn/modules/timesnet/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/transformer/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/transformer/attention.py` & `pypots-0.6rc1/pypots/nn/modules/transformer/attention.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/transformer/autoencoder.py` & `pypots-0.6rc1/pypots/nn/modules/transformer/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/transformer/embedding.py` & `pypots-0.6rc1/pypots/nn/modules/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/transformer/layers.py` & `pypots-0.6rc1/pypots/nn/modules/transformer/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/usgan/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/usgan/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/usgan/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/usgan/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/usgan/layers.py` & `pypots-0.6rc1/pypots/nn/modules/usgan/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/vader/__init__.py` & `pypots-0.6rc1/pypots/nn/modules/vader/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/vader/backbone.py` & `pypots-0.6rc1/pypots/nn/modules/vader/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/nn/modules/vader/layers.py` & `pypots-0.6rc1/pypots/nn/modules/vader/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/adadelta.py` & `pypots-0.6rc1/pypots/optim/adadelta.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/adagrad.py` & `pypots-0.6rc1/pypots/optim/adagrad.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/adam.py` & `pypots-0.6rc1/pypots/optim/adam.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/adamw.py` & `pypots-0.6rc1/pypots/optim/adamw.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/base.py` & `pypots-0.6rc1/pypots/optim/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/__init__.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/base.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/constant_lrs.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/constant_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/exponential_lrs.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/exponential_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/lambda_lrs.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/lambda_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/linear_lrs.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/linear_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/multiplicative_lrs.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/multiplicative_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/multistep_lrs.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/multistep_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/lr_scheduler/step_lrs.py` & `pypots-0.6rc1/pypots/optim/lr_scheduler/step_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/rmsprop.py` & `pypots-0.6rc1/pypots/optim/rmsprop.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/optim/sgd.py` & `pypots-0.6rc1/pypots/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/utils/file.py` & `pypots-0.6rc1/pypots/utils/file.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/utils/metrics/__init__.py` & `pypots-0.6rc1/pypots/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/utils/metrics/classification.py` & `pypots-0.6rc1/pypots/utils/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/utils/metrics/clustering.py` & `pypots-0.6rc1/pypots/utils/metrics/clustering.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/utils/metrics/error.py` & `pypots-0.6rc1/pypots/utils/metrics/error.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/utils/random.py` & `pypots-0.6rc1/pypots/utils/random.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 """
 PyPOTS util module about random seed setting.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
+import random
+
 import numpy as np
 import torch
 
 from .logging import logger
 
-RANDOM_SEED = 2204
+# Take the birth year of PyPOTS as the default random seed
+RANDOM_SEED: int = 2022
 
 
 def set_random_seed(random_seed: int = RANDOM_SEED) -> None:
     """Manually set the random state to make PyPOTS output reproducible results.
 
     Parameters
     ----------
     random_seed :
         The seed to be set for generating random numbers in PyPOTS.
 
     """
     globals()["RANDOM_SEED"] = random_seed
+    random.seed(random_seed)
     np.random.seed(random_seed)
     torch.manual_seed(random_seed)
+    torch.cuda.manual_seed_all(random_seed)
+    # torch.backends.cudnn.deterministic = True  # This will slow down the training process.
     logger.info(f"Have set the random seed as {random_seed} for numpy and pytorch.")
 
 
 def get_random_seed() -> int:
     """Get the random seed used in PyPOTS.
 
     Returns
```

### Comparing `pypots-0.5/pypots/utils/visual/clustering.py` & `pypots-0.6rc1/pypots/utils/visual/clustering.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots/utils/visual/data.py` & `pypots-0.6rc1/pypots/utils/visual/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.5/pypots.egg-info/PKG-INFO` & `pypots-0.6rc1/pypots.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.5
-Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
+Version: 0.6rc1
+Summary: A Python Toolbox for Machine Learning on Partially-Observed Time Series
 Home-page: https://pypots.com/
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/
 Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
 Project-URL: Tracker, https://github.com/WenjieDu/PyPOTS/issues/
@@ -45,15 +45,15 @@
 <p align="center"><i>a Python toolbox for machine learning on Partially-Observed Time Series</i></p>
 
 <p align="center">
     <a href="https://docs.pypots.com/en/latest/install.html#reasons-of-version-limitations-on-dependencies">
        <img alt="Python version" src="https://img.shields.io/badge/Python-v3.7+-E97040?logo=python&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS">
-        <img alt="powered by Pytorch" src="https://img.shields.io/badge/PyTorch-❤️-F8C6B5?logo=pytorch&logoColor=white">
+        <img alt="powered by Pytorch" src="https://img.shields.io/badge/PyTorch-%E2%9D%A4%EF%B8%8F-F8C6B5?logo=pytorch&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/releases">
         <img alt="the latest release version" src="https://img.shields.io/github/v/release/wenjiedu/pypots?color=EE781F&include_prereleases&label=Release&logo=github&logoColor=white">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/LICENSE">
         <img alt="BSD-3 license" src="https://img.shields.io/badge/License-BSD--3-E9BB41?logo=opensourceinitiative&logoColor=white">
     </a>
@@ -87,15 +87,18 @@
     <a href="https://pepy.tech/project/pypots">
         <img alt="PyPI downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pypots_downloads.json">
     </a>
     <a href="https://arxiv.org/abs/2305.18811">
         <img alt="arXiv DOI" src="https://img.shields.io/badge/DOI-10.48550/arXiv.2305.18811-F8F7F0">
     </a>
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README_zh.md">
-        <img alt="README in Chinese" src="https://img.shields.io/badge/README-🇨🇳中文版-FCEFE8">
+        <img alt="README in Chinese" src="https://pypots.com/figs/pypots_logos/readme/CN.svg">
+    </a>
+   <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README.md">
+        <img alt="README in English" src="https://pypots.com/figs/pypots_logos/readme/US.svg">
     </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error,
 and unexpected malfunction, missing values are common to see in time series from the real-world environment.
 This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced
 data analysis. Although this problem is important, the area of machine learning on POTS still lacks a dedicated toolkit.
@@ -120,63 +123,72 @@
 [**❖ Contribution**](#-contribution),
 [**❖ Community**](#-community).
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, forecasting, and anomaly detection tasks on multivariate partially-observed
 time series with missing values. The table below shows the availability of each algorithm (sorted by Year) in PyPOTS for different tasks.
-The symbol ✅ indicates the algorithm is available for the corresponding task (note that models will be continuously updated
+The symbol `✅` indicates the algorithm is available for the corresponding task (note that models will be continuously updated
 in the future to handle tasks that are not currently supported. Stay tuned❗️).
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to refer to our time-series
 imputation survey repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation) to see how to config and
 tune the hyperparameters.
 
-🔥 Note that Transformer, iTransformer, FreTS, Crossformer, PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer
-are not proposed as imputation methods in their original papers, and they cannot accept POTS as input.
-**To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
-the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+🔥 Note that all models whose name with `🧑‍🔧` in the table (e.g. Transformer, iTransformer, Informer etc.) are not originally
+proposed as algorithms for POTS data in their papers, and they cannot directly accept time series with missing values as input,
+let alone imputation. **To make them applicable to POTS data, we specifically apply the embedding strategy and
+training approach (ORT+MIT) the same as we did in [the SAITS paper](https://arxiv.org/pdf/2202.08516)[^1].**
 
 The task types are abbreviated as follows:
 **`IMPU`**: Imputation;
 **`FORE`**: Forecasting;
 **`CLAS`**: Classification;
 **`CLUS`**: Clustering;
 **`ANOD`**: Anomaly Detection.
 The paper references and links are all listed at the bottom of this file.
 
-| **Type**      | **Algo**                           | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** |
-|:--------------|:-----------------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-----------------|
-| Neural Net    | iTransformer[^24]                  |    ✅     |          |          |          |          | 2024 - ICLR      |
-| Neural Net    | FreTS[^23]                         |    ✅     |          |          |          |          | 2024 - NeurIPS   |
-| Neural Net    | SAITS[^1]                          |    ✅     |          |          |          |          | 2023 - ESWA      |
-| Neural Net    | Crossformer[^16]                   |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | TimesNet[^14]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | PatchTST[^18]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | ETSformer[^19]                     |    ✅     |          |          |          |          | 2023 - ICLR      |
-| Neural Net    | DLinear[^17]                       |    ✅     |          |          |          |          | 2023 - AAAI      |
-| Neural Net    | FiLM[^22]                          |    ✅     |          |          |          |          | 2022 - NeurIPS   |
-| Neural Net    | Raindrop[^5]                       |          |          |    ✅     |          |          | 2022 - ICLR      |
-| Neural Net    | FEDformer[^20]                     |    ✅     |          |          |          |          | 2022 - ICML      |
-| Neural Net    | Autoformer[^15]                    |    ✅     |          |          |          |          | 2021 - NeurIPS   |
-| Neural Net    | CSDI[^12]                          |    ✅     |    ✅     |          |          |          | 2021 - NeurIPS   |
-| Neural Net    | Informer[^21]                      |    ✅     |          |          |          |          | 2021 - AAAI      |
-| Neural Net    | US-GAN[^10]                        |    ✅     |          |          |          |          | 2021 - AAAI      |
-| Neural Net    | CRLI[^6]                           |          |          |          |    ✅     |          | 2021 - AAAI      |
-| Probabilistic | BTTF[^8]                           |          |    ✅     |          |          |          | 2021 - TPAMI     |
-| Neural Net    | GP-VAE[^11]                        |    ✅     |          |          |          |          | 2020 - AISTATS   |
-| Neural Net    | VaDER[^7]                          |          |          |          |    ✅     |          | 2019 - GigaSci.  |
-| Neural Net    | M-RNN[^9]                          |    ✅     |          |          |          |          | 2019 - TBME      |
-| Neural Net    | BRITS[^3]                          |    ✅     |          |    ✅     |          |          | 2018 - NeurIPS   |
-| Neural Net    | GRU-D[^4]                          |    ✅     |          |    ✅     |          |          | 2018 - Sci. Rep. |
-| Neural Net    | Transformer[^2]                    |    ✅     |          |          |          |          | 2017 - NeurIPS   |
-| Naive         | LOCF/NOCB                          |    ✅     |          |          |          |          |                  |
-| Naive         | Mean                               |    ✅     |          |          |          |          |                  |
-| Naive         | Median                             |    ✅     |          |          |          |          |                  |
+| **Type**      | **Algo**                    | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue**   |
+|:--------------|:----------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-------------------|
+| Neural Net    | iTransformer🧑‍🔧[^24]      |    ✅     |          |          |          |          | `2024 - ICLR`      |
+| Neural Net    | SAITS[^1]                   |    ✅     |          |          |          |          | `2023 - ESWA`      |
+| Neural Net    | FreTS🧑‍🔧[^23]             |    ✅     |          |          |          |          | `2023 - NeurIPS`   |
+| Neural Net    | Koopa🧑‍🔧[^29]             |    ✅     |          |          |          |          | `2023 - NeurIPS`   |
+| Neural Net    | Crossformer🧑‍🔧[^16]       |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | TimesNet[^14]               |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | PatchTST🧑‍🔧[^18]          |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | ETSformer🧑‍🔧[^19]         |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | MICN🧑‍🔧[^27]              |    ✅     |          |          |          |          | `2023 - ICLR`      |
+| Neural Net    | DLinear🧑‍🔧[^17]           |    ✅     |          |          |          |          | `2023 - AAAI`      |
+| Neural Net    | TiDE🧑‍🔧[^28]              |    ✅     |          |          |          |          | `2023 - TMLR`      |
+| Neural Net    | SCINet🧑‍🔧[^30]            |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | Nonstationary Tr.🧑‍🔧[^25] |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | FiLM🧑‍🔧[^22]              |    ✅     |          |          |          |          | `2022 - NeurIPS`   |
+| Neural Net    | RevIN_SCINet🧑‍🔧[^31]      |    ✅     |          |          |          |          | `2022 - ICLR`      |
+| Neural Net    | Pyraformer🧑‍🔧[^26]        |    ✅     |          |          |          |          | `2022 - ICLR`      |
+| Neural Net    | Raindrop[^5]                |          |          |    ✅     |          |          | `2022 - ICLR`      |
+| Neural Net    | FEDformer🧑‍🔧[^20]         |    ✅     |          |          |          |          | `2022 - ICML`      |
+| Neural Net    | Autoformer🧑‍🔧[^15]        |    ✅     |          |          |          |          | `2021 - NeurIPS`   |
+| Neural Net    | CSDI[^12]                   |    ✅     |    ✅     |          |          |          | `2021 - NeurIPS`   |
+| Neural Net    | Informer🧑‍🔧[^21]          |    ✅     |          |          |          |          | `2021 - AAAI`      |
+| Neural Net    | US-GAN[^10]                 |    ✅     |          |          |          |          | `2021 - AAAI`      |
+| Neural Net    | CRLI[^6]                    |          |          |          |    ✅     |          | `2021 - AAAI`      |
+| Probabilistic | BTTF[^8]                    |          |    ✅     |          |          |          | `2021 - TPAMI`     |
+| Neural Net    | StemGNN🧑‍🔧[^33]           |    ✅     |          |          |          |          | `2020 - NeurIPS`   |
+| Neural Net    | Reformer🧑‍🔧[^32]          |    ✅     |          |          |          |          | `2020 - ICLR`      |
+| Neural Net    | GP-VAE[^11]                 |    ✅     |          |          |          |          | `2020 - AISTATS`   |
+| Neural Net    | VaDER[^7]                   |          |          |          |    ✅     |          | `2019 - GigaSci.`  |
+| Neural Net    | M-RNN[^9]                   |    ✅     |          |          |          |          | `2019 - TBME`      |
+| Neural Net    | BRITS[^3]                   |    ✅     |          |    ✅     |          |          | `2018 - NeurIPS`   |
+| Neural Net    | GRU-D[^4]                   |    ✅     |          |    ✅     |          |          | `2018 - Sci. Rep.` |
+| Neural Net    | Transformer🧑‍🔧[^2]        |    ✅     |          |          |          |          | `2017 - NeurIPS`   |
+| Naive         | LOCF/NOCB                   |    ✅     |          |          |          |          |                    |
+| Naive         | Mean                        |    ✅     |          |          |          |          |                    |
+| Naive         | Median                      |    ✅     |          |          |          |          |                    |
 
 
 ## ❖ PyPOTS Ecosystem
 At PyPOTS, things are related to coffee, which we're familiar with. Yes, this is a coffee universe!
 As you can see, there is a coffee pot in the PyPOTS logo.
 And what else? Please read on ;-)
 
@@ -384,17 +396,25 @@
 [^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
 [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
 [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
 [^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
 [^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
 [^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
 [^22]: Zhou, T., Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency improved Legendre Memory Model for Long-term Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
-[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2024*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2023). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2023*.
 [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H., Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are Effective for Time Series Forecasting](https://openreview.net/forum?id=JePfAI8fah). *ICLR 2024*.
-
+[^25]: Liu, Y., Wu, H., Wang, J., & Long, M. (2022). [Non-stationary Transformers: Exploring the Stationarity in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/4054556fcaa934b0bf76da52cf4f92cb-Abstract-Conference.html). *NeurIPS 2022*.
+[^26]: Liu, S., Yu, H., Liao, C., Li, J., Lin, W., Liu, A. X., & Dustdar, S. (2022). [Pyraformer: Low-Complexity Pyramidal Attention for Long-Range Time Series Modeling and Forecasting](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2022*.
+[^27]: Wang, H., Peng, J., Huang, F., Wang, J., Chen, J., & Xiao, Y. (2023). [MICN: Multi-scale Local and Global Context Modeling for Long-term Series Forecasting](https://openreview.net/forum?id=zt53IDUR1U). *ICLR 2023*.
+[^28]: Das, A., Kong, W., Leach, A., Mathur, S., Sen, R., & Yu, R. (2023). [Long-term Forecasting with TiDE: Time-series Dense Encoder](https://openreview.net/forum?id=pCbC3aQB5W). *TMLR 2023*.
+[^29]: Liu, Y., Li, C., Wang, J., & Long, M. (2023). [Koopa: Learning Non-stationary Time Series Dynamics with Koopman Predictors](https://proceedings.neurips.cc/paper_files/paper/2023/hash/28b3dc0970fa4624a63278a4268de997-Abstract-Conference.html). *NeurIPS 2023*.
+[^30]: Liu, M., Zeng, A., Chen, M., Xu, Z., Lai, Q., Ma, L., & Xu, Q. (2022). [SCINet: Time Series Modeling and Forecasting with Sample Convolution and Interaction](https://proceedings.neurips.cc/paper_files/paper/2022/hash/266983d0949aed78a16fa4782237dea7-Abstract-Conference.html). *NeurIPS 2022*.
+[^31]: Kim, T., Kim, J., Tae, Y., Park, C., Choi, J. H., & Choo, J. (2022). [Reversible Instance Normalization for Accurate Time-Series Forecasting against Distribution Shift](https://openreview.net/forum?id=cGDAkQo1C0p). *ICLR 2022*.
+[^32]: Kitaev, N., Kaiser, Ł., & Levskaya, A. (2020). [Reformer: The Efficient Transformer](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2020*.
+[^33]: Cao, D., Wang, Y., Duan, J., Zhang, C., Zhu, X., Huang, C., Tong, Y., Xu, B., Bai, J., Tong, J., & Zhang, Q. (2020). [Spectral Temporal Graph Neural Network for Multivariate Time-series Forecasting](https://proceedings.neurips.cc/paper/2020/hash/cdf6581cb7aca4b7e19ef136c6e601a5-Abstract.html). *NeurIPS 2020*.
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
 </a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.5 Summary: A Python Toolbox for
-Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
-Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
-Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
-https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
-WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
-PyPOTS/archive/main.zip Keywords: data science,data mining,neural
+Metadata-Version: 2.1 Name: pypots Version: 0.6rc1 Summary: A Python Toolbox
+for Machine Learning on Partially-Observed Time Series Home-page: https://
+pypots.com/ Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-
+Clause Project-URL: Documentation, https://docs.pypots.com/ Project-URL:
+Source, https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://
+github.com/WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/
+WenjieDu/PyPOTS/archive/main.zip Keywords: data science,data mining,neural
 networks,machine learning,deep learning,artificial intelligence,time-series
 analysis,time
 series,imputation,interpolation,classification,clustering,forecasting,partially
 observed,irregular sampled,partially-observed time series,incomplete time
 series,missing data,missing values Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
@@ -25,15 +25,16 @@
 Provides-Extra: test Provides-Extra: doc Provides-Extra: dev License-File:
 LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
                           ******** WWeellccoommee ttoo PPyyPPOOTTSS ********
     a Python toolbox for machine learning on Partially-Observed Time Series
 _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_p_o_w_e_r_e_d_ _b_y_ _P_y_t_o_r_c_h_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]
   _[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e
   _C_l_i_m_a_t_e_ _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _c_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_D_o_c_s_ _b_u_i_l_d_i_n_g_]
-        _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]
+   _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]_[_R_E_A_D_M_E_ _i_n
+                                   _E_n_g_l_i_s_h_]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of machine learning on POTS still lacks a dedicated
 toolkit. PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS
@@ -53,74 +54,87 @@
 available-algorithms), [**â PyPOTS Ecosystem**](#-pypots-ecosystem), [**â
 Installation**](#-installation), [**â Usage**](#-usage), [**â Citing
 PyPOTS**](#-citing-pypots), [**â Contribution**](#-contribution), [**â
 Community**](#-community). ## â Available Algorithms PyPOTS supports
 imputation, classification, clustering, forecasting, and anomaly detection
 tasks on multivariate partially-observed time series with missing values. The
 table below shows the availability of each algorithm (sorted by Year) in PyPOTS
-for different tasks. The symbol â indicates the algorithm is available for
+for different tasks. The symbol `â` indicates the algorithm is available for
 the corresponding task (note that models will be continuously updated in the
 future to handle tasks that are not currently supported. Stay tunedâï¸).
 ð Since **v0.2**, all neural-network models in PyPOTS has got
 hyperparameter-optimization support. This functionality is implemented with the
 [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to
 refer to our time-series imputation survey repo [Awesome_Imputation](https://
 github.com/WenjieDu/Awesome_Imputation) to see how to config and tune the
-hyperparameters. ð¥ Note that Transformer, iTransformer, FreTS, Crossformer,
-PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer are not
-proposed as imputation methods in their original papers, and they cannot accept
-POTS as input. **To make them applicable on POTS data, we apply the embedding
-strategy and training approach (ORT+MIT) the same as we did in [SAITS paper]
-(https://arxiv.org/pdf/2202.08516).** The task types are abbreviated as
-follows: **`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**:
-Classification; **`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The
-paper references and links are all listed at the bottom of this file. |
-**Type** | **Algo** | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** |
-**Year - Venue** | |:--------------|:-----------------------------------|:-----
----:|:--------:|:--------:|:--------:|:--------:|:-----------------| | Neural
-Net | iTransformer[^24] | â | | | | | 2024 - ICLR | | Neural Net | FreTS[^23]
-| â | | | | | 2024 - NeurIPS | | Neural Net | SAITS[^1] | â | | | | | 2023
-- ESWA | | Neural Net | Crossformer[^16] | â | | | | | 2023 - ICLR | | Neural
-Net | TimesNet[^14] | â | | | | | 2023 - ICLR | | Neural Net | PatchTST[^18]
-| â | | | | | 2023 - ICLR | | Neural Net | ETSformer[^19] | â | | | | |
-2023 - ICLR | | Neural Net | DLinear[^17] | â | | | | | 2023 - AAAI | |
-Neural Net | FiLM[^22] | â | | | | | 2022 - NeurIPS | | Neural Net | Raindrop
-[^5] | | | â | | | 2022 - ICLR | | Neural Net | FEDformer[^20] | â | | | |
-| 2022 - ICML | | Neural Net | Autoformer[^15] | â | | | | | 2021 - NeurIPS |
-| Neural Net | CSDI[^12] | â | â | | | | 2021 - NeurIPS | | Neural Net |
-Informer[^21] | â | | | | | 2021 - AAAI | | Neural Net | US-GAN[^10] | â |
-| | | | 2021 - AAAI | | Neural Net | CRLI[^6] | | | | â | | 2021 - AAAI | |
-Probabilistic | BTTF[^8] | | â | | | | 2021 - TPAMI | | Neural Net | GP-VAE
-[^11] | â | | | | | 2020 - AISTATS | | Neural Net | VaDER[^7] | | | | â | |
-2019 - GigaSci. | | Neural Net | M-RNN[^9] | â | | | | | 2019 - TBME | |
-Neural Net | BRITS[^3] | â | | â | | | 2018 - NeurIPS | | Neural Net | GRU-
-D[^4] | â | | â | | | 2018 - Sci. Rep. | | Neural Net | Transformer[^2] |
-â | | | | | 2017 - NeurIPS | | Naive | LOCF/NOCB | â | | | | | | | Naive |
-Mean | â | | | | | | | Naive | Median | â | | | | | | ## â PyPOTS
-Ecosystem At PyPOTS, things are related to coffee, which we're familiar with.
-Yes, this is a coffee universe! As you can see, there is a coffee pot in the
-PyPOTS logo. And what else? Please read on ;-) _[_T_S_D_B_ _l_o_g_o_]ð Time series
-datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete
-coffee beans with missing parts that have their own meanings. To make various
-public time-series datasets readily available to users, Time Series Data Beans
-(TSDB) is created to make loading time-series datasets super easy! Visit [TSDB]
-(https://github.com/WenjieDu/TSDB) right now to know more about this handy tool
-ð , and it now supports a total of 169 open-source datasets! _[_P_y_G_r_i_n_d_e_r
-_l_o_g_o_]ð To simulate the real-world data beans with missingness, the ecosystem
-library [PyGrinder](https://github.com/WenjieDu/PyGrinder), a toolkit helping
-grind your coffee beans into incomplete ones, is created. Missing patterns fall
-into three categories according to Robin's theory[^13]: MCAR (missing
-completely at random), MAR (missing at random), and MNAR (missing not at
-random). PyGrinder supports all of them and additional functionalities related
-to missingness. With PyGrinder, you can introduce synthetic missing values into
-your datasets with a single line of code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the
-beans, the grinder, and the pot, how to brew us a cup of coffee? Tutorials are
-necessary! Considering the future workload, PyPOTS tutorials are released in a
-single repo, and you can find them in [BrewPOTS](https://github.com/WenjieDu/
-BrewPOTS). Take a look at it now, and learn how to brew your POTS datasets!
+hyperparameters. ð¥ Note that all models whose name with `ð§âð§` in the
+table (e.g. Transformer, iTransformer, Informer etc.) are not originally
+proposed as algorithms for POTS data in their papers, and they cannot directly
+accept time series with missing values as input, let alone imputation. **To
+make them applicable to POTS data, we specifically apply the embedding strategy
+and training approach (ORT+MIT) the same as we did in [the SAITS paper](https:/
+/arxiv.org/pdf/2202.08516)[^1].** The task types are abbreviated as follows:
+**`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**: Classification;
+**`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The paper references and
+links are all listed at the bottom of this file. | **Type** | **Algo** |
+**IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** | |:---
+-----------|:----------------------------|:--------:|:--------:|:--------:|:---
+-----:|:--------:|:-------------------| | Neural Net | iTransformerð§âð§
+[^24] | â | | | | | `2024 - ICLR` | | Neural Net | SAITS[^1] | â | | | | |
+`2023 - ESWA` | | Neural Net | FreTSð§âð§[^23] | â | | | | | `2023 -
+NeurIPS` | | Neural Net | Koopað§âð§[^29] | â | | | | | `2023 -
+NeurIPS` | | Neural Net | Crossformerð§âð§[^16] | â | | | | | `2023 -
+ICLR` | | Neural Net | TimesNet[^14] | â | | | | | `2023 - ICLR` | | Neural
+Net | PatchTSTð§âð§[^18] | â | | | | | `2023 - ICLR` | | Neural Net |
+ETSformerð§âð§[^19] | â | | | | | `2023 - ICLR` | | Neural Net |
+MICNð§âð§[^27] | â | | | | | `2023 - ICLR` | | Neural Net |
+DLinearð§âð§[^17] | â | | | | | `2023 - AAAI` | | Neural Net |
+TiDEð§âð§[^28] | â | | | | | `2023 - TMLR` | | Neural Net |
+SCINetð§âð§[^30] | â | | | | | `2022 - NeurIPS` | | Neural Net |
+Nonstationary Tr.ð§âð§[^25] | â | | | | | `2022 - NeurIPS` | | Neural
+Net | FiLMð§âð§[^22] | â | | | | | `2022 - NeurIPS` | | Neural Net |
+RevIN_SCINetð§âð§[^31] | â | | | | | `2022 - ICLR` | | Neural Net |
+Pyraformerð§âð§[^26] | â | | | | | `2022 - ICLR` | | Neural Net |
+Raindrop[^5] | | | â | | | `2022 - ICLR` | | Neural Net |
+FEDformerð§âð§[^20] | â | | | | | `2022 - ICML` | | Neural Net |
+Autoformerð§âð§[^15] | â | | | | | `2021 - NeurIPS` | | Neural Net |
+CSDI[^12] | â | â | | | | `2021 - NeurIPS` | | Neural Net |
+Informerð§âð§[^21] | â | | | | | `2021 - AAAI` | | Neural Net | US-GAN
+[^10] | â | | | | | `2021 - AAAI` | | Neural Net | CRLI[^6] | | | | â | |
+`2021 - AAAI` | | Probabilistic | BTTF[^8] | | â | | | | `2021 - TPAMI` | |
+Neural Net | StemGNNð§âð§[^33] | â | | | | | `2020 - NeurIPS` | |
+Neural Net | Reformerð§âð§[^32] | â | | | | | `2020 - ICLR` | | Neural
+Net | GP-VAE[^11] | â | | | | | `2020 - AISTATS` | | Neural Net | VaDER[^7] |
+| | | â | | `2019 - GigaSci.` | | Neural Net | M-RNN[^9] | â | | | | |
+`2019 - TBME` | | Neural Net | BRITS[^3] | â | | â | | | `2018 - NeurIPS` |
+| Neural Net | GRU-D[^4] | â | | â | | | `2018 - Sci. Rep.` | | Neural Net
+| Transformerð§âð§[^2] | â | | | | | `2017 - NeurIPS` | | Naive | LOCF/
+NOCB | â | | | | | | | Naive | Mean | â | | | | | | | Naive | Median | â
+| | | | | | ## â PyPOTS Ecosystem At PyPOTS, things are related to coffee,
+which we're familiar with. Yes, this is a coffee universe! As you can see,
+there is a coffee pot in the PyPOTS logo. And what else? Please read on ;-)
+_[_T_S_D_B_ _l_o_g_o_]ð Time series datasets are taken as coffee beans at PyPOTS, and
+POTS datasets are incomplete coffee beans with missing parts that have their
+own meanings. To make various public time-series datasets readily available to
+users, Time Series Data Beans (TSDB) is created to make loading time-series
+datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB) right now
+to know more about this handy tool ð , and it now supports a total of 169
+open-source datasets! _[_P_y_G_r_i_n_d_e_r_ _l_o_g_o_]ð To simulate the real-world data
+beans with missingness, the ecosystem library [PyGrinder](https://github.com/
+WenjieDu/PyGrinder), a toolkit helping grind your coffee beans into incomplete
+ones, is created. Missing patterns fall into three categories according to
+Robin's theory[^13]: MCAR (missing completely at random), MAR (missing at
+random), and MNAR (missing not at random). PyGrinder supports all of them and
+additional functionalities related to missingness. With PyGrinder, you can
+introduce synthetic missing values into your datasets with a single line of
+code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the beans, the grinder, and the pot, how
+to brew us a cup of coffee? Tutorials are necessary! Considering the future
+workload, PyPOTS tutorials are released in a single repo, and you can find them
+in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and
+learn how to brew your POTS datasets!
 _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
 install PyPOTS like below as well as TSDB and PyGrinder: ``` bash # via pip pip
@@ -276,14 +290,43 @@
 Beyond efficient transformer for long sequence time-series forecasting](https:/
 /ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. [^22]: Zhou, T.,
 Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency
 improved Legendre Memory Model for Long-term Time Series Forecasting](https://
 proceedings.neurips.cc/paper_files/paper/2022/hash/
 524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
 [^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian,
-D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective
+D., Cao, L., & Niu, Z. (2023). [Frequency-domain MLPs are More Effective
 Learners in Time Series Forecasting](https://proceedings.neurips.cc/
 paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-
-Conference.html). *NeurIPS 2024*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
+Conference.html). *NeurIPS 2023*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
 Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are
 Effective for Time Series Forecasting](https://openreview.net/
-forum?id=JePfAI8fah). *ICLR 2024*. ð  Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+forum?id=JePfAI8fah). *ICLR 2024*. [^25]: Liu, Y., Wu, H., Wang, J., & Long, M.
+(2022). [Non-stationary Transformers: Exploring the Stationarity in Time Series
+Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/
+4054556fcaa934b0bf76da52cf4f92cb-Abstract-Conference.html). *NeurIPS 2022*.
+[^26]: Liu, S., Yu, H., Liao, C., Li, J., Lin, W., Liu, A. X., & Dustdar, S.
+(2022). [Pyraformer: Low-Complexity Pyramidal Attention for Long-Range Time
+Series Modeling and Forecasting](https://openreview.net/forum?id=0EXmFzUn5I).
+*ICLR 2022*. [^27]: Wang, H., Peng, J., Huang, F., Wang, J., Chen, J., & Xiao,
+Y. (2023). [MICN: Multi-scale Local and Global Context Modeling for Long-term
+Series Forecasting](https://openreview.net/forum?id=zt53IDUR1U). *ICLR 2023*.
+[^28]: Das, A., Kong, W., Leach, A., Mathur, S., Sen, R., & Yu, R. (2023).
+[Long-term Forecasting with TiDE: Time-series Dense Encoder](https://
+openreview.net/forum?id=pCbC3aQB5W). *TMLR 2023*. [^29]: Liu, Y., Li, C., Wang,
+J., & Long, M. (2023). [Koopa: Learning Non-stationary Time Series Dynamics
+with Koopman Predictors](https://proceedings.neurips.cc/paper_files/paper/2023/
+hash/28b3dc0970fa4624a63278a4268de997-Abstract-Conference.html). *NeurIPS
+2023*. [^30]: Liu, M., Zeng, A., Chen, M., Xu, Z., Lai, Q., Ma, L., & Xu, Q.
+(2022). [SCINet: Time Series Modeling and Forecasting with Sample Convolution
+and Interaction](https://proceedings.neurips.cc/paper_files/paper/2022/hash/
+266983d0949aed78a16fa4782237dea7-Abstract-Conference.html). *NeurIPS 2022*.
+[^31]: Kim, T., Kim, J., Tae, Y., Park, C., Choi, J. H., & Choo, J. (2022).
+[Reversible Instance Normalization for Accurate Time-Series Forecasting against
+Distribution Shift](https://openreview.net/forum?id=cGDAkQo1C0p). *ICLR 2022*.
+[^32]: Kitaev, N., Kaiser, Å., & Levskaya, A. (2020). [Reformer: The Efficient
+Transformer](https://openreview.net/forum?id=0EXmFzUn5I). *ICLR 2020*. [^33]:
+Cao, D., Wang, Y., Duan, J., Zhang, C., Zhu, X., Huang, C., Tong, Y., Xu, B.,
+Bai, J., Tong, J., & Zhang, Q. (2020). [Spectral Temporal Graph Neural Network
+for Multivariate Time-series Forecasting](https://proceedings.neurips.cc/paper/
+2020/hash/cdf6581cb7aca4b7e19ef136c6e601a5-Abstract.html). *NeurIPS 2020*. ð 
+Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.5/pypots.egg-info/SOURCES.txt` & `pypots-0.6rc1/pypots.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -103,41 +103,77 @@
 pypots/imputation/frets/core.py
 pypots/imputation/frets/data.py
 pypots/imputation/frets/model.py
 pypots/imputation/gpvae/__init__.py
 pypots/imputation/gpvae/core.py
 pypots/imputation/gpvae/data.py
 pypots/imputation/gpvae/model.py
+pypots/imputation/grud/__init__.py
+pypots/imputation/grud/core.py
+pypots/imputation/grud/data.py
+pypots/imputation/grud/model.py
 pypots/imputation/informer/__init__.py
 pypots/imputation/informer/core.py
 pypots/imputation/informer/data.py
 pypots/imputation/informer/model.py
 pypots/imputation/itransformer/__init__.py
 pypots/imputation/itransformer/core.py
 pypots/imputation/itransformer/data.py
 pypots/imputation/itransformer/model.py
+pypots/imputation/koopa/__init__.py
+pypots/imputation/koopa/core.py
+pypots/imputation/koopa/data.py
+pypots/imputation/koopa/model.py
 pypots/imputation/locf/__init__.py
 pypots/imputation/locf/core.py
 pypots/imputation/locf/model.py
 pypots/imputation/mean/__init__.py
 pypots/imputation/mean/model.py
 pypots/imputation/median/__init__.py
 pypots/imputation/median/model.py
+pypots/imputation/micn/__init__.py
+pypots/imputation/micn/core.py
+pypots/imputation/micn/data.py
+pypots/imputation/micn/model.py
 pypots/imputation/mrnn/__init__.py
 pypots/imputation/mrnn/core.py
 pypots/imputation/mrnn/data.py
 pypots/imputation/mrnn/model.py
+pypots/imputation/nonstationary_transformer/__init__.py
+pypots/imputation/nonstationary_transformer/core.py
+pypots/imputation/nonstationary_transformer/data.py
+pypots/imputation/nonstationary_transformer/model.py
 pypots/imputation/patchtst/__init__.py
 pypots/imputation/patchtst/core.py
 pypots/imputation/patchtst/data.py
 pypots/imputation/patchtst/model.py
+pypots/imputation/pyraformer/__init__.py
+pypots/imputation/pyraformer/core.py
+pypots/imputation/pyraformer/data.py
+pypots/imputation/pyraformer/model.py
+pypots/imputation/revinscinet/__init__.py
+pypots/imputation/revinscinet/core.py
+pypots/imputation/revinscinet/data.py
+pypots/imputation/revinscinet/model.py
 pypots/imputation/saits/__init__.py
 pypots/imputation/saits/core.py
 pypots/imputation/saits/data.py
 pypots/imputation/saits/model.py
+pypots/imputation/scinet/__init__.py
+pypots/imputation/scinet/core.py
+pypots/imputation/scinet/data.py
+pypots/imputation/scinet/model.py
+pypots/imputation/stemgnn/__init__.py
+pypots/imputation/stemgnn/core.py
+pypots/imputation/stemgnn/data.py
+pypots/imputation/stemgnn/model.py
+pypots/imputation/tide/__init__.py
+pypots/imputation/tide/core.py
+pypots/imputation/tide/data.py
+pypots/imputation/tide/model.py
 pypots/imputation/timesnet/__init__.py
 pypots/imputation/timesnet/core.py
 pypots/imputation/timesnet/data.py
 pypots/imputation/timesnet/model.py
 pypots/imputation/transformer/__init__.py
 pypots/imputation/transformer/core.py
 pypots/imputation/transformer/data.py
@@ -183,27 +219,50 @@
 pypots/nn/modules/gpvae/layers.py
 pypots/nn/modules/grud/__init__.py
 pypots/nn/modules/grud/backbone.py
 pypots/nn/modules/grud/layers.py
 pypots/nn/modules/informer/__init__.py
 pypots/nn/modules/informer/autoencoder.py
 pypots/nn/modules/informer/layers.py
+pypots/nn/modules/koopa/__init__.py
+pypots/nn/modules/koopa/backbone.py
+pypots/nn/modules/koopa/layers.py
+pypots/nn/modules/micn/__init__.py
+pypots/nn/modules/micn/backbone.py
+pypots/nn/modules/micn/layers.py
 pypots/nn/modules/mrnn/__init__.py
 pypots/nn/modules/mrnn/backbone.py
 pypots/nn/modules/mrnn/layers.py
+pypots/nn/modules/nonstationary_transformer/__init__.py
+pypots/nn/modules/nonstationary_transformer/autoencoder.py
+pypots/nn/modules/nonstationary_transformer/layers.py
 pypots/nn/modules/patchtst/__init__.py
 pypots/nn/modules/patchtst/autoencoder.py
 pypots/nn/modules/patchtst/layers.py
+pypots/nn/modules/pyraformer/__init__.py
+pypots/nn/modules/pyraformer/autoencoder.py
+pypots/nn/modules/pyraformer/layers.py
 pypots/nn/modules/raindrop/__init__.py
 pypots/nn/modules/raindrop/backbone.py
 pypots/nn/modules/raindrop/layers.py
+pypots/nn/modules/revin/__init__.py
+pypots/nn/modules/revin/layers.py
 pypots/nn/modules/saits/__init__.py
 pypots/nn/modules/saits/backbone.py
 pypots/nn/modules/saits/embedding.py
 pypots/nn/modules/saits/loss.py
+pypots/nn/modules/scinet/__init__.py
+pypots/nn/modules/scinet/backbone.py
+pypots/nn/modules/scinet/layers.py
+pypots/nn/modules/stemgnn/__init__.py
+pypots/nn/modules/stemgnn/backbone.py
+pypots/nn/modules/stemgnn/layers.py
+pypots/nn/modules/tide/__init__.py
+pypots/nn/modules/tide/autoencoder.py
+pypots/nn/modules/tide/layers.py
 pypots/nn/modules/timesnet/__init__.py
 pypots/nn/modules/timesnet/backbone.py
 pypots/nn/modules/timesnet/layers.py
 pypots/nn/modules/transformer/__init__.py
 pypots/nn/modules/transformer/attention.py
 pypots/nn/modules/transformer/autoencoder.py
 pypots/nn/modules/transformer/embedding.py
```

### Comparing `pypots-0.5/pypots.egg-info/requires.txt` & `pypots-0.6rc1/pypots.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pypots-0.5/setup.cfg` & `pypots-0.6rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pypots-0.5/setup.py` & `pypots-0.6rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("./README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="pypots",
     version=__version__,
-    description="A Python Toolbox for Data Mining on Partially-Observed Time Series",
+    description="A Python Toolbox for Machine Learning on Partially-Observed Time Series",
     long_description=README,
     long_description_content_type="text/markdown",
     license="BSD-3-Clause",
     author="Wenjie Du",
     author_email="wenjay.du@gmail.com",
     url="https://pypots.com/",
     project_urls={
```

