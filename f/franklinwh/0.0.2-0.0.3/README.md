# Comparing `tmp/franklinwh-0.0.2.tar.gz` & `tmp/franklinwh-0.0.3.tar.gz`

## Comparing `franklinwh-0.0.2.tar` & `franklinwh-0.0.3.tar`

### file list

```diff
@@ -1,713 +1,1825 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 franklinwh-0.0.2/requirements.txt
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 franklinwh-0.0.2/bin/.fetch.py.swp
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 franklinwh-0.0.2/bin/fetch.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/.gitignore
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/pyvenv.cfg
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/activate
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/activate.csh
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/activate.fish
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/activate.nu
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/activate.ps1
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/activate_this.py
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/normalizer
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/pip
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/pip-3.12
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/pip3
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/pip3.12
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/python -> /opt/homebrew/opt/python@3.12/bin/python3.12
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/bin/python3.12 -> python
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/__editable__.franklinwh-0.0.1.pth
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/__editable___franklinwh_0_0_1_finder.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/_virtualenv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.virtualenv
--rw-r--r--   0        0        0    14451 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build/__init__.py
--rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build/__main__.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build/_exceptions.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build/_importlib.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build/_util.py
--rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build/env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build/py.typed
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build/util.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/LICENSE
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/METADATA
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/WHEEL
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/entry_points.txt
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi/__main__.py
--rw-r--r--   0        0        0   292541 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi/cacert.pem
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/LICENSE
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/top_level.txt
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/__main__.py
--rw-r--r--   0        0        0    21097 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/api.py
--rw-r--r--   0        0        0    12560 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/cd.py
--rw-r--r--   0        0        0    40481 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/constant.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/legacy.py
--rwxr-xr-x   0        0        0    50117 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/md.cpython-312-darwin.so
--rw-r--r--   0        0        0    19624 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/md.py
--rwxr-xr-x   0        0        0   232652 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/md__mypyc.cpython-312-darwin.so
--rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/py.typed
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/version.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0        0        0     9744 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/cli/__main__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0    33550 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/METADATA
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/WHEEL
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/METADATA
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/direct_url.json
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/compat.py
--rw-r--r--   0        0        0    12908 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/core.py
--rw-r--r--   0        0        0    44351 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/py.typed
--rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/uts46data.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna-3.6.dist-info/INSTALLER
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna-3.6.dist-info/LICENSE.md
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna-3.6.dist-info/METADATA
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna-3.6.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/idna-3.6.dist-info/WHEEL
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_elffile.py
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_musllinux.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/markers.py
--rw-r--r--   0        0        0    32750 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/py.typed
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/specifiers.py
--rw-r--r--   0        0        0    18355 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/tags.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/utils.py
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/METADATA
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/WHEEL
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/py.typed
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13839 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23737 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30117 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28920 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37889 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18607 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28155 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27457 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    19028 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35130 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24676 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    21320 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    31317 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    23739 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_api.py
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_windows.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10253 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/METADATA
--rw-r--r--   0        0        0    72974 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/_internal_utils.py
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/auth.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/certs.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/cookies.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/exceptions.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/hooks.py
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/models.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/structures.py
--rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/METADATA
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/__init__.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/_base_connection.py
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/_collections.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/_request_methods.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/_version.py
--rw-r--r--   0        0        0    34704 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/connection.py
--rw-r--r--   0        0        0    43556 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/exceptions.py
--rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/filepost.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/http2.py
--rw-r--r--   0        0        0    22935 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/py.typed
--rw-r--r--   0        0        0    43874 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19161 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/socks.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/__init__.py
--rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/connection.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/fetch.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/request.py
--rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/response.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/response.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/retry.py
--rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/wait.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/METADATA
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 franklinwh-0.0.2/franklinwh/.client.py.swp
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.2/franklinwh/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.2/franklinwh/api.py
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 franklinwh-0.0.2/franklinwh/client.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 franklinwh-0.0.2/LICENSE
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 franklinwh-0.0.2/README.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 franklinwh-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 franklinwh-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 franklinwh-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 franklinwh-0.0.3/bin/fetch.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 franklinwh-0.0.3/bin/login.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/.gitignore
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/pyvenv.cfg
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/activate
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/activate.csh
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/activate.fish
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/activate.nu
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/activate.ps1
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/activate_this.py
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/docutils
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/hatchling
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/keyring
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/markdown-it
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/normalizer
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/pip
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/pip-3.12
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/pip3
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/pip3.12
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/pkginfo
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/pygmentize
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/pyproject-build
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/python -> /opt/homebrew/opt/python@3.12/bin/python3.12
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/python3.12 -> python
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2html
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2html4
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2html5
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2latex
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2man
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2odt
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2pseudoxml
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2s5
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2xetex
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/rst2xml
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/bin/twine
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.virtualenv
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/__init__.py
+-rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/__main__.py
+-rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_builder.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_ctx.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_exceptions.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_types.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_util.py
+-rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/py.typed
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_compat/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_compat/importlib.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_compat/tarfile.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_compat/tomllib.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi/__main__.py
+-rw-r--r--   0        0        0   292541 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi/cacert.pem
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/__main__.py
+-rw-r--r--   0        0        0    21097 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/api.py
+-rw-r--r--   0        0        0    12560 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/cd.py
+-rw-r--r--   0        0        0    40481 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/constant.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/legacy.py
+-rwxr-xr-x   0        0        0    50117 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/md.cpython-312-darwin.so
+-rw-r--r--   0        0        0    19624 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/md.py
+-rwxr-xr-x   0        0        0   232652 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/md__mypyc.cpython-312-darwin.so
+-rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/version.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0        0        0     9744 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/cli/__main__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
+-rw-r--r--   0        0        0    33550 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/WHEEL
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0    10293 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/__init__.py
+-rwxr-xr-x   0        0        0     3625 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/__main__.py
+-rw-r--r--   0        0        0    33045 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/core.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/docutils.conf
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/examples.py
+-rw-r--r--   0        0        0    44396 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/frontend.py
+-rw-r--r--   0        0        0    22583 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/io.py
+-rw-r--r--   0        0        0    80628 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/nodes.py
+-rw-r--r--   0        0        0    56956 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/statemachine.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/af.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/ar.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/ca.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/cs.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/da.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/de.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/en.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/eo.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/es.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/fa.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/fi.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/fr.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/gl.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/he.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/it.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/ja.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/ka.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/ko.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/lt.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/lv.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/nl.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/pl.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/pt_br.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/ru.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/sk.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/sv.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/uk.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/zh_cn.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/languages/zh_tw.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/__init__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/commonmark_wrapper.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/null.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/recommonmark_wrapper.py
+-rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/__init__.py
+-rw-r--r--   0        0        0    16119 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/roles.py
+-rw-r--r--   0        0        0   133123 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/states.py
+-rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/tableparser.py
+-rw-r--r--   0        0        0    14812 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/admonitions.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/body.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/html.py
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/images.py
+-rw-r--r--   0        0        0    26700 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/misc.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/parts.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/references.py
+-rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/directives/tables.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/README.txt
+-rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isoamsa.txt
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isoamsb.txt
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isoamsc.txt
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isoamsn.txt
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isoamso.txt
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isoamsr.txt
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isobox.txt
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isocyr1.txt
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isocyr2.txt
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isodia.txt
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isogrk1.txt
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isogrk2.txt
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isogrk3.txt
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isogrk4.txt
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isolat1.txt
+-rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isolat2.txt
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isomfrk.txt
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isomopf.txt
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isomscr.txt
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isonum.txt
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isopub.txt
+-rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/isotech.txt
+-rw-r--r--   0        0        0    45428 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/mmlalias.txt
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/mmlextra.txt
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/s5defs.txt
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/__init__.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/af.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/ar.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/ca.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/cs.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/da.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/de.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/en.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/eo.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/es.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/fa.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/fi.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/fr.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/gl.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/he.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/it.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/ja.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/ka.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/ko.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/lt.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/lv.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/nl.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/pl.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/pt_br.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/ru.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/sk.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/sv.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/uk.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/zh_cn.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/parsers/rst/languages/zh_tw.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/readers/__init__.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/readers/doctree.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/readers/pep.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/readers/standalone.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/components.py
+-rw-r--r--   0        0        0    20809 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/frontmatter.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/misc.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/parts.py
+-rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/peps.py
+-rw-r--r--   0        0        0    36821 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/references.py
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/universal.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/transforms/writer_aux.py
+-rw-r--r--   0        0        0    30381 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/__init__.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/code_analyzer.py
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/error_reporting.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/punctuation_chars.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/roman.py
+-rwxr-xr-x   0        0        0    39136 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/smartquotes.py
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/urischemes.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/math/__init__.py
+-rw-r--r--   0        0        0    46961 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/math/latex2mathml.py
+-rwxr-xr-x   0        0        0   107808 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/math/math2html.py
+-rw-r--r--   0        0        0    56217 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/math/mathalphabet2unichar.py
+-rw-r--r--   0        0        0    14564 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/math/mathml_elements.py
+-rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/math/tex2mathml_extern.py
+-rw-r--r--   0        0        0    37497 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/math/tex2unichar.py
+-rw-r--r--   0        0        0    18393 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/utils/math/unichar2tex.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/__init__.py
+-rw-r--r--   0        0        0    75401 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/_html_base.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/docutils_xml.py
+-rw-r--r--   0        0        0    38128 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/manpage.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/null.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/pseudoxml.py
+-rw-r--r--   0        0        0    38125 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html4css1/__init__.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html4css1/html4css1.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html4css1/template.txt
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html5_polyglot/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html5_polyglot/italic-field-names.css
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html5_polyglot/math.css
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html5_polyglot/minimal.css
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html5_polyglot/plain.css
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html5_polyglot/responsive.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html5_polyglot/template.txt
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/html5_polyglot/tuftig.css
+-rw-r--r--   0        0        0   138165 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/latex2e/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/latex2e/default.tex
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/latex2e/docutils.sty
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/latex2e/titlepage.tex
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/latex2e/titlingpage.tex
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/latex2e/xelatex.tex
+-rw-r--r--   0        0        0   132081 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/odf_odt/__init__.py
+-rwxr-xr-x   0        0        0     2142 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/odf_odt/prepstyles.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/odf_odt/styles.odt
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/pep_html/__init__.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/pep_html/pep.css
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/pep_html/template.txt
+-rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/README.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/big-black/__base__
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/default/framing.css
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/default/opera.css
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/default/outline.css
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/default/pretty.css
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/default/print.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/default/slides.css
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/default/slides.js
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/small-black/__base__
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils/writers/xetex/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils-0.21.2.dist-info/COPYING.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils-0.21.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils-0.21.2.dist-info/METADATA
+-rw-r--r--   0        0        0    28040 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils-0.21.2.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils-0.21.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/docutils-0.21.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh/api.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh/client.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/METADATA
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/WHEEL
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/direct_url.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/__main__.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/build.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/ouroboros.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/bridge/__init__.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/bridge/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/app.py
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/binary.py
+-rw-r--r--   0        0        0    40735 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/config.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/constants.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/custom.py
+-rw-r--r--   0        0        0    13469 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/sdist.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/utils.py
+-rw-r--r--   0        0        0    34790 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/hooks/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/hooks/custom.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/hooks/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/hooks/plugin/__init__.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/hooks/plugin/hooks.py
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/hooks/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/plugin/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/plugin/hooks.py
+-rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/builders/plugin/interface.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/cli/__init__.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/cli/build/__init__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/cli/dep/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/cli/metadata/__init__.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/cli/version/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/dep/__init__.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/dep/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/licenses/__init__.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/licenses/parse.py
+-rw-r--r--   0        0        0    45903 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/licenses/supported.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/metadata/__init__.py
+-rw-r--r--   0        0        0    63039 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/metadata/core.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/metadata/custom.py
+-rw-r--r--   0        0        0    19970 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/metadata/spec.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/metadata/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/metadata/plugin/__init__.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/metadata/plugin/hooks.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/metadata/plugin/interface.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/plugin/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/plugin/exceptions.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/plugin/manager.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/plugin/specs.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/plugin/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/utils/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/utils/constants.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/utils/context.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/utils/fs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/__init__.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/scheme/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/scheme/standard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/scheme/plugin/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/scheme/plugin/hooks.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/scheme/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/source/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/source/code.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/source/env.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/source/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/source/plugin/__init__.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/source/plugin/hooks.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling/version/source/plugin/interface.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling-1.24.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling-1.24.2.dist-info/METADATA
+-rw-r--r--   0        0        0    10493 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling-1.24.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling-1.24.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling-1.24.2.dist-info/WHEEL
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling-1.24.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/hatchling-1.24.2.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/__init__.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/compat.py
+-rw-r--r--   0        0        0    12908 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/core.py
+-rw-r--r--   0        0        0    44351 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/py.typed
+-rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/uts46data.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/LICENSE.md
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/METADATA
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/WHEEL
+-rw-r--r--   0        0        0    34302 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/diagnose.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/compat/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata/compat/py39.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata-7.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata-7.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata-7.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata-7.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/importlib_metadata-7.1.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/classes/__init__.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/classes/ancestry.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/classes/meta.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/classes/properties.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/classes/py.typed
+-rw-r--r--   0        0        0    16642 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/functools/__init__.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/functools/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco/functools/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.classes-3.4.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.classes-3.4.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.classes-3.4.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.classes-3.4.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.classes-3.4.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.context-5.3.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.context-5.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.context-5.3.0.dist-info/METADATA
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.context-5.3.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.context-5.3.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.context-5.3.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.functools-4.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.functools-4.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.functools-4.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.functools-4.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.functools-4.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.functools-4.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/__main__.py
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backend.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backend_complete.bash
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backend_complete.zsh
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/cli.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/completion.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/core.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/credentials.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/devpi_client.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/errors.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/http.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/py.typed
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/SecretService.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/Windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/__init__.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/chainer.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/fail.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/kwallet.py
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/libsecret.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/null.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/macOS/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/backends/macOS/api.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/compat/__init__.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/compat/properties.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/compat/py312.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/compat/py38.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/testing/__init__.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/testing/backend.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/testing/util.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/util/__init__.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring/util/platform_.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring-25.2.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring-25.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring-25.2.1.dist-info/METADATA
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring-25.2.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring-25.2.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring-25.2.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/keyring-25.2.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/_compat.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/_punycode.py
+-rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/main.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/parser_block.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/parser_core.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/parser_inline.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/port.yaml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/py.typed
+-rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/renderer.py
+-rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/ruler.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/token.py
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/tree.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/cli/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/cli/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/common/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/common/entities.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/common/html_blocks.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/common/html_re.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/common/normalize_url.py
+-rw-r--r--   0        0        0    10728 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/common/utils.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/helpers/__init__.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/helpers/parse_link_destination.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/helpers/parse_link_label.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/helpers/parse_link_title.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/presets/__init__.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/presets/commonmark.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/presets/default.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/presets/zero.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/__init__.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/blockquote.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/code.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/fence.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/heading.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/hr.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/html_block.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/lheading.py
+-rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/list.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/paragraph.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/reference.py
+-rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/state_block.py
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_block/table.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/block.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/inline.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/linkify.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/normalize.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/replacements.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/smartquotes.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/state_core.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_core/text_join.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/__init__.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/autolink.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/backticks.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/emphasis.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/entity.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/escape.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/fragments_join.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/html_inline.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/image.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/link.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/linkify.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/newline.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/state_inline.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/strikethrough.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it/rules_inline/text.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it_py-3.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it_py-3.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0    10827 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it_py-3.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it_py-3.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl/_decode.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl/_encode.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl/_format.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl/_parse.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl/_url.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl-0.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl-0.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl-0.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/mdurl-0.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools/__init__.pyi
+-rwxr-xr-x   0        0        0   143045 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools/more.py
+-rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools/py.typed
+-rw-r--r--   0        0        0    27548 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools/recipes.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools-10.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools-10.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    34886 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools-10.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools-10.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/more_itertools-10.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/nh3/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/nh3/__init__.pyi
+-rwxr-xr-x   0        0        0  3452496 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/nh3/nh3.abi3.so
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/nh3/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/nh3-0.2.17.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/nh3-0.2.17.dist-info/METADATA
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/nh3-0.2.17.dist-info/RECORD
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/nh3-0.2.17.dist-info/WHEEL
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_elffile.py
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/markers.py
+-rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/requirements.py
+-rw-r--r--   0        0        0    39784 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/specifiers.py
+-rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/utils.py
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/__init__.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/_meta.py
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/gitignore.py
+-rw-r--r--   0        0        0    13273 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/pathspec.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/pattern.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/py.typed
+-rw-r--r--   0        0        0    22680 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/util.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/patterns/__init__.py
+-rw-r--r--   0        0        0    12623 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec/patterns/gitwildmatch.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec-0.12.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec-0.12.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec-0.12.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec-0.12.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pathspec-0.12.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+-rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/__init__.py
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_api.py
+-rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_macos.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_openssl.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py
+-rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0    74033 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/__init__.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/__init__.pyi
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/bdist.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/bdist.pyi
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/commandline.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/commandline.pyi
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/develop.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/develop.pyi
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/distribution.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/distribution.pyi
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/index.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/index.pyi
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/installed.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/installed.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/py.typed
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/sdist.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/sdist.pyi
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/utils.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/utils.pyi
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/wheel.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/wheel.pyi
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_bdist.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_commandline.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_develop.py
+-rw-r--r--   0        0        0    19713 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_distribution.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_index.py
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_installed.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_sdist.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_utils.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo/tests/test_wheel.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo-1.10.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo-1.10.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo-1.10.0.dist-info/METADATA
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo-1.10.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo-1.10.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo-1.10.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pkginfo-1.10.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/__init__.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/_callers.py
+-rw-r--r--   0        0        0    25108 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/_hooks.py
+-rw-r--r--   0        0        0    20265 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/_manager.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/_result.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/_tracing.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/_version.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/_warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy-1.5.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy-1.5.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy-1.5.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy-1.5.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy-1.5.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pluggy-1.5.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/__init__.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/__main__.py
+-rw-r--r--   0        0        0    23536 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/cmdline.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/console.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/filter.py
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatter.py
+-rw-r--r--   0        0        0    35109 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexer.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/modeline.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/scanner.py
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/style.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/token.py
+-rw-r--r--   0        0        0    63208 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/unistring.py
+-rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/util.py
+-rw-r--r--   0        0        0    40344 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/__init__.py
+-rwxr-xr-x   0        0        0     4176 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35633 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/html.py
+-rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19258 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0    11921 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_ada_builtins.py
+-rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_asy_builtins.py
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_cl_builtins.py
+-rw-r--r--   0        0        0   105173 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_cocoa_builtins.py
+-rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_csound_builtins.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_css_builtins.py
+-rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_julia_builtins.py
+-rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_lasso_builtins.py
+-rw-r--r--   0        0        0   108094 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_lilypond_builtins.py
+-rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_lua_builtins.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_luau_builtins.py
+-rw-r--r--   0        0        0    69089 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_mql_builtins.py
+-rw-r--r--   0        0        0    25838 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_mysql_builtins.py
+-rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_openedge_builtins.py
+-rw-r--r--   0        0        0   107922 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_php_builtins.py
+-rw-r--r--   0        0        0    13343 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_postgres_builtins.py
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_qlik_builtins.py
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_scheme_builtins.py
+-rw-r--r--   0        0        0    52411 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_scilab_builtins.py
+-rw-r--r--   0        0        0    26777 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_stan_builtins.py
+-rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_stata_builtins.py
+-rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_tsql_builtins.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_usd_builtins.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_vbscript_builtins.py
+-rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/_vim_builtins.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/actionscript.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ada.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/agile.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/algebra.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ambient.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/amdgpu.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ampl.py
+-rw-r--r--   0        0        0    30800 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/apdlexer.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/apl.py
+-rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/archetype.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/arrow.py
+-rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/arturo.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/asc.py
+-rw-r--r--   0        0        0    41934 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/asm.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/asn1.py
+-rw-r--r--   0        0        0    19831 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/automation.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/bare.py
+-rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/basic.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/bdd.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/berry.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/bibtex.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/blueprint.py
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/boa.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/bqn.py
+-rw-r--r--   0        0        0    28345 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/business.py
+-rw-r--r--   0        0        0    18059 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/c_cpp.py
+-rw-r--r--   0        0        0    32021 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/c_like.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/capnproto.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/carbon.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/cddl.py
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/chapel.py
+-rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/clean.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/comal.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/compiled.py
+-rw-r--r--   0        0        0    50534 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/configs.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/console.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/cplint.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/crystal.py
+-rw-r--r--   0        0        0    16998 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/csound.py
+-rw-r--r--   0        0        0    25366 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/css.py
+-rw-r--r--   0        0        0     9920 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/d.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/dalvik.py
+-rw-r--r--   0        0        0    27026 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/data.py
+-rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/dax.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/devicetree.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/diff.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/dns.py
+-rw-r--r--   0        0        0    37958 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/dotnet.py
+-rw-r--r--   0        0        0    36746 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/dsls.py
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/dylan.py
+-rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ecl.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/eiffel.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/elm.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/elpi.py
+-rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/email.py
+-rw-r--r--   0        0        0    19147 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/erlang.py
+-rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/esoteric.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ezhil.py
+-rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/factor.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/fantom.py
+-rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/felix.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/fift.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/floscript.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/forth.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/fortran.py
+-rw-r--r--   0        0        0    26295 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/foxpro.py
+-rw-r--r--   0        0        0    26913 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/freefem.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/func.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/functional.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/futhark.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/gcodelexer.py
+-rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/gdscript.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/go.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/grammar_notation.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/graph.py
+-rw-r--r--   0        0        0    39145 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/graphics.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/graphql.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/graphviz.py
+-rwxr-xr-x   0        0        0     3990 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/gsql.py
+-rw-r--r--   0        0        0    33239 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/haskell.py
+-rw-r--r--   0        0        0    30974 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/haxe.py
+-rw-r--r--   0        0        0    22738 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/hdl.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/hexdump.py
+-rw-r--r--   0        0        0    20574 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/html.py
+-rw-r--r--   0        0        0    15449 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/idl.py
+-rw-r--r--   0        0        0    31626 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/igor.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/inferno.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/installers.py
+-rw-r--r--   0        0        0    56544 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/int_fiction.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/iolang.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/j.py
+-rw-r--r--   0        0        0    63101 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/javascript.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/jmespath.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/jslt.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/jsonnet.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/jsx.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/julia.py
+-rw-r--r--   0        0        0    72666 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/jvm.py
+-rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/kuin.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/kusto.py
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ldap.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/lean.py
+-rw-r--r--   0        0        0     9752 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/lilypond.py
+-rw-r--r--   0        0        0   157668 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/lisp.py
+-rw-r--r--   0        0        0    32844 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/macaulay2.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/make.py
+-rw-r--r--   0        0        0    65088 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/markup.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/math.py
+-rw-r--r--   0        0        0   132962 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/matlab.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/maxima.py
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/meson.py
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/mime.py
+-rw-r--r--   0        0        0    13696 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/minecraft.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/mips.py
+-rw-r--r--   0        0        0    35390 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ml.py
+-rw-r--r--   0        0        0    13683 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/modeling.py
+-rw-r--r--   0        0        0    53072 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/modula2.py
+-rw-r--r--   0        0        0    24181 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/mojo.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/monte.py
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/mosel.py
+-rw-r--r--   0        0        0    63999 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ncl.py
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/nimrod.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/nit.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/nix.py
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/oberon.py
+-rw-r--r--   0        0        0    23240 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/objective.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ooc.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/openscad.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/other.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/parasail.py
+-rw-r--r--   0        0        0    26596 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/parsers.py
+-rw-r--r--   0        0        0    30989 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/pascal.py
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/pawn.py
+-rw-r--r--   0        0        0    39192 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/perl.py
+-rw-r--r--   0        0        0    23249 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/phix.py
+-rw-r--r--   0        0        0    13061 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/php.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/pointless.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/pony.py
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/praat.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/procfile.py
+-rw-r--r--   0        0        0    12866 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/prolog.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/promql.py
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/prql.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ptx.py
+-rw-r--r--   0        0        0    53639 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/python.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/q.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/qlik.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/qvt.py
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/r.py
+-rw-r--r--   0        0        0    16042 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/rdf.py
+-rw-r--r--   0        0        0    18259 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/rebol.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/resource.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ride.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/rita.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/rnc.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/roboconf.py
+-rw-r--r--   0        0        0    18448 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/robotframework.py
+-rw-r--r--   0        0        0    22753 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ruby.py
+-rw-r--r--   0        0        0     8260 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/rust.py
+-rw-r--r--   0        0        0     9456 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/sas.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/savi.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/scdoc.py
+-rw-r--r--   0        0        0    81062 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/scripting.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/sgf.py
+-rw-r--r--   0        0        0    36234 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/shell.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/sieve.py
+-rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/slash.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/smalltalk.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/smithy.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/smv.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/snobol.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/solidity.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/soong.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/sophia.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/special.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/spice.py
+-rw-r--r--   0        0        0    42594 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/sql.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/srcinfo.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/stata.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/supercollider.py
+-rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/tact.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/tal.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/tcl.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/teal.py
+-rw-r--r--   0        0        0    75719 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/templates.py
+-rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/teraterm.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/testing.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/text.py
+-rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/textedit.py
+-rw-r--r--   0        0        0    15524 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/textfmts.py
+-rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/theorem.py
+-rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/thingsdb.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/tlb.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/tls.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/tnt.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/trafficscript.py
+-rw-r--r--   0        0        0     8332 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/typoscript.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/typst.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/ul4.py
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/unicon.py
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/urbi.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/usd.py
+-rw-r--r--   0        0        0     7473 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/varnish.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/verification.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/verifpal.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/vip.py
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/vyper.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/web.py
+-rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/webassembly.py
+-rw-r--r--   0        0        0    10516 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/webidl.py
+-rw-r--r--   0        0        0    40564 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/webmisc.py
+-rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/wgsl.py
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/whiley.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/wowtoc.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/wren.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/x10.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/xorg.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/yang.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/yara.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/lexers/zig.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/_mapping.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/abap.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/algol.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/algol_nu.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/arduino.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/autumn.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/borland.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/bw.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/coffee.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/colorful.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/default.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/dracula.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/emacs.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/friendly.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/friendly_grayscale.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/fruity.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/gh_dark.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/gruvbox.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/igor.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/inkpot.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/lightbulb.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/lilypond.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/lovelace.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/manni.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/material.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/monokai.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/murphy.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/native.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/nord.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/onedark.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/paraiso_dark.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/paraiso_light.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/pastie.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/perldoc.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/rainbow_dash.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/rrt.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/sas.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/solarized.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/staroffice.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/stata_dark.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/stata_light.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/tango.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/trac.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/vim.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/vs.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/xcode.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments/styles/zenburn.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments-2.18.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments-2.18.0.dist-info/METADATA
+-rw-r--r--   0        0        0    45891 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments-2.18.0.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments-2.18.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments-2.18.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments-2.18.0.dist-info/licenses/AUTHORS
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pygments-2.18.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks/py.typed
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks-1.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks-1.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks-1.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks-1.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer/__init__.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer/__main__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer/clean.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer/markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer/py.typed
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer/rst.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer/txt.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer-43.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer-43.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer-43.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer-43.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer-43.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/readme_renderer-43.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/auth.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/certs.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/cookies.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/exceptions.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/hooks.py
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/models.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/structures.py
+-rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/utils.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/__init__.py
+-rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/_compat.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/exceptions.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/sessions.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/streaming_iterator.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/adapters/__init__.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/adapters/appengine.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/adapters/fingerprint.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/adapters/host_header_ssl.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/adapters/socket_options.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/adapters/source.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/adapters/ssl.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/adapters/x509.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/auth/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/auth/guess.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/auth/handler.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/auth/http_proxy_digest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/cookies/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/cookies/forgetful.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/downloadutils/__init__.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/downloadutils/stream.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/downloadutils/tee.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/multipart/__init__.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/multipart/decoder.py
+-rw-r--r--   0        0        0    20769 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/multipart/encoder.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/threaded/__init__.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/threaded/pool.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/threaded/thread.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/utils/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/utils/deprecated.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/utils/dump.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/utils/formdata.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt/utils/user_agent.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt-1.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    14638 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt-1.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/__init__.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/_mixin.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/abnf_regexp.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/api.py
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/builder.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/compat.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/exceptions.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/iri.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/misc.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/normalizers.py
+-rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/parseresult.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/uri.py
+-rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986/validators.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986-2.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986-2.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986-2.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986-2.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/__init__.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/__main__.py
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_export_format.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_inspect.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_pick.py
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_timer.py
+-rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_win32_console.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_windows.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/_wrap.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/abc.py
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/ansi.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/bar.py
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/box.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/cells.py
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/columns.py
+-rw-r--r--   0        0        0    99101 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/constrain.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/containers.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/control.py
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/default_styles.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/diagnose.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/filesize.py
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/highlighter.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/json.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/jupyter.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/layout.py
+-rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/live.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/live_render.py
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/logging.py
+-rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/markdown.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/measure.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/pager.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/palette.py
+-rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/panel.py
+-rw-r--r--   0        0        0    35812 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/pretty.py
+-rw-r--r--   0        0        0    59703 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/progress.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/progress_bar.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/prompt.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/region.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/repr.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/rule.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/scope.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/screen.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/spinner.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/style.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/styled.py
+-rw-r--r--   0        0        0    35367 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/syntax.py
+-rw-r--r--   0        0        0    39644 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/terminal_theme.py
+-rw-r--r--   0        0        0    47300 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/themes.py
+-rw-r--r--   0        0        0    29529 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/traceback.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich/tree.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich-13.7.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich-13.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich-13.7.1.dist-info/METADATA
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich-13.7.1.dist-info/RECORD
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/rich-13.7.1.dist-info/WHEEL
+-rw-r--r--   0        0        0    41433 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers-2024.5.22.dist-info/INSTALLER
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers-2024.5.22.dist-info/LICENSE
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers-2024.5.22.dist-info/METADATA
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers-2024.5.22.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers-2024.5.22.dist-info/WHEEL
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/trove_classifiers-2024.5.22.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/__main__.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/auth.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/cli.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/exceptions.py
+-rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/py.typed
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/repository.py
+-rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/settings.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/utils.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/wheel.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/wininst.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/commands/__init__.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/commands/check.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/commands/register.py
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine/commands/upload.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine-5.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine-5.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine-5.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine-5.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine-5.1.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine-5.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine-5.1.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/twine-5.1.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/__init__.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/_base_connection.py
+-rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/_collections.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/_request_methods.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/_version.py
+-rw-r--r--   0        0        0    34704 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/connection.py
+-rw-r--r--   0        0        0    43556 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/exceptions.py
+-rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/fields.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/filepost.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/http2.py
+-rw-r--r--   0        0        0    22935 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/py.typed
+-rw-r--r--   0        0        0    43874 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0    19161 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/__init__.py
+-rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/connection.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/fetch.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/request.py
+-rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/response.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/request.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/response.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/retry.py
+-rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/wait.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/METADATA
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0    11431 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp/glob.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp/compat/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp/compat/py310.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp-3.19.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp-3.19.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp-3.19.0.dist-info/METADATA
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp-3.19.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp-3.19.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 franklinwh-0.0.3/env/lib/python3.12/site-packages/zipp-3.19.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 franklinwh-0.0.3/franklinwh/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 franklinwh-0.0.3/franklinwh/api.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 franklinwh-0.0.3/franklinwh/client.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 franklinwh-0.0.3/LICENSE
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 franklinwh-0.0.3/README.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 franklinwh-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 franklinwh-0.0.3/PKG-INFO
```

### Comparing `franklinwh-0.0.2/env/bin/activate` & `franklinwh-0.0.3/env/bin/activate`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         unset -f deactivate
     fi
 }
 
 # unset irrelevant variables
 deactivate nondestructive
 
-VIRTUAL_ENV='/Users/richo/src/franklinwh-python/env'
+VIRTUAL_ENV='/Users/richo/src/franklinwh-python-public/env'
 if ([ "$OSTYPE" = "cygwin" ] || [ "$OSTYPE" = "msys" ]) && $(command -v cygpath &> /dev/null) ; then
     VIRTUAL_ENV=$(cygpath -u "$VIRTUAL_ENV")
 fi
 export VIRTUAL_ENV
 
 _OLD_VIRTUAL_PATH="$PATH"
 PATH="$VIRTUAL_ENV/bin:$PATH"
```

### Comparing `franklinwh-0.0.2/env/bin/activate.csh` & `franklinwh-0.0.3/env/bin/activate.csh`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 '
 
 alias deactivate 'test $?_OLD_VIRTUAL_PATH != 0 && setenv PATH "$_OLD_VIRTUAL_PATH:q" && unset _OLD_VIRTUAL_PATH; rehash; test $?_OLD_VIRTUAL_PROMPT != 0 && set prompt="$_OLD_VIRTUAL_PROMPT:q" && unset _OLD_VIRTUAL_PROMPT; unsetenv VIRTUAL_ENV; unsetenv VIRTUAL_ENV_PROMPT; test "\!:*" != "nondestructive" && unalias deactivate && unalias pydoc'
 
 # Unset irrelevant variables.
 deactivate nondestructive
 
-setenv VIRTUAL_ENV '/Users/richo/src/franklinwh-python/env'
+setenv VIRTUAL_ENV '/Users/richo/src/franklinwh-python-public/env'
 
 set _OLD_VIRTUAL_PATH="$PATH:q"
 setenv PATH "$VIRTUAL_ENV:q/bin:$PATH:q"
 
 
 
 if ('' != "") then
```

### Comparing `franklinwh-0.0.2/env/bin/activate.fish` & `franklinwh-0.0.3/env/bin/activate.fish`

 * *Files 1% similar despite different names*

```diff
@@ -54,19 +54,19 @@
         functions -e _fishify_path
     end
 end
 
 # Unset irrelevant variables.
 deactivate nondestructive
 
-set -gx VIRTUAL_ENV '/Users/richo/src/franklinwh-python/env'
+set -gx VIRTUAL_ENV '/Users/richo/src/franklinwh-python-public/env'
 
 # https://github.com/fish-shell/fish-shell/issues/436 altered PATH handling
 if test (echo $FISH_VERSION | head -c 1) -lt 3
-   set -gx _OLD_VIRTUAL_PATH (_bashify_path $PATH)
+    set -gx _OLD_VIRTUAL_PATH (_bashify_path $PATH)
 else
     set -gx _OLD_VIRTUAL_PATH $PATH
 end
 set -gx PATH "$VIRTUAL_ENV"'/bin' $PATH
 
 # Prompt override provided?
 # If not, just use the environment name.
```

### Comparing `franklinwh-0.0.2/env/bin/activate.nu` & `franklinwh-0.0.3/env/bin/activate.nu`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
           not ($env | get -i $name | is-empty)
         }
       } else {
         false
       }
     }
 
-    let virtual_env = '/Users/richo/src/franklinwh-python/env'
+    let virtual_env = '/Users/richo/src/franklinwh-python-public/env'
     let bin = 'bin'
 
     let is_windows = ($nu.os-info.family) == 'windows'
     let path_name = (if (has-env 'Path') {
             'Path'
         } else {
             'PATH'
```

### Comparing `franklinwh-0.0.2/env/bin/activate.ps1` & `franklinwh-0.0.3/env/bin/activate.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-$script:THIS_PATH = $myinvocation.mycommand.path
+﻿$script:THIS_PATH = $myinvocation.mycommand.path
 $script:BASE_DIR = Split-Path (Resolve-Path "$THIS_PATH/..") -Parent
 
 function global:deactivate([switch] $NonDestructive) {
     if (Test-Path variable:_OLD_VIRTUAL_PATH) {
         $env:PATH = $variable:_OLD_VIRTUAL_PATH
         Remove-Variable "_OLD_VIRTUAL_PATH" -Scope global
     }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `franklinwh-0.0.2/env/bin/activate_this.py` & `franklinwh-0.0.3/env/bin/activate_this.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Activate virtualenv for current interpreter:
 
 Use exec(open(this_file).read(), {'__file__': this_file}).
 
 This can be used when you must use an existing Python interpreter, not the virtualenv bin/python.
 """  # noqa: D415
+
 from __future__ import annotations
 
 import os
 import site
 import sys
 
 try:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/_virtualenv.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/_virtualenv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Patches that are applied at runtime to the virtual environment."""
 
 from __future__ import annotations
 
 import os
 import sys
-from contextlib import suppress
 
 VIRTUALENV_PATCH_FILE = os.path.join(__file__)
 
 
 def patch_dist(dist):
     """
     Distutils allows user to configure some arguments via a configuration file:
@@ -47,43 +46,45 @@
 
     # lock[0] is threading.Lock(), but initialized lazily to avoid importing threading very early at startup,
     # because there are gevent-based applications that need to be first to import threading by themselves.
     # See https://github.com/pypa/virtualenv/issues/1895 for details.
     lock = []  # noqa: RUF012
 
     def find_spec(self, fullname, path, target=None):  # noqa: ARG002
-        if fullname in _DISTUTILS_PATCH and self.fullname is None:
+        if fullname in _DISTUTILS_PATCH and self.fullname is None:  # noqa: PLR1702
             # initialize lock[0] lazily
             if len(self.lock) == 0:
-                import threading
+                import threading  # noqa: PLC0415
 
                 lock = threading.Lock()
                 # there is possibility that two threads T1 and T2 are simultaneously running into find_spec,
                 # observing .lock as empty, and further going into hereby initialization. However due to the GIL,
                 # list.append() operation is atomic and this way only one of the threads will "win" to put the lock
                 # - that every thread will use - into .lock[0].
                 # https://docs.python.org/3/faq/library.html#what-kinds-of-global-value-mutation-are-thread-safe
                 self.lock.append(lock)
 
-            from functools import partial
-            from importlib.util import find_spec
+            from functools import partial  # noqa: PLC0415
+            from importlib.util import find_spec  # noqa: PLC0415
 
             with self.lock[0]:
                 self.fullname = fullname
                 try:
                     spec = find_spec(fullname, path)
                     if spec is not None:
                         # https://www.python.org/dev/peps/pep-0451/#how-loading-will-work
                         is_new_api = hasattr(spec.loader, "exec_module")
                         func_name = "exec_module" if is_new_api else "load_module"
                         old = getattr(spec.loader, func_name)
                         func = self.exec_module if is_new_api else self.load_module
                         if old is not func:
-                            with suppress(AttributeError):  # C-Extension loaders are r/o such as zipimporter with <3.7
+                            try:  # noqa: SIM105
                                 setattr(spec.loader, func_name, partial(func, old))
+                            except AttributeError:
+                                pass  # C-Extension loaders are r/o such as zipimporter with <3.7
                         return spec
                 finally:
                     self.fullname = None
         return None
 
     @staticmethod
     def exec_module(old, module):
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/build/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,87 +1,67 @@
 # SPDX-License-Identifier: MIT
 
-"""
-build - A simple, correct PEP 517 build frontend
-"""
-
 from __future__ import annotations
 
-
-__version__ = '1.0.3'
-
 import contextlib
 import difflib
-import logging
 import os
 import subprocess
 import sys
 import warnings
 import zipfile
 
 from collections.abc import Iterator
-from typing import Any, Callable, Mapping, Optional, Sequence, TypeVar, Union
+from typing import Any, Mapping, Sequence, TypeVar
 
 import pyproject_hooks
 
-from . import env
+from . import _ctx, env
+from ._compat import tomllib
 from ._exceptions import (
     BuildBackendException,
     BuildException,
     BuildSystemTableValidationError,
-    FailedProcessError,
     TypoWarning,
 )
+from ._types import ConfigSettings, Distribution, StrPath, SubprocessRunner
 from ._util import check_dependency, parse_wheel_filename
 
 
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    import tomli as tomllib
-
-
-RunnerType = Callable[[Sequence[str], Optional[str], Optional[Mapping[str, str]]], None]
-ConfigSettingsType = Mapping[str, Union[str, Sequence[str]]]
-PathType = Union[str, 'os.PathLike[str]']
-
 _TProjectBuilder = TypeVar('_TProjectBuilder', bound='ProjectBuilder')
 
 
 _DEFAULT_BACKEND = {
     'build-backend': 'setuptools.build_meta:__legacy__',
-    'requires': ['setuptools >= 40.8.0', 'wheel'],
+    'requires': ['setuptools >= 40.8.0'],
 }
 
 
-_logger = logging.getLogger(__name__)
-
-
 def _find_typo(dictionary: Mapping[str, str], expected: str) -> None:
     for obj in dictionary:
         if difflib.SequenceMatcher(None, expected, obj).ratio() >= 0.8:
             warnings.warn(
                 f"Found '{obj}' in pyproject.toml, did you mean '{expected}'?",
                 TypoWarning,
                 stacklevel=2,
             )
 
 
-def _validate_source_directory(source_dir: PathType) -> None:
+def _validate_source_directory(source_dir: StrPath) -> None:
     if not os.path.isdir(source_dir):
         msg = f'Source {source_dir} is not a directory'
         raise BuildException(msg)
     pyproject_toml = os.path.join(source_dir, 'pyproject.toml')
     setup_py = os.path.join(source_dir, 'setup.py')
     if not os.path.exists(pyproject_toml) and not os.path.exists(setup_py):
         msg = f'Source {source_dir} does not appear to be a Python project: no pyproject.toml or setup.py'
         raise BuildException(msg)
 
 
-def _read_pyproject_toml(path: PathType) -> Mapping[str, Any]:
+def _read_pyproject_toml(path: StrPath) -> Mapping[str, Any]:
     try:
         with open(path, 'rb') as f:
             return tomllib.loads(f.read().decode())
     except FileNotFoundError:
         return {}
     except PermissionError as e:
         msg = f"{e.strerror}: '{e.filename}' "
@@ -131,31 +111,31 @@
     if unknown_props:
         msg = f'Unknown properties: {", ".join(unknown_props)}'
         raise BuildSystemTableValidationError(msg)
 
     return build_system_table
 
 
-def _wrap_subprocess_runner(runner: RunnerType, env: env.IsolatedEnv) -> RunnerType:
+def _wrap_subprocess_runner(runner: SubprocessRunner, env: env.IsolatedEnv) -> SubprocessRunner:
     def _invoke_wrapped_runner(cmd: Sequence[str], cwd: str | None, extra_environ: Mapping[str, str] | None) -> None:
         runner(cmd, cwd, {**(env.make_extra_environ() or {}), **(extra_environ or {})})
 
     return _invoke_wrapped_runner
 
 
 class ProjectBuilder:
     """
     The PEP 517 consumer API.
     """
 
     def __init__(
         self,
-        source_dir: PathType,
+        source_dir: StrPath,
         python_executable: str = sys.executable,
-        runner: RunnerType = pyproject_hooks.default_subprocess_runner,
+        runner: SubprocessRunner = pyproject_hooks.default_subprocess_runner,
     ) -> None:
         """
         :param source_dir: The source directory
         :param python_executable: The python executable where the backend lives
         :param runner: Runner for backend subprocesses
 
         The ``runner``, if provided, must accept the following arguments:
@@ -189,16 +169,16 @@
             runner=self._runner,
         )
 
     @classmethod
     def from_isolated_env(
         cls: type[_TProjectBuilder],
         env: env.IsolatedEnv,
-        source_dir: PathType,
-        runner: RunnerType = pyproject_hooks.default_subprocess_runner,
+        source_dir: StrPath,
+        runner: SubprocessRunner = pyproject_hooks.default_subprocess_runner,
     ) -> _TProjectBuilder:
         return cls(
             source_dir=source_dir,
             python_executable=env.python_executable,
             runner=_wrap_subprocess_runner(runner, env),
         )
 
@@ -219,89 +199,94 @@
         """
         The dependencies defined in the ``pyproject.toml``'s
         ``build-system.requires`` field or the default build dependencies
         if ``pyproject.toml`` is missing or ``build-system`` is undefined.
         """
         return set(self._build_system['requires'])
 
-    def get_requires_for_build(self, distribution: str, config_settings: ConfigSettingsType | None = None) -> set[str]:
+    def get_requires_for_build(self, distribution: Distribution, config_settings: ConfigSettings | None = None) -> set[str]:
         """
         Return the dependencies defined by the backend in addition to
         :attr:`build_system_requires` for a given distribution.
 
         :param distribution: Distribution to get the dependencies of
             (``sdist`` or ``wheel``)
         :param config_settings: Config settings for the build backend
         """
-        self.log(f'Getting build dependencies for {distribution}...')
+        _ctx.log(f'Getting build dependencies for {distribution}...')
         hook_name = f'get_requires_for_build_{distribution}'
         get_requires = getattr(self._hook, hook_name)
 
         with self._handle_backend(hook_name):
             return set(get_requires(config_settings))
 
-    def check_dependencies(self, distribution: str, config_settings: ConfigSettingsType | None = None) -> set[tuple[str, ...]]:
+    def check_dependencies(
+        self, distribution: Distribution, config_settings: ConfigSettings | None = None
+    ) -> set[tuple[str, ...]]:
         """
         Return the dependencies which are not satisfied from the combined set of
         :attr:`build_system_requires` and :meth:`get_requires_for_build` for a given
         distribution.
 
         :param distribution: Distribution to check (``sdist`` or ``wheel``)
         :param config_settings: Config settings for the build backend
         :returns: Set of variable-length unmet dependency tuples
         """
         dependencies = self.get_requires_for_build(distribution, config_settings).union(self.build_system_requires)
         return {u for d in dependencies for u in check_dependency(d)}
 
     def prepare(
-        self, distribution: str, output_directory: PathType, config_settings: ConfigSettingsType | None = None
+        self,
+        distribution: Distribution,
+        output_directory: StrPath,
+        config_settings: ConfigSettings | None = None,
     ) -> str | None:
         """
         Prepare metadata for a distribution.
 
         :param distribution: Distribution to build (must be ``wheel``)
         :param output_directory: Directory to put the prepared metadata in
         :param config_settings: Config settings for the build backend
         :returns: The full path to the prepared metadata directory
         """
-        self.log(f'Getting metadata for {distribution}...')
+        _ctx.log(f'Getting metadata for {distribution}...')
         try:
             return self._call_backend(
                 f'prepare_metadata_for_build_{distribution}',
                 output_directory,
                 config_settings,
                 _allow_fallback=False,
             )
         except BuildBackendException as exception:
             if isinstance(exception.exception, pyproject_hooks.HookMissing):
                 return None
             raise
 
     def build(
         self,
-        distribution: str,
-        output_directory: PathType,
-        config_settings: ConfigSettingsType | None = None,
+        distribution: Distribution,
+        output_directory: StrPath,
+        config_settings: ConfigSettings | None = None,
         metadata_directory: str | None = None,
     ) -> str:
         """
         Build a distribution.
 
         :param distribution: Distribution to build (``sdist`` or ``wheel``)
         :param output_directory: Directory to put the built distribution in
         :param config_settings: Config settings for the build backend
         :param metadata_directory: If provided, should be the return value of a
             previous ``prepare`` call on the same ``distribution`` kind
         :returns: The full path to the built distribution
         """
-        self.log(f'Building {distribution}...')
+        _ctx.log(f'Building {distribution}...')
         kwargs = {} if metadata_directory is None else {'metadata_directory': metadata_directory}
         return self._call_backend(f'build_{distribution}', output_directory, config_settings, **kwargs)
 
-    def metadata_path(self, output_directory: PathType) -> str:
+    def metadata_path(self, output_directory: StrPath) -> str:
         """
         Generate the metadata directory of a distribution and return its path.
 
         If the backend does not support the ``prepare_metadata_for_build_wheel``
         hook, a wheel will be built and the metadata will be extracted from it.
 
         :param output_directory: Directory to put the metadata distribution in
@@ -324,15 +309,15 @@
             w.extractall(
                 output_directory,
                 (member for member in w.namelist() if member.startswith(member_prefix)),
             )
         return os.path.join(output_directory, distinfo)
 
     def _call_backend(
-        self, hook_name: str, outdir: PathType, config_settings: ConfigSettingsType | None = None, **kwargs: Any
+        self, hook_name: str, outdir: StrPath, config_settings: ConfigSettings | None = None, **kwargs: Any
     ) -> str:
         outdir = os.path.abspath(outdir)
 
         callback = getattr(self._hook, hook_name)
 
         if os.path.exists(outdir):
             if not os.path.isdir(outdir):
@@ -356,40 +341,7 @@
                 f"Backend '{self._backend}' is not available.",
                 sys.exc_info(),
             ) from None
         except subprocess.CalledProcessError as exception:
             raise BuildBackendException(exception, f'Backend subprocess exited when trying to invoke {hook}') from None
         except Exception as exception:
             raise BuildBackendException(exception, exc_info=sys.exc_info()) from None
-
-    @staticmethod
-    def log(message: str) -> None:
-        """
-        Log a message.
-
-        The default implementation uses the logging module but this function can be
-        overridden by users to have a different implementation.
-
-        :param message: Message to output
-        """
-        if sys.version_info >= (3, 8):
-            _logger.log(logging.INFO, message, stacklevel=2)
-        else:
-            _logger.log(logging.INFO, message)
-
-
-__all__ = [
-    '__version__',
-    'BuildSystemTableValidationError',
-    'BuildBackendException',
-    'BuildException',
-    'ConfigSettingsType',
-    'FailedProcessError',
-    'ProjectBuilder',
-    'RunnerType',
-    'TypoWarning',
-    'check_dependency',
-]
-
-
-def __dir__() -> list[str]:
-    return __all__
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/build/__main__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/build/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 import contextlib
+import contextvars
 import os
 import platform
 import shutil
 import subprocess
 import sys
 import tempfile
 import textwrap
@@ -16,16 +17,18 @@
 
 from collections.abc import Iterator, Sequence
 from functools import partial
 from typing import NoReturn, TextIO
 
 import build
 
-from . import ConfigSettingsType, PathType, ProjectBuilder
+from . import ProjectBuilder, _ctx
+from . import env as _env
 from ._exceptions import BuildBackendException, BuildException, FailedProcessError
+from ._types import ConfigSettings, Distribution, StrPath
 from .env import DefaultIsolatedEnv
 
 
 _COLORS = {
     'red': '\33[91m',
     'green': '\33[92m',
     'yellow': '\33[93m',
@@ -33,122 +36,142 @@
     'dim': '\33[2m',
     'underline': '\33[4m',
     'reset': '\33[0m',
 }
 _NO_COLORS = {color: '' for color in _COLORS}
 
 
-def _init_colors() -> dict[str, str]:
+_styles = contextvars.ContextVar('_styles', default=_COLORS)
+
+
+def _init_colors() -> None:
     if 'NO_COLOR' in os.environ:
         if 'FORCE_COLOR' in os.environ:
             warnings.warn('Both NO_COLOR and FORCE_COLOR environment variables are set, disabling color', stacklevel=2)
-        return _NO_COLORS
+        _styles.set(_NO_COLORS)
     elif 'FORCE_COLOR' in os.environ or sys.stdout.isatty():
-        return _COLORS
-    return _NO_COLORS
-
+        return
+    _styles.set(_NO_COLORS)
 
-_STYLES = _init_colors()
 
-
-def _cprint(fmt: str = '', msg: str = '') -> None:
-    print(fmt.format(msg, **_STYLES), flush=True)
+def _cprint(fmt: str = '', msg: str = '', file: TextIO | None = None) -> None:
+    print(fmt.format(msg, **_styles.get()), file=file, flush=True)
 
 
 def _showwarning(
     message: Warning | str,
     category: type[Warning],
     filename: str,
     lineno: int,
     file: TextIO | None = None,
     line: str | None = None,
 ) -> None:  # pragma: no cover
     _cprint('{yellow}WARNING{reset} {}', str(message))
 
 
-def _setup_cli() -> None:
+_max_terminal_width = shutil.get_terminal_size().columns - 2
+if _max_terminal_width <= 0:
+    _max_terminal_width = 78
+
+
+_fill = partial(textwrap.fill, subsequent_indent='  ', width=_max_terminal_width)
+
+
+def _log(message: str, *, origin: tuple[str, ...] | None = None) -> None:
+    if origin is None:
+        (first, *rest) = message.splitlines()
+        _cprint('{bold}{}{reset}', _fill(first, initial_indent='* '))
+        for line in rest:
+            print(_fill(line, initial_indent='  '))
+
+    elif origin[0] == 'subprocess':
+        initial_indent = '> ' if origin[1] == 'cmd' else '< '
+        file = sys.stderr if origin[1] == 'stderr' else None
+        for line in message.splitlines():
+            _cprint('{dim}{}{reset}', _fill(line, initial_indent=initial_indent), file=file)
+
+
+def _setup_cli(*, verbosity: int) -> None:
     warnings.showwarning = _showwarning
 
     if platform.system() == 'Windows':
         try:
             import colorama
 
             colorama.init()
         except ModuleNotFoundError:
             pass
 
+    _init_colors()
+
+    _ctx.LOGGER.set(_log)
+    _ctx.VERBOSITY.set(verbosity)
+
 
 def _error(msg: str, code: int = 1) -> NoReturn:  # pragma: no cover
     """
     Print an error message and exit. Will color the output when writing to a TTY.
 
     :param msg: Error message
     :param code: Error code
     """
     _cprint('{red}ERROR{reset} {}', msg)
     raise SystemExit(code)
 
 
-class _ProjectBuilder(ProjectBuilder):
-    @staticmethod
-    def log(message: str) -> None:
-        _cprint('{bold}* {}{reset}', message)
-
-
-class _DefaultIsolatedEnv(DefaultIsolatedEnv):
-    @staticmethod
-    def log(message: str) -> None:
-        _cprint('{bold}* {}{reset}', message)
-
-
 def _format_dep_chain(dep_chain: Sequence[str]) -> str:
     return ' -> '.join(dep.partition(';')[0].strip() for dep in dep_chain)
 
 
 def _build_in_isolated_env(
-    srcdir: PathType, outdir: PathType, distribution: str, config_settings: ConfigSettingsType | None
+    srcdir: StrPath,
+    outdir: StrPath,
+    distribution: Distribution,
+    config_settings: ConfigSettings | None,
+    installer: _env.Installer,
 ) -> str:
-    with _DefaultIsolatedEnv() as env:
-        builder = _ProjectBuilder.from_isolated_env(env, srcdir)
+    with DefaultIsolatedEnv(installer=installer) as env:
+        builder = ProjectBuilder.from_isolated_env(env, srcdir)
         # first install the build dependencies
         env.install(builder.build_system_requires)
         # then get the extra required dependencies from the backend (which was installed in the call above :P)
         env.install(builder.get_requires_for_build(distribution, config_settings or {}))
         return builder.build(distribution, outdir, config_settings or {})
 
 
 def _build_in_current_env(
-    srcdir: PathType,
-    outdir: PathType,
-    distribution: str,
-    config_settings: ConfigSettingsType | None,
+    srcdir: StrPath,
+    outdir: StrPath,
+    distribution: Distribution,
+    config_settings: ConfigSettings | None,
     skip_dependency_check: bool = False,
 ) -> str:
-    builder = _ProjectBuilder(srcdir)
+    builder = ProjectBuilder(srcdir)
 
     if not skip_dependency_check:
         missing = builder.check_dependencies(distribution, config_settings or {})
         if missing:
             dependencies = ''.join('\n\t' + dep for deps in missing for dep in (deps[0], _format_dep_chain(deps[1:])) if dep)
             _cprint()
             _error(f'Missing dependencies:{dependencies}')
 
     return builder.build(distribution, outdir, config_settings or {})
 
 
 def _build(
     isolation: bool,
-    srcdir: PathType,
-    outdir: PathType,
-    distribution: str,
-    config_settings: ConfigSettingsType | None,
+    srcdir: StrPath,
+    outdir: StrPath,
+    distribution: Distribution,
+    config_settings: ConfigSettings | None,
     skip_dependency_check: bool,
+    installer: _env.Installer,
 ) -> str:
     if isolation:
-        return _build_in_isolated_env(srcdir, outdir, distribution, config_settings)
+        return _build_in_isolated_env(srcdir, outdir, distribution, config_settings, installer)
     else:
         return _build_in_current_env(srcdir, outdir, distribution, config_settings, skip_dependency_check)
 
 
 @contextlib.contextmanager
 def _handle_build_error() -> Iterator[None]:
     try:
@@ -168,14 +191,18 @@
                 limit=-1,
             )
             tb = ''.join(tb_lines)
         else:
             tb = traceback.format_exc(-1)
         _cprint('\n{dim}{}{reset}\n', tb.strip('\n'))
         _error(str(e))
+    except Exception as e:  # pragma: no cover
+        tb = traceback.format_exc().strip('\n')
+        _cprint('\n{dim}{}{reset}\n', tb)
+        _error(str(e))
 
 
 def _natural_language_list(elements: Sequence[str]) -> str:
     if len(elements) == 0:
         msg = 'no elements'
         raise IndexError(msg)
     elif len(elements) == 1:
@@ -184,111 +211,110 @@
         return '{} and {}'.format(
             ', '.join(elements[:-1]),
             elements[-1],
         )
 
 
 def build_package(
-    srcdir: PathType,
-    outdir: PathType,
-    distributions: Sequence[str],
-    config_settings: ConfigSettingsType | None = None,
+    srcdir: StrPath,
+    outdir: StrPath,
+    distributions: Sequence[Distribution],
+    config_settings: ConfigSettings | None = None,
     isolation: bool = True,
     skip_dependency_check: bool = False,
+    installer: _env.Installer = 'pip',
 ) -> Sequence[str]:
     """
     Run the build process.
 
     :param srcdir: Source directory
     :param outdir: Output directory
     :param distribution: Distribution to build (sdist or wheel)
     :param config_settings: Configuration settings to be passed to the backend
     :param isolation: Isolate the build in a separate environment
     :param skip_dependency_check: Do not perform the dependency check
     """
     built: list[str] = []
     for distribution in distributions:
-        out = _build(isolation, srcdir, outdir, distribution, config_settings, skip_dependency_check)
+        out = _build(isolation, srcdir, outdir, distribution, config_settings, skip_dependency_check, installer)
         built.append(os.path.basename(out))
     return built
 
 
 def build_package_via_sdist(
-    srcdir: PathType,
-    outdir: PathType,
-    distributions: Sequence[str],
-    config_settings: ConfigSettingsType | None = None,
+    srcdir: StrPath,
+    outdir: StrPath,
+    distributions: Sequence[Distribution],
+    config_settings: ConfigSettings | None = None,
     isolation: bool = True,
     skip_dependency_check: bool = False,
+    installer: _env.Installer = 'pip',
 ) -> Sequence[str]:
     """
     Build a sdist and then the specified distributions from it.
 
     :param srcdir: Source directory
     :param outdir: Output directory
     :param distribution: Distribution to build (only wheel)
     :param config_settings: Configuration settings to be passed to the backend
     :param isolation: Isolate the build in a separate environment
     :param skip_dependency_check: Do not perform the dependency check
     """
-    from ._util import TarFile
+    from ._compat import tarfile
 
     if 'sdist' in distributions:
         msg = 'Only binary distributions are allowed but sdist was specified'
         raise ValueError(msg)
 
-    sdist = _build(isolation, srcdir, outdir, 'sdist', config_settings, skip_dependency_check)
+    sdist = _build(isolation, srcdir, outdir, 'sdist', config_settings, skip_dependency_check, installer)
 
     sdist_name = os.path.basename(sdist)
     sdist_out = tempfile.mkdtemp(prefix='build-via-sdist-')
     built: list[str] = []
     if distributions:
         # extract sdist
-        with TarFile.open(sdist) as t:
+        with tarfile.TarFile.open(sdist) as t:
             t.extractall(sdist_out)
             try:
-                _ProjectBuilder.log(f'Building {_natural_language_list(distributions)} from sdist')
+                _ctx.log(f'Building {_natural_language_list(distributions)} from sdist')
                 srcdir = os.path.join(sdist_out, sdist_name[: -len('.tar.gz')])
                 for distribution in distributions:
-                    out = _build(isolation, srcdir, outdir, distribution, config_settings, skip_dependency_check)
+                    out = _build(isolation, srcdir, outdir, distribution, config_settings, skip_dependency_check, installer)
                     built.append(os.path.basename(out))
             finally:
                 shutil.rmtree(sdist_out, ignore_errors=True)
     return [sdist_name, *built]
 
 
 def main_parser() -> argparse.ArgumentParser:
     """
     Construct the main parser.
     """
     parser = argparse.ArgumentParser(
         description=textwrap.indent(
             textwrap.dedent(
-                '''
+                """
                 A simple, correct Python build frontend.
 
                 By default, a source distribution (sdist) is built from {srcdir}
                 and a binary distribution (wheel) is built from the sdist.
                 This is recommended as it will ensure the sdist can be used
                 to build wheels.
 
                 Pass -s/--sdist and/or -w/--wheel to build a specific distribution.
                 If you do this, the default behavior will be disabled, and all
                 artifacts will be built from {srcdir} (even if you combine
                 -w/--wheel with -s/--sdist, the wheel will be built from {srcdir}).
-                '''
+                """
             ).strip(),
             '    ',
         ),
-        formatter_class=partial(
-            argparse.RawDescriptionHelpFormatter,
-            # Prevent argparse from taking up the entire width of the terminal window
-            # which impedes readability.
-            width=min(shutil.get_terminal_size().columns - 2, 127),
-        ),
+        # Prevent argparse from taking up the entire width of the terminal window
+        # which impedes readability.
+        formatter_class=partial(argparse.RawDescriptionHelpFormatter, width=min(_max_terminal_width, 127)),
     )
     parser.add_argument(
         'srcdir',
         type=str,
         nargs='?',
         default=os.getcwd(),
         help='source directory (defaults to current directory)',
@@ -296,23 +322,35 @@
     parser.add_argument(
         '--version',
         '-V',
         action='version',
         version=f"build {build.__version__} ({','.join(build.__path__)})",
     )
     parser.add_argument(
+        '--verbose',
+        '-v',
+        dest='verbosity',
+        action='count',
+        default=0,
+        help='increase verbosity',
+    )
+    parser.add_argument(
         '--sdist',
         '-s',
-        action='store_true',
+        dest='distributions',
+        action='append_const',
+        const='sdist',
         help='build a source distribution (disables the default behavior)',
     )
     parser.add_argument(
         '--wheel',
         '-w',
-        action='store_true',
+        dest='distributions',
+        action='append_const',
+        const='wheel',
         help='build a wheel (disables the default behavior)',
     )
     parser.add_argument(
         '--outdir',
         '-o',
         type=str,
         help=f'output directory (defaults to {{srcdir}}{os.sep}dist)',
@@ -320,24 +358,31 @@
     )
     parser.add_argument(
         '--skip-dependency-check',
         '-x',
         action='store_true',
         help='do not check that build dependencies are installed',
     )
-    parser.add_argument(
+    env_group = parser.add_mutually_exclusive_group()
+    env_group.add_argument(
         '--no-isolation',
         '-n',
         action='store_true',
         help='disable building the project in an isolated virtual environment. '
         'Build dependencies must be installed separately when this option is used',
     )
+    env_group.add_argument(
+        '--installer',
+        choices=_env.INSTALLERS,
+        help='Python package installer to use (defaults to pip)',
+    )
     parser.add_argument(
         '--config-setting',
         '-C',
+        dest='config_settings',
         action='append',
         help='settings to pass to the backend.  Multiple settings can be provided. '
         'Settings beginning with a hyphen will erroneously be interpreted as options to build if separated '
         'by a space character; use ``--config-setting=--my-setting -C--my-other-setting``',
         metavar='KEY[=VALUE]',
     )
     return parser
@@ -346,60 +391,58 @@
 def main(cli_args: Sequence[str], prog: str | None = None) -> None:
     """
     Parse the CLI arguments and invoke the build process.
 
     :param cli_args: CLI arguments
     :param prog: Program name to show in help text
     """
-    _setup_cli()
     parser = main_parser()
     if prog:
         parser.prog = prog
     args = parser.parse_args(cli_args)
 
-    distributions = []
+    _setup_cli(verbosity=args.verbosity)
+
     config_settings = {}
 
-    if args.config_setting:
-        for arg in args.config_setting:
+    if args.config_settings:
+        for arg in args.config_settings:
             setting, _, value = arg.partition('=')
             if setting not in config_settings:
                 config_settings[setting] = value
             else:
                 if not isinstance(config_settings[setting], list):
                     config_settings[setting] = [config_settings[setting]]
 
                 config_settings[setting].append(value)
 
-    if args.sdist:
-        distributions.append('sdist')
-    if args.wheel:
-        distributions.append('wheel')
-
     # outdir is relative to srcdir only if omitted.
     outdir = os.path.join(args.srcdir, 'dist') if args.outdir is None else args.outdir
 
+    distributions: list[Distribution] = args.distributions
     if distributions:
         build_call = build_package
     else:
         build_call = build_package_via_sdist
         distributions = ['wheel']
-    try:
-        with _handle_build_error():
-            built = build_call(
-                args.srcdir, outdir, distributions, config_settings, not args.no_isolation, args.skip_dependency_check
-            )
-            artifact_list = _natural_language_list(
-                ['{underline}{}{reset}{bold}{green}'.format(artifact, **_STYLES) for artifact in built]
-            )
-            _cprint('{bold}{green}Successfully built {}{reset}', artifact_list)
-    except Exception as e:  # pragma: no cover
-        tb = traceback.format_exc().strip('\n')
-        _cprint('\n{dim}{}{reset}\n', tb)
-        _error(str(e))
+
+    with _handle_build_error():
+        built = build_call(
+            args.srcdir,
+            outdir,
+            distributions,
+            config_settings,
+            not args.no_isolation,
+            args.skip_dependency_check,
+            args.installer,
+        )
+        artifact_list = _natural_language_list(
+            ['{underline}{}{reset}{bold}{green}'.format(artifact, **_styles.get()) for artifact in built]
+        )
+        _cprint('{bold}{green}Successfully built {}{reset}', artifact_list)
 
 
 def entrypoint() -> None:
     main(sys.argv[1:])
 
 
 if __name__ == '__main__':  # pragma: no cover
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/build/_exceptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/build/_exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import subprocess
-import textwrap
 import types
 
 
 class BuildException(Exception):
     """
     Exception raised by :class:`build.ProjectBuilder`.
     """
@@ -16,16 +15,19 @@
     Exception raised when a backend operation fails.
     """
 
     def __init__(
         self,
         exception: Exception,
         description: str | None = None,
-        exc_info: tuple[type[BaseException], BaseException, types.TracebackType]
-        | tuple[None, None, None] = (None, None, None),
+        exc_info: tuple[type[BaseException], BaseException, types.TracebackType] | tuple[None, None, None] = (
+            None,
+            None,
+            None,
+        ),
     ) -> None:
         super().__init__()
         self.exception = exception
         self.exc_info = exc_info
         self._description = description
 
     def __str__(self) -> str:
@@ -50,21 +52,14 @@
 
     def __init__(self, exception: subprocess.CalledProcessError, description: str) -> None:
         super().__init__()
         self.exception = exception
         self._description = description
 
     def __str__(self) -> str:
-        cmd = ' '.join(self.exception.cmd)
-        description = f"{self._description}\n  Command '{cmd}' failed with return code {self.exception.returncode}"
-        for stream_name in ('stdout', 'stderr'):
-            stream = getattr(self.exception, stream_name)
-            if stream:
-                description += f'\n  {stream_name}:\n'
-                description += textwrap.indent(stream.decode(), '    ')
-        return description
+        return self._description
 
 
 class TypoWarning(Warning):
     """
     Warning raised when a possible typo is found.
     """
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/build/env.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,290 +1,330 @@
-from __future__ import annotations
-
-import abc
-import functools
-import importlib.util
-import logging
+import json
 import os
-import platform
-import shutil
-import subprocess
 import sys
-import sysconfig
 import tempfile
-import typing
-import warnings
+from contextlib import contextmanager
+from os.path import abspath
+from os.path import join as pjoin
+from subprocess import STDOUT, check_call, check_output
 
-from collections.abc import Collection, Mapping
+from ._in_process import _in_proc_script_path
 
-from ._exceptions import FailedProcessError
-from ._util import check_dependency
 
+def write_json(obj, path, **kwargs):
+    with open(path, 'w', encoding='utf-8') as f:
+        json.dump(obj, f, **kwargs)
 
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-elif typing.TYPE_CHECKING:
-    from typing_extensions import Protocol
-else:
-    Protocol = abc.ABC
 
+def read_json(path):
+    with open(path, encoding='utf-8') as f:
+        return json.load(f)
 
-_logger = logging.getLogger(__name__)
 
+class BackendUnavailable(Exception):
+    """Will be raised if the backend cannot be imported in the hook process."""
+    def __init__(self, traceback):
+        self.traceback = traceback
 
-class IsolatedEnv(Protocol):
-    """Isolated build environment ABC."""
 
-    @property
-    @abc.abstractmethod
-    def python_executable(self) -> str:
-        """The Python executable of the isolated environment."""
+class BackendInvalid(Exception):
+    """Will be raised if the backend is invalid."""
+    def __init__(self, backend_name, backend_path, message):
+        super().__init__(message)
+        self.backend_name = backend_name
+        self.backend_path = backend_path
 
-    @abc.abstractmethod
-    def make_extra_environ(self) -> Mapping[str, str] | None:
-        """Generate additional env vars specific to the isolated environment."""
 
+class HookMissing(Exception):
+    """Will be raised on missing hooks (if a fallback can't be used)."""
+    def __init__(self, hook_name):
+        super().__init__(hook_name)
+        self.hook_name = hook_name
 
-@functools.lru_cache(maxsize=None)
-def _should_use_virtualenv() -> bool:
-    import packaging.requirements
 
-    # virtualenv might be incompatible if it was installed separately
-    # from build. This verifies that virtualenv and all of its
-    # dependencies are installed as specified by build.
-    return importlib.util.find_spec('virtualenv') is not None and not any(
-        packaging.requirements.Requirement(d[1]).name == 'virtualenv'
-        for d in check_dependency('build[virtualenv]')
-        if len(d) > 1
-    )
+class UnsupportedOperation(Exception):
+    """May be raised by build_sdist if the backend indicates that it can't."""
+    def __init__(self, traceback):
+        self.traceback = traceback
 
 
-def _subprocess(cmd: list[str]) -> None:
-    """Invoke subprocess and output stdout and stderr if it fails."""
-    try:
-        subprocess.run(cmd, check=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-    except subprocess.CalledProcessError as e:
-        print(e.output.decode(), end='', file=sys.stderr)
-        raise
+def default_subprocess_runner(cmd, cwd=None, extra_environ=None):
+    """The default method of calling the wrapper subprocess.
 
+    This uses :func:`subprocess.check_call` under the hood.
+    """
+    env = os.environ.copy()
+    if extra_environ:
+        env.update(extra_environ)
 
-class DefaultIsolatedEnv(IsolatedEnv):
-    """An isolated environment which combines venv and virtualenv with pip."""
+    check_call(cmd, cwd=cwd, env=env)
 
-    def __enter__(self) -> DefaultIsolatedEnv:
-        try:
-            self._path = tempfile.mkdtemp(prefix='build-env-')
-            # use virtualenv when available (as it's faster than venv)
-            if _should_use_virtualenv():
-                self.log('Creating virtualenv isolated environment...')
-                self._python_executable, self._scripts_dir = _create_isolated_env_virtualenv(self._path)
-            else:
-                self.log('Creating venv isolated environment...')
-
-                # Call ``realpath`` to prevent spurious warning from being emitted
-                # that the venv location has changed on Windows. The username is
-                # DOS-encoded in the output of tempfile - the location is the same
-                # but the representation of it is different, which confuses venv.
-                # Ref: https://bugs.python.org/issue46171
-                self._path = os.path.realpath(tempfile.mkdtemp(prefix='build-env-'))
-                self._python_executable, self._scripts_dir = _create_isolated_env_venv(self._path)
-        except Exception:  # cleanup folder if creation fails
-            self.__exit__(*sys.exc_info())
-            raise
-
-        return self
-
-    def __exit__(self, *args: object) -> None:
-        if os.path.exists(self._path):  # in case the user already deleted skip remove
-            shutil.rmtree(self._path)
-
-    @property
-    def path(self) -> str:
-        """The location of the isolated build environment."""
-        return self._path
-
-    @property
-    def python_executable(self) -> str:
-        """The python executable of the isolated build environment."""
-        return self._python_executable
-
-    def make_extra_environ(self) -> dict[str, str]:
-        path = os.environ.get('PATH')
-        return {'PATH': os.pathsep.join([self._scripts_dir, path]) if path is not None else self._scripts_dir}
-
-    def install(self, requirements: Collection[str]) -> None:
-        """
-        Install packages from PEP 508 requirements in the isolated build environment.
-
-        :param requirements: PEP 508 requirement specification to install
-
-        :note: Passing non-PEP 508 strings will result in undefined behavior, you *should not* rely on it. It is
-               merely an implementation detail, it may change any time without warning.
-        """
-        if not requirements:
-            return
-
-        self.log(f'Installing packages in isolated environment... ({", ".join(sorted(requirements))})')
-
-        # pip does not honour environment markers in command line arguments
-        # but it does for requirements from a file
-        with tempfile.NamedTemporaryFile('w', prefix='build-reqs-', suffix='.txt', delete=False, encoding='utf-8') as req_file:
-            req_file.write(os.linesep.join(requirements))
-        try:
-            cmd = [
-                self.python_executable,
-                '-Im',
-                'pip',
-                'install',
-                '--use-pep517',
-                '--no-warn-script-location',
-                '-r',
-                os.path.abspath(req_file.name),
-            ]
-            _subprocess(cmd)
-        finally:
-            os.unlink(req_file.name)
 
-    @staticmethod
-    def log(message: str) -> None:
-        """
-        Prints message
+def quiet_subprocess_runner(cmd, cwd=None, extra_environ=None):
+    """Call the subprocess while suppressing output.
 
-        The default implementation uses the logging module but this function can be
-        overwritten by users to have a different implementation.
+    This uses :func:`subprocess.check_output` under the hood.
+    """
+    env = os.environ.copy()
+    if extra_environ:
+        env.update(extra_environ)
 
-        :param msg: Message to output
-        """
-        if sys.version_info >= (3, 8):
-            _logger.log(logging.INFO, message, stacklevel=2)
-        else:
-            _logger.log(logging.INFO, message)
+    check_output(cmd, cwd=cwd, env=env, stderr=STDOUT)
 
 
-def _create_isolated_env_virtualenv(path: str) -> tuple[str, str]:
+def norm_and_check(source_tree, requested):
+    """Normalise and check a backend path.
+
+    Ensure that the requested backend path is specified as a relative path,
+    and resolves to a location under the given source tree.
+
+    Return an absolute version of the requested path.
     """
-    We optionally can use the virtualenv package to provision a virtual environment.
+    if os.path.isabs(requested):
+        raise ValueError("paths must be relative")
+
+    abs_source = os.path.abspath(source_tree)
+    abs_requested = os.path.normpath(os.path.join(abs_source, requested))
+    # We have to use commonprefix for Python 2.7 compatibility. So we
+    # normalise case to avoid problems because commonprefix is a character
+    # based comparison :-(
+    norm_source = os.path.normcase(abs_source)
+    norm_requested = os.path.normcase(abs_requested)
+    if os.path.commonprefix([norm_source, norm_requested]) != norm_source:
+        raise ValueError("paths must be inside source tree")
+
+    return abs_requested
+
 
-    :param path: The path where to create the isolated build environment
-    :return: The Python executable and script folder
+class BuildBackendHookCaller:
+    """A wrapper to call the build backend hooks for a source directory.
     """
-    import virtualenv
 
-    cmd = [str(path), '--no-setuptools', '--no-wheel', '--activators', '']
-    result = virtualenv.cli_run(cmd, setup_logging=False)
-    executable = str(result.creator.exe)
-    script_dir = str(result.creator.script_dir)
-    return executable, script_dir
-
-
-@functools.lru_cache(maxsize=None)
-def _fs_supports_symlink() -> bool:
-    """Return True if symlinks are supported"""
-    # Using definition used by venv.main()
-    if not sys.platform.startswith('win'):
-        return True
-
-    # Windows may support symlinks (setting in Windows 10)
-    with tempfile.NamedTemporaryFile(prefix='build-symlink-') as tmp_file:
-        dest = f'{tmp_file}-b'
+    def __init__(
+            self,
+            source_dir,
+            build_backend,
+            backend_path=None,
+            runner=None,
+            python_executable=None,
+    ):
+        """
+        :param source_dir: The source directory to invoke the build backend for
+        :param build_backend: The build backend spec
+        :param backend_path: Additional path entries for the build backend spec
+        :param runner: The :ref:`subprocess runner <Subprocess Runners>` to use
+        :param python_executable:
+            The Python executable used to invoke the build backend
+        """
+        if runner is None:
+            runner = default_subprocess_runner
+
+        self.source_dir = abspath(source_dir)
+        self.build_backend = build_backend
+        if backend_path:
+            backend_path = [
+                norm_and_check(self.source_dir, p) for p in backend_path
+            ]
+        self.backend_path = backend_path
+        self._subprocess_runner = runner
+        if not python_executable:
+            python_executable = sys.executable
+        self.python_executable = python_executable
+
+    @contextmanager
+    def subprocess_runner(self, runner):
+        """A context manager for temporarily overriding the default
+        :ref:`subprocess runner <Subprocess Runners>`.
+
+        .. code-block:: python
+
+            hook_caller = BuildBackendHookCaller(...)
+            with hook_caller.subprocess_runner(quiet_subprocess_runner):
+                ...
+        """
+        prev = self._subprocess_runner
+        self._subprocess_runner = runner
         try:
-            os.symlink(tmp_file.name, dest)
-            os.unlink(dest)
-        except (OSError, NotImplementedError, AttributeError):
-            return False
-        return True
+            yield
+        finally:
+            self._subprocess_runner = prev
 
+    def _supported_features(self):
+        """Return the list of optional features supported by the backend."""
+        return self._call_hook('_supported_features', {})
 
-def _create_isolated_env_venv(path: str) -> tuple[str, str]:
-    """
-    On Python 3 we use the venv package from the standard library.
+    def get_requires_for_build_wheel(self, config_settings=None):
+        """Get additional dependencies required for building a wheel.
 
-    :param path: The path where to create the isolated build environment
-    :return: The Python executable and script folder
-    """
-    import venv
+        :returns: A list of :pep:`dependency specifiers <508>`.
+        :rtype: list[str]
 
-    import packaging.version
+        .. admonition:: Fallback
 
-    if sys.version_info < (3, 8):
-        import importlib_metadata as metadata
-    else:
-        from importlib import metadata
-
-    symlinks = _fs_supports_symlink()
-    try:
-        with warnings.catch_warnings():
-            if sys.version_info[:3] == (3, 11, 0):
-                warnings.filterwarnings('ignore', 'check_home argument is deprecated and ignored.', DeprecationWarning)
-            venv.EnvBuilder(with_pip=True, symlinks=symlinks).create(path)
-    except subprocess.CalledProcessError as exc:
-        raise FailedProcessError(exc, 'Failed to create venv. Maybe try installing virtualenv.') from None
-
-    executable, script_dir, purelib = _find_executable_and_scripts(path)
-
-    # Get the version of pip in the environment
-    pip_distribution = next(iter(metadata.distributions(name='pip', path=[purelib])))
-    current_pip_version = packaging.version.Version(pip_distribution.version)
-
-    if platform.system() == 'Darwin' and int(platform.mac_ver()[0].split('.')[0]) >= 11:
-        # macOS 11+ name scheme change requires 20.3. Intel macOS 11.0 can be told to report 10.16 for backwards
-        # compatibility; but that also fixes earlier versions of pip so this is only needed for 11+.
-        is_apple_silicon_python = platform.machine() != 'x86_64'
-        minimum_pip_version = '21.0.1' if is_apple_silicon_python else '20.3.0'
-    else:
-        # PEP-517 and manylinux1 was first implemented in 19.1
-        minimum_pip_version = '19.1.0'
-
-    if current_pip_version < packaging.version.Version(minimum_pip_version):
-        _subprocess([executable, '-m', 'pip', 'install', f'pip>={minimum_pip_version}'])
-
-    # Avoid the setuptools from ensurepip to break the isolation
-    _subprocess([executable, '-m', 'pip', 'uninstall', 'setuptools', '-y'])
-    return executable, script_dir
+            If the build backend does not defined a hook with this name, an
+            empty list will be returned.
+        """
+        return self._call_hook('get_requires_for_build_wheel', {
+            'config_settings': config_settings
+        })
+
+    def prepare_metadata_for_build_wheel(
+            self, metadata_directory, config_settings=None,
+            _allow_fallback=True):
+        """Prepare a ``*.dist-info`` folder with metadata for this project.
+
+        :returns: Name of the newly created subfolder within
+                  ``metadata_directory``, containing the metadata.
+        :rtype: str
+
+        .. admonition:: Fallback
+
+            If the build backend does not define a hook with this name and
+            ``_allow_fallback`` is truthy, the backend will be asked to build a
+            wheel via the ``build_wheel`` hook and the dist-info extracted from
+            that will be returned.
+        """
+        return self._call_hook('prepare_metadata_for_build_wheel', {
+            'metadata_directory': abspath(metadata_directory),
+            'config_settings': config_settings,
+            '_allow_fallback': _allow_fallback,
+        })
+
+    def build_wheel(
+            self, wheel_directory, config_settings=None,
+            metadata_directory=None):
+        """Build a wheel from this project.
+
+        :returns:
+            The name of the newly created wheel within ``wheel_directory``.
+
+        .. admonition:: Interaction with fallback
+
+            If the ``build_wheel`` hook was called in the fallback for
+            :meth:`prepare_metadata_for_build_wheel`, the build backend would
+            not be invoked. Instead, the previously built wheel will be copied
+            to ``wheel_directory`` and the name of that file will be returned.
+        """
+        if metadata_directory is not None:
+            metadata_directory = abspath(metadata_directory)
+        return self._call_hook('build_wheel', {
+            'wheel_directory': abspath(wheel_directory),
+            'config_settings': config_settings,
+            'metadata_directory': metadata_directory,
+        })
+
+    def get_requires_for_build_editable(self, config_settings=None):
+        """Get additional dependencies required for building an editable wheel.
 
+        :returns: A list of :pep:`dependency specifiers <508>`.
+        :rtype: list[str]
 
-def _find_executable_and_scripts(path: str) -> tuple[str, str, str]:
-    """
-    Detect the Python executable and script folder of a virtual environment.
+        .. admonition:: Fallback
 
-    :param path: The location of the virtual environment
-    :return: The Python executable, script folder, and purelib folder
-    """
-    config_vars = sysconfig.get_config_vars().copy()  # globally cached, copy before altering it
-    config_vars['base'] = path
-    scheme_names = sysconfig.get_scheme_names()
-    if 'venv' in scheme_names:
-        # Python distributors with custom default installation scheme can set a
-        # scheme that can't be used to expand the paths in a venv.
-        # This can happen if build itself is not installed in a venv.
-        # The distributors are encouraged to set a "venv" scheme to be used for this.
-        # See https://bugs.python.org/issue45413
-        # and https://github.com/pypa/virtualenv/issues/2208
-        paths = sysconfig.get_paths(scheme='venv', vars=config_vars)
-    elif 'posix_local' in scheme_names:
-        # The Python that ships on Debian/Ubuntu varies the default scheme to
-        # install to /usr/local
-        # But it does not (yet) set the "venv" scheme.
-        # If we're the Debian "posix_local" scheme is available, but "venv"
-        # is not, we use "posix_prefix" instead which is venv-compatible there.
-        paths = sysconfig.get_paths(scheme='posix_prefix', vars=config_vars)
-    elif 'osx_framework_library' in scheme_names:
-        # The Python that ships with the macOS developer tools varies the
-        # default scheme depending on whether the ``sys.prefix`` is part of a framework.
-        # But it does not (yet) set the "venv" scheme.
-        # If the Apple-custom "osx_framework_library" scheme is available but "venv"
-        # is not, we use "posix_prefix" instead which is venv-compatible there.
-        paths = sysconfig.get_paths(scheme='posix_prefix', vars=config_vars)
-    else:
-        paths = sysconfig.get_paths(vars=config_vars)
-    executable = os.path.join(paths['scripts'], 'python.exe' if sys.platform.startswith('win') else 'python')
-    if not os.path.exists(executable):
-        msg = f'Virtual environment creation failed, executable {executable} missing'
-        raise RuntimeError(msg)
-
-    return executable, paths['scripts'], paths['purelib']
-
-
-__all__ = [
-    'IsolatedEnv',
-    'DefaultIsolatedEnv',
-]
+            If the build backend does not defined a hook with this name, an
+            empty list will be returned.
+        """
+        return self._call_hook('get_requires_for_build_editable', {
+            'config_settings': config_settings
+        })
+
+    def prepare_metadata_for_build_editable(
+            self, metadata_directory, config_settings=None,
+            _allow_fallback=True):
+        """Prepare a ``*.dist-info`` folder with metadata for this project.
+
+        :returns: Name of the newly created subfolder within
+                  ``metadata_directory``, containing the metadata.
+        :rtype: str
+
+        .. admonition:: Fallback
+
+            If the build backend does not define a hook with this name and
+            ``_allow_fallback`` is truthy, the backend will be asked to build a
+            wheel via the ``build_editable`` hook and the dist-info
+            extracted from that will be returned.
+        """
+        return self._call_hook('prepare_metadata_for_build_editable', {
+            'metadata_directory': abspath(metadata_directory),
+            'config_settings': config_settings,
+            '_allow_fallback': _allow_fallback,
+        })
+
+    def build_editable(
+            self, wheel_directory, config_settings=None,
+            metadata_directory=None):
+        """Build an editable wheel from this project.
+
+        :returns:
+            The name of the newly created wheel within ``wheel_directory``.
+
+        .. admonition:: Interaction with fallback
+
+            If the ``build_editable`` hook was called in the fallback for
+            :meth:`prepare_metadata_for_build_editable`, the build backend
+            would not be invoked. Instead, the previously built wheel will be
+            copied to ``wheel_directory`` and the name of that file will be
+            returned.
+        """
+        if metadata_directory is not None:
+            metadata_directory = abspath(metadata_directory)
+        return self._call_hook('build_editable', {
+            'wheel_directory': abspath(wheel_directory),
+            'config_settings': config_settings,
+            'metadata_directory': metadata_directory,
+        })
+
+    def get_requires_for_build_sdist(self, config_settings=None):
+        """Get additional dependencies required for building an sdist.
+
+        :returns: A list of :pep:`dependency specifiers <508>`.
+        :rtype: list[str]
+        """
+        return self._call_hook('get_requires_for_build_sdist', {
+            'config_settings': config_settings
+        })
+
+    def build_sdist(self, sdist_directory, config_settings=None):
+        """Build an sdist from this project.
+
+        :returns:
+            The name of the newly created sdist within ``wheel_directory``.
+        """
+        return self._call_hook('build_sdist', {
+            'sdist_directory': abspath(sdist_directory),
+            'config_settings': config_settings,
+        })
+
+    def _call_hook(self, hook_name, kwargs):
+        extra_environ = {'PEP517_BUILD_BACKEND': self.build_backend}
+
+        if self.backend_path:
+            backend_path = os.pathsep.join(self.backend_path)
+            extra_environ['PEP517_BACKEND_PATH'] = backend_path
+
+        with tempfile.TemporaryDirectory() as td:
+            hook_input = {'kwargs': kwargs}
+            write_json(hook_input, pjoin(td, 'input.json'), indent=2)
+
+            # Run the hook in a subprocess
+            with _in_proc_script_path() as script:
+                python = self.python_executable
+                self._subprocess_runner(
+                    [python, abspath(str(script)), hook_name, td],
+                    cwd=self.source_dir,
+                    extra_environ=extra_environ
+                )
+
+            data = read_json(pjoin(td, 'output.json'))
+            if data.get('unsupported'):
+                raise UnsupportedOperation(data.get('traceback', ''))
+            if data.get('no_backend'):
+                raise BackendUnavailable(data.get('traceback', ''))
+            if data.get('backend_invalid'):
+                raise BackendInvalid(
+                    backend_name=self.build_backend,
+                    backend_path=self.backend_path,
+                    message=data.get('backend_error', '')
+                )
+            if data.get('hook_missing'):
+                raise HookMissing(data.get('missing_hook_name') or hook_name)
+            return data['return_val']
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/build/util.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/build/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 from __future__ import annotations
 
 import pathlib
 import tempfile
 
 import pyproject_hooks
 
-from . import PathType, ProjectBuilder, RunnerType
-from ._importlib import metadata
+from . import ProjectBuilder
+from ._compat import importlib
+from ._types import StrPath, SubprocessRunner
 from .env import DefaultIsolatedEnv
 
 
-def _project_wheel_metadata(builder: ProjectBuilder) -> metadata.PackageMetadata:
+def _project_wheel_metadata(builder: ProjectBuilder) -> importlib.metadata.PackageMetadata:
     with tempfile.TemporaryDirectory() as tmpdir:
         path = pathlib.Path(builder.metadata_path(tmpdir))
-        return metadata.PathDistribution(path).metadata
+        return importlib.metadata.PathDistribution(path).metadata
 
 
 def project_wheel_metadata(
-    source_dir: PathType,
+    source_dir: StrPath,
     isolated: bool = True,
     *,
-    runner: RunnerType = pyproject_hooks.quiet_subprocess_runner,
-) -> metadata.PackageMetadata:
+    runner: SubprocessRunner = pyproject_hooks.quiet_subprocess_runner,
+) -> importlib.metadata.PackageMetadata:
     """
     Return the wheel metadata for a project.
 
     Uses the ``prepare_metadata_for_build_wheel`` hook if available,
     otherwise ``build_wheel``.
 
     :param source_dir: Project source directory
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/LICENSE` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/build-1.0.3.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/build-1.2.1.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,76 @@
 Metadata-Version: 2.1
 Name: build
-Version: 1.0.3
+Version: 1.2.1
 Summary: A simple, correct Python build frontend
 Author-email: Filipe Laíns <lains@riseup.net>, Bernát Gábor <gaborjbernat@gmail.com>, layday <layday@protonmail.com>, Henry Schreiner <henryschreineriii@gmail.com>
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: packaging >= 19.0
+Requires-Dist: packaging >= 19.1
 Requires-Dist: pyproject_hooks
 Requires-Dist: colorama; os_name == "nt"
-Requires-Dist: importlib-metadata >= 4.6; python_version < "3.10"
+Requires-Dist: importlib-metadata >= 4.6; python_full_version < "3.10.2"
 Requires-Dist: tomli >= 1.1.0; python_version < "3.11"
 Requires-Dist: furo >= 2023.08.17 ; extra == "docs"
 Requires-Dist: sphinx ~= 7.0 ; extra == "docs"
 Requires-Dist: sphinx-argparse-cli >= 1.5 ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints >= 1.10 ; extra == "docs"
 Requires-Dist: sphinx-issues >= 3.0.0 ; extra == "docs"
+Requires-Dist: build[uv, virtualenv] ; extra == "test"
 Requires-Dist: filelock >= 3 ; extra == "test"
 Requires-Dist: pytest >= 6.2.4 ; extra == "test"
 Requires-Dist: pytest-cov >= 2.12 ; extra == "test"
 Requires-Dist: pytest-mock >= 2 ; extra == "test"
 Requires-Dist: pytest-rerunfailures >= 9.1 ; extra == "test"
 Requires-Dist: pytest-xdist >= 1.34 ; extra == "test"
 Requires-Dist: wheel >= 0.36.0 ; extra == "test"
 Requires-Dist: setuptools >= 42.0.0 ; extra == "test" and ( python_version < "3.10")
 Requires-Dist: setuptools >= 56.0.0 ; extra == "test" and ( python_version == "3.10")
 Requires-Dist: setuptools >= 56.0.0 ; extra == "test" and ( python_version == "3.11")
 Requires-Dist: setuptools >= 67.8.0 ; extra == "test" and ( python_version >= "3.12")
+Requires-Dist: build[uv] ; extra == "typing"
 Requires-Dist: importlib-metadata >= 5.1 ; extra == "typing"
-Requires-Dist: mypy ~= 1.5.0 ; extra == "typing"
+Requires-Dist: mypy ~= 1.9.0 ; extra == "typing"
 Requires-Dist: tomli ; extra == "typing"
 Requires-Dist: typing-extensions >= 3.7.4.3 ; extra == "typing"
+Requires-Dist: uv >= 0.1.18 ; extra == "uv"
 Requires-Dist: virtualenv >= 20.0.35 ; extra == "virtualenv"
-Project-URL: changelog, https://pypa-build.readthedocs.io/en/stable/changelog.html
-Project-URL: homepage, https://github.com/pypa/build
+Project-URL: changelog, https://build.pypa.io/en/stable/changelog.html
+Project-URL: homepage, https://build.pypa.io
+Project-URL: issues, https://github.com/pypa/build/issues
+Project-URL: source, https://github.com/pypa/build
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: typing
+Provides-Extra: uv
 Provides-Extra: virtualenv
 
 # build
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pypa/build/main.svg)](https://results.pre-commit.ci/latest/github/pypa/build/main)
 [![CI test](https://github.com/pypa/build/actions/workflows/test.yml/badge.svg)](https://github.com/pypa/build/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/pypa/build/branch/main/graph/badge.svg)](https://codecov.io/gh/pypa/build)
 
-[![Documentation Status](https://readthedocs.org/projects/pypa-build/badge/?version=latest)](https://pypa-build.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/pypa-build/badge/?version=latest)](https://build.pypa.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/build.svg)](https://pypi.org/project/build/)
 [![Discord](https://img.shields.io/discord/803025117553754132?label=Discord%20chat%20%23build)](https://discord.gg/pypa)
 
 A simple, correct Python build frontend.
 
-See the [documentation](https://pypa-build.readthedocs.io/en/latest/) for more information.
+See the [documentation](https://build.pypa.io) for more information.
 
 ### Installation
 
 `build` can be installed via `pip` or an equivalent via:
 
 ```console
 $ pip install build
@@ -75,15 +80,15 @@
 
 ```console
 $ python -m build
 ```
 
 This will build the package in an isolated environment, generating a
 source-distribution and wheel in the directory `dist/`.
-See the [documentation](https://pypa-build.readthedocs.io/en/latest/) for full information.
+See the [documentation](https://build.pypa.io) for full information.
 
 ### Code of Conduct
 
 Everyone interacting in the build's codebase, issue trackers, chat rooms, and mailing lists is expected to follow
 the [PSF Code of Conduct].
 
 [psf code of conduct]: https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi/cacert.pem` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi/core.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/LICENSE` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/RECORD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 certifi-2024.2.2.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
 certifi-2024.2.2.dist-info/LICENSE,sha256=6TcW2mucDVpKHfYP5pWzcPBpVgPSH2-D8FPkLPwQyvc,989
 certifi-2024.2.2.dist-info/METADATA,sha256=1noreLRChpOgeSj0uJT1mehiBl8ngh33Guc7KdvzYYM,2170
 certifi-2024.2.2.dist-info/RECORD,,
+certifi-2024.2.2.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 certifi-2024.2.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
 certifi-2024.2.2.dist-info/top_level.txt,sha256=KMu4vUCfsjLrkPbSNdgdekS-pVJzBAJFO__nI8NF6-U,8
 certifi/__init__.py,sha256=ljtEx-EmmPpTe2SOd5Kzsujm_lUD0fKJVnE9gzce320,94
 certifi/__main__.py,sha256=xBBoj905TUWBLRGANOcf7oi6e-3dMP4cEoG9OyMs11g,243
 certifi/__pycache__/__init__.cpython-312.pyc,,
 certifi/__pycache__/__main__.cpython-312.pyc,,
 certifi/__pycache__/core.cpython-312.pyc,,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/api.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/cd.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/constant.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/legacy.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/md.cpython-312-darwin.so` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/md.cpython-312-darwin.so`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/md.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/md__mypyc.cpython-312-darwin.so` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/md__mypyc.cpython-312-darwin.so`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/models.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer/cli/__main__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/RECORD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/charset_normalizer-3.3.2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-../../../bin/normalizer,sha256=ZUKkYNp2wlzzsc1UHNrX3umz-15qi1B-lJbZG9YsaxU,266
+../../../bin/normalizer,sha256=XzRNLqVvuoU9KWq6tJhDIx3Nq-bXn53kcgYkvZIC0o0,273
 charset_normalizer-3.3.2.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
 charset_normalizer-3.3.2.dist-info/LICENSE,sha256=6zGgxaT7Cbik4yBV0lweX5w1iidS_vPNcgIT0cz-4kE,1070
 charset_normalizer-3.3.2.dist-info/METADATA,sha256=cfLhl5A6SI-F0oclm8w8ux9wshL1nipdeCdVnYb4AaA,33550
 charset_normalizer-3.3.2.dist-info/RECORD,,
+charset_normalizer-3.3.2.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 charset_normalizer-3.3.2.dist-info/WHEEL,sha256=FCrbbeH_Uuw2ZMaB8nW-JE7XeUWVfF-XtWcVJYU0Zm8,110
 charset_normalizer-3.3.2.dist-info/entry_points.txt,sha256=ADSTKrkXZ3hhdOVFi6DcUEHQRS0xfxDIE_pEz4wLIXA,65
 charset_normalizer-3.3.2.dist-info/top_level.txt,sha256=7ASyzePr8_xuZWJsnqJjIBtyV8vhEo0wBCv1MPRRi3Q,19
 charset_normalizer/__init__.py,sha256=UzI3xC8PhmcLRMzSgPb6minTmRq0kWznnCBJ8ZCc2XI,1577
 charset_normalizer/__main__.py,sha256=JxY8bleaENOFlLRb9HfoeZCzAMnn2A1oGR5Xm2eyqg0,73
 charset_normalizer/__pycache__/__init__.cpython-312.pyc,,
 charset_normalizer/__pycache__/__main__.cpython-312.pyc,,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/franklinwh-0.0.1.dist-info/LICENSE` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/codec.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/core.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/idnadata.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/intranges.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna/uts46data.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna-3.6.dist-info/LICENSE.md` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/LICENSE.md`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna-3.6.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/idna-3.6.dist-info/RECORD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/idna-3.6.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 idna-3.6.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
 idna-3.6.dist-info/LICENSE.md,sha256=yy-vDKGMbTh-x8tm8yGTn7puZ-nawJ0xR3y52NP-aJk,1541
 idna-3.6.dist-info/METADATA,sha256=N93B509dkvvkd_Y0E_VxCHPkVkrD6InxoyfXvX4egds,9888
 idna-3.6.dist-info/RECORD,,
+idna-3.6.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 idna-3.6.dist-info/WHEEL,sha256=EZbGkh7Ie4PoZfRQ8I0ZuP9VklN_TvcZ6DSE5Uar4z4,81
 idna/__init__.py,sha256=KJQN1eQBr8iIK5SKrJ47lXvxG0BJ7Lm38W4zT0v_8lk,849
 idna/__pycache__/__init__.cpython-312.pyc,,
 idna/__pycache__/codec.cpython-312.pyc,,
 idna/__pycache__/compat.cpython-312.pyc,,
 idna/__pycache__/core.cpython-312.pyc,,
 idna/__pycache__/idnadata.cpython-312.pyc,,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_elffile.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_manylinux.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_manylinux.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,23 @@
 
 
 def _have_compatible_abi(executable: str, archs: Sequence[str]) -> bool:
     if "armv7l" in archs:
         return _is_linux_armhf(executable)
     if "i686" in archs:
         return _is_linux_i686(executable)
-    allowed_archs = {"x86_64", "aarch64", "ppc64", "ppc64le", "s390x", "loongarch64"}
+    allowed_archs = {
+        "x86_64",
+        "aarch64",
+        "ppc64",
+        "ppc64le",
+        "s390x",
+        "loongarch64",
+        "riscv64",
+    }
     return any(arch in allowed_archs for arch in archs)
 
 
 # If glibc ever changes its major version, we need to know what the last
 # minor version was, so we can build the complete list of all versions.
 # For now, guess what the highest minor version might be, assume it will
 # be 50 for testing. Once this actually happens, update the dictionary
@@ -78,15 +86,15 @@
     """
     # os.confstr is quite a bit faster than ctypes.DLL. It's also less likely
     # to be broken or missing. This strategy is used in the standard library
     # platform module.
     # https://github.com/python/cpython/blob/fcf1d003bf4f0100c/Lib/platform.py#L175-L183
     try:
         # Should be a string like "glibc 2.17".
-        version_string: str = getattr(os, "confstr")("CS_GNU_LIBC_VERSION")
+        version_string: Optional[str] = os.confstr("CS_GNU_LIBC_VERSION")
         assert version_string is not None
         _, version = version_string.rsplit()
     except (AssertionError, AttributeError, OSError, ValueError):
         # os.confstr() or CS_GNU_LIBC_VERSION not available (or a bad value)...
         return None
     return version
 
@@ -170,15 +178,15 @@
 # From PEP 513, PEP 600
 def _is_compatible(arch: str, version: _GLibCVersion) -> bool:
     sys_glibc = _get_glibc_version()
     if sys_glibc < version:
         return False
     # Check for presence of _manylinux module.
     try:
-        import _manylinux  # noqa
+        import _manylinux
     except ImportError:
         return True
     if hasattr(_manylinux, "manylinux_compatible"):
         result = _manylinux.manylinux_compatible(version[0], version[1], arch)
         if result is not None:
             return bool(result)
         return True
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_musllinux.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_parser.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,18 +320,15 @@
     else:
         tokenizer.raise_syntax_error(
             message="Expected a marker variable or quoted string"
         )
 
 
 def process_env_var(env_var: str) -> Variable:
-    if (
-        env_var == "platform_python_implementation"
-        or env_var == "python_implementation"
-    ):
+    if env_var in ("platform_python_implementation", "python_implementation"):
         return Variable("platform_python_implementation")
     else:
         return Variable(env_var)
 
 
 def process_python_str(python_str: str) -> Value:
     value = ast.literal_eval(python_str)
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_structures.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/_tokenizer.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/markers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/metadata.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 
             class TypedDict:
                 def __init_subclass__(*_args, **_kwargs):
                     pass
 
 
 try:
-    ExceptionGroup = __builtins__.ExceptionGroup  # type: ignore[attr-defined]
-except AttributeError:
+    ExceptionGroup
+except NameError:  # pragma: no cover
 
-    class ExceptionGroup(Exception):  # type: ignore[no-redef]  # noqa: N818
+    class ExceptionGroup(Exception):  # noqa: N818
         """A minimal implementation of :external:exc:`ExceptionGroup` from Python 3.11.
 
         If :external:exc:`ExceptionGroup` is already defined by Python itself,
         that version is used instead.
         """
 
         message: str
@@ -57,14 +57,17 @@
         def __init__(self, message: str, exceptions: List[Exception]) -> None:
             self.message = message
             self.exceptions = exceptions
 
         def __repr__(self) -> str:
             return f"{self.__class__.__name__}({self.message!r}, {self.exceptions!r})"
 
+else:  # pragma: no cover
+    ExceptionGroup = ExceptionGroup
+
 
 class InvalidMetadata(ValueError):
     """A metadata field contains invalid data."""
 
     field: str
     """The name of the field that contains invalid data."""
 
@@ -501,32 +504,27 @@
         self.raw_name = _RAW_TO_EMAIL_MAPPING[name]
 
     def __get__(self, instance: "Metadata", _owner: Type["Metadata"]) -> T:
         # With Python 3.8, the caching can be replaced with functools.cached_property().
         # No need to check the cache as attribute lookup will resolve into the
         # instance's __dict__ before __get__ is called.
         cache = instance.__dict__
-        try:
-            value = instance._raw[self.name]  # type: ignore[literal-required]
-        except KeyError:
-            if self.name in _STRING_FIELDS:
-                value = ""
-            elif self.name in _LIST_FIELDS:
-                value = []
-            elif self.name in _DICT_FIELDS:
-                value = {}
-            else:  # pragma: no cover
-                assert False
+        value = instance._raw.get(self.name)
 
-        try:
-            converter: Callable[[Any], T] = getattr(self, f"_process_{self.name}")
-        except AttributeError:
-            pass
-        else:
-            value = converter(value)
+        # To make the _process_* methods easier, we'll check if the value is None
+        # and if this field is NOT a required attribute, and if both of those
+        # things are true, we'll skip the the converter. This will mean that the
+        # converters never have to deal with the None union.
+        if self.name in _REQUIRED_ATTRS or value is not None:
+            try:
+                converter: Callable[[Any], T] = getattr(self, f"_process_{self.name}")
+            except AttributeError:
+                pass
+            else:
+                value = converter(value)
 
         cache[self.name] = value
         try:
             del instance._raw[self.name]  # type: ignore[misc]
         except KeyError:
             pass
 
@@ -673,15 +671,15 @@
         If *validate* is true, all metadata will be validated. All exceptions
         related to validation will be gathered and raised as an :class:`ExceptionGroup`.
         """
         ins = cls()
         ins._raw = data.copy()  # Mutations occur due to caching enriched values.
 
         if validate:
-            exceptions: List[InvalidMetadata] = []
+            exceptions: List[Exception] = []
             try:
                 metadata_version = ins.metadata_version
                 metadata_age = _VALID_METADATA_VERSIONS.index(metadata_version)
             except InvalidMetadata as metadata_version_exc:
                 exceptions.append(metadata_version_exc)
                 metadata_version = None
 
@@ -728,95 +726,100 @@
         cls, data: Union[bytes, str], *, validate: bool = True
     ) -> "Metadata":
         """Parse metadata from email headers.
 
         If *validate* is true, the metadata will be validated. All exceptions
         related to validation will be gathered and raised as an :class:`ExceptionGroup`.
         """
-        exceptions: list[InvalidMetadata] = []
         raw, unparsed = parse_email(data)
 
         if validate:
+            exceptions: list[Exception] = []
             for unparsed_key in unparsed:
                 if unparsed_key in _EMAIL_TO_RAW_MAPPING:
                     message = f"{unparsed_key!r} has invalid data"
                 else:
                     message = f"unrecognized field: {unparsed_key!r}"
                 exceptions.append(InvalidMetadata(unparsed_key, message))
 
             if exceptions:
                 raise ExceptionGroup("unparsed", exceptions)
 
         try:
             return cls.from_raw(raw, validate=validate)
         except ExceptionGroup as exc_group:
-            exceptions.extend(exc_group.exceptions)
-            raise ExceptionGroup("invalid or unparsed metadata", exceptions) from None
+            raise ExceptionGroup(
+                "invalid or unparsed metadata", exc_group.exceptions
+            ) from None
 
     metadata_version: _Validator[_MetadataVersion] = _Validator()
     """:external:ref:`core-metadata-metadata-version`
     (required; validated to be a valid metadata version)"""
     name: _Validator[str] = _Validator()
     """:external:ref:`core-metadata-name`
     (required; validated using :func:`~packaging.utils.canonicalize_name` and its
     *validate* parameter)"""
     version: _Validator[version_module.Version] = _Validator()
     """:external:ref:`core-metadata-version` (required)"""
-    dynamic: _Validator[List[str]] = _Validator(
+    dynamic: _Validator[Optional[List[str]]] = _Validator(
         added="2.2",
     )
     """:external:ref:`core-metadata-dynamic`
     (validated against core metadata field names and lowercased)"""
-    platforms: _Validator[List[str]] = _Validator()
+    platforms: _Validator[Optional[List[str]]] = _Validator()
     """:external:ref:`core-metadata-platform`"""
-    supported_platforms: _Validator[List[str]] = _Validator(added="1.1")
+    supported_platforms: _Validator[Optional[List[str]]] = _Validator(added="1.1")
     """:external:ref:`core-metadata-supported-platform`"""
-    summary: _Validator[str] = _Validator()
+    summary: _Validator[Optional[str]] = _Validator()
     """:external:ref:`core-metadata-summary` (validated to contain no newlines)"""
-    description: _Validator[str] = _Validator()  # TODO 2.1: can be in body
+    description: _Validator[Optional[str]] = _Validator()  # TODO 2.1: can be in body
     """:external:ref:`core-metadata-description`"""
-    description_content_type: _Validator[str] = _Validator(added="2.1")
+    description_content_type: _Validator[Optional[str]] = _Validator(added="2.1")
     """:external:ref:`core-metadata-description-content-type` (validated)"""
-    keywords: _Validator[List[str]] = _Validator()
+    keywords: _Validator[Optional[List[str]]] = _Validator()
     """:external:ref:`core-metadata-keywords`"""
-    home_page: _Validator[str] = _Validator()
+    home_page: _Validator[Optional[str]] = _Validator()
     """:external:ref:`core-metadata-home-page`"""
-    download_url: _Validator[str] = _Validator(added="1.1")
+    download_url: _Validator[Optional[str]] = _Validator(added="1.1")
     """:external:ref:`core-metadata-download-url`"""
-    author: _Validator[str] = _Validator()
+    author: _Validator[Optional[str]] = _Validator()
     """:external:ref:`core-metadata-author`"""
-    author_email: _Validator[str] = _Validator()
+    author_email: _Validator[Optional[str]] = _Validator()
     """:external:ref:`core-metadata-author-email`"""
-    maintainer: _Validator[str] = _Validator(added="1.2")
+    maintainer: _Validator[Optional[str]] = _Validator(added="1.2")
     """:external:ref:`core-metadata-maintainer`"""
-    maintainer_email: _Validator[str] = _Validator(added="1.2")
+    maintainer_email: _Validator[Optional[str]] = _Validator(added="1.2")
     """:external:ref:`core-metadata-maintainer-email`"""
-    license: _Validator[str] = _Validator()
+    license: _Validator[Optional[str]] = _Validator()
     """:external:ref:`core-metadata-license`"""
-    classifiers: _Validator[List[str]] = _Validator(added="1.1")
+    classifiers: _Validator[Optional[List[str]]] = _Validator(added="1.1")
     """:external:ref:`core-metadata-classifier`"""
-    requires_dist: _Validator[List[requirements.Requirement]] = _Validator(added="1.2")
+    requires_dist: _Validator[Optional[List[requirements.Requirement]]] = _Validator(
+        added="1.2"
+    )
     """:external:ref:`core-metadata-requires-dist`"""
-    requires_python: _Validator[specifiers.SpecifierSet] = _Validator(added="1.2")
+    requires_python: _Validator[Optional[specifiers.SpecifierSet]] = _Validator(
+        added="1.2"
+    )
     """:external:ref:`core-metadata-requires-python`"""
     # Because `Requires-External` allows for non-PEP 440 version specifiers, we
     # don't do any processing on the values.
-    requires_external: _Validator[List[str]] = _Validator(added="1.2")
+    requires_external: _Validator[Optional[List[str]]] = _Validator(added="1.2")
     """:external:ref:`core-metadata-requires-external`"""
-    project_urls: _Validator[Dict[str, str]] = _Validator(added="1.2")
+    project_urls: _Validator[Optional[Dict[str, str]]] = _Validator(added="1.2")
     """:external:ref:`core-metadata-project-url`"""
     # PEP 685 lets us raise an error if an extra doesn't pass `Name` validation
     # regardless of metadata version.
-    provides_extra: _Validator[List[utils.NormalizedName]] = _Validator(
+    provides_extra: _Validator[Optional[List[utils.NormalizedName]]] = _Validator(
         added="2.1",
     )
     """:external:ref:`core-metadata-provides-extra`"""
-    provides_dist: _Validator[List[str]] = _Validator(added="1.2")
+    provides_dist: _Validator[Optional[List[str]]] = _Validator(added="1.2")
     """:external:ref:`core-metadata-provides-dist`"""
-    obsoletes_dist: _Validator[List[str]] = _Validator(added="1.2")
+    obsoletes_dist: _Validator[Optional[List[str]]] = _Validator(added="1.2")
     """:external:ref:`core-metadata-obsoletes-dist`"""
-    requires: _Validator[List[str]] = _Validator(added="1.1")
+    requires: _Validator[Optional[List[str]]] = _Validator(added="1.1")
     """``Requires`` (deprecated)"""
-    provides: _Validator[List[str]] = _Validator(added="1.1")
+    provides: _Validator[Optional[List[str]]] = _Validator(added="1.1")
     """``Provides`` (deprecated)"""
-    obsoletes: _Validator[List[str]] = _Validator(added="1.1")
+    obsoletes: _Validator[Optional[List[str]]] = _Validator(added="1.1")
     """``Obsoletes`` (deprecated)"""
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/requirements.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/requirements.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         try:
             parsed = _parse_requirement(requirement_string)
         except ParserSyntaxError as e:
             raise InvalidRequirement(str(e)) from e
 
         self.name: str = parsed.name
         self.url: Optional[str] = parsed.url or None
-        self.extras: Set[str] = set(parsed.extras if parsed.extras else [])
+        self.extras: Set[str] = set(parsed.extras or [])
         self.specifier: SpecifierSet = SpecifierSet(parsed.specifier)
         self.marker: Optional[Marker] = None
         if parsed.marker is not None:
             self.marker = Marker.__new__(Marker)
             self.marker._markers = _normalize_extra_values(parsed.marker)
 
     def _iter_parts(self, name: str) -> Iterator[str]:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/specifiers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/specifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,15 @@
     from packaging.specifiers import Specifier, SpecifierSet, InvalidSpecifier
     from packaging.version import Version
 """
 
 import abc
 import itertools
 import re
-from typing import (
-    Callable,
-    Iterable,
-    Iterator,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from typing import Callable, Iterable, Iterator, List, Optional, Tuple, TypeVar, Union
 
 from .utils import canonicalize_version
 from .version import Version
 
 UnparsedVersion = Union[Version, str]
 UnparsedVersionVar = TypeVar("UnparsedVersionVar", bound=UnparsedVersion)
 CallableOperator = Callable[[Version, str], bool]
@@ -379,15 +369,15 @@
         # is that ~=2.2 is equivalent to >=2.2,==2.*. This allows us to
         # implement this in terms of the other specifiers instead of
         # implementing it ourselves. The only thing we need to do is construct
         # the other specifiers.
 
         # We want everything but the last item in the version, but we want to
         # ignore suffix segments.
-        prefix = ".".join(
+        prefix = _version_join(
             list(itertools.takewhile(_is_not_suffix, _version_split(spec)))[:-1]
         )
 
         # Add the prefix notation to the end of our string
         prefix += ".*"
 
         return self._get_operator(">=")(prospective, spec) and self._get_operator("==")(
@@ -400,21 +390,21 @@
         if spec.endswith(".*"):
             # In the case of prefix matching we want to ignore local segment.
             normalized_prospective = canonicalize_version(
                 prospective.public, strip_trailing_zero=False
             )
             # Get the normalized version string ignoring the trailing .*
             normalized_spec = canonicalize_version(spec[:-2], strip_trailing_zero=False)
-            # Split the spec out by dots, and pretend that there is an implicit
-            # dot in between a release segment and a pre-release segment.
+            # Split the spec out by bangs and dots, and pretend that there is
+            # an implicit dot in between a release segment and a pre-release segment.
             split_spec = _version_split(normalized_spec)
 
-            # Split the prospective version out by dots, and pretend that there
-            # is an implicit dot in between a release segment and a pre-release
-            # segment.
+            # Split the prospective version out by bangs and dots, and pretend
+            # that there is an implicit dot in between a release segment and
+            # a pre-release segment.
             split_prospective = _version_split(normalized_prospective)
 
             # 0-pad the prospective version before shortening it to get the correct
             # shortened version.
             padded_prospective, _ = _pad_version(split_prospective, split_spec)
 
             # Shorten the prospective version to be the same length as the spec
@@ -640,24 +630,46 @@
                 yield version
 
 
 _prefix_regex = re.compile(r"^([0-9]+)((?:a|b|c|rc)[0-9]+)$")
 
 
 def _version_split(version: str) -> List[str]:
+    """Split version into components.
+
+    The split components are intended for version comparison. The logic does
+    not attempt to retain the original version string, so joining the
+    components back with :func:`_version_join` may not produce the original
+    version string.
+    """
     result: List[str] = []
-    for item in version.split("."):
+
+    epoch, _, rest = version.rpartition("!")
+    result.append(epoch or "0")
+
+    for item in rest.split("."):
         match = _prefix_regex.search(item)
         if match:
             result.extend(match.groups())
         else:
             result.append(item)
     return result
 
 
+def _version_join(components: List[str]) -> str:
+    """Join split version components into a version string.
+
+    This function assumes the input came from :func:`_version_split`, where the
+    first component must be the epoch (either empty or numeric), and all other
+    components numeric.
+    """
+    epoch, *rest = components
+    return f"{epoch}!{'.'.join(rest)}"
+
+
 def _is_not_suffix(segment: str) -> bool:
     return not any(
         segment.startswith(prefix) for prefix in ("dev", "a", "b", "rc", "post")
     )
 
 
 def _pad_version(left: List[str], right: List[str]) -> Tuple[List[str], List[str]]:
@@ -671,15 +683,18 @@
     left_split.append(left[len(left_split[0]) :])
     right_split.append(right[len(right_split[0]) :])
 
     # Insert our padding
     left_split.insert(1, ["0"] * max(0, len(right_split[0]) - len(left_split[0])))
     right_split.insert(1, ["0"] * max(0, len(left_split[0]) - len(right_split[0])))
 
-    return (list(itertools.chain(*left_split)), list(itertools.chain(*right_split)))
+    return (
+        list(itertools.chain.from_iterable(left_split)),
+        list(itertools.chain.from_iterable(right_split)),
+    )
 
 
 class SpecifierSet(BaseSpecifier):
     """This class abstracts handling of a set of version specifiers.
 
     It can be passed a single specifier (``>=3.0``), a comma-separated list of
     specifiers (``>=3.0,!=3.1``), or no specifier at all.
@@ -703,22 +718,16 @@
             raised.
         """
 
         # Split on `,` to break each individual specifier into it's own item, and
         # strip each item to remove leading/trailing whitespace.
         split_specifiers = [s.strip() for s in specifiers.split(",") if s.strip()]
 
-        # Parsed each individual specifier, attempting first to make it a
-        # Specifier.
-        parsed: Set[Specifier] = set()
-        for specifier in split_specifiers:
-            parsed.add(Specifier(specifier))
-
-        # Turn our parsed specifiers into a frozen set and save them for later.
-        self._specs = frozenset(parsed)
+        # Make each individual specifier a Specifier and save in a frozen set for later.
+        self._specs = frozenset(map(Specifier, split_specifiers))
 
         # Store our prereleases value so we can use it later to determine if
         # we accept prereleases or not.
         self._prereleases = prereleases
 
     @property
     def prereleases(self) -> Optional[bool]:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/tags.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 import logging
 import platform
+import re
 import struct
 import subprocess
 import sys
 import sysconfig
 from importlib.machinery import EXTENSION_SUFFIXES
 from typing import (
     Dict,
@@ -120,56 +121,70 @@
     return value
 
 
 def _normalize_string(string: str) -> str:
     return string.replace(".", "_").replace("-", "_").replace(" ", "_")
 
 
-def _abi3_applies(python_version: PythonVersion) -> bool:
+def _is_threaded_cpython(abis: List[str]) -> bool:
+    """
+    Determine if the ABI corresponds to a threaded (`--disable-gil`) build.
+
+    The threaded builds are indicated by a "t" in the abiflags.
+    """
+    if len(abis) == 0:
+        return False
+    # expect e.g., cp313
+    m = re.match(r"cp\d+(.*)", abis[0])
+    if not m:
+        return False
+    abiflags = m.group(1)
+    return "t" in abiflags
+
+
+def _abi3_applies(python_version: PythonVersion, threading: bool) -> bool:
     """
     Determine if the Python version supports abi3.
 
-    PEP 384 was first implemented in Python 3.2.
+    PEP 384 was first implemented in Python 3.2. The threaded (`--disable-gil`)
+    builds do not support abi3.
     """
-    return len(python_version) > 1 and tuple(python_version) >= (3, 2)
+    return len(python_version) > 1 and tuple(python_version) >= (3, 2) and not threading
 
 
 def _cpython_abis(py_version: PythonVersion, warn: bool = False) -> List[str]:
     py_version = tuple(py_version)  # To allow for version comparison.
     abis = []
     version = _version_nodot(py_version[:2])
-    debug = pymalloc = ucs4 = ""
+    threading = debug = pymalloc = ucs4 = ""
     with_debug = _get_config_var("Py_DEBUG", warn)
     has_refcount = hasattr(sys, "gettotalrefcount")
     # Windows doesn't set Py_DEBUG, so checking for support of debug-compiled
     # extension modules is the best option.
     # https://github.com/pypa/pip/issues/3383#issuecomment-173267692
     has_ext = "_d.pyd" in EXTENSION_SUFFIXES
     if with_debug or (with_debug is None and (has_refcount or has_ext)):
         debug = "d"
+    if py_version >= (3, 13) and _get_config_var("Py_GIL_DISABLED", warn):
+        threading = "t"
     if py_version < (3, 8):
         with_pymalloc = _get_config_var("WITH_PYMALLOC", warn)
         if with_pymalloc or with_pymalloc is None:
             pymalloc = "m"
         if py_version < (3, 3):
             unicode_size = _get_config_var("Py_UNICODE_SIZE", warn)
             if unicode_size == 4 or (
                 unicode_size is None and sys.maxunicode == 0x10FFFF
             ):
                 ucs4 = "u"
     elif debug:
         # Debug builds can also load "normal" extension modules.
         # We can also assume no UCS-4 or pymalloc requirement.
-        abis.append(f"cp{version}")
-    abis.insert(
-        0,
-        "cp{version}{debug}{pymalloc}{ucs4}".format(
-            version=version, debug=debug, pymalloc=pymalloc, ucs4=ucs4
-        ),
-    )
+        abis.append(f"cp{version}{threading}")
+    abis.insert(0, f"cp{version}{threading}{debug}{pymalloc}{ucs4}")
     return abis
 
 
 def cpython_tags(
     python_version: Optional[PythonVersion] = None,
     abis: Optional[Iterable[str]] = None,
     platforms: Optional[Iterable[str]] = None,
@@ -209,19 +224,22 @@
         except ValueError:
             pass
 
     platforms = list(platforms or platform_tags())
     for abi in abis:
         for platform_ in platforms:
             yield Tag(interpreter, abi, platform_)
-    if _abi3_applies(python_version):
+
+    threading = _is_threaded_cpython(abis)
+    use_abi3 = _abi3_applies(python_version, threading)
+    if use_abi3:
         yield from (Tag(interpreter, "abi3", platform_) for platform_ in platforms)
     yield from (Tag(interpreter, "none", platform_) for platform_ in platforms)
 
-    if _abi3_applies(python_version):
+    if use_abi3:
         for minor_version in range(python_version[1] - 1, 1, -1):
             for platform_ in platforms:
                 interpreter = "cp{version}".format(
                     version=_version_nodot((python_version[0], minor_version))
                 )
                 yield Tag(interpreter, "abi3", platform_)
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging/version.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging/version.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/LICENSE.APACHE` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/LICENSE.BSD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging
-Version: 23.2
+Version: 24.0
 Summary: Core utilities for Python packages
 Author-email: Donald Stufft <donald@stufft.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/packaging-23.2.dist-info/RECORD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/packaging-24.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-packaging-23.2.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
-packaging-23.2.dist-info/LICENSE,sha256=ytHvW9NA1z4HS6YU0m996spceUDD2MNIUuZcSQlobEg,197
-packaging-23.2.dist-info/LICENSE.APACHE,sha256=DVQuDIgE45qn836wDaWnYhSdxoLXgpRRKH4RuTjpRZQ,10174
-packaging-23.2.dist-info/LICENSE.BSD,sha256=tw5-m3QvHMb5SLNMFqo5_-zpQZY2S8iP8NIYDwAo-sU,1344
-packaging-23.2.dist-info/METADATA,sha256=s1dJQ86EjZBul_UCkQNGdHcbLts6Zg4_mxCqk60X6xs,3203
-packaging-23.2.dist-info/RECORD,,
-packaging-23.2.dist-info/WHEEL,sha256=EZbGkh7Ie4PoZfRQ8I0ZuP9VklN_TvcZ6DSE5Uar4z4,81
-packaging/__init__.py,sha256=EhCMuCSz60IgQJ93b_4wJyAoHpU9J-uddG4QaMT0Pu4,496
+packaging-24.0.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
+packaging-24.0.dist-info/LICENSE,sha256=ytHvW9NA1z4HS6YU0m996spceUDD2MNIUuZcSQlobEg,197
+packaging-24.0.dist-info/LICENSE.APACHE,sha256=DVQuDIgE45qn836wDaWnYhSdxoLXgpRRKH4RuTjpRZQ,10174
+packaging-24.0.dist-info/LICENSE.BSD,sha256=tw5-m3QvHMb5SLNMFqo5_-zpQZY2S8iP8NIYDwAo-sU,1344
+packaging-24.0.dist-info/METADATA,sha256=0dESdhY_wHValuOrbgdebiEw04EbX4dkujlxPdEsFus,3203
+packaging-24.0.dist-info/RECORD,,
+packaging-24.0.dist-info/WHEEL,sha256=EZbGkh7Ie4PoZfRQ8I0ZuP9VklN_TvcZ6DSE5Uar4z4,81
+packaging/__init__.py,sha256=UzotcV07p8vcJzd80S-W0srhgY8NMVD_XvJcZ7JN-tA,496
 packaging/__pycache__/__init__.cpython-312.pyc,,
 packaging/__pycache__/_elffile.cpython-312.pyc,,
 packaging/__pycache__/_manylinux.cpython-312.pyc,,
 packaging/__pycache__/_musllinux.cpython-312.pyc,,
 packaging/__pycache__/_parser.cpython-312.pyc,,
 packaging/__pycache__/_structures.cpython-312.pyc,,
 packaging/__pycache__/_tokenizer.cpython-312.pyc,,
@@ -17,20 +17,20 @@
 packaging/__pycache__/metadata.cpython-312.pyc,,
 packaging/__pycache__/requirements.cpython-312.pyc,,
 packaging/__pycache__/specifiers.cpython-312.pyc,,
 packaging/__pycache__/tags.cpython-312.pyc,,
 packaging/__pycache__/utils.cpython-312.pyc,,
 packaging/__pycache__/version.cpython-312.pyc,,
 packaging/_elffile.py,sha256=hbmK8OD6Z7fY6hwinHEUcD1by7czkGiNYu7ShnFEk2k,3266
-packaging/_manylinux.py,sha256=Rq6ppXAxH8XFtNf6tC-B-1SKuvCODPBvcCoSulMtbtk,9526
+packaging/_manylinux.py,sha256=1ng_TqyH49hY6s3W_zVHyoJIaogbJqbIF1jJ0fAehc4,9590
 packaging/_musllinux.py,sha256=kgmBGLFybpy8609-KTvzmt2zChCPWYvhp5BWP4JX7dE,2676
-packaging/_parser.py,sha256=5DhK_zYJE4U4yzSkgEBT4F7tT2xZ6Pkx4gSRKyvXneQ,10382
+packaging/_parser.py,sha256=zlsFB1FpMRjkUdQb6WLq7xON52ruQadxFpYsDXWhLb4,10347
 packaging/_structures.py,sha256=q3eVNmbWJGG_S0Dit_S3Ao8qQqz_5PYTXFAKBZe5yr4,1431
 packaging/_tokenizer.py,sha256=alCtbwXhOFAmFGZ6BQ-wCTSFoRAJ2z-ysIf7__MTJ_k,5292
 packaging/markers.py,sha256=eH-txS2zq1HdNpTd9LcZUcVIwewAiNU0grmq5wjKnOk,8208
-packaging/metadata.py,sha256=ToxjINOmSn8mbEeXRSVNMidEJsPUYHEYFnnN4MaqvH0,32750
+packaging/metadata.py,sha256=w7jPEg6mDf1FTZMn79aFxFuk4SKtynUJtxr2InTxlV4,33036
 packaging/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-packaging/requirements.py,sha256=wswG4mXHSgE9w4NjNnlSvgLGo6yYvfHVEFnWhuEmXxg,2952
-packaging/specifiers.py,sha256=ZOpqL_w_Kj6ZF_OWdliQUzhEyHlDbi6989kr-sF5GHs,39206
-packaging/tags.py,sha256=pkG6gQ28RlhS09VzymVhVpGrWF5doHXfK1VxG9cdhoY,18355
+packaging/requirements.py,sha256=dgoBeVprPu2YE6Q8nGfwOPTjATHbRa_ZGLyXhFEln6Q,2933
+packaging/specifiers.py,sha256=dB2DwbmvSbEuVilEyiIQ382YfW5JfwzXTfRRPVtaENY,39784
+packaging/tags.py,sha256=fedHXiOHkBxNZTXotXv8uXPmMFU9ae-TKBujgYHigcA,18950
 packaging/utils.py,sha256=XgdmP3yx9-wQEFjO7OvMj9RjEf5JlR5HFFR69v7SQ9E,5268
 packaging/version.py,sha256=XjRBLNK17UMDgLeP8UHnqwiY3TdSi03xFQURtec211A,16236
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/__main__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/__pip-runner__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/build_env.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cache.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/configuration.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     return name
 
 
 def _disassemble_key(name: str) -> List[str]:
     if "." not in name:
         error_message = (
             "Key does not contain dot separated section and key. "
-            "Perhaps you wanted to use 'global.{}' instead?"
-        ).format(name)
+            f"Perhaps you wanted to use 'global.{name}' instead?"
+        )
         raise ConfigurationError(error_message)
     return name.split(".", 1)
 
 
 def get_configuration_files() -> Dict[Kind, List[str]]:
     global_config_files = [
         os.path.join(path, CONFIG_BASENAME) for path in appdirs.site_config_dirs("pip")
@@ -323,41 +323,43 @@
                 if name not in ENV_NAMES_IGNORED:
                     yield name, val
 
     # XXX: This is patched in the tests.
     def iter_config_files(self) -> Iterable[Tuple[Kind, List[str]]]:
         """Yields variant and configuration files associated with it.
 
-        This should be treated like items of a dictionary.
+        This should be treated like items of a dictionary. The order
+        here doesn't affect what gets overridden. That is controlled
+        by OVERRIDE_ORDER. However this does control the order they are
+        displayed to the user. It's probably most ergononmic to display
+        things in the same order as OVERRIDE_ORDER
         """
         # SMELL: Move the conditions out of this function
 
-        # environment variables have the lowest priority
-        config_file = os.environ.get("PIP_CONFIG_FILE", None)
-        if config_file is not None:
-            yield kinds.ENV, [config_file]
-        else:
-            yield kinds.ENV, []
-
+        env_config_file = os.environ.get("PIP_CONFIG_FILE", None)
         config_files = get_configuration_files()
 
-        # at the base we have any global configuration
         yield kinds.GLOBAL, config_files[kinds.GLOBAL]
 
-        # per-user configuration next
+        # per-user config is not loaded when env_config_file exists
         should_load_user_config = not self.isolated and not (
-            config_file and os.path.exists(config_file)
+            env_config_file and os.path.exists(env_config_file)
         )
         if should_load_user_config:
             # The legacy config file is overridden by the new config file
             yield kinds.USER, config_files[kinds.USER]
 
-        # finally virtualenv configuration first trumping others
+        # virtualenv config
         yield kinds.SITE, config_files[kinds.SITE]
 
+        if env_config_file is not None:
+            yield kinds.ENV, [env_config_file]
+        else:
+            yield kinds.ENV, []
+
     def get_values_in_config(self, variant: Kind) -> Dict[str, Any]:
         """Get values present in a config file"""
         return self._config[variant]
 
     def _get_parser_to_modify(self) -> Tuple[str, RawConfigParser]:
         # Determine which parser to modify
         assert self.load_only
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/exceptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,18 +243,15 @@
         """
         self.dist = dist
         self.metadata_name = metadata_name
 
     def __str__(self) -> str:
         # Use `dist` in the error message because its stringification
         # includes more information, like the version and location.
-        return "None {} metadata found for distribution: {}".format(
-            self.metadata_name,
-            self.dist,
-        )
+        return f"None {self.metadata_name} metadata found for distribution: {self.dist}"
 
 
 class UserInstallationInvalid(InstallationError):
     """A --user install is requested on an environment without user site."""
 
     def __str__(self) -> str:
         return "User base directory is not specified"
@@ -590,15 +587,15 @@
         :param gots: A dict of algorithm names pointing to hashes we
             actually got from the files under suspicion
         """
         self.allowed = allowed
         self.gots = gots
 
     def body(self) -> str:
-        return "    {}:\n{}".format(self._requirement_name(), self._hash_comparison())
+        return f"    {self._requirement_name()}:\n{self._hash_comparison()}"
 
     def _hash_comparison(self) -> str:
         """
         Return a comparison of actual and expected hash values.
 
         Example::
 
@@ -612,19 +609,17 @@
             # For now, all the decent hashes have 6-char names, so we can get
             # away with hard-coding space literals.
             return chain([hash_name], repeat("    or"))
 
         lines: List[str] = []
         for hash_name, expecteds in self.allowed.items():
             prefix = hash_then_or(hash_name)
-            lines.extend(
-                ("        Expected {} {}".format(next(prefix), e)) for e in expecteds
-            )
+            lines.extend((f"        Expected {next(prefix)} {e}") for e in expecteds)
             lines.append(
-                "             Got        {}\n".format(self.gots[hash_name].hexdigest())
+                f"             Got        {self.gots[hash_name].hexdigest()}\n"
             )
         return "\n".join(lines)
 
 
 class UnsupportedPythonVersion(InstallationError):
     """Unsupported python version according to Requires-Python package
     metadata."""
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/pyproject.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/pyproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         # explicitly via --use-pep517.
         # In the absence of any explicit backend specification, we
         # assume the setuptools backend that most closely emulates the
         # traditional direct setup.py execution, and require wheel and
         # a version of setuptools that supports that backend.
 
         build_system = {
-            "requires": ["setuptools>=40.8.0", "wheel"],
+            "requires": ["setuptools>=40.8.0"],
             "build-backend": "setuptools.build_meta:__legacy__",
         }
 
     # If we're using PEP 517, we have build system information (either
     # from pyproject.toml, or defaulted by the code above).
     # Note that at this point, we do not know if the user has actually
     # specified a backend, though.
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/self_outdated_check.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/wheel_builder.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/wheel_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,36 +136,35 @@
 
 
 def _verify_one(req: InstallRequirement, wheel_path: str) -> None:
     canonical_name = canonicalize_name(req.name or "")
     w = Wheel(os.path.basename(wheel_path))
     if canonicalize_name(w.name) != canonical_name:
         raise InvalidWheelFilename(
-            "Wheel has unexpected file name: expected {!r}, "
-            "got {!r}".format(canonical_name, w.name),
+            f"Wheel has unexpected file name: expected {canonical_name!r}, "
+            f"got {w.name!r}",
         )
     dist = get_wheel_distribution(FilesystemWheel(wheel_path), canonical_name)
     dist_verstr = str(dist.version)
     if canonicalize_version(dist_verstr) != canonicalize_version(w.version):
         raise InvalidWheelFilename(
-            "Wheel has unexpected file name: expected {!r}, "
-            "got {!r}".format(dist_verstr, w.version),
+            f"Wheel has unexpected file name: expected {dist_verstr!r}, "
+            f"got {w.version!r}",
         )
     metadata_version_value = dist.metadata_version
     if metadata_version_value is None:
         raise UnsupportedWheel("Missing Metadata-Version")
     try:
         metadata_version = Version(metadata_version_value)
     except InvalidVersion:
         msg = f"Invalid Metadata-Version: {metadata_version_value}"
         raise UnsupportedWheel(msg)
     if metadata_version >= Version("1.2") and not isinstance(dist.version, Version):
         raise UnsupportedWheel(
-            "Metadata 1.2 mandates PEP 440 version, "
-            "but {!r} is not".format(dist_verstr)
+            f"Metadata 1.2 mandates PEP 440 version, but {dist_verstr!r} is not"
         )
 
 
 def _build_one(
     req: InstallRequirement,
     output_dir: str,
     verify: bool,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/autocompletion.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/base_command.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/cmdoptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,18 +578,15 @@
     option: Option, opt_str: str, value: str, parser: OptionParser
 ) -> None:
     """
     Handle a provided --python-version value.
     """
     version_info, error_msg = _convert_python_version(value)
     if error_msg is not None:
-        msg = "invalid --python-version value: {!r}: {}".format(
-            value,
-            error_msg,
-        )
+        msg = f"invalid --python-version value: {value!r}: {error_msg}"
         raise_option_error(parser, option=option, msg=msg)
 
     parser.values.python_version = version_info
 
 
 python_version: Callable[..., Option] = partial(
     Option,
@@ -917,17 +914,17 @@
     pointed to in a dict by the algo name."""
     if not parser.values.hashes:
         parser.values.hashes = {}
     try:
         algo, digest = value.split(":", 1)
     except ValueError:
         parser.error(
-            "Arguments to {} must be a hash name "
+            f"Arguments to {opt_str} must be a hash name "
             "followed by a value, like --hash=sha256:"
-            "abcde...".format(opt_str)
+            "abcde..."
         )
     if algo not in STRONG_HASHES:
         parser.error(
             "Allowed hash algorithms for {} are {}.".format(
                 opt_str, ", ".join(STRONG_HASHES)
             )
         )
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/command_context.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/main.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/main_parser.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/parser.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,29 +225,29 @@
             assert option.dest is not None
 
             if option.action in ("store_true", "store_false"):
                 try:
                     val = strtobool(val)
                 except ValueError:
                     self.error(
-                        "{} is not a valid value for {} option, "
+                        f"{val} is not a valid value for {key} option, "
                         "please specify a boolean value like yes/no, "
-                        "true/false or 1/0 instead.".format(val, key)
+                        "true/false or 1/0 instead."
                     )
             elif option.action == "count":
                 with suppress(ValueError):
                     val = strtobool(val)
                 with suppress(ValueError):
                     val = int(val)
                 if not isinstance(val, int) or val < 0:
                     self.error(
-                        "{} is not a valid value for {} option, "
+                        f"{val} is not a valid value for {key} option, "
                         "please instead specify either a non-negative integer "
                         "or a boolean value like yes/no or false/true "
-                        "which is equivalent to 1/0.".format(val, key)
+                        "which is equivalent to 1/0."
                     )
             elif option.action == "append":
                 val = val.split()
                 val = [self.check_default(option, key, v) for v in val]
             elif option.action == "callback":
                 assert option.callback is not None
                 late_eval.add(option.dest)
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/progress_bars.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/req_command.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/cli/spinners.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/cache.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
         no_matching_msg = "No matching packages"
         if args[0] == "*":
             # Only fetch http files if no specific pattern given
             files += self._find_http_files(options)
         else:
             # Add the pattern to the log message
-            no_matching_msg += ' for pattern "{}"'.format(args[0])
+            no_matching_msg += f' for pattern "{args[0]}"'
 
         if not files:
             logger.warning(no_matching_msg)
 
         for filename in files:
             os.unlink(filename)
             logger.verbose("Removed %s", filename)
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/check.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/completion.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/configuration.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,25 +238,23 @@
         try:
             subprocess.check_call(f'{editor} "{fname}"', shell=True)
         except FileNotFoundError as e:
             if not e.filename:
                 e.filename = editor
             raise
         except subprocess.CalledProcessError as e:
-            raise PipError(
-                "Editor Subprocess exited with exit code {}".format(e.returncode)
-            )
+            raise PipError(f"Editor Subprocess exited with exit code {e.returncode}")
 
     def _get_n_args(self, args: List[str], example: str, n: int) -> Any:
         """Helper to make sure the command got the right number of arguments"""
         if len(args) != n:
             msg = (
-                "Got unexpected number of arguments, expected {}. "
-                '(example: "{} config {}")'
-            ).format(n, get_prog(), example)
+                f"Got unexpected number of arguments, expected {n}. "
+                f'(example: "{get_prog()} config {example}")'
+            )
             raise PipError(msg)
 
         if n == 1:
             return args[0]
         else:
             return args
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/debug.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 " (Unable to locate actual module version, using"
                 " vendor.txt specified version)"
             )
             actual_version = expected_version
         elif parse_version(actual_version) != parse_version(expected_version):
             extra_message = (
                 " (CONFLICT: vendor.txt suggests version should"
-                " be {})".format(expected_version)
+                f" be {expected_version})"
             )
         logger.info("%s==%s%s", module_name, actual_version, extra_message)
 
 
 def show_vendor_versions() -> None:
     logger.info("vendored library versions:")
 
@@ -116,31 +116,29 @@
 
     # Display the target options that were explicitly provided.
     formatted_target = target_python.format_given()
     suffix = ""
     if formatted_target:
         suffix = f" (target: {formatted_target})"
 
-    msg = "Compatible tags: {}{}".format(len(tags), suffix)
+    msg = f"Compatible tags: {len(tags)}{suffix}"
     logger.info(msg)
 
     if options.verbose < 1 and len(tags) > tag_limit:
         tags_limited = True
         tags = tags[:tag_limit]
     else:
         tags_limited = False
 
     with indent_log():
         for tag in tags:
             logger.info(str(tag))
 
         if tags_limited:
-            msg = (
-                "...\n[First {tag_limit} tags shown. Pass --verbose to show all.]"
-            ).format(tag_limit=tag_limit)
+            msg = f"...\n[First {tag_limit} tags shown. Pass --verbose to show all.]"
             logger.info(msg)
 
 
 def ca_bundle_info(config: Configuration) -> str:
     levels = {key.split(".", 1)[0] for key, _ in config.items()}
     if not levels:
         return "Not specified"
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/download.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/freeze.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/hash.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/help.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/index.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,16 +124,16 @@
                 versions = (
                     version for version in versions if not version.is_prerelease
                 )
             versions = set(versions)
 
             if not versions:
                 raise DistributionNotFound(
-                    "No matching distribution found for {}".format(query)
+                    f"No matching distribution found for {query}"
                 )
 
             formatted_versions = [str(ver) for ver in sorted(versions, reverse=True)]
             latest = formatted_versions[0]
 
-        write_output("{} ({})".format(query, latest))
+        write_output(f"{query} ({latest})")
         write_output("Available versions: {}".format(", ".join(formatted_versions)))
         print_dist_installation_info(query, latest)
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/inspect.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/install.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,20 +603,16 @@
             )
 
         # NOTE: There is some duplication here, with commands/check.py
         for project_name in missing:
             version = package_set[project_name][0]
             for dependency in missing[project_name]:
                 message = (
-                    "{name} {version} requires {requirement}, "
+                    f"{project_name} {version} requires {dependency[1]}, "
                     "which is not installed."
-                ).format(
-                    name=project_name,
-                    version=version,
-                    requirement=dependency[1],
                 )
                 parts.append(message)
 
         for project_name in conflicting:
             version = package_set[project_name][0]
             for dep_name, dep_version, req in conflicting[project_name]:
                 message = (
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/list.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/search.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/show.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/uninstall.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/commands/wheel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/base.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/installed.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/sdist.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/distributions/wheel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/index/collector.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/index/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,24 +469,26 @@
         index_url_sources = collections.OrderedDict(
             build_source(
                 loc,
                 candidates_from_page=candidates_from_page,
                 page_validator=self.session.is_secure_origin,
                 expand_dir=False,
                 cache_link_parsing=False,
+                project_name=project_name,
             )
             for loc in self.search_scope.get_index_urls_locations(project_name)
         ).values()
         find_links_sources = collections.OrderedDict(
             build_source(
                 loc,
                 candidates_from_page=candidates_from_page,
                 page_validator=self.session.is_secure_origin,
                 expand_dir=True,
                 cache_link_parsing=True,
+                project_name=project_name,
             )
             for loc in self.find_links
         ).values()
 
         if logger.isEnabledFor(logging.DEBUG):
             lines = [
                 f"* {s.link}"
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/index/package_finder.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/index/package_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,16 +529,16 @@
                 pri = -(
                     wheel.find_most_preferred_tag(
                         valid_tags, self._wheel_tag_preferences
                     )
                 )
             except ValueError:
                 raise UnsupportedWheel(
-                    "{} is not a supported wheel for this platform. It "
-                    "can't be sorted.".format(wheel.filename)
+                    f"{wheel.filename} is not a supported wheel for this platform. It "
+                    "can't be sorted."
                 )
             if self._prefer_binary:
                 binary_preference = 1
             if wheel.build_tag is not None:
                 match = re.match(r"^(\d+)(.*)$", wheel.build_tag)
                 assert match is not None, "guaranteed by filename validation"
                 build_tag_groups = match.groups()
@@ -935,17 +935,15 @@
             logger.critical(
                 "Could not find a version that satisfies the requirement %s "
                 "(from versions: %s)",
                 req,
                 _format_versions(best_candidate_result.iter_all()),
             )
 
-            raise DistributionNotFound(
-                "No matching distribution found for {}".format(req)
-            )
+            raise DistributionNotFound(f"No matching distribution found for {req}")
 
         def _should_install_candidate(
             candidate: Optional[InstallationCandidate],
         ) -> "TypeGuard[InstallationCandidate]":
             if installed_version is None:
                 return True
             if best_candidate is None:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/locations/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/locations/_distutils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/locations/_distutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,15 @@
         dist_args["script_args"] = ["--no-user-cfg"]
 
     d = Distribution(dist_args)
     if not ignore_config_files:
         try:
             d.parse_config_files()
         except UnicodeDecodeError:
-            # Typeshed does not include find_config_files() for some reason.
-            paths = d.find_config_files()  # type: ignore
+            paths = d.find_config_files()
             logger.warning(
                 "Ignore distutils configs in %s due to encoding errors.",
                 ", ".join(os.path.basename(p) for p in paths),
             )
     obj: Optional[DistutilsCommand] = None
     obj = d.get_command_obj("install", create=True)
     assert obj is not None
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/locations/_sysconfig.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/locations/base.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/_json.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,18 @@
     result = {}
     for field, multi in METADATA_FIELDS:
         if field not in msg:
             continue
         key = json_name(field)
         if multi:
             value: Union[str, List[str]] = [
-                sanitise_header(v) for v in msg.get_all(field)
+                sanitise_header(v) for v in msg.get_all(field)  # type: ignore
             ]
         else:
-            value = sanitise_header(msg.get(field))
+            value = sanitise_header(msg.get(field))  # type: ignore
             if key == "keywords":
                 # Accept both comma-separated and space-separated
                 # forms, for better compatibility with old data.
                 if "," in value:
                     value = [v.strip() for v in value.split(",")]
                 else:
                     value = value.split()
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/base.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/candidate.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/candidate.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,12 +23,8 @@
         return "<InstallationCandidate({!r}, {!r}, {!r})>".format(
             self.name,
             self.version,
             self.link,
         )
 
     def __str__(self) -> str:
-        return "{!r} candidate (version {} at {})".format(
-            self.name,
-            self.version,
-            self.link,
-        )
+        return f"{self.name!r} candidate (version {self.version} at {self.link})"
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/direct_url.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/direct_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 ) -> Optional[T]:
     """Get value from dictionary and verify expected type."""
     if key not in d:
         return default
     value = d[key]
     if not isinstance(value, expected_type):
         raise DirectUrlValidationError(
-            "{!r} has unexpected type for {} (expected {})".format(
-                value, key, expected_type
-            )
+            f"{value!r} has unexpected type for {key} (expected {expected_type})"
         )
     return value
 
 
 def _get_required(
     d: Dict[str, Any], expected_type: Type[T], key: str, default: Optional[T] = None
 ) -> T:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/format_control.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/format_control.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,17 +29,15 @@
 
         if self.__slots__ != other.__slots__:
             return False
 
         return all(getattr(self, k) == getattr(other, k) for k in self.__slots__)
 
     def __repr__(self) -> str:
-        return "{}({}, {})".format(
-            self.__class__.__name__, self.no_binary, self.only_binary
-        )
+        return f"{self.__class__.__name__}({self.no_binary}, {self.only_binary})"
 
     @staticmethod
     def handle_mutual_excludes(value: str, target: Set[str], other: Set[str]) -> None:
         if value.startswith("-"):
             raise CommandError(
                 "--no-binary / --only-binary option requires 1 argument."
             )
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/index.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/installation_report.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/link.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,17 +364,15 @@
 
     def __str__(self) -> str:
         if self.requires_python:
             rp = f" (requires-python:{self.requires_python})"
         else:
             rp = ""
         if self.comes_from:
-            return "{} (from {}){}".format(
-                redact_auth_from_url(self._url), self.comes_from, rp
-            )
+            return f"{redact_auth_from_url(self._url)} (from {self.comes_from}){rp}"
         else:
             return redact_auth_from_url(str(self._url))
 
     def __repr__(self) -> str:
         return f"<Link {self}>"
 
     @property
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/scheme.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/search_scope.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/selection_prefs.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/target_python.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/models/wheel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/auth.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/cache.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/download.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         url = link.show_url
     else:
         url = link.url_without_fragment
 
     logged_url = redact_auth_from_url(url)
 
     if total_length:
-        logged_url = "{} ({})".format(logged_url, format_size(total_length))
+        logged_url = f"{logged_url} ({format_size(total_length)})"
 
     if is_from_cache(resp):
         logger.info("Using cached %s", logged_url)
     else:
         logger.info("Downloading %s", logged_url)
 
     if logger.getEffectiveLevel() > logging.INFO:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/lazy_wheel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/session.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,16 +351,17 @@
             # have.
             total=retries,
             # A 503 error from PyPI typically means that the Fastly -> Origin
             # connection got interrupted in some way. A 503 error in general
             # is typically considered a transient error so we'll go ahead and
             # retry it.
             # A 500 may indicate transient error in Amazon S3
+            # A 502 may be a transient error from a CDN like CloudFlare or CloudFront
             # A 520 or 527 - may indicate transient error in CloudFlare
-            status_forcelist=[500, 503, 520, 527],
+            status_forcelist=[500, 502, 503, 520, 527],
             # Add a small amount of back off between failed requests in
             # order to prevent hammering the service.
             backoff_factor=0.25,
         )  # type: ignore
 
         # Our Insecure HTTPAdapter disables HTTPS validation. It does not
         # support caching so we'll use it for all http:// URLs.
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/network/xmlrpc.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from pip._internal.exceptions import NetworkConnectionError
 from pip._internal.network.session import PipSession
 from pip._internal.network.utils import raise_for_status
 
 if TYPE_CHECKING:
     from xmlrpc.client import _HostType, _Marshallable
 
+    from _typeshed import SizedBuffer
+
 logger = logging.getLogger(__name__)
 
 
 class PipXmlrpcTransport(xmlrpc.client.Transport):
     """Provide a `xmlrpclib.Transport` implementation via a `PipSession`
     object.
     """
@@ -29,15 +31,15 @@
         self._scheme = index_parts.scheme
         self._session = session
 
     def request(
         self,
         host: "_HostType",
         handler: str,
-        request_body: bytes,
+        request_body: "SizedBuffer",
         verbose: bool = False,
     ) -> Tuple["_Marshallable", ...]:
         assert isinstance(host, str)
         parts = (self._scheme, host, handler, None, None, None)
         url = urllib.parse.urlunparse(parts)
         try:
             headers = {"Content-Type": "text/xml"}
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/check.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,24 +164,24 @@
                 ),
                 replacement=(
                     f"to upgrade to a newer version of {project_name} "
                     f"or contact the author to suggest that they "
                     f"release a version with a conforming version number"
                 ),
                 issue=12063,
-                gone_in="24.0",
+                gone_in="24.1",
             )
         for dep in package_details.dependencies:
             if any(isinstance(spec, LegacySpecifier) for spec in dep.specifier):
                 deprecated(
                     reason=(
                         f"{project_name} {package_details.version} "
                         f"has a non-standard dependency specifier {dep}."
                     ),
                     replacement=(
                         f"to upgrade to a newer version of {project_name} "
                         f"or contact the author to suggest that they "
                         f"release a version with a conforming dependency specifiers"
                     ),
                     issue=12063,
-                    gone_in="24.0",
+                    gone_in="24.1",
                 )
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/freeze.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/prepare.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -599,16 +599,16 @@
                     self._download,
                     self.verbosity,
                     self.download_dir,
                     hashes,
                 )
             except NetworkConnectionError as exc:
                 raise InstallationError(
-                    "Could not install requirement {} because of HTTP "
-                    "error {} for URL {}".format(req, exc, link)
+                    f"Could not install requirement {req} because of HTTP "
+                    f"error {exc} for URL {link}"
                 )
         else:
             file_path = self._downloaded[link.url]
             if hashes:
                 hashes.check_against_path(file_path)
             local_file = File(file_path, content_type=None)
 
@@ -680,17 +680,17 @@
         assert req.editable, "cannot prepare a non-editable req as editable"
 
         logger.info("Obtaining %s", req)
 
         with indent_log():
             if self.require_hashes:
                 raise InstallationError(
-                    "The editable requirement {} cannot be installed when "
+                    f"The editable requirement {req} cannot be installed when "
                     "requiring hashes, because there is no single file to "
-                    "hash.".format(req)
+                    "hash."
                 )
             req.ensure_has_source_dir(self.src_dir)
             req.update_editable()
             assert req.source_dir
             req.download_info = direct_url_for_editable(req.unpacked_source_directory)
 
             dist = _get_prepared_distribution(
@@ -710,15 +710,15 @@
         req: InstallRequirement,
         skip_reason: str,
     ) -> BaseDistribution:
         """Prepare an already-installed requirement."""
         assert req.satisfied_by, "req should have been satisfied but isn't"
         assert skip_reason is not None, (
             "did not get skip reason skipped but req.satisfied_by "
-            "is set to {}".format(req.satisfied_by)
+            f"is set to {req.satisfied_by}"
         )
         logger.info(
             "Requirement %s: %s (%s)", skip_reason, req, req.satisfied_by.version
         )
         with indent_log():
             if self.require_hashes:
                 logger.debug(
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/operations/install/wheel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,24 +160,22 @@
         return None
 
     # Format a message
     msg_lines = []
     for parent_dir, dir_scripts in warn_for.items():
         sorted_scripts: List[str] = sorted(dir_scripts)
         if len(sorted_scripts) == 1:
-            start_text = "script {} is".format(sorted_scripts[0])
+            start_text = f"script {sorted_scripts[0]} is"
         else:
             start_text = "scripts {} are".format(
                 ", ".join(sorted_scripts[:-1]) + " and " + sorted_scripts[-1]
             )
 
         msg_lines.append(
-            "The {} installed in '{}' which is not on PATH.".format(
-                start_text, parent_dir
-            )
+            f"The {start_text} installed in '{parent_dir}' which is not on PATH."
         )
 
     last_line_fmt = (
         "Consider adding {} to PATH or, if you prefer "
         "to suppress this warning, use --no-warn-script-location."
     )
     if len(msg_lines) == 1:
@@ -317,32 +315,28 @@
     #     and easy_install-X.Y.
     pip_script = console.pop("pip", None)
     if pip_script:
         if "ENSUREPIP_OPTIONS" not in os.environ:
             scripts_to_generate.append("pip = " + pip_script)
 
         if os.environ.get("ENSUREPIP_OPTIONS", "") != "altinstall":
-            scripts_to_generate.append(
-                "pip{} = {}".format(sys.version_info[0], pip_script)
-            )
+            scripts_to_generate.append(f"pip{sys.version_info[0]} = {pip_script}")
 
         scripts_to_generate.append(f"pip{get_major_minor_version()} = {pip_script}")
         # Delete any other versioned pip entry points
         pip_ep = [k for k in console if re.match(r"pip(\d+(\.\d+)?)?$", k)]
         for k in pip_ep:
             del console[k]
     easy_install_script = console.pop("easy_install", None)
     if easy_install_script:
         if "ENSUREPIP_OPTIONS" not in os.environ:
             scripts_to_generate.append("easy_install = " + easy_install_script)
 
         scripts_to_generate.append(
-            "easy_install-{} = {}".format(
-                get_major_minor_version(), easy_install_script
-            )
+            f"easy_install-{get_major_minor_version()} = {easy_install_script}"
         )
         # Delete any other versioned easy_install entry points
         easy_install_ep = [
             k for k in console if re.match(r"easy_install(-\d+\.\d+)?$", k)
         ]
         for k in easy_install_ep:
             del console[k]
@@ -404,18 +398,18 @@
         self._file.save()
         self.changed = fix_script(self.dest_path)
 
 
 class MissingCallableSuffix(InstallationError):
     def __init__(self, entry_point: str) -> None:
         super().__init__(
-            "Invalid script entry point: {} - A callable "
+            f"Invalid script entry point: {entry_point} - A callable "
             "suffix is required. Cf https://packaging.python.org/"
             "specifications/entry-points/#use-for-scripts for more "
-            "information.".format(entry_point)
+            "information."
         )
 
 
 def _raise_for_invalid_entrypoint(specification: str) -> None:
     entry = get_export_entry(specification)
     if entry is not None and entry.suffix is None:
         raise MissingCallableSuffix(str(entry))
@@ -708,15 +702,15 @@
 
 
 @contextlib.contextmanager
 def req_error_context(req_description: str) -> Generator[None, None, None]:
     try:
         yield
     except InstallationError as e:
-        message = "For req: {}. {}".format(req_description, e.args[0])
+        message = f"For req: {req_description}. {e.args[0]}"
         raise InstallationError(message) from e
 
 
 def install_wheel(
     name: str,
     wheel_path: str,
     scheme: Scheme,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/constructors.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/constructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,15 @@
         and comes_from.link
         and comes_from.link.netloc in domains_not_allowed
     ):
         # Explicitly disallow pypi packages that depend on external urls
         raise InstallationError(
             "Packages installed from PyPI cannot depend on packages "
             "which are not also hosted on PyPI.\n"
-            "{} depends on {} ".format(comes_from.name, req)
+            f"{comes_from.name} depends on {req} "
         )
 
     return InstallRequirement(
         req,
         comes_from,
         isolated=isolated,
         use_pep517=use_pep517,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/req_file.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/req_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,16 +71,24 @@
 # options to be passed to requirements
 SUPPORTED_OPTIONS_REQ: List[Callable[..., optparse.Option]] = [
     cmdoptions.global_options,
     cmdoptions.hash,
     cmdoptions.config_settings,
 ]
 
+SUPPORTED_OPTIONS_EDITABLE_REQ: List[Callable[..., optparse.Option]] = [
+    cmdoptions.config_settings,
+]
+
+
 # the 'dest' string values
 SUPPORTED_OPTIONS_REQ_DEST = [str(o().dest) for o in SUPPORTED_OPTIONS_REQ]
+SUPPORTED_OPTIONS_EDITABLE_REQ_DEST = [
+    str(o().dest) for o in SUPPORTED_OPTIONS_EDITABLE_REQ
+]
 
 logger = logging.getLogger(__name__)
 
 
 class ParsedRequirement:
     def __init__(
         self,
@@ -174,39 +182,33 @@
         "-c" if line.constraint else "-r",
         line.filename,
         line.lineno,
     )
 
     assert line.is_requirement
 
+    # get the options that apply to requirements
     if line.is_editable:
-        # For editable requirements, we don't support per-requirement
-        # options, so just return the parsed requirement.
-        return ParsedRequirement(
-            requirement=line.requirement,
-            is_editable=line.is_editable,
-            comes_from=line_comes_from,
-            constraint=line.constraint,
-        )
+        supported_dest = SUPPORTED_OPTIONS_EDITABLE_REQ_DEST
     else:
-        # get the options that apply to requirements
-        req_options = {}
-        for dest in SUPPORTED_OPTIONS_REQ_DEST:
-            if dest in line.opts.__dict__ and line.opts.__dict__[dest]:
-                req_options[dest] = line.opts.__dict__[dest]
-
-        line_source = f"line {line.lineno} of {line.filename}"
-        return ParsedRequirement(
-            requirement=line.requirement,
-            is_editable=line.is_editable,
-            comes_from=line_comes_from,
-            constraint=line.constraint,
-            options=req_options,
-            line_source=line_source,
-        )
+        supported_dest = SUPPORTED_OPTIONS_REQ_DEST
+    req_options = {}
+    for dest in supported_dest:
+        if dest in line.opts.__dict__ and line.opts.__dict__[dest]:
+            req_options[dest] = line.opts.__dict__[dest]
+
+    line_source = f"line {line.lineno} of {line.filename}"
+    return ParsedRequirement(
+        requirement=line.requirement,
+        is_editable=line.is_editable,
+        comes_from=line_comes_from,
+        constraint=line.constraint,
+        options=req_options,
+        line_source=line_source,
+    )
 
 
 def handle_option_line(
     opts: Values,
     filename: str,
     lineno: int,
     finder: Optional["PackageFinder"] = None,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/req_install.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/req_install.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,25 +177,35 @@
         # Are we using PEP 517 for this requirement?
         # After pyproject.toml has been loaded, the only valid values are True
         # and False. Before loading, None is valid (meaning "use the default").
         # Setting an explicit value before loading pyproject.toml is supported,
         # but after loading this flag should be treated as read only.
         self.use_pep517 = use_pep517
 
+        # If config settings are provided, enforce PEP 517.
+        if self.config_settings:
+            if self.use_pep517 is False:
+                logger.warning(
+                    "--no-use-pep517 ignored for %s "
+                    "because --config-settings are specified.",
+                    self,
+                )
+            self.use_pep517 = True
+
         # This requirement needs more preparation before it can be built
         self.needs_more_preparation = False
 
         # This requirement needs to be unpacked before it can be installed.
         self._archive_source: Optional[Path] = None
 
     def __str__(self) -> str:
         if self.req:
             s = redact_auth_from_requirement(self.req)
             if self.link:
-                s += " from {}".format(redact_auth_from_url(self.link.url))
+                s += f" from {redact_auth_from_url(self.link.url)}"
         elif self.link:
             s = redact_auth_from_url(self.link.url)
         else:
             s = "<InstallRequirement>"
         if self.satisfied_by is not None:
             if self.satisfied_by.location is not None:
                 location = display_path(self.satisfied_by.location)
@@ -217,15 +227,15 @@
         )
 
     def format_debug(self) -> str:
         """An un-tested helper for getting state, for debugging."""
         attributes = vars(self)
         names = sorted(attributes)
 
-        state = ("{}={!r}".format(attr, attributes[attr]) for attr in sorted(names))
+        state = (f"{attr}={attributes[attr]!r}" for attr in sorted(names))
         return "<{name} object: {{{state}}}>".format(
             name=self.__class__.__name__,
             state=", ".join(state),
         )
 
     # Things that are valid for all kinds of requirements?
     @property
@@ -504,23 +514,15 @@
         follow the PEP 517 or legacy (setup.py) code path.
         """
         pyproject_toml_data = load_pyproject_toml(
             self.use_pep517, self.pyproject_toml_path, self.setup_py_path, str(self)
         )
 
         if pyproject_toml_data is None:
-            if self.config_settings:
-                deprecated(
-                    reason=f"Config settings are ignored for project {self}.",
-                    replacement=(
-                        "to use --use-pep517 or add a "
-                        "pyproject.toml file to the project"
-                    ),
-                    gone_in="24.0",
-                )
+            assert not self.config_settings
             self.use_pep517 = False
             return
 
         self.use_pep517 = True
         requires, backend, check, backend_path = pyproject_toml_data
         self.requirements_to_check = check
         self.pyproject_requires = requires
@@ -750,16 +752,16 @@
 
         create_archive = True
         archive_name = "{}-{}.zip".format(self.name, self.metadata["version"])
         archive_path = os.path.join(build_dir, archive_name)
 
         if os.path.exists(archive_path):
             response = ask_path_exists(
-                "The file {} exists. (i)gnore, (w)ipe, "
-                "(b)ackup, (a)bort ".format(display_path(archive_path)),
+                f"The file {display_path(archive_path)} exists. (i)gnore, (w)ipe, "
+                "(b)ackup, (a)bort ",
                 ("i", "w", "b", "a"),
             )
             if response == "i":
                 create_archive = False
             elif response == "w":
                 logger.warning("Deleting %s", display_path(archive_path))
                 os.remove(archive_path)
@@ -823,14 +825,21 @@
             home=home,
             root=root,
             isolated=self.isolated,
             prefix=prefix,
         )
 
         if self.editable and not self.is_wheel:
+            if self.config_settings:
+                logger.warning(
+                    "--config-settings ignored for legacy editable install of %s. "
+                    "Consider upgrading to a version of setuptools "
+                    "that supports PEP 660 (>= 64).",
+                    self,
+                )
             install_editable_legacy(
                 global_options=global_options if global_options is not None else [],
                 prefix=prefix,
                 home=home,
                 use_user_site=use_user_site,
                 name=self.req.name,
                 setup_py_path=self.setup_py_path,
@@ -901,14 +910,14 @@
     has_build_options = _has_option(options, reqs, "build_options")
     has_global_options = _has_option(options, reqs, "global_options")
     if has_build_options or has_global_options:
         deprecated(
             reason="--build-option and --global-option are deprecated.",
             issue=11859,
             replacement="to use --config-settings",
-            gone_in="24.0",
+            gone_in="24.2",
         )
         logger.warning(
             "Implying --no-binary=:all: due to the presence of "
             "--build-option / --global-option. "
         )
         options.format_control.disallow_binaries()
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/req_set.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/req_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                         f"ignored as it isn't standard compliant."
                     ),
                     replacement=(
                         "set or update constraints to select another version "
                         "or contact the package author to fix the version number"
                     ),
                     issue=12063,
-                    gone_in="24.0",
+                    gone_in="24.1",
                 )
             for dep in req.get_dist().iter_dependencies():
                 if any(isinstance(spec, LegacySpecifier) for spec in dep.specifier):
                     deprecated(
                         reason=(
                             f"pip has selected {req} {version} which has non "
                             f"standard dependency specifier {dep}. "
@@ -111,9 +111,9 @@
                             f"ignored as it isn't standard compliant."
                         ),
                         replacement=(
                             "set or update constraints to select another version "
                             "or contact the package author to fix the version number"
                         ),
                         issue=12063,
-                        gone_in="24.0",
+                        gone_in="24.1",
                     )
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/req/req_uninstall.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,24 @@
     https://packaging.python.org/specifications/recording-installed-packages/
     """
     location = dist.location
     assert location is not None, "not installed"
 
     entries = dist.iter_declared_entries()
     if entries is None:
-        msg = "Cannot uninstall {dist}, RECORD file not found.".format(dist=dist)
+        msg = f"Cannot uninstall {dist}, RECORD file not found."
         installer = dist.installer
         if not installer or installer == "pip":
-            dep = "{}=={}".format(dist.raw_name, dist.version)
+            dep = f"{dist.raw_name}=={dist.version}"
             msg += (
                 " You might be able to recover from this via: "
-                "'pip install --force-reinstall --no-deps {}'.".format(dep)
+                f"'pip install --force-reinstall --no-deps {dep}'."
             )
         else:
-            msg += " Hint: The package was installed by {}.".format(installer)
+            msg += f" Hint: The package was installed by {installer}."
         raise UninstallationError(msg)
 
     for entry in entries:
         path = os.path.join(location, entry)
         yield path
         if path.endswith(".py"):
             dn, fn = os.path.split(path)
@@ -168,16 +168,15 @@
     for path in will_remove:
         if path.endswith(".pyc"):
             continue
         if path.endswith("__init__.py") or ".dist-info" in path:
             folders.add(os.path.dirname(path))
         files.add(path)
 
-    # probably this one https://github.com/python/mypy/issues/390
-    _normcased_files = set(map(os.path.normcase, files))  # type: ignore
+    _normcased_files = set(map(os.path.normcase, files))
 
     folders = compact(folders)
 
     # This walks the tree using os.walk to not miss extra folders
     # that might get added.
     for folder in folders:
         for dirpath, _, dirfiles in os.walk(folder):
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/base.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,17 +227,15 @@
         # allow specifying different wheels based on the environment/OS, in a
         # single requirements file.
         if install_req.link and install_req.link.is_wheel:
             wheel = Wheel(install_req.link.filename)
             tags = compatibility_tags.get_supported()
             if requirement_set.check_supported_wheels and not wheel.supported(tags):
                 raise InstallationError(
-                    "{} is not a supported wheel on this platform.".format(
-                        wheel.filename
-                    )
+                    f"{wheel.filename} is not a supported wheel on this platform."
                 )
 
         # This next bit is really a sanity check.
         assert (
             not install_req.user_supplied or parent_req_name is None
         ), "a user supplied req shouldn't have a parent"
 
@@ -283,17 +281,17 @@
             return [], existing_req
 
         does_not_satisfy_constraint = install_req.link and not (
             existing_req.link and install_req.link.path == existing_req.link.path
         )
         if does_not_satisfy_constraint:
             raise InstallationError(
-                "Could not satisfy constraints for '{}': "
+                f"Could not satisfy constraints for '{install_req.name}': "
                 "installation from path or url cannot be "
-                "constrained to a version".format(install_req.name)
+                "constrained to a version"
             )
         # If we're now installing a constraint, mark the existing
         # object for real installation.
         existing_req.constraint = False
         # If we're now installing a user supplied requirement,
         # mark the existing object as such.
         if install_req.user_supplied:
@@ -394,17 +392,17 @@
         if link.is_yanked:
             reason = link.yanked_reason or "<none given>"
             msg = (
                 # Mark this as a unicode string to prevent
                 # "UnicodeEncodeError: 'ascii' codec can't encode character"
                 # in Python 2 when the reason contains non-ascii characters.
                 "The candidate selected for download or install is a "
-                "yanked version: {candidate}\n"
-                "Reason for being yanked: {reason}"
-            ).format(candidate=best_candidate, reason=reason)
+                f"yanked version: {best_candidate}\n"
+                f"Reason for being yanked: {reason}"
+            )
             logger.warning(msg)
 
         return link
 
     def _populate_link(self, req: InstallRequirement) -> None:
         """Ensure that if a link can be found for this, that it is found.
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,18 +155,15 @@
         self._version = version
         self.dist = self._prepare()
 
     def __str__(self) -> str:
         return f"{self.name} {self.version}"
 
     def __repr__(self) -> str:
-        return "{class_name}({link!r})".format(
-            class_name=self.__class__.__name__,
-            link=str(self._link),
-        )
+        return f"{self.__class__.__name__}({str(self._link)!r})"
 
     def __hash__(self) -> int:
         return hash((self.__class__, self._link))
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, self.__class__):
             return links_equivalent(self._link, other._link)
@@ -350,18 +347,15 @@
         skip_reason = "already satisfied"
         factory.preparer.prepare_installed_requirement(self._ireq, skip_reason)
 
     def __str__(self) -> str:
         return str(self.dist)
 
     def __repr__(self) -> str:
-        return "{class_name}({distribution!r})".format(
-            class_name=self.__class__.__name__,
-            distribution=self.dist,
-        )
+        return f"{self.__class__.__name__}({self.dist!r})"
 
     def __hash__(self) -> int:
         return hash((self.__class__, self.name, self.version))
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, self.__class__):
             return self.name == other.name and self.version == other.version
@@ -451,19 +445,15 @@
         self._comes_from = comes_from if comes_from is not None else self.base._ireq
 
     def __str__(self) -> str:
         name, rest = str(self.base).split(" ", 1)
         return "{}[{}] {}".format(name, ",".join(self.extras), rest)
 
     def __repr__(self) -> str:
-        return "{class_name}(base={base!r}, extras={extras!r})".format(
-            class_name=self.__class__.__name__,
-            base=self.base,
-            extras=self.extras,
-        )
+        return f"{self.__class__.__name__}(base={self.base!r}, extras={self.extras!r})"
 
     def __hash__(self) -> int:
         return hash((self.base, self.extras))
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, self.__class__):
             return self.base == other.base and self.extras == other.extras
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,18 @@
     UnsupportedWheel,
 )
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.metadata import BaseDistribution, get_default_environment
 from pip._internal.models.link import Link
 from pip._internal.models.wheel import Wheel
 from pip._internal.operations.prepare import RequirementPreparer
-from pip._internal.req.constructors import install_req_from_link_and_ireq
+from pip._internal.req.constructors import (
+    install_req_drop_extras,
+    install_req_from_link_and_ireq,
+)
 from pip._internal.req.req_install import (
     InstallRequirement,
     check_invalid_constraint_type,
 )
 from pip._internal.resolution.base import InstallRequirementProvider
 from pip._internal.utils.compatibility_tags import get_supported
 from pip._internal.utils.hashes import Hashes
@@ -172,14 +175,28 @@
         self,
         link: Link,
         extras: FrozenSet[str],
         template: InstallRequirement,
         name: Optional[NormalizedName],
         version: Optional[CandidateVersion],
     ) -> Optional[Candidate]:
+        base: Optional[BaseCandidate] = self._make_base_candidate_from_link(
+            link, template, name, version
+        )
+        if not extras or base is None:
+            return base
+        return self._make_extras_candidate(base, extras, comes_from=template)
+
+    def _make_base_candidate_from_link(
+        self,
+        link: Link,
+        template: InstallRequirement,
+        name: Optional[NormalizedName],
+        version: Optional[CandidateVersion],
+    ) -> Optional[BaseCandidate]:
         # TODO: Check already installed candidate, and use it if the link and
         # editable flag match.
 
         if link in self._build_failures:
             # We already tried this candidate before, and it does not build.
             # Don't bother trying again.
             return None
@@ -200,15 +217,15 @@
                         link,
                         e,
                         extra={"markup": True},
                     )
                     self._build_failures[link] = e
                     return None
 
-            base: BaseCandidate = self._editable_candidate_cache[link]
+            return self._editable_candidate_cache[link]
         else:
             if link not in self._link_candidate_cache:
                 try:
                     self._link_candidate_cache[link] = LinkCandidate(
                         link,
                         template,
                         factory=self,
@@ -220,19 +237,15 @@
                         "Discarding [blue underline]%s[/]: [yellow]%s[reset]",
                         link,
                         e,
                         extra={"markup": True},
                     )
                     self._build_failures[link] = e
                     return None
-            base = self._link_candidate_cache[link]
-
-        if not extras:
-            return base
-        return self._make_extras_candidate(base, extras, comes_from=template)
+            return self._link_candidate_cache[link]
 
     def _iter_found_candidates(
         self,
         ireqs: Sequence[InstallRequirement],
         specifier: SpecifierSet,
         hashes: Hashes,
         prefers_installed: bool,
@@ -358,17 +371,16 @@
         """Produce explicit candidates from constraints.
 
         This creates "fake" InstallRequirement objects that are basically clones
         of what "should" be the template, but with original_link set to link.
         """
         for link in constraint.links:
             self._fail_if_link_is_unsupported_wheel(link)
-            candidate = self._make_candidate_from_link(
+            candidate = self._make_base_candidate_from_link(
                 link,
-                extras=frozenset(),
                 template=install_req_from_link_and_ireq(link, template),
                 name=canonicalize_name(identifier),
                 version=None,
             )
             if candidate:
                 yield candidate
 
@@ -450,50 +462,59 @@
     def _make_requirements_from_install_req(
         self, ireq: InstallRequirement, requested_extras: Iterable[str]
     ) -> Iterator[Requirement]:
         """
         Returns requirement objects associated with the given InstallRequirement. In
         most cases this will be a single object but the following special cases exist:
             - the InstallRequirement has markers that do not apply -> result is empty
-            - the InstallRequirement has both a constraint and extras -> result is split
-                in two requirement objects: one with the constraint and one with the
-                extra. This allows centralized constraint handling for the base,
-                resulting in fewer candidate rejections.
+            - the InstallRequirement has both a constraint (or link) and extras
+                -> result is split in two requirement objects: one with the constraint
+                (or link) and one with the extra. This allows centralized constraint
+                handling for the base, resulting in fewer candidate rejections.
         """
         if not ireq.match_markers(requested_extras):
             logger.info(
                 "Ignoring %s: markers '%s' don't match your environment",
                 ireq.name,
                 ireq.markers,
             )
         elif not ireq.link:
             if ireq.extras and ireq.req is not None and ireq.req.specifier:
                 yield SpecifierWithoutExtrasRequirement(ireq)
             yield SpecifierRequirement(ireq)
         else:
             self._fail_if_link_is_unsupported_wheel(ireq.link)
-            cand = self._make_candidate_from_link(
+            # Always make the link candidate for the base requirement to make it
+            # available to `find_candidates` for explicit candidate lookup for any
+            # set of extras.
+            # The extras are required separately via a second requirement.
+            cand = self._make_base_candidate_from_link(
                 ireq.link,
-                extras=frozenset(ireq.extras),
-                template=ireq,
+                template=install_req_drop_extras(ireq) if ireq.extras else ireq,
                 name=canonicalize_name(ireq.name) if ireq.name else None,
                 version=None,
             )
             if cand is None:
                 # There's no way we can satisfy a URL requirement if the underlying
                 # candidate fails to build. An unnamed URL must be user-supplied, so
                 # we fail eagerly. If the URL is named, an unsatisfiable requirement
                 # can make the resolver do the right thing, either backtrack (and
                 # maybe find some other requirement that's buildable) or raise a
                 # ResolutionImpossible eventually.
                 if not ireq.name:
                     raise self._build_failures[ireq.link]
                 yield UnsatisfiableRequirement(canonicalize_name(ireq.name))
             else:
+                # require the base from the link
                 yield self.make_requirement_from_candidate(cand)
+                if ireq.extras:
+                    # require the extras on top of the base candidate
+                    yield self.make_requirement_from_candidate(
+                        self._make_extras_candidate(cand, frozenset(ireq.extras))
+                    )
 
     def collect_root_requirements(
         self, root_ireqs: List[InstallRequirement]
     ) -> CollectedRootRequirements:
         collected = CollectedRootRequirements([], {}, {})
         for i, ireq in enumerate(root_ireqs):
             if ireq.constraint:
@@ -749,16 +770,16 @@
 
         if triggers:
             info = text_join(sorted(triggers))
         else:
             info = "the requested packages"
 
         msg = (
-            "Cannot install {} because these package versions "
-            "have conflicting dependencies.".format(info)
+            f"Cannot install {info} because these package versions "
+            "have conflicting dependencies."
         )
         logger.critical(msg)
         msg = "\nThe conflict is caused by:"
 
         relevant_constraints = set()
         for req, parent in e.causes:
             if req.name in constraints:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,15 @@
     def __init__(self, candidate: Candidate) -> None:
         self.candidate = candidate
 
     def __str__(self) -> str:
         return str(self.candidate)
 
     def __repr__(self) -> str:
-        return "{class_name}({candidate!r})".format(
-            class_name=self.__class__.__name__,
-            candidate=self.candidate,
-        )
+        return f"{self.__class__.__name__}({self.candidate!r})"
 
     @property
     def project_name(self) -> NormalizedName:
         # No need to canonicalize - the candidate did this
         return self.candidate.project_name
 
     @property
@@ -46,18 +43,15 @@
         self._ireq = ireq
         self._extras = frozenset(canonicalize_name(e) for e in self._ireq.extras)
 
     def __str__(self) -> str:
         return str(self._ireq.req)
 
     def __repr__(self) -> str:
-        return "{class_name}({requirement!r})".format(
-            class_name=self.__class__.__name__,
-            requirement=str(self._ireq.req),
-        )
+        return f"{self.__class__.__name__}({str(self._ireq.req)!r})"
 
     @property
     def project_name(self) -> NormalizedName:
         assert self._ireq.req, "Specifier-backed ireq is always PEP 508"
         return canonicalize_name(self._ireq.req.name)
 
     @property
@@ -112,18 +106,15 @@
         self.specifier = specifier
         self._candidate = match
 
     def __str__(self) -> str:
         return f"Python {self.specifier}"
 
     def __repr__(self) -> str:
-        return "{class_name}({specifier!r})".format(
-            class_name=self.__class__.__name__,
-            specifier=str(self.specifier),
-        )
+        return f"{self.__class__.__name__}({str(self.specifier)!r})"
 
     @property
     def project_name(self) -> NormalizedName:
         return self._candidate.project_name
 
     @property
     def name(self) -> str:
@@ -151,18 +142,15 @@
     def __init__(self, name: NormalizedName) -> None:
         self._name = name
 
     def __str__(self) -> str:
         return f"{self._name} (unavailable)"
 
     def __repr__(self) -> str:
-        return "{class_name}({name!r})".format(
-            class_name=self.__class__.__name__,
-            name=str(self._name),
-        )
+        return f"{self.__class__.__name__}({str(self._name)!r})"
 
     @property
     def project_name(self) -> NormalizedName:
         return self._name
 
     @property
     def name(self) -> str:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/_log.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/appdirs.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/compat.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/deprecation.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/egg_link.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/egg_link.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,32 +11,39 @@
 
 __all__ = [
     "egg_link_path_from_sys_path",
     "egg_link_path_from_location",
 ]
 
 
-def _egg_link_name(raw_name: str) -> str:
+def _egg_link_names(raw_name: str) -> List[str]:
     """
     Convert a Name metadata value to a .egg-link name, by applying
     the same substitution as pkg_resources's safe_name function.
     Note: we cannot use canonicalize_name because it has a different logic.
+
+    We also look for the raw name (without normalization) as setuptools 69 changed
+    the way it names .egg-link files (https://github.com/pypa/setuptools/issues/4167).
     """
-    return re.sub("[^A-Za-z0-9.]+", "-", raw_name) + ".egg-link"
+    return [
+        re.sub("[^A-Za-z0-9.]+", "-", raw_name) + ".egg-link",
+        f"{raw_name}.egg-link",
+    ]
 
 
 def egg_link_path_from_sys_path(raw_name: str) -> Optional[str]:
     """
     Look for a .egg-link file for project name, by walking sys.path.
     """
-    egg_link_name = _egg_link_name(raw_name)
+    egg_link_names = _egg_link_names(raw_name)
     for path_item in sys.path:
-        egg_link = os.path.join(path_item, egg_link_name)
-        if os.path.isfile(egg_link):
-            return egg_link
+        for egg_link_name in egg_link_names:
+            egg_link = os.path.join(path_item, egg_link_name)
+            if os.path.isfile(egg_link):
+                return egg_link
     return None
 
 
 def egg_link_path_from_location(raw_name: str) -> Optional[str]:
     """
     Return the path for the .egg-link file if it exists, otherwise, None.
 
@@ -60,13 +67,14 @@
         if not virtualenv_no_global() and user_site:
             sites.append(user_site)
     else:
         if user_site:
             sites.append(user_site)
         sites.append(site_packages)
 
-    egg_link_name = _egg_link_name(raw_name)
+    egg_link_names = _egg_link_names(raw_name)
     for site in sites:
-        egglink = os.path.join(site, egg_link_name)
-        if os.path.isfile(egglink):
-            return egglink
+        for egg_link_name in egg_link_names:
+            egglink = os.path.join(site, egg_link_name)
+            if os.path.isfile(egglink):
+                return egglink
     return None
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/encoding.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/entrypoints.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/filesystem.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/filetypes.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/glibc.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/hashes.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/logging.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/misc.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,19 +73,15 @@
 OnErr = Callable[[FunctionType, Path, ExcInfo], Any]
 
 
 def get_pip_version() -> str:
     pip_pkg_dir = os.path.join(os.path.dirname(__file__), "..", "..")
     pip_pkg_dir = os.path.abspath(pip_pkg_dir)
 
-    return "pip {} from {} (python {})".format(
-        __version__,
-        pip_pkg_dir,
-        get_major_minor_version(),
-    )
+    return f"pip {__version__} from {pip_pkg_dir} (python {get_major_minor_version()})"
 
 
 def normalize_version_info(py_version_info: Tuple[int, ...]) -> Tuple[int, int, int]:
     """
     Convert a tuple of ints representing a Python version to one of length
     three.
 
@@ -141,17 +137,17 @@
         # `[func, path, Union[ExcInfo, BaseException]] -> Any` is equivalent to
         # `Union[([func, path, ExcInfo] -> Any), ([func, path, BaseException] -> Any)]`.
         cast(Union[OnExc, OnErr], rmtree_errorhandler),
         onexc=onexc,
     )
     if sys.version_info >= (3, 12):
         # See https://docs.python.org/3.12/whatsnew/3.12.html#shutil.
-        shutil.rmtree(dir, onexc=handler)
+        shutil.rmtree(dir, onexc=handler)  # type: ignore
     else:
-        shutil.rmtree(dir, onerror=handler)
+        shutil.rmtree(dir, onerror=handler)  # type: ignore
 
 
 def _onerror_ignore(*_args: Any) -> None:
     pass
 
 
 def _onerror_reraise(*_args: Any) -> None:
@@ -275,21 +271,21 @@
         return 0
     else:
         raise ValueError(f"invalid truth value {val!r}")
 
 
 def format_size(bytes: float) -> str:
     if bytes > 1000 * 1000:
-        return "{:.1f} MB".format(bytes / 1000.0 / 1000)
+        return f"{bytes / 1000.0 / 1000:.1f} MB"
     elif bytes > 10 * 1000:
-        return "{} kB".format(int(bytes / 1000))
+        return f"{int(bytes / 1000)} kB"
     elif bytes > 1000:
-        return "{:.1f} kB".format(bytes / 1000.0)
+        return f"{bytes / 1000.0:.1f} kB"
     else:
-        return "{} bytes".format(int(bytes))
+        return f"{int(bytes)} bytes"
 
 
 def tabulate(rows: Iterable[Iterable[Any]]) -> Tuple[List[str], List[int]]:
     """Return a list of formatted rows and a list of column sizes.
 
     For example::
 
@@ -518,17 +514,15 @@
         return netloc
     if password is None:
         user = "****"
         password = ""
     else:
         user = urllib.parse.quote(user)
         password = ":****"
-    return "{user}{password}@{netloc}".format(
-        user=user, password=password, netloc=netloc
-    )
+    return f"{user}{password}@{netloc}"
 
 
 def _transform_url(
     url: str, transform_netloc: Callable[[str], Tuple[Any, ...]]
 ) -> Tuple[str, NetlocTuple]:
     """Transform and replace netloc in a url.
 
@@ -588,15 +582,15 @@
 
 class HiddenText:
     def __init__(self, secret: str, redacted: str) -> None:
         self.secret = secret
         self.redacted = redacted
 
     def __repr__(self) -> str:
-        return "<HiddenText {!r}>".format(str(self))
+        return f"<HiddenText {str(self)!r}>"
 
     def __str__(self) -> str:
         return self.redacted
 
     # This is useful for testing.
     def __eq__(self, other: Any) -> bool:
         if type(self) != type(other):
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/models.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/packaging.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/setuptools_build.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/subprocess.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/temp_dir.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/unpacking.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/urls.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/virtualenv.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/utils/wheel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/utils/wheel.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Returns the name of the .dist-info directory and the parsed WHEEL metadata.
     """
     try:
         info_dir = wheel_dist_info_dir(wheel_zip, name)
         metadata = wheel_metadata(wheel_zip, info_dir)
         version = wheel_version(metadata)
     except UnsupportedWheel as e:
-        raise UnsupportedWheel("{} has an invalid wheel, {}".format(name, str(e)))
+        raise UnsupportedWheel(f"{name} has an invalid wheel, {str(e)}")
 
     check_compatibility(version, name)
 
     return info_dir, metadata
 
 
 def wheel_dist_info_dir(source: ZipFile, name: str) -> str:
@@ -56,17 +56,15 @@
 
     info_dir = info_dirs[0]
 
     info_dir_name = canonicalize_name(info_dir)
     canonical_name = canonicalize_name(name)
     if not info_dir_name.startswith(canonical_name):
         raise UnsupportedWheel(
-            ".dist-info directory {!r} does not start with {!r}".format(
-                info_dir, canonical_name
-            )
+            f".dist-info directory {info_dir!r} does not start with {canonical_name!r}"
         )
 
     return info_dir
 
 
 def read_wheel_metadata_file(source: ZipFile, path: str) -> bytes:
     try:
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/bazaar.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/git.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/mercurial.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "hg+https",
         "hg+ssh",
         "hg+static-http",
     )
 
     @staticmethod
     def get_base_rev_args(rev: str) -> List[str]:
-        return [f"-r={rev}"]
+        return [f"--rev={rev}"]
 
     def fetch_new(
         self, dest: str, url: HiddenText, rev_options: RevOptions, verbosity: int
     ) -> None:
         rev_display = rev_options.to_display()
         logger.info(
             "Cloning hg %s%s to %s",
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/subversion.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,29 +401,29 @@
         and auth info to use.
 
         Returns: (url, rev, (username, password)).
         """
         scheme, netloc, path, query, frag = urllib.parse.urlsplit(url)
         if "+" not in scheme:
             raise ValueError(
-                "Sorry, {!r} is a malformed VCS url. "
+                f"Sorry, {url!r} is a malformed VCS url. "
                 "The format is <vcs>+<protocol>://<url>, "
-                "e.g. svn+http://myrepo/svn/MyApp#egg=MyApp".format(url)
+                "e.g. svn+http://myrepo/svn/MyApp#egg=MyApp"
             )
         # Remove the vcs prefix.
         scheme = scheme.split("+", 1)[1]
         netloc, user_pass = cls.get_netloc_and_auth(netloc, scheme)
         rev = None
         if "@" in path:
             path, rev = path.rsplit("@", 1)
             if not rev:
                 raise InstallationError(
-                    "The URL {!r} has an empty revision (after @) "
+                    f"The URL {url!r} has an empty revision (after @) "
                     "which is not supported. Include a revision after @ "
-                    "or remove @ from the URL.".format(url)
+                    "or remove @ from the URL."
                 )
         url = urllib.parse.urlunsplit((scheme, netloc, path, query, ""))
         return url, rev, user_pass
 
     @staticmethod
     def make_rev_args(
         username: Optional[str], password: Optional[HiddenText]
@@ -562,15 +562,15 @@
             prompt = ("(i)gnore, (w)ipe, (b)ackup ", ("i", "w", "b"))  # type: ignore
 
         logger.warning(
             "The plan is to install the %s repository %s",
             self.name,
             url,
         )
-        response = ask_path_exists("What to do?  {}".format(prompt[0]), prompt[1])
+        response = ask_path_exists(f"What to do?  {prompt[0]}", prompt[1])
 
         if response == "a":
             sys.exit(-1)
 
         if response == "w":
             logger.warning("Deleting %s", display_path(dest))
             rmtree(dest)
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/six.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/typing_extensions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/certifi/cacert.pem` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/certifi/core.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/big5freq.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/big5prober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/enums.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/escprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/escsm.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/johabprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/ansi.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/initialise.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/win32.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/winterm.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/compat.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Licensed to the Python Software Foundation under a contributor agreement.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 from __future__ import absolute_import
 
 import os
 import re
+import shutil
 import sys
 
 try:
     import ssl
 except ImportError:  # pragma: no cover
     ssl = None
 
@@ -29,77 +30,73 @@
     def quote(s):
         if isinstance(s, unicode):
             s = s.encode('utf-8')
         return _quote(s)
 
     import urllib2
     from urllib2 import (Request, urlopen, URLError, HTTPError,
-                         HTTPBasicAuthHandler, HTTPPasswordMgr,
-                         HTTPHandler, HTTPRedirectHandler,
-                         build_opener)
+                         HTTPBasicAuthHandler, HTTPPasswordMgr, HTTPHandler,
+                         HTTPRedirectHandler, build_opener)
     if ssl:
         from urllib2 import HTTPSHandler
     import httplib
     import xmlrpclib
     import Queue as queue
     from HTMLParser import HTMLParser
     import htmlentitydefs
     raw_input = raw_input
     from itertools import ifilter as filter
     from itertools import ifilterfalse as filterfalse
 
     # Leaving this around for now, in case it needs resurrecting in some way
     # _userprog = None
     # def splituser(host):
-        # """splituser('user[:passwd]@host[:port]') --> 'user[:passwd]', 'host[:port]'."""
-        # global _userprog
-        # if _userprog is None:
-            # import re
-            # _userprog = re.compile('^(.*)@(.*)$')
-
-        # match = _userprog.match(host)
-        # if match: return match.group(1, 2)
-        # return None, host
+    # """splituser('user[:passwd]@host[:port]') --> 'user[:passwd]', 'host[:port]'."""
+    # global _userprog
+    # if _userprog is None:
+    # import re
+    # _userprog = re.compile('^(.*)@(.*)$')
+
+    # match = _userprog.match(host)
+    # if match: return match.group(1, 2)
+    # return None, host
 
 else:  # pragma: no cover
     from io import StringIO
     string_types = str,
     text_type = str
     from io import TextIOWrapper as file_type
     import builtins
     import configparser
-    import shutil
-    from urllib.parse import (urlparse, urlunparse, urljoin, quote,
-                              unquote, urlsplit, urlunsplit, splittype)
+    from urllib.parse import (urlparse, urlunparse, urljoin, quote, unquote,
+                              urlsplit, urlunsplit, splittype)
     from urllib.request import (urlopen, urlretrieve, Request, url2pathname,
-                                pathname2url,
-                                HTTPBasicAuthHandler, HTTPPasswordMgr,
-                                HTTPHandler, HTTPRedirectHandler,
-                                build_opener)
+                                pathname2url, HTTPBasicAuthHandler,
+                                HTTPPasswordMgr, HTTPHandler,
+                                HTTPRedirectHandler, build_opener)
     if ssl:
         from urllib.request import HTTPSHandler
     from urllib.error import HTTPError, URLError, ContentTooShortError
     import http.client as httplib
     import urllib.request as urllib2
     import xmlrpc.client as xmlrpclib
     import queue
     from html.parser import HTMLParser
     import html.entities as htmlentitydefs
     raw_input = input
     from itertools import filterfalse
     filter = filter
 
-
 try:
     from ssl import match_hostname, CertificateError
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
+
     class CertificateError(ValueError):
         pass
 
-
     def _dnsname_match(dn, hostname, max_wildcards=1):
         """Matching according to RFC 6125, section 6.4.3
 
         http://tools.ietf.org/html/rfc6125#section-6.4.3
         """
         pats = []
         if not dn:
@@ -141,15 +138,14 @@
         # add the remaining fragments, ignore any wildcards
         for frag in remainder:
             pats.append(re.escape(frag))
 
         pat = re.compile(r'\A' + r'\.'.join(pats) + r'\Z', re.IGNORECASE)
         return pat.match(hostname)
 
-
     def match_hostname(cert, hostname):
         """Verify that *cert* (in decoded format as returned by
         SSLSocket.getpeercert()) matches the *hostname*.  RFC 2818 and RFC 6125
         rules are followed, but IP addresses are not accepted for *hostname*.
 
         CertificateError is raised on failure. On success, the function
         returns nothing.
@@ -174,32 +170,34 @@
                     # must be used.
                     if key == 'commonName':
                         if _dnsname_match(value, hostname):
                             return
                         dnsnames.append(value)
         if len(dnsnames) > 1:
             raise CertificateError("hostname %r "
-                "doesn't match either of %s"
-                % (hostname, ', '.join(map(repr, dnsnames))))
+                                   "doesn't match either of %s" %
+                                   (hostname, ', '.join(map(repr, dnsnames))))
         elif len(dnsnames) == 1:
             raise CertificateError("hostname %r "
-                "doesn't match %r"
-                % (hostname, dnsnames[0]))
+                                   "doesn't match %r" %
+                                   (hostname, dnsnames[0]))
         else:
             raise CertificateError("no appropriate commonName or "
-                "subjectAltName fields were found")
+                                   "subjectAltName fields were found")
 
 
 try:
     from types import SimpleNamespace as Container
 except ImportError:  # pragma: no cover
+
     class Container(object):
         """
         A generic container for when multiple values need to be returned
         """
+
         def __init__(self, **kwargs):
             self.__dict__.update(kwargs)
 
 
 try:
     from shutil import which
 except ImportError:  # pragma: no cover
@@ -210,14 +208,15 @@
         file.
 
         `mode` defaults to os.F_OK | os.X_OK. `path` defaults to the result
         of os.environ.get("PATH"), or can be overridden with a custom search
         path.
 
         """
+
         # Check that a given file can be accessed with the correct mode.
         # Additionally check that `file` is not a directory, as on Windows
         # directories pass the os.access check.
         def _access_check(fn, mode):
             return (os.path.exists(fn) and os.access(fn, mode)
                     and not os.path.isdir(fn))
 
@@ -233,15 +232,15 @@
             path = os.environ.get("PATH", os.defpath)
         if not path:
             return None
         path = path.split(os.pathsep)
 
         if sys.platform == "win32":
             # The current directory takes precedence on Windows.
-            if not os.curdir in path:
+            if os.curdir not in path:
                 path.insert(0, os.curdir)
 
             # PATHEXT is necessary to check on Windows.
             pathext = os.environ.get("PATHEXT", "").split(os.pathsep)
             # See if the given file matches any of the expected path extensions.
             # This will allow us to short circuit when given "python.exe".
             # If it does match, only test that one, otherwise we have to try
@@ -254,15 +253,15 @@
             # On other platforms you don't have things like PATHEXT to tell you
             # what file suffixes are executable, so just pass on cmd as-is.
             files = [cmd]
 
         seen = set()
         for dir in path:
             normdir = os.path.normcase(dir)
-            if not normdir in seen:
+            if normdir not in seen:
                 seen.add(normdir)
                 for thefile in files:
                     name = os.path.join(dir, thefile)
                     if _access_check(name, mode):
                         return name
         return None
 
@@ -273,55 +272,59 @@
 
 if hasattr(BaseZipFile, '__enter__'):  # pragma: no cover
     ZipFile = BaseZipFile
 else:  # pragma: no cover
     from zipfile import ZipExtFile as BaseZipExtFile
 
     class ZipExtFile(BaseZipExtFile):
+
         def __init__(self, base):
             self.__dict__.update(base.__dict__)
 
         def __enter__(self):
             return self
 
         def __exit__(self, *exc_info):
             self.close()
             # return None, so if an exception occurred, it will propagate
 
     class ZipFile(BaseZipFile):
+
         def __enter__(self):
             return self
 
         def __exit__(self, *exc_info):
             self.close()
             # return None, so if an exception occurred, it will propagate
 
         def open(self, *args, **kwargs):
             base = BaseZipFile.open(self, *args, **kwargs)
             return ZipExtFile(base)
 
+
 try:
     from platform import python_implementation
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
+
     def python_implementation():
         """Return a string identifying the Python implementation."""
         if 'PyPy' in sys.version:
             return 'PyPy'
         if os.name == 'java':
             return 'Jython'
         if sys.version.startswith('IronPython'):
             return 'IronPython'
         return 'CPython'
 
-import shutil
+
 import sysconfig
 
 try:
     callable = callable
-except NameError:   # pragma: no cover
+except NameError:  # pragma: no cover
     from collections.abc import Callable
 
     def callable(obj):
         return isinstance(obj, Callable)
 
 
 try:
@@ -354,19 +357,19 @@
             return filename
         elif isinstance(filename, bytes):
             return filename.decode(_fsencoding, _fserrors)
         else:
             raise TypeError("expect bytes or str, not %s" %
                             type(filename).__name__)
 
+
 try:
     from tokenize import detect_encoding
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
     from codecs import BOM_UTF8, lookup
-    import re
 
     cookie_re = re.compile(r"coding[:=]\s*([-\w.]+)")
 
     def _get_normal_name(orig_enc):
         """Imitates get_normal_name in tokenizer.c."""
         # Only care about the first 12 characters.
         enc = orig_enc[:12].lower().replace("_", "-")
@@ -397,14 +400,15 @@
         try:
             filename = readline.__self__.name
         except AttributeError:
             filename = None
         bom_found = False
         encoding = None
         default = 'utf-8'
+
         def read_or_stop():
             try:
                 return readline()
             except StopIteration:
                 return b''
 
         def find_cookie(line):
@@ -426,25 +430,26 @@
             try:
                 codec = lookup(encoding)
             except LookupError:
                 # This behaviour mimics the Python interpreter
                 if filename is None:
                     msg = "unknown encoding: " + encoding
                 else:
-                    msg = "unknown encoding for {!r}: {}".format(filename,
-                            encoding)
+                    msg = "unknown encoding for {!r}: {}".format(
+                        filename, encoding)
                 raise SyntaxError(msg)
 
             if bom_found:
                 if codec.name != 'utf-8':
                     # This behaviour mimics the Python interpreter
                     if filename is None:
                         msg = 'encoding problem: utf-8'
                     else:
-                        msg = 'encoding problem for {!r}: utf-8'.format(filename)
+                        msg = 'encoding problem for {!r}: utf-8'.format(
+                            filename)
                     raise SyntaxError(msg)
                 encoding += '-sig'
             return encoding
 
         first = read_or_stop()
         if first.startswith(BOM_UTF8):
             bom_found = True
@@ -463,32 +468,34 @@
 
         encoding = find_cookie(second)
         if encoding:
             return encoding, [first, second]
 
         return default, [first, second]
 
+
 # For converting & <-> &amp; etc.
 try:
     from html import escape
 except ImportError:
     from cgi import escape
 if sys.version_info[:2] < (3, 4):
     unescape = HTMLParser().unescape
 else:
     from html import unescape
 
 try:
     from collections import ChainMap
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
     from collections import MutableMapping
 
     try:
         from reprlib import recursive_repr as _recursive_repr
     except ImportError:
+
         def _recursive_repr(fillvalue='...'):
             '''
             Decorator to make a repr function return fillvalue for a recursive
             call
             '''
 
             def decorating_function(user_function):
@@ -505,55 +512,59 @@
                         repr_running.discard(key)
                     return result
 
                 # Can't use functools.wraps() here because of bootstrap issues
                 wrapper.__module__ = getattr(user_function, '__module__')
                 wrapper.__doc__ = getattr(user_function, '__doc__')
                 wrapper.__name__ = getattr(user_function, '__name__')
-                wrapper.__annotations__ = getattr(user_function, '__annotations__', {})
+                wrapper.__annotations__ = getattr(user_function,
+                                                  '__annotations__', {})
                 return wrapper
 
             return decorating_function
 
     class ChainMap(MutableMapping):
-        ''' A ChainMap groups multiple dicts (or other mappings) together
+        '''
+        A ChainMap groups multiple dicts (or other mappings) together
         to create a single, updateable view.
 
         The underlying mappings are stored in a list.  That list is public and can
         accessed or updated using the *maps* attribute.  There is no other state.
 
         Lookups search the underlying mappings successively until a key is found.
         In contrast, writes, updates, and deletions only operate on the first
         mapping.
-
         '''
 
         def __init__(self, *maps):
             '''Initialize a ChainMap by setting *maps* to the given mappings.
             If no mappings are provided, a single empty dictionary is used.
 
             '''
-            self.maps = list(maps) or [{}]          # always at least one map
+            self.maps = list(maps) or [{}]  # always at least one map
 
         def __missing__(self, key):
             raise KeyError(key)
 
         def __getitem__(self, key):
             for mapping in self.maps:
                 try:
-                    return mapping[key]             # can't use 'key in mapping' with defaultdict
+                    return mapping[
+                        key]  # can't use 'key in mapping' with defaultdict
                 except KeyError:
                     pass
-            return self.__missing__(key)            # support subclasses that define __missing__
+            return self.__missing__(
+                key)  # support subclasses that define __missing__
 
         def get(self, key, default=None):
             return self[key] if key in self else default
 
         def __len__(self):
-            return len(set().union(*self.maps))     # reuses stored hash values if possible
+            return len(set().union(
+                *self.maps))  # reuses stored hash values if possible
 
         def __iter__(self):
             return iter(set().union(*self.maps))
 
         def __contains__(self, key):
             return any(key in m for m in self.maps)
 
@@ -572,82 +583,87 @@
 
         def copy(self):
             'New ChainMap or subclass with a new copy of maps[0] and refs to maps[1:]'
             return self.__class__(self.maps[0].copy(), *self.maps[1:])
 
         __copy__ = copy
 
-        def new_child(self):                        # like Django's Context.push()
+        def new_child(self):  # like Django's Context.push()
             'New ChainMap with a new dict followed by all previous maps.'
             return self.__class__({}, *self.maps)
 
         @property
-        def parents(self):                          # like Django's Context.pop()
+        def parents(self):  # like Django's Context.pop()
             'New ChainMap from maps[1:].'
             return self.__class__(*self.maps[1:])
 
         def __setitem__(self, key, value):
             self.maps[0][key] = value
 
         def __delitem__(self, key):
             try:
                 del self.maps[0][key]
             except KeyError:
-                raise KeyError('Key not found in the first mapping: {!r}'.format(key))
+                raise KeyError(
+                    'Key not found in the first mapping: {!r}'.format(key))
 
         def popitem(self):
             'Remove and return an item pair from maps[0]. Raise KeyError is maps[0] is empty.'
             try:
                 return self.maps[0].popitem()
             except KeyError:
                 raise KeyError('No keys found in the first mapping.')
 
         def pop(self, key, *args):
             'Remove *key* from maps[0] and return its value. Raise KeyError if *key* not in maps[0].'
             try:
                 return self.maps[0].pop(key, *args)
             except KeyError:
-                raise KeyError('Key not found in the first mapping: {!r}'.format(key))
+                raise KeyError(
+                    'Key not found in the first mapping: {!r}'.format(key))
 
         def clear(self):
             'Clear maps[0], leaving maps[1:] intact.'
             self.maps[0].clear()
 
+
 try:
     from importlib.util import cache_from_source  # Python >= 3.4
 except ImportError:  # pragma: no cover
+
     def cache_from_source(path, debug_override=None):
         assert path.endswith('.py')
         if debug_override is None:
             debug_override = __debug__
         if debug_override:
             suffix = 'c'
         else:
             suffix = 'o'
         return path + suffix
 
+
 try:
     from collections import OrderedDict
-except ImportError: # pragma: no cover
-## {{{ http://code.activestate.com/recipes/576693/ (r9)
-# Backport of OrderedDict() class that runs on Python 2.4, 2.5, 2.6, 2.7 and pypy.
-# Passes Python2.7's test suite and incorporates all the latest updates.
+except ImportError:  # pragma: no cover
+    # {{{ http://code.activestate.com/recipes/576693/ (r9)
+    # Backport of OrderedDict() class that runs on Python 2.4, 2.5, 2.6, 2.7 and pypy.
+    # Passes Python2.7's test suite and incorporates all the latest updates.
     try:
         from thread import get_ident as _get_ident
     except ImportError:
         from dummy_thread import get_ident as _get_ident
 
     try:
         from _abcoll import KeysView, ValuesView, ItemsView
     except ImportError:
         pass
 
-
     class OrderedDict(dict):
         'Dictionary that remembers insertion order'
+
         # An inherited dict maps keys to values.
         # The inherited dict provides __getitem__, __len__, __contains__, and get.
         # The remaining methods are order-aware.
         # Big-O running times for all methods are the same as for regular dictionaries.
 
         # The internal self.__map dictionary maps keys to links in a doubly linked list.
         # The circular doubly linked list starts and ends with a sentinel element.
@@ -657,19 +673,20 @@
         def __init__(self, *args, **kwds):
             '''Initialize an ordered dictionary.  Signature is the same as for
             regular dictionaries, but keyword arguments are not recommended
             because their insertion order is arbitrary.
 
             '''
             if len(args) > 1:
-                raise TypeError('expected at most 1 arguments, got %d' % len(args))
+                raise TypeError('expected at most 1 arguments, got %d' %
+                                len(args))
             try:
                 self.__root
             except AttributeError:
-                self.__root = root = []                     # sentinel node
+                self.__root = root = []  # sentinel node
                 root[:] = [root, root, None]
                 self.__map = {}
             self.__update(*args, **kwds)
 
         def __setitem__(self, key, value, dict_setitem=dict.__setitem__):
             'od.__setitem__(i, y) <==> od[i]=y'
             # Setting a new item creates a new link which goes at the end of the linked
@@ -775,15 +792,15 @@
             If E has a .keys() method, does:         for k in E.keys(): od[k] = E[k]
             Or if E is an iterable of items, does:   for k, v in E: od[k] = v
             In either case, this is followed by:     for k, v in F.items(): od[k] = v
 
             '''
             if len(args) > 2:
                 raise TypeError('update() takes at most 2 positional '
-                                'arguments (%d given)' % (len(args),))
+                                'arguments (%d given)' % (len(args), ))
             elif not args:
                 raise TypeError('update() takes at least 1 argument (0 given)')
             self = args[0]
             # Make progressively weaker assumptions about "other"
             other = ()
             if len(args) == 2:
                 other = args[1]
@@ -821,35 +838,36 @@
             if key in self:
                 return self[key]
             self[key] = default
             return default
 
         def __repr__(self, _repr_running=None):
             'od.__repr__() <==> repr(od)'
-            if not _repr_running: _repr_running = {}
+            if not _repr_running:
+                _repr_running = {}
             call_key = id(self), _get_ident()
             if call_key in _repr_running:
                 return '...'
             _repr_running[call_key] = 1
             try:
                 if not self:
-                    return '%s()' % (self.__class__.__name__,)
+                    return '%s()' % (self.__class__.__name__, )
                 return '%s(%r)' % (self.__class__.__name__, self.items())
             finally:
                 del _repr_running[call_key]
 
         def __reduce__(self):
             'Return state information for pickling'
             items = [[k, self[k]] for k in self]
             inst_dict = vars(self).copy()
             for k in vars(OrderedDict()):
                 inst_dict.pop(k, None)
             if inst_dict:
-                return (self.__class__, (items,), inst_dict)
-            return self.__class__, (items,)
+                return (self.__class__, (items, ), inst_dict)
+            return self.__class__, (items, )
 
         def copy(self):
             'od.copy() -> a shallow copy of od'
             return self.__class__(self)
 
         @classmethod
         def fromkeys(cls, iterable, value=None):
@@ -864,15 +882,16 @@
 
         def __eq__(self, other):
             '''od.__eq__(y) <==> od==y.  Comparison to another OD is order-sensitive
             while comparison to a regular mapping is order-insensitive.
 
             '''
             if isinstance(other, OrderedDict):
-                return len(self)==len(other) and self.items() == other.items()
+                return len(self) == len(
+                    other) and self.items() == other.items()
             return dict.__eq__(self, other)
 
         def __ne__(self, other):
             return not self == other
 
         # -- the following methods are only used in Python 2.7 --
 
@@ -884,27 +903,26 @@
             "od.viewvalues() -> an object providing a view on od's values"
             return ValuesView(self)
 
         def viewitems(self):
             "od.viewitems() -> a set-like object providing a view on od's items"
             return ItemsView(self)
 
+
 try:
     from logging.config import BaseConfigurator, valid_ident
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
     IDENTIFIER = re.compile('^[a-z_][a-z0-9_]*$', re.I)
 
-
     def valid_ident(s):
         m = IDENTIFIER.match(s)
         if not m:
             raise ValueError('Not a valid Python identifier: %r' % s)
         return True
 
-
     # The ConvertingXXX classes are wrappers around standard Python containers,
     # and they serve to convert any suitable values in the container. The
     # conversion converts base dicts, lists and tuples to their wrapped
     # equivalents, whereas strings which match a conversion format are converted
     # appropriately.
     #
     # Each wrapper should have a configurator attribute holding the actual
@@ -912,27 +930,27 @@
 
     class ConvertingDict(dict):
         """A converting dictionary wrapper."""
 
         def __getitem__(self, key):
             value = dict.__getitem__(self, key)
             result = self.configurator.convert(value)
-            #If the converted value is different, save for next time
+            # If the converted value is different, save for next time
             if value is not result:
                 self[key] = result
                 if type(result) in (ConvertingDict, ConvertingList,
                                     ConvertingTuple):
                     result.parent = self
                     result.key = key
             return result
 
         def get(self, key, default=None):
             value = dict.get(self, key, default)
             result = self.configurator.convert(value)
-            #If the converted value is different, save for next time
+            # If the converted value is different, save for next time
             if value is not result:
                 self[key] = result
                 if type(result) in (ConvertingDict, ConvertingList,
                                     ConvertingTuple):
                     result.parent = self
                     result.key = key
             return result
@@ -945,18 +963,19 @@
                                 ConvertingTuple):
                 result.parent = self
                 result.key = key
         return result
 
     class ConvertingList(list):
         """A converting list wrapper."""
+
         def __getitem__(self, key):
             value = list.__getitem__(self, key)
             result = self.configurator.convert(value)
-            #If the converted value is different, save for next time
+            # If the converted value is different, save for next time
             if value is not result:
                 self[key] = result
                 if type(result) in (ConvertingDict, ConvertingList,
                                     ConvertingTuple):
                     result.parent = self
                     result.key = key
             return result
@@ -968,14 +987,15 @@
                 if type(result) in (ConvertingDict, ConvertingList,
                                     ConvertingTuple):
                     result.parent = self
             return result
 
     class ConvertingTuple(tuple):
         """A converting tuple wrapper."""
+
         def __getitem__(self, key):
             value = tuple.__getitem__(self, key)
             result = self.configurator.convert(value)
             if value is not result:
                 if type(result) in (ConvertingDict, ConvertingList,
                                     ConvertingTuple):
                     result.parent = self
@@ -991,16 +1011,16 @@
 
         WORD_PATTERN = re.compile(r'^\s*(\w+)\s*')
         DOT_PATTERN = re.compile(r'^\.\s*(\w+)\s*')
         INDEX_PATTERN = re.compile(r'^\[\s*(\w+)\s*\]\s*')
         DIGIT_PATTERN = re.compile(r'^\d+$')
 
         value_converters = {
-            'ext' : 'ext_convert',
-            'cfg' : 'cfg_convert',
+            'ext': 'ext_convert',
+            'cfg': 'cfg_convert',
         }
 
         # We might want to use a different one, e.g. importlib
         importer = staticmethod(__import__)
 
         def __init__(self, config):
             self.config = ConvertingDict(config)
@@ -1038,53 +1058,55 @@
             rest = value
             m = self.WORD_PATTERN.match(rest)
             if m is None:
                 raise ValueError("Unable to convert %r" % value)
             else:
                 rest = rest[m.end():]
                 d = self.config[m.groups()[0]]
-                #print d, rest
                 while rest:
                     m = self.DOT_PATTERN.match(rest)
                     if m:
                         d = d[m.groups()[0]]
                     else:
                         m = self.INDEX_PATTERN.match(rest)
                         if m:
                             idx = m.groups()[0]
                             if not self.DIGIT_PATTERN.match(idx):
                                 d = d[idx]
                             else:
                                 try:
-                                    n = int(idx) # try as number first (most likely)
+                                    n = int(
+                                        idx
+                                    )  # try as number first (most likely)
                                     d = d[n]
                                 except TypeError:
                                     d = d[idx]
                     if m:
                         rest = rest[m.end():]
                     else:
                         raise ValueError('Unable to convert '
                                          '%r at %r' % (value, rest))
-            #rest should be empty
+            # rest should be empty
             return d
 
         def convert(self, value):
             """
             Convert values to an appropriate type. dicts, lists and tuples are
             replaced by their converting alternatives. Strings are checked to
             see if they have a conversion format and are converted if they do.
             """
-            if not isinstance(value, ConvertingDict) and isinstance(value, dict):
+            if not isinstance(value, ConvertingDict) and isinstance(
+                    value, dict):
                 value = ConvertingDict(value)
                 value.configurator = self
-            elif not isinstance(value, ConvertingList) and isinstance(value, list):
+            elif not isinstance(value, ConvertingList) and isinstance(
+                    value, list):
                 value = ConvertingList(value)
                 value.configurator = self
-            elif not isinstance(value, ConvertingTuple) and\
-                     isinstance(value, tuple):
+            elif not isinstance(value, ConvertingTuple) and isinstance(value, tuple):
                 value = ConvertingTuple(value)
                 value.configurator = self
             elif isinstance(value, string_types):
                 m = self.CONVERT_PATTERN.match(value)
                 if m:
                     d = m.groupdict()
                     prefix = d['prefix']
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/database.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2012-2017 The Python Software Foundation.
+# Copyright (C) 2012-2023 The Python Software Foundation.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 """PEP 376 implementation."""
 
 from __future__ import unicode_literals
 
 import base64
@@ -21,19 +21,18 @@
 from .compat import StringIO
 from .version import get_scheme, UnsupportedVersionError
 from .metadata import (Metadata, METADATA_FILENAME, WHEEL_METADATA_FILENAME,
                        LEGACY_METADATA_FILENAME)
 from .util import (parse_requirement, cached_property, parse_name_and_version,
                    read_exports, write_exports, CSVReader, CSVWriter)
 
-
-__all__ = ['Distribution', 'BaseInstalledDistribution',
-           'InstalledDistribution', 'EggInfoDistribution',
-           'DistributionPath']
-
+__all__ = [
+    'Distribution', 'BaseInstalledDistribution', 'InstalledDistribution',
+    'EggInfoDistribution', 'DistributionPath'
+]
 
 logger = logging.getLogger(__name__)
 
 EXPORTS_FILENAME = 'pydist-exports.json'
 COMMANDS_FILENAME = 'pydist-commands.json'
 
 DIST_FILES = ('INSTALLER', METADATA_FILENAME, 'RECORD', 'REQUESTED',
@@ -42,14 +41,15 @@
 DISTINFO_EXT = '.dist-info'
 
 
 class _Cache(object):
     """
     A simple cache mapping names and .dist-info paths to distributions
     """
+
     def __init__(self):
         """
         Initialise an instance. There is normally one for each DistributionPath.
         """
         self.name = {}
         self.path = {}
         self.generated = False
@@ -72,14 +72,15 @@
             self.name.setdefault(dist.key, []).append(dist)
 
 
 class DistributionPath(object):
     """
     Represents a set of distributions installed on a path (typically sys.path).
     """
+
     def __init__(self, path=None, include_egg=False):
         """
         Create an instance from a path, optionally including legacy (distutils/
         setuptools/distribute) distributions.
         :param path: The path to use, as a list of directories. If not specified,
                      sys.path is used.
         :param include_egg: If True, this instance will look for and return legacy
@@ -107,15 +108,14 @@
     def clear_cache(self):
         """
         Clears the internal cache.
         """
         self._cache.clear()
         self._cache_egg.clear()
 
-
     def _yield_distributions(self):
         """
         Yield .dist-info and/or .egg(-info) distributions.
         """
         # We need to check if we've seen some resources already, because on
         # some Linux systems (e.g. some Debian/Ubuntu variants) there are
         # symlinks which alias other files in the environment.
@@ -130,33 +130,37 @@
             rset = sorted(r.resources)
             for entry in rset:
                 r = finder.find(entry)
                 if not r or r.path in seen:
                     continue
                 try:
                     if self._include_dist and entry.endswith(DISTINFO_EXT):
-                        possible_filenames = [METADATA_FILENAME,
-                                              WHEEL_METADATA_FILENAME,
-                                              LEGACY_METADATA_FILENAME]
+                        possible_filenames = [
+                            METADATA_FILENAME, WHEEL_METADATA_FILENAME,
+                            LEGACY_METADATA_FILENAME
+                        ]
                         for metadata_filename in possible_filenames:
-                            metadata_path = posixpath.join(entry, metadata_filename)
+                            metadata_path = posixpath.join(
+                                entry, metadata_filename)
                             pydist = finder.find(metadata_path)
                             if pydist:
                                 break
                         else:
                             continue
 
                         with contextlib.closing(pydist.as_stream()) as stream:
-                            metadata = Metadata(fileobj=stream, scheme='legacy')
+                            metadata = Metadata(fileobj=stream,
+                                                scheme='legacy')
                         logger.debug('Found %s', r.path)
                         seen.add(r.path)
-                        yield new_dist_class(r.path, metadata=metadata,
+                        yield new_dist_class(r.path,
+                                             metadata=metadata,
                                              env=self)
-                    elif self._include_egg and entry.endswith(('.egg-info',
-                                                              '.egg')):
+                    elif self._include_egg and entry.endswith(
+                            ('.egg-info', '.egg')):
                         logger.debug('Found %s', r.path)
                         seen.add(r.path)
                         yield old_dist_class(r.path, self)
                 except Exception as e:
                     msg = 'Unable to read distribution at %s, perhaps due to bad metadata: %s'
                     logger.warning(msg, r.path, e)
                     import warnings
@@ -267,15 +271,15 @@
         """
         matcher = None
         if version is not None:
             try:
                 matcher = self._scheme.matcher('%s (%s)' % (name, version))
             except ValueError:
                 raise DistlibException('invalid name or version: %r, %r' %
-                                      (name, version))
+                                       (name, version))
 
         for dist in self.get_distributions():
             # We hit a problem on Travis where enum34 was installed and doesn't
             # have a provides attribute ...
             if not hasattr(dist, 'provides'):
                 logger.debug('No "provides": %s', dist)
             else:
@@ -342,31 +346,31 @@
         """
         Initialise an instance.
         :param metadata: The instance of :class:`Metadata` describing this
         distribution.
         """
         self.metadata = metadata
         self.name = metadata.name
-        self.key = self.name.lower()    # for case-insensitive comparisons
+        self.key = self.name.lower()  # for case-insensitive comparisons
         self.version = metadata.version
         self.locator = None
         self.digest = None
-        self.extras = None      # additional features requested
-        self.context = None     # environment marker overrides
+        self.extras = None  # additional features requested
+        self.context = None  # environment marker overrides
         self.download_urls = set()
         self.digests = {}
 
     @property
     def source_url(self):
         """
         The source archive download URL for this distribution.
         """
         return self.metadata.source_url
 
-    download_url = source_url   # Backward compatibility
+    download_url = source_url  # Backward compatibility
 
     @property
     def name_and_version(self):
         """
         A utility property which displays the name and version in parentheses.
         """
         return '%s (%s)' % (self.name, self.version)
@@ -382,18 +386,18 @@
         if s not in plist:
             plist.append(s)
         return plist
 
     def _get_requirements(self, req_attr):
         md = self.metadata
         reqts = getattr(md, req_attr)
-        logger.debug('%s: got requirements %r from metadata: %r', self.name, req_attr,
-                     reqts)
-        return set(md.get_requirements(reqts, extras=self.extras,
-                                       env=self.context))
+        logger.debug('%s: got requirements %r from metadata: %r', self.name,
+                     req_attr, reqts)
+        return set(
+            md.get_requirements(reqts, extras=self.extras, env=self.context))
 
     @property
     def run_requires(self):
         return self._get_requirements('run_requires')
 
     @property
     def meta_requires(self):
@@ -422,20 +426,19 @@
         # from what's passed to the matcher
         r = parse_requirement(req)
         scheme = get_scheme(self.metadata.scheme)
         try:
             matcher = scheme.matcher(r.requirement)
         except UnsupportedVersionError:
             # XXX compat-mode if cannot read the version
-            logger.warning('could not read version %r - using name only',
-                           req)
+            logger.warning('could not read version %r - using name only', req)
             name = req.split()[0]
             matcher = scheme.matcher(name)
 
-        name = matcher.key   # case-insensitive
+        name = matcher.key  # case-insensitive
 
         result = False
         for p in self.provides:
             p_name, p_ver = parse_name_and_version(p)
             if p_name != name:
                 continue
             try:
@@ -462,17 +465,16 @@
                       another. distributions must have the same type, name,
                       version and source_url.
         :return: True if it is the same, else False.
         """
         if type(other) is not type(self):
             result = False
         else:
-            result = (self.name == other.name and
-                      self.version == other.version and
-                      self.source_url == other.source_url)
+            result = (self.name == other.name and self.version == other.version
+                      and self.source_url == other.source_url)
         return result
 
     def __hash__(self):
         """
         Compute hash in a way which matches the equality test.
         """
         return hash(self.name) + hash(self.version) + hash(self.source_url)
@@ -555,27 +557,27 @@
             # Temporary - for Wheel 0.23 support
             if r is None:
                 r = finder.find(WHEEL_METADATA_FILENAME)
             # Temporary - for legacy support
             if r is None:
                 r = finder.find(LEGACY_METADATA_FILENAME)
             if r is None:
-                raise ValueError('no %s found in %s' % (METADATA_FILENAME,
-                                                        path))
+                raise ValueError('no %s found in %s' %
+                                 (METADATA_FILENAME, path))
             with contextlib.closing(r.as_stream()) as stream:
                 metadata = Metadata(fileobj=stream, scheme='legacy')
 
         super(InstalledDistribution, self).__init__(metadata, path, env)
 
         if env and env._cache_enabled:
             env._cache.add(self)
 
         r = finder.find('REQUESTED')
         self.requested = r is not None
-        p  = os.path.join(path, 'top_level.txt')
+        p = os.path.join(path, 'top_level.txt')
         if os.path.exists(p):
             with open(p, 'rb') as f:
                 data = f.read().decode('utf-8')
             self.modules = data.splitlines()
 
     def __repr__(self):
         return '<InstalledDistribution %r %s at %r>' % (
@@ -592,22 +594,22 @@
                  as stored in the file (which is as in PEP 376).
         """
         results = []
         r = self.get_distinfo_resource('RECORD')
         with contextlib.closing(r.as_stream()) as stream:
             with CSVReader(stream=stream) as record_reader:
                 # Base location is parent dir of .dist-info dir
-                #base_location = os.path.dirname(self.path)
-                #base_location = os.path.abspath(base_location)
+                # base_location = os.path.dirname(self.path)
+                # base_location = os.path.abspath(base_location)
                 for row in record_reader:
                     missing = [None for i in range(len(row), 3)]
                     path, checksum, size = row + missing
-                    #if not os.path.isabs(path):
-                    #    path = path.replace('/', os.sep)
-                    #    path = os.path.join(base_location, path)
+                    # if not os.path.isabs(path):
+                    #     path = path.replace('/', os.sep)
+                    #     path = os.path.join(base_location, path)
                     results.append((path, checksum, size))
         return results
 
     @cached_property
     def exports(self):
         """
         Return the information exported by this distribution.
@@ -697,16 +699,16 @@
                 if os.path.isdir(path) or path.endswith(('.pyc', '.pyo')):
                     # do not put size and hash, as in PEP-376
                     hash_value = size = ''
                 else:
                     size = '%d' % os.path.getsize(path)
                     with open(path, 'rb') as fp:
                         hash_value = self.get_hash(fp.read())
-                if path.startswith(base) or (base_under_prefix and
-                                             path.startswith(prefix)):
+                if path.startswith(base) or (base_under_prefix
+                                             and path.startswith(prefix)):
                     path = os.path.relpath(path, base)
                 writer.writerow((path, hash_value, size))
 
             # add the RECORD file itself
             if record_path.startswith(base):
                 record_path = os.path.relpath(record_path, base)
             writer.writerow((record_path, '', ''))
@@ -740,15 +742,16 @@
                         hasher = hash_value.split('=', 1)[0]
                     else:
                         hasher = None
 
                     with open(path, 'rb') as f:
                         actual_hash = self.get_hash(f.read(), hasher)
                         if actual_hash != hash_value:
-                            mismatches.append((path, 'hash', hash_value, actual_hash))
+                            mismatches.append(
+                                (path, 'hash', hash_value, actual_hash))
         return mismatches
 
     @cached_property
     def shared_locations(self):
         """
         A dictionary of shared locations whose keys are in the set 'prefix',
         'purelib', 'platlib', 'scripts', 'headers', 'data' and 'namespace'.
@@ -787,15 +790,15 @@
         logger.info('creating %s', shared_path)
         if dry_run:
             return None
         lines = []
         for key in ('prefix', 'lib', 'headers', 'scripts', 'data'):
             path = paths[key]
             if os.path.isdir(paths[key]):
-                lines.append('%s=%s' % (key,  path))
+                lines.append('%s=%s' % (key, path))
         for ns in paths.get('namespace', ()):
             lines.append('namespace=%s' % ns)
 
         with codecs.open(shared_path, 'w', encoding='utf-8') as f:
             f.write('\n'.join(lines))
         return shared_path
 
@@ -850,34 +853,35 @@
             # XXX add separator or use real relpath algo
             if not os.path.isabs(path):
                 path = os.path.join(base, path)
             if path.startswith(self.path):
                 yield path
 
     def __eq__(self, other):
-        return (isinstance(other, InstalledDistribution) and
-                self.path == other.path)
+        return (isinstance(other, InstalledDistribution)
+                and self.path == other.path)
 
     # See http://docs.python.org/reference/datamodel#object.__hash__
     __hash__ = object.__hash__
 
 
 class EggInfoDistribution(BaseInstalledDistribution):
     """Created with the *path* of the ``.egg-info`` directory or file provided
     to the constructor. It reads the metadata contained in the file itself, or
     if the given path happens to be a directory, the metadata is read from the
     file ``PKG-INFO`` under that directory."""
 
-    requested = True    # as we have no way of knowing, assume it was
+    requested = True  # as we have no way of knowing, assume it was
     shared_locations = {}
 
     def __init__(self, path, env=None):
+
         def set_name_and_version(s, n, v):
             s.name = n
-            s.key = n.lower()   # for case-insensitive comparisons
+            s.key = n.lower()  # for case-insensitive comparisons
             s.version = v
 
         self.path = path
         self.dist_path = env
         if env and env._cache_enabled and path in env._cache_egg.path:
             metadata = env._cache_egg.path[path].metadata
             set_name_and_version(self, metadata.name, metadata.version)
@@ -899,23 +903,26 @@
 
             *data*: the contents of a setuptools-produced requires.txt file.
             """
             reqs = []
             lines = data.splitlines()
             for line in lines:
                 line = line.strip()
-                if line.startswith('['):
-                    logger.warning('Unexpected line: quitting requirement scan: %r',
-                                   line)
+                # sectioned files have bare newlines (separating sections)
+                if not line:  # pragma: no cover
+                    continue
+                if line.startswith('['):  # pragma: no cover
+                    logger.warning(
+                        'Unexpected line: quitting requirement scan: %r', line)
                     break
                 r = parse_requirement(line)
-                if not r:
+                if not r:  # pragma: no cover
                     logger.warning('Not recognised as a requirement: %r', line)
                     continue
-                if r.extras:
+                if r.extras:  # pragma: no cover
                     logger.warning('extra requirements in requires.txt are '
                                    'not supported')
                 if not r.constraints:
                     reqs.append(r.name)
                 else:
                     cons = ', '.join('%s%s' % c for c in r.constraints)
                     reqs.append('%s (%s)' % (r.name, cons))
@@ -948,15 +955,16 @@
                 # FIXME handle the case where zipfile is not available
                 zipf = zipimport.zipimporter(path)
                 fileobj = StringIO(
                     zipf.get_data('EGG-INFO/PKG-INFO').decode('utf8'))
                 metadata = Metadata(fileobj=fileobj, scheme='legacy')
                 try:
                     data = zipf.get_data('EGG-INFO/requires.txt')
-                    tl_data = zipf.get_data('EGG-INFO/top_level.txt').decode('utf-8')
+                    tl_data = zipf.get_data('EGG-INFO/top_level.txt').decode(
+                        'utf-8')
                     requires = parse_requires_data(data.decode('utf-8'))
                 except IOError:
                     requires = None
         elif path.endswith('.egg-info'):
             if os.path.isdir(path):
                 req_path = os.path.join(path, 'requires.txt')
                 requires = parse_requires_path(req_path)
@@ -978,16 +986,16 @@
             tl_data = []
         else:
             tl_data = tl_data.splitlines()
         self.modules = tl_data
         return metadata
 
     def __repr__(self):
-        return '<EggInfoDistribution %r %s at %r>' % (
-            self.name, self.version, self.path)
+        return '<EggInfoDistribution %r %s at %r>' % (self.name, self.version,
+                                                      self.path)
 
     def __str__(self):
         return "%s %s" % (self.name, self.version)
 
     def check_installed_files(self):
         """
         Checks that the hashes and sizes of the files in ``RECORD`` are
@@ -1035,15 +1043,15 @@
                     p = os.path.normpath(os.path.join(self.path, line))
                     # "./" is present as a marker between installed files
                     # and installation metadata files
                     if not os.path.exists(p):
                         logger.warning('Non-existent file: %s', p)
                         if p.endswith(('.pyc', '.pyo')):
                             continue
-                        #otherwise fall through and fail
+                        # otherwise fall through and fail
                     if not os.path.isdir(p):
                         result.append((p, _md5(p), _size(p)))
             result.append((record_path, None, None))
         return result
 
     def list_distinfo_files(self, absolute=False):
         """
@@ -1071,20 +1079,21 @@
                         if p.startswith(self.path):
                             if absolute:
                                 yield p
                             else:
                                 yield line
 
     def __eq__(self, other):
-        return (isinstance(other, EggInfoDistribution) and
-                self.path == other.path)
+        return (isinstance(other, EggInfoDistribution)
+                and self.path == other.path)
 
     # See http://docs.python.org/reference/datamodel#object.__hash__
     __hash__ = object.__hash__
 
+
 new_dist_class = InstalledDistribution
 old_dist_class = EggInfoDistribution
 
 
 class DependencyGraph(object):
     """
     Represents a dependency graph between distributions.
@@ -1110,15 +1119,15 @@
         """Add the *distribution* to the graph.
 
         :type distribution: :class:`distutils2.database.InstalledDistribution`
                             or :class:`distutils2.database.EggInfoDistribution`
         """
         self.adjacency_list[distribution] = []
         self.reverse_list[distribution] = []
-        #self.missing[distribution] = []
+        # self.missing[distribution] = []
 
     def add_edge(self, x, y, label=None):
         """Add an edge from distribution *x* to distribution *y* with the given
         *label*.
 
         :type x: :class:`distutils2.database.InstalledDistribution` or
                  :class:`distutils2.database.EggInfoDistribution`
@@ -1170,15 +1179,15 @@
         disconnected = []
 
         f.write("digraph dependencies {\n")
         for dist, adjs in self.adjacency_list.items():
             if len(adjs) == 0 and not skip_disconnected:
                 disconnected.append(dist)
             for other, label in adjs:
-                if not label is None:
+                if label is not None:
                     f.write('"%s" -> "%s" [label="%s"]\n' %
                             (dist.name, other.name, label))
                 else:
                     f.write('"%s" -> "%s"\n' % (dist.name, other.name))
         if not skip_disconnected and len(disconnected) > 0:
             f.write('subgraph disconnected {\n')
             f.write('label = "Disconnected"\n')
@@ -1248,27 +1257,27 @@
         for p in dist.provides:
             name, version = parse_name_and_version(p)
             logger.debug('Add to provided: %s, %s, %s', name, version, dist)
             provided.setdefault(name, []).append((version, dist))
 
     # now make the edges
     for dist in dists:
-        requires = (dist.run_requires | dist.meta_requires |
-                    dist.build_requires | dist.dev_requires)
+        requires = (dist.run_requires | dist.meta_requires
+                    | dist.build_requires | dist.dev_requires)
         for req in requires:
             try:
                 matcher = scheme.matcher(req)
             except UnsupportedVersionError:
                 # XXX compat-mode if cannot read the version
                 logger.warning('could not read version %r - using name only',
                                req)
                 name = req.split()[0]
                 matcher = scheme.matcher(name)
 
-            name = matcher.key   # case-insensitive
+            name = matcher.key  # case-insensitive
 
             matched = False
             if name in provided:
                 for version, provider in provided[name]:
                     try:
                         match = matcher.match(version)
                     except UnsupportedVersionError:
@@ -1320,15 +1329,15 @@
     if dist not in dists:
         raise DistlibException('given distribution %r is not a member '
                                'of the list' % dist.name)
     graph = make_graph(dists)
 
     req = set()  # required distributions
     todo = graph.adjacency_list[dist]  # list of nodes we should inspect
-    seen = set(t[0] for t in todo) # already added to todo
+    seen = set(t[0] for t in todo)  # already added to todo
 
     while todo:
         d = todo.pop()[0]
         req.add(d)
         pred_list = graph.adjacency_list[d]
         for pred in pred_list:
             d = pred[0]
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/index.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2013 Vinay Sajip.
+# Copyright (C) 2013-2023 Vinay Sajip.
 # Licensed to the Python Software Foundation under a contributor agreement.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 import hashlib
 import logging
 import os
 import shutil
@@ -21,14 +21,15 @@
 from .util import zip_dir, ServerProxy
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_INDEX = 'https://pypi.org/pypi'
 DEFAULT_REALM = 'pypi'
 
+
 class PackageIndex(object):
     """
     This class represents a package index compatible with PyPI, the Python
     Package Index.
     """
 
     boundary = b'----------ThIs_Is_tHe_distlib_index_bouNdaRY_$'
@@ -115,15 +116,15 @@
                 request.
         """
         self.check_credentials()
         metadata.validate()
         d = metadata.todict()
         d[':action'] = 'verify'
         request = self.encode_request(d.items(), [])
-        response = self.send_request(request)
+        self.send_request(request)
         d[':action'] = 'submit'
         request = self.encode_request(d.items(), [])
         return self.send_request(request)
 
     def _reader(self, name, stream, outbuf):
         """
         Thread runner for reading lines of from a subprocess into a buffer.
@@ -354,16 +355,15 @@
         if not self.gpg:
             raise DistlibException('verification unavailable because gpg '
                                    'unavailable')
         cmd = self.get_verify_command(signature_filename, data_filename,
                                       keystore)
         rc, stdout, stderr = self.run_command(cmd)
         if rc not in (0, 1):
-            raise DistlibException('verify command failed with error '
-                             'code %s' % rc)
+            raise DistlibException('verify command failed with error code %s' % rc)
         return rc == 0
 
     def download_file(self, url, destfile, digest=None, reporthook=None):
         """
         This is a convenience method for downloading a file from an URL.
         Normally, this will be a file from the index, though currently
         no check is made for this (i.e. a file can be downloaded from
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/locators.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/locators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2012-2015 Vinay Sajip.
+# Copyright (C) 2012-2023 Vinay Sajip.
 # Licensed to the Python Software Foundation under a contributor agreement.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 
 import gzip
 from io import BytesIO
 import json
@@ -34,28 +34,30 @@
 logger = logging.getLogger(__name__)
 
 HASHER_HASH = re.compile(r'^(\w+)=([a-f0-9]+)')
 CHARSET = re.compile(r';\s*charset\s*=\s*(.*)\s*$', re.I)
 HTML_CONTENT_TYPE = re.compile('text/html|application/x(ht)?ml')
 DEFAULT_INDEX = 'https://pypi.org/pypi'
 
+
 def get_all_distribution_names(url=None):
     """
     Return all distribution names known by an index.
     :param url: The URL of the index.
     :return: A list of all known distribution names.
     """
     if url is None:
         url = DEFAULT_INDEX
     client = ServerProxy(url, timeout=3.0)
     try:
         return client.list_packages()
     finally:
         client('close')()
 
+
 class RedirectHandler(BaseRedirectHandler):
     """
     A class to work around a bug in some Python 3.2.x releases.
     """
     # There's a bug in the base version for some 3.2.x
     # (e.g. 3.2.2 on Ubuntu Oneiric). If a Location header
     # returns e.g. /abc, it bails because it says the scheme ''
@@ -79,14 +81,15 @@
             else:
                 headers[key] = newurl
         return BaseRedirectHandler.http_error_302(self, req, fp, code, msg,
                                                   headers)
 
     http_error_301 = http_error_303 = http_error_307 = http_error_302
 
+
 class Locator(object):
     """
     A base class for locators - things that locate distributions.
     """
     source_extensions = ('.tar.gz', '.tar.bz2', '.tar', '.zip', '.tgz', '.tbz')
     binary_extensions = ('.egg', '.exe', '.whl')
     excluded_extensions = ('.pdf',)
@@ -268,15 +271,15 @@
                             'version': wheel.version,
                             'filename': wheel.filename,
                             'url': urlunparse((scheme, netloc, origpath,
                                                params, query, '')),
                             'python-version': ', '.join(
                                 ['.'.join(list(v[2:])) for v in wheel.pyver]),
                         }
-            except Exception as e:  # pragma: no cover
+            except Exception:  # pragma: no cover
                 logger.warning('invalid path for wheel: %s', path)
         elif not path.endswith(self.downloadable_extensions):  # pragma: no cover
             logger.debug('Not downloadable: %s', path)
         else:  # downloadable extension
             path = filename = posixpath.basename(path)
             for ext in self.downloadable_extensions:
                 if path.endswith(ext):
@@ -289,15 +292,14 @@
                         if not project_name or same_project(project_name, name):
                             result = {
                                 'name': name,
                                 'version': version,
                                 'filename': filename,
                                 'url': urlunparse((scheme, netloc, origpath,
                                                    params, query, '')),
-                                #'packagetype': 'sdist',
                             }
                             if pyver:  # pragma: no cover
                                 result['python-version'] = pyver
                     break
         if result and algo:
             result['%s_digest' % algo] = digest
         return result
@@ -378,20 +380,17 @@
                     continue
                 try:
                     if not matcher.match(k):
                         pass  # logger.debug('%s did not match %r', matcher, k)
                     else:
                         if prereleases or not vcls(k).is_prerelease:
                             slist.append(k)
-                        # else:
-                            # logger.debug('skipping pre-release '
-                                         # 'version %s of %s', k, matcher.name)
                 except Exception:  # pragma: no cover
                     logger.warning('error matching %s with %r', matcher, k)
-                    pass # slist.append(k)
+                    pass  # slist.append(k)
             if len(slist) > 1:
                 slist = sorted(slist, key=scheme.key)
             if slist:
                 logger.debug('sorted list: %s', slist)
                 version = slist[-1]
                 result = versions[version]
         if result:
@@ -452,14 +451,15 @@
                 for info in urls:
                     url = info['url']
                     digest = self._get_digest(info)
                     result['urls'].setdefault(v, set()).add(url)
                     result['digests'][url] = digest
         return result
 
+
 class PyPIJSONLocator(Locator):
     """
     This locator uses PyPI's JSON interface. It's very limited in functionality
     and probably not worth using.
     """
     def __init__(self, url, **kwargs):
         super(PyPIJSONLocator, self).__init__(**kwargs)
@@ -472,26 +472,26 @@
         raise NotImplementedError('Not available from this locator')
 
     def _get_project(self, name):
         result = {'urls': {}, 'digests': {}}
         url = urljoin(self.base_url, '%s/json' % quote(name))
         try:
             resp = self.opener.open(url)
-            data = resp.read().decode() # for now
+            data = resp.read().decode()  # for now
             d = json.loads(data)
             md = Metadata(scheme=self.scheme)
             data = d['info']
             md.name = data['name']
             md.version = data['version']
             md.license = data.get('license')
             md.keywords = data.get('keywords', [])
             md.summary = data.get('summary')
             dist = Distribution(md)
             dist.locator = self
-            urls = d['urls']
+            # urls = d['urls']
             result[md.version] = dist
             for info in d['urls']:
                 url = info['url']
                 dist.download_urls.add(url)
                 dist.digests[url] = self._get_digest(info)
                 result['urls'].setdefault(md.version, set()).add(url)
                 result['digests'][url] = self._get_digest(info)
@@ -741,26 +741,26 @@
                     if page is None:    # e.g. after an error
                         continue
                     for link, rel in page.links:
                         if link not in self._seen:
                             try:
                                 self._seen.add(link)
                                 if (not self._process_download(link) and
-                                    self._should_queue(link, url, rel)):
+                                        self._should_queue(link, url, rel)):
                                     logger.debug('Queueing %s from %s', link, url)
                                     self._to_fetch.put(link)
                             except MetadataInvalidError:  # e.g. invalid versions
                                 pass
             except Exception as e:  # pragma: no cover
                 self.errors.put(text_type(e))
             finally:
                 # always do this, to avoid hangs :-)
                 self._to_fetch.task_done()
             if not url:
-                #logger.debug('Sentinel seen, quitting.')
+                # logger.debug('Sentinel seen, quitting.')
                 break
 
     def get_page(self, url):
         """
         Get the HTML for an URL, possibly from an in-memory cache.
 
         XXX TODO Note: this cache is never actually cleared. It's assumed that
@@ -828,14 +828,15 @@
         page = self.get_page(self.base_url)
         if not page:
             raise DistlibException('Unable to get %s' % self.base_url)
         for match in self._distname_re.finditer(page.data):
             result.add(match.group(1))
         return result
 
+
 class DirectoryLocator(Locator):
     """
     This class locates distributions in a directory tree.
     """
 
     def __init__(self, path, **kwargs):
         """
@@ -893,14 +894,15 @@
                     info = self.convert_url_to_download_info(url, None)
                     if info:
                         result.add(info['name'])
             if not self.recursive:
                 break
         return result
 
+
 class JSONLocator(Locator):
     """
     This locator uses special extended metadata (not available on PyPI) and is
     the basis of performant dependency resolution in distlib. Other locators
     require archive downloads before dependencies can be determined! As you
     might imagine, that can be slow.
     """
@@ -931,14 +933,15 @@
                     dist.digest = ('md5', info['digest'])
                 md.dependencies = info.get('requirements', {})
                 dist.exports = info.get('exports', {})
                 result[dist.version] = dist
                 result['urls'].setdefault(dist.version, set()).add(info['url'])
         return result
 
+
 class DistPathLocator(Locator):
     """
     This locator finds installed distributions in a path. It can be useful for
     adding to an :class:`AggregatingLocator`.
     """
     def __init__(self, distpath, **kwargs):
         """
@@ -1241,15 +1244,15 @@
         install_dists = set([odist])
         while todo:
             dist = todo.pop()
             name = dist.key     # case-insensitive
             if name not in self.dists_by_name:
                 self.add_distribution(dist)
             else:
-                #import pdb; pdb.set_trace()
+                # import pdb; pdb.set_trace()
                 other = self.dists_by_name[name]
                 if other != dist:
                     self.try_to_replace(dist, other, problems)
 
             ireqts = dist.run_requires | dist.meta_requires
             sreqts = dist.build_requires
             ereqts = set()
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/manifest.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2012-2013 Python Software Foundation.
+# Copyright (C) 2012-2023 Python Software Foundation.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 """
 Class representing the list of files in a distribution.
 
 Equivalent to distutils.filelist, but fixes some problems.
 """
@@ -30,17 +30,19 @@
 #
 # Due to the different results returned by fnmatch.translate, we need
 # to do slightly different processing for Python 2.7 and 3.2 ... this needed
 # to be brought in for Python 3.6 onwards.
 #
 _PYTHON_VERSION = sys.version_info[:2]
 
+
 class Manifest(object):
-    """A list of files built by on exploring the filesystem and filtered by
-    applying various patterns to what we find there.
+    """
+    A list of files built by exploring the filesystem and filtered by applying various
+    patterns to what we find there.
     """
 
     def __init__(self, base=None):
         """
         Initialise an instance.
 
         :param base: The base directory to explore under.
@@ -150,46 +152,35 @@
         if action == 'include':
             for pattern in patterns:
                 if not self._include_pattern(pattern, anchor=True):
                     logger.warning('no files found matching %r', pattern)
 
         elif action == 'exclude':
             for pattern in patterns:
-                found = self._exclude_pattern(pattern, anchor=True)
-                #if not found:
-                #    logger.warning('no previously-included files '
-                #                   'found matching %r', pattern)
+                self._exclude_pattern(pattern, anchor=True)
 
         elif action == 'global-include':
             for pattern in patterns:
                 if not self._include_pattern(pattern, anchor=False):
                     logger.warning('no files found matching %r '
                                    'anywhere in distribution', pattern)
 
         elif action == 'global-exclude':
             for pattern in patterns:
-                found = self._exclude_pattern(pattern, anchor=False)
-                #if not found:
-                #    logger.warning('no previously-included files '
-                #                   'matching %r found anywhere in '
-                #                   'distribution', pattern)
+                self._exclude_pattern(pattern, anchor=False)
 
         elif action == 'recursive-include':
             for pattern in patterns:
                 if not self._include_pattern(pattern, prefix=thedir):
                     logger.warning('no files found matching %r '
                                    'under directory %r', pattern, thedir)
 
         elif action == 'recursive-exclude':
             for pattern in patterns:
-                found = self._exclude_pattern(pattern, prefix=thedir)
-                #if not found:
-                #    logger.warning('no previously-included files '
-                #                   'matching %r found under directory %r',
-                #                   pattern, thedir)
+                self._exclude_pattern(pattern, prefix=thedir)
 
         elif action == 'graft':
             if not self._include_pattern(None, prefix=dirpattern):
                 logger.warning('no directories found matching %r',
                                dirpattern)
 
         elif action == 'prune':
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/markers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/markers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2012-2017 Vinay Sajip.
+# Copyright (C) 2012-2023 Vinay Sajip.
 # Licensed to the Python Software Foundation under a contributor agreement.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 """
 Parser for the environment markers micro-language defined in PEP 508.
 """
 
@@ -15,45 +15,51 @@
 import os
 import re
 import sys
 import platform
 
 from .compat import string_types
 from .util import in_venv, parse_marker
-from .version import NormalizedVersion as NV
+from .version import LegacyVersion as LV
 
 __all__ = ['interpret']
 
-_VERSION_PATTERN = re.compile(r'((\d+(\.\d+)*\w*)|\'(\d+(\.\d+)*\w*)\'|\"(\d+(\.\d+)*\w*)\")')
+_VERSION_PATTERN = re.compile(
+    r'((\d+(\.\d+)*\w*)|\'(\d+(\.\d+)*\w*)\'|\"(\d+(\.\d+)*\w*)\")')
+_VERSION_MARKERS = {'python_version', 'python_full_version'}
+
+
+def _is_version_marker(s):
+    return isinstance(s, string_types) and s in _VERSION_MARKERS
+
 
 def _is_literal(o):
     if not isinstance(o, string_types) or not o:
         return False
     return o[0] in '\'"'
 
+
 def _get_versions(s):
-    result = []
-    for m in _VERSION_PATTERN.finditer(s):
-        result.append(NV(m.groups()[0]))
-    return set(result)
+    return {LV(m.groups()[0]) for m in _VERSION_PATTERN.finditer(s)}
+
 
 class Evaluator(object):
     """
-    This class is used to evaluate marker expessions.
+    This class is used to evaluate marker expressions.
     """
 
     operations = {
         '==': lambda x, y: x == y,
         '===': lambda x, y: x == y,
         '~=': lambda x, y: x == y or x > y,
         '!=': lambda x, y: x != y,
-        '<':  lambda x, y: x < y,
-        '<=':  lambda x, y: x == y or x < y,
-        '>':  lambda x, y: x > y,
-        '>=':  lambda x, y: x == y or x > y,
+        '<': lambda x, y: x < y,
+        '<=': lambda x, y: x == y or x < y,
+        '>': lambda x, y: x > y,
+        '>=': lambda x, y: x == y or x > y,
         'and': lambda x, y: x and y,
         'or': lambda x, y: x or y,
         'in': lambda x, y: x in y,
         'not in': lambda x, y: x not in y,
     }
 
     def evaluate(self, expr, context):
@@ -72,40 +78,45 @@
             assert isinstance(expr, dict)
             op = expr['op']
             if op not in self.operations:
                 raise NotImplementedError('op not implemented: %s' % op)
             elhs = expr['lhs']
             erhs = expr['rhs']
             if _is_literal(expr['lhs']) and _is_literal(expr['rhs']):
-                raise SyntaxError('invalid comparison: %s %s %s' % (elhs, op, erhs))
+                raise SyntaxError('invalid comparison: %s %s %s' %
+                                  (elhs, op, erhs))
 
             lhs = self.evaluate(elhs, context)
             rhs = self.evaluate(erhs, context)
-            if ((elhs == 'python_version' or erhs == 'python_version') and
-                op in ('<', '<=', '>', '>=', '===', '==', '!=', '~=')):
-                lhs = NV(lhs)
-                rhs = NV(rhs)
-            elif elhs == 'python_version' and op in ('in', 'not in'):
-                lhs = NV(lhs)
+            if ((_is_version_marker(elhs) or _is_version_marker(erhs))
+                    and op in ('<', '<=', '>', '>=', '===', '==', '!=', '~=')):
+                lhs = LV(lhs)
+                rhs = LV(rhs)
+            elif _is_version_marker(elhs) and op in ('in', 'not in'):
+                lhs = LV(lhs)
                 rhs = _get_versions(rhs)
             result = self.operations[op](lhs, rhs)
         return result
 
+
 _DIGITS = re.compile(r'\d+\.\d+')
 
+
 def default_context():
+
     def format_full_version(info):
         version = '%s.%s.%s' % (info.major, info.minor, info.micro)
         kind = info.releaselevel
         if kind != 'final':
             version += kind[0] + str(info.serial)
         return version
 
     if hasattr(sys, 'implementation'):
-        implementation_version = format_full_version(sys.implementation.version)
+        implementation_version = format_full_version(
+            sys.implementation.version)
         implementation_name = sys.implementation.name
     else:
         implementation_version = '0'
         implementation_name = ''
 
     ppv = platform.python_version()
     m = _DIGITS.match(ppv)
@@ -122,31 +133,35 @@
         'platform_in_venv': str(in_venv()),
         'python_full_version': ppv,
         'python_version': pv,
         'sys_platform': sys.platform,
     }
     return result
 
+
 DEFAULT_CONTEXT = default_context()
 del default_context
 
 evaluator = Evaluator()
 
+
 def interpret(marker, execution_context=None):
     """
     Interpret a marker and return a result depending on environment.
 
     :param marker: The marker to interpret.
     :type marker: str
     :param execution_context: The context used for name lookup.
     :type execution_context: mapping
     """
     try:
         expr, rest = parse_marker(marker)
     except Exception as e:
-        raise SyntaxError('Unable to interpret marker syntax: %s: %s' % (marker, e))
+        raise SyntaxError('Unable to interpret marker syntax: %s: %s' %
+                          (marker, e))
     if rest and rest[0] != '#':
-        raise SyntaxError('unexpected trailing data in marker: %s: %s' % (marker, rest))
+        raise SyntaxError('unexpected trailing data in marker: %s: %s' %
+                          (marker, rest))
     context = dict(DEFAULT_CONTEXT)
     if execution_context:
         context.update(execution_context)
     return evaluator.evaluate(expr, context)
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/metadata.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,25 +132,17 @@
         return _643_FIELDS
     raise MetadataUnrecognizedVersionError(version)
 
 
 def _best_version(fields):
     """Detect the best version depending on the fields used."""
     def _has_marker(keys, markers):
-        for marker in markers:
-            if marker in keys:
-                return True
-        return False
-
-    keys = []
-    for key, value in fields.items():
-        if value in ([], 'UNKNOWN', None):
-            continue
-        keys.append(key)
+        return any(marker in keys for marker in markers)
 
+    keys = [key for key, value in fields.items() if value not in ([], 'UNKNOWN', None)]
     possible_versions = ['1.0', '1.1', '1.2', '1.3', '2.1', '2.2']  # 2.0 removed
 
     # first let's try to see if a field is not part of one of the version
     for key in keys:
         if key not in _241_FIELDS and '1.0' in possible_versions:
             possible_versions.remove('1.0')
             logger.debug('Removed 1.0 due to %s', key)
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/resources.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/scripts.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2013-2015 Vinay Sajip.
+# Copyright (C) 2013-2023 Vinay Sajip.
 # Licensed to the Python Software Foundation under a contributor agreement.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 from io import BytesIO
 import logging
 import os
 import re
@@ -61,51 +61,58 @@
             if ' ' in _executable and not _executable.startswith('"'):
                 executable = '%s "%s"' % (env, _executable)
         else:
             if not executable.startswith('"'):
                 executable = '"%s"' % executable
     return executable
 
+
 # Keep the old name around (for now), as there is at least one project using it!
 _enquote_executable = enquote_executable
 
+
 class ScriptMaker(object):
     """
     A class to copy or create scripts from source scripts or callable
     specifications.
     """
     script_template = SCRIPT_TEMPLATE
 
     executable = None  # for shebangs
 
-    def __init__(self, source_dir, target_dir, add_launchers=True,
-                 dry_run=False, fileop=None):
+    def __init__(self,
+                 source_dir,
+                 target_dir,
+                 add_launchers=True,
+                 dry_run=False,
+                 fileop=None):
         self.source_dir = source_dir
         self.target_dir = target_dir
         self.add_launchers = add_launchers
         self.force = False
         self.clobber = False
         # It only makes sense to set mode bits on POSIX.
-        self.set_mode = (os.name == 'posix') or (os.name == 'java' and
-                                                 os._name == 'posix')
+        self.set_mode = (os.name == 'posix') or (os.name == 'java'
+                                                 and os._name == 'posix')
         self.variants = set(('', 'X.Y'))
         self._fileop = fileop or FileOperator(dry_run)
 
-        self._is_nt = os.name == 'nt' or (
-            os.name == 'java' and os._name == 'nt')
+        self._is_nt = os.name == 'nt' or (os.name == 'java'
+                                          and os._name == 'nt')
         self.version_info = sys.version_info
 
     def _get_alternate_executable(self, executable, options):
         if options.get('gui', False) and self._is_nt:  # pragma: no cover
             dn, fn = os.path.split(executable)
             fn = fn.replace('python', 'pythonw')
             executable = os.path.join(dn, fn)
         return executable
 
     if sys.platform.startswith('java'):  # pragma: no cover
+
         def _is_shell(self, executable):
             """
             Determine if the specified executable is a script
             (contains a #! line)
             """
             try:
                 with open(executable) as fp:
@@ -142,45 +149,48 @@
         else:
             # Add 3 for '#!' prefix and newline suffix.
             shebang_length = len(executable) + len(post_interp) + 3
             if sys.platform == 'darwin':
                 max_shebang_length = 512
             else:
                 max_shebang_length = 127
-            simple_shebang = ((b' ' not in executable) and
-                              (shebang_length <= max_shebang_length))
+            simple_shebang = ((b' ' not in executable)
+                              and (shebang_length <= max_shebang_length))
 
         if simple_shebang:
             result = b'#!' + executable + post_interp + b'\n'
         else:
             result = b'#!/bin/sh\n'
             result += b"'''exec' " + executable + post_interp + b' "$0" "$@"\n'
             result += b"' '''"
         return result
 
     def _get_shebang(self, encoding, post_interp=b'', options=None):
         enquote = True
         if self.executable:
             executable = self.executable
-            enquote = False     # assume this will be taken care of
+            enquote = False  # assume this will be taken care of
         elif not sysconfig.is_python_build():
             executable = get_executable()
         elif in_venv():  # pragma: no cover
-            executable = os.path.join(sysconfig.get_path('scripts'),
-                            'python%s' % sysconfig.get_config_var('EXE'))
-        else:  # pragma: no cover
             executable = os.path.join(
-                sysconfig.get_config_var('BINDIR'),
-               'python%s%s' % (sysconfig.get_config_var('VERSION'),
-                               sysconfig.get_config_var('EXE')))
-            if not os.path.isfile(executable):
+                sysconfig.get_path('scripts'),
+                'python%s' % sysconfig.get_config_var('EXE'))
+        else:  # pragma: no cover
+            if os.name == 'nt':
                 # for Python builds from source on Windows, no Python executables with
                 # a version suffix are created, so we use python.exe
-                executable = os.path.join(sysconfig.get_config_var('BINDIR'),
-                                'python%s' % (sysconfig.get_config_var('EXE')))
+                executable = os.path.join(
+                    sysconfig.get_config_var('BINDIR'),
+                    'python%s' % (sysconfig.get_config_var('EXE')))
+            else:
+                executable = os.path.join(
+                    sysconfig.get_config_var('BINDIR'),
+                    'python%s%s' % (sysconfig.get_config_var('VERSION'),
+                                    sysconfig.get_config_var('EXE')))
         if options:
             executable = self._get_alternate_executable(executable, options)
 
         if sys.platform.startswith('java'):  # pragma: no cover
             executable = self._fix_jython_executable(executable)
 
         # Normalise case for Windows - COMMENTED OUT
@@ -197,43 +207,44 @@
         if enquote:
             executable = enquote_executable(executable)
         # Issue #51: don't use fsencode, since we later try to
         # check that the shebang is decodable using utf-8.
         executable = executable.encode('utf-8')
         # in case of IronPython, play safe and enable frames support
         if (sys.platform == 'cli' and '-X:Frames' not in post_interp
-            and '-X:FullFrames' not in post_interp):  # pragma: no cover
+                and '-X:FullFrames' not in post_interp):  # pragma: no cover
             post_interp += b' -X:Frames'
         shebang = self._build_shebang(executable, post_interp)
         # Python parser starts to read a script using UTF-8 until
         # it gets a #coding:xxx cookie. The shebang has to be the
         # first line of a file, the #coding:xxx cookie cannot be
         # written before. So the shebang has to be decodable from
         # UTF-8.
         try:
             shebang.decode('utf-8')
         except UnicodeDecodeError:  # pragma: no cover
-            raise ValueError(
-                'The shebang (%r) is not decodable from utf-8' % shebang)
+            raise ValueError('The shebang (%r) is not decodable from utf-8' %
+                             shebang)
         # If the script is encoded to a custom encoding (use a
         # #coding:xxx cookie), the shebang has to be decodable from
         # the script encoding too.
         if encoding != 'utf-8':
             try:
                 shebang.decode(encoding)
             except UnicodeDecodeError:  # pragma: no cover
-                raise ValueError(
-                    'The shebang (%r) is not decodable '
-                    'from the script encoding (%r)' % (shebang, encoding))
+                raise ValueError('The shebang (%r) is not decodable '
+                                 'from the script encoding (%r)' %
+                                 (shebang, encoding))
         return shebang
 
     def _get_script_text(self, entry):
-        return self.script_template % dict(module=entry.prefix,
-                                           import_name=entry.suffix.split('.')[0],
-                                           func=entry.suffix)
+        return self.script_template % dict(
+            module=entry.prefix,
+            import_name=entry.suffix.split('.')[0],
+            func=entry.suffix)
 
     manifest = _DEFAULT_MANIFEST
 
     def get_manifest(self, exename):
         base = os.path.basename(exename)
         return self.manifest % base
 
@@ -250,15 +261,16 @@
             else:
                 launcher = self._get_launcher('w')
             stream = BytesIO()
             with ZipFile(stream, 'w') as zf:
                 source_date_epoch = os.environ.get('SOURCE_DATE_EPOCH')
                 if source_date_epoch:
                     date_time = time.gmtime(int(source_date_epoch))[:6]
-                    zinfo = ZipInfo(filename='__main__.py', date_time=date_time)
+                    zinfo = ZipInfo(filename='__main__.py',
+                                    date_time=date_time)
                     zf.writestr(zinfo, script_bytes)
                 else:
                     zf.writestr('__main__.py', script_bytes)
             zip_data = stream.getvalue()
             script_bytes = launcher + shebang + zip_data
         for name in names:
             outname = os.path.join(self.target_dir, name)
@@ -271,25 +283,26 @@
                     self._fileop.write_binary_file(outname, script_bytes)
                 except Exception:
                     # Failed writing an executable - it might be in use.
                     logger.warning('Failed to write executable - trying to '
                                    'use .deleteme logic')
                     dfname = '%s.deleteme' % outname
                     if os.path.exists(dfname):
-                        os.remove(dfname)       # Not allowed to fail here
+                        os.remove(dfname)  # Not allowed to fail here
                     os.rename(outname, dfname)  # nor here
                     self._fileop.write_binary_file(outname, script_bytes)
                     logger.debug('Able to replace executable using '
                                  '.deleteme logic')
                     try:
                         os.remove(dfname)
                     except Exception:
-                        pass    # still in use - ignore error
+                        pass  # still in use - ignore error
             else:
-                if self._is_nt and not outname.endswith('.' + ext):  # pragma: no cover
+                if self._is_nt and not outname.endswith(
+                        '.' + ext):  # pragma: no cover
                     outname = '%s.%s' % (outname, ext)
                 if os.path.exists(outname) and not self.clobber:
                     logger.warning('Skipping existing file %s', outname)
                     continue
                 self._fileop.write_binary_file(outname, script_bytes)
                 if self.set_mode:
                     self._fileop.set_executable_mode([outname])
@@ -300,16 +313,17 @@
     def get_script_filenames(self, name):
         result = set()
         if '' in self.variants:
             result.add(name)
         if 'X' in self.variants:
             result.add('%s%s' % (name, self.version_info[0]))
         if 'X.Y' in self.variants:
-            result.add('%s%s%s.%s' % (name, self.variant_separator,
-                                      self.version_info[0], self.version_info[1]))
+            result.add('%s%s%s.%s' %
+                       (name, self.variant_separator, self.version_info[0],
+                        self.version_info[1]))
         return result
 
     def _make_script(self, entry, filenames, options=None):
         post_interp = b''
         if options:
             args = options.get('interpreter_args', [])
             if args:
@@ -379,32 +393,33 @@
     def dry_run(self):
         return self._fileop.dry_run
 
     @dry_run.setter
     def dry_run(self, value):
         self._fileop.dry_run = value
 
-    if os.name == 'nt' or (os.name == 'java' and os._name == 'nt'):  # pragma: no cover
+    if os.name == 'nt' or (os.name == 'java'
+                           and os._name == 'nt'):  # pragma: no cover
         # Executable launcher support.
         # Launchers are from https://bitbucket.org/vinay.sajip/simple_launcher/
 
         def _get_launcher(self, kind):
-            if struct.calcsize('P') == 8:   # 64-bit
+            if struct.calcsize('P') == 8:  # 64-bit
                 bits = '64'
             else:
                 bits = '32'
             platform_suffix = '-arm' if get_platform() == 'win-arm64' else ''
             name = '%s%s%s.exe' % (kind, bits, platform_suffix)
             # Issue 31: don't hardcode an absolute package name, but
             # determine it relative to the current package
             distlib_package = __name__.rsplit('.', 1)[0]
             resource = finder(distlib_package).find(name)
             if not resource:
-                msg = ('Unable to find resource %s in package %s' % (name,
-                       distlib_package))
+                msg = ('Unable to find resource %s in package %s' %
+                       (name, distlib_package))
                 raise ValueError(msg)
             return resource.bytes
 
     # Public API follows
 
     def make(self, specification, options=None):
         """
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/t32.exe` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/t64.exe` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/util.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2012-2021 The Python Software Foundation.
+# Copyright (C) 2012-2023 The Python Software Foundation.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 import codecs
 from collections import deque
 import contextlib
 import csv
 from glob import iglob as std_iglob
@@ -29,15 +29,15 @@
 except ImportError:  # pragma: no cover
     import dummy_threading as threading
 import time
 
 from . import DistlibException
 from .compat import (string_types, text_type, shutil, raw_input, StringIO,
                      cache_from_source, urlopen, urljoin, httplib, xmlrpclib,
-                     splittype, HTTPHandler, BaseConfigurator, valid_ident,
+                     HTTPHandler, BaseConfigurator, valid_ident,
                      Container, configparser, URLError, ZipFile, fsdecode,
                      unquote, urlparse)
 
 logger = logging.getLogger(__name__)
 
 #
 # Requirement parsing code as per PEP 508
@@ -58,14 +58,15 @@
     Parse a marker string and return a dictionary containing a marker expression.
 
     The dictionary will contain keys "op", "lhs" and "rhs" for non-terminals in
     the expression grammar, or strings. A string contained in quotes is to be
     interpreted as a literal string, and a string not contained in quotes is a
     variable (such as os_name).
     """
+
     def marker_var(remaining):
         # either identifier, or literal string
         m = IDENTIFIER.match(remaining)
         if m:
             result = m.groups()[0]
             remaining = remaining[m.end():]
         elif not remaining:
@@ -83,23 +84,24 @@
                     break
                 elif remaining[0] == oq:
                     parts.append(oq)
                     remaining = remaining[1:]
                 else:
                     m = STRING_CHUNK.match(remaining)
                     if not m:
-                        raise SyntaxError('error in string literal: %s' % remaining)
+                        raise SyntaxError('error in string literal: %s' %
+                                          remaining)
                     parts.append(m.groups()[0])
                     remaining = remaining[m.end():]
             else:
                 s = ''.join(parts)
                 raise SyntaxError('unterminated string: %s' % s)
             parts.append(q)
             result = ''.join(parts)
-            remaining = remaining[1:].lstrip() # skip past closing quote
+            remaining = remaining[1:].lstrip()  # skip past closing quote
         return result, remaining
 
     def marker_expr(remaining):
         if remaining and remaining[0] == '(':
             result, remaining = marker(remaining[1:].lstrip())
             if remaining[0] != ')':
                 raise SyntaxError('unterminated parenthesis: %s' % remaining)
@@ -204,38 +206,41 @@
                 if m:
                     versions = []
                     while True:
                         op = m.groups()[0]
                         ver_remaining = ver_remaining[m.end():]
                         m = VERSION_IDENTIFIER.match(ver_remaining)
                         if not m:
-                            raise SyntaxError('invalid version: %s' % ver_remaining)
+                            raise SyntaxError('invalid version: %s' %
+                                              ver_remaining)
                         v = m.groups()[0]
                         versions.append((op, v))
                         ver_remaining = ver_remaining[m.end():]
                         if not ver_remaining or ver_remaining[0] != ',':
                             break
                         ver_remaining = ver_remaining[1:].lstrip()
                         # Some packages have a trailing comma which would break things
                         # See issue #148
                         if not ver_remaining:
                             break
                         m = COMPARE_OP.match(ver_remaining)
                         if not m:
-                            raise SyntaxError('invalid constraint: %s' % ver_remaining)
+                            raise SyntaxError('invalid constraint: %s' %
+                                              ver_remaining)
                     if not versions:
                         versions = None
                 return versions, ver_remaining
 
             if remaining[0] != '(':
                 versions, remaining = get_versions(remaining)
             else:
                 i = remaining.find(')', 1)
                 if i < 0:
-                    raise SyntaxError('unterminated parenthesis: %s' % remaining)
+                    raise SyntaxError('unterminated parenthesis: %s' %
+                                      remaining)
                 s = remaining[1:i]
                 remaining = remaining[i + 1:].lstrip()
                 # As a special diversion from PEP 508, allow a version number
                 # a.b.c in parentheses as a synonym for ~= a.b.c (because this
                 # is allowed in earlier PEPs)
                 if COMPARE_OP.match(s):
                     versions, _ = get_versions(s)
@@ -258,17 +263,22 @@
 
     if remaining and remaining[0] != '#':
         raise SyntaxError('unexpected trailing data: %s' % remaining)
 
     if not versions:
         rs = distname
     else:
-        rs = '%s %s' % (distname, ', '.join(['%s %s' % con for con in versions]))
-    return Container(name=distname, extras=extras, constraints=versions,
-                     marker=mark_expr, url=uri, requirement=rs)
+        rs = '%s %s' % (distname, ', '.join(
+            ['%s %s' % con for con in versions]))
+    return Container(name=distname,
+                     extras=extras,
+                     constraints=versions,
+                     marker=mark_expr,
+                     url=uri,
+                     requirement=rs)
 
 
 def get_resources_dests(resources_root, rules):
     """Find destinations for resources files"""
 
     def get_rel_path(root, path):
         # normalizes and returns a lstripped-/-separated path
@@ -300,23 +310,23 @@
     else:
         # PEP 405 venvs
         result = sys.prefix != getattr(sys, 'base_prefix', sys.prefix)
     return result
 
 
 def get_executable():
-# The __PYVENV_LAUNCHER__ dance is apparently no longer needed, as
-# changes to the stub launcher mean that sys.executable always points
-# to the stub on OS X
-#    if sys.platform == 'darwin' and ('__PYVENV_LAUNCHER__'
-#                                     in os.environ):
-#        result =  os.environ['__PYVENV_LAUNCHER__']
-#    else:
-#        result = sys.executable
-#    return result
+    # The __PYVENV_LAUNCHER__ dance is apparently no longer needed, as
+    # changes to the stub launcher mean that sys.executable always points
+    # to the stub on OS X
+    #    if sys.platform == 'darwin' and ('__PYVENV_LAUNCHER__'
+    #                                     in os.environ):
+    #        result =  os.environ['__PYVENV_LAUNCHER__']
+    #    else:
+    #        result = sys.executable
+    #    return result
     # Avoid normcasing: see issue #143
     # result = os.path.normcase(sys.executable)
     result = sys.executable
     if not isinstance(result, text_type):
         result = fsdecode(result)
     return result
 
@@ -342,14 +352,15 @@
         keys = keys.split()
     result = {}
     for key in keys:
         if key in d:
             result[key] = d[key]
     return result
 
+
 def read_exports(stream):
     if sys.version_info[0] >= 3:
         # needs to be a text stream
         stream = codecs.getreader('utf-8')(stream)
     # Try to load as JSON, falling back on legacy format
     data = stream.read()
     stream = StringIO(data)
@@ -384,15 +395,15 @@
     result = {}
     for key in cp.sections():
         result[key] = entries = {}
         for name, value in cp.items(key):
             s = '%s = %s' % (name, value)
             entry = get_export_entry(s)
             assert entry is not None
-            #entry.dist = self
+            # entry.dist = self
             entries[name] = entry
     return result
 
 
 def write_exports(exports, stream):
     if sys.version_info[0] >= 3:
         # needs to be a text stream
@@ -416,14 +427,15 @@
 def tempdir():
     td = tempfile.mkdtemp()
     try:
         yield td
     finally:
         shutil.rmtree(td)
 
+
 @contextlib.contextmanager
 def chdir(d):
     cwd = os.getcwd()
     try:
         os.chdir(d)
         yield
     finally:
@@ -437,27 +449,29 @@
         socket.setdefaulttimeout(seconds)
         yield
     finally:
         socket.setdefaulttimeout(cto)
 
 
 class cached_property(object):
+
     def __init__(self, func):
         self.func = func
-        #for attr in ('__name__', '__module__', '__doc__'):
-        #    setattr(self, attr, getattr(func, attr, None))
+        # for attr in ('__name__', '__module__', '__doc__'):
+        #     setattr(self, attr, getattr(func, attr, None))
 
     def __get__(self, obj, cls=None):
         if obj is None:
             return self
         value = self.func(obj)
         object.__setattr__(obj, self.func.__name__, value)
-        #obj.__dict__[self.func.__name__] = value = self.func(obj)
+        # obj.__dict__[self.func.__name__] = value = self.func(obj)
         return value
 
+
 def convert_path(pathname):
     """Return 'pathname' as a name that will work on the native filesystem.
 
     The path is split on '/' and put back together again using the current
     directory separator.  Needed because filenames in the setup script are
     always supplied in Unix style, and have to be converted to the local
     convention before we can actually use them in the filesystem.  Raises
@@ -478,14 +492,15 @@
         paths.remove(os.curdir)
     if not paths:
         return os.curdir
     return os.path.join(*paths)
 
 
 class FileOperator(object):
+
     def __init__(self, dry_run=False):
         self.dry_run = dry_run
         self.ensured = set()
         self._init_record()
 
     def _init_record(self):
         self.record = False
@@ -582,28 +597,36 @@
             self.ensure_dir(d)
             logger.info('Creating %s' % path)
             if not self.dry_run:
                 os.mkdir(path)
             if self.record:
                 self.dirs_created.add(path)
 
-    def byte_compile(self, path, optimize=False, force=False, prefix=None, hashed_invalidation=False):
+    def byte_compile(self,
+                     path,
+                     optimize=False,
+                     force=False,
+                     prefix=None,
+                     hashed_invalidation=False):
         dpath = cache_from_source(path, not optimize)
         logger.info('Byte-compiling %s to %s', path, dpath)
         if not self.dry_run:
             if force or self.newer(path, dpath):
                 if not prefix:
                     diagpath = None
                 else:
                     assert path.startswith(prefix)
                     diagpath = path[len(prefix):]
             compile_kwargs = {}
-            if hashed_invalidation and hasattr(py_compile, 'PycInvalidationMode'):
-                compile_kwargs['invalidation_mode'] = py_compile.PycInvalidationMode.CHECKED_HASH
-            py_compile.compile(path, dpath, diagpath, True, **compile_kwargs)     # raise error
+            if hashed_invalidation and hasattr(py_compile,
+                                               'PycInvalidationMode'):
+                compile_kwargs[
+                    'invalidation_mode'] = py_compile.PycInvalidationMode.CHECKED_HASH
+            py_compile.compile(path, dpath, diagpath, True,
+                               **compile_kwargs)  # raise error
         self.record_as_written(dpath)
         return dpath
 
     def ensure_removed(self, path):
         if os.path.exists(path):
             if os.path.isdir(path) and not os.path.islink(path):
                 logger.debug('Removing directory tree at %s', path)
@@ -657,17 +680,18 @@
             dirs = sorted(self.dirs_created, reverse=True)
             for d in dirs:
                 flist = os.listdir(d)
                 if flist:
                     assert flist == ['__pycache__']
                     sd = os.path.join(d, flist[0])
                     os.rmdir(sd)
-                os.rmdir(d)     # should fail if non-empty
+                os.rmdir(d)  # should fail if non-empty
         self._init_record()
 
+
 def resolve(module_name, dotted_path):
     if module_name in sys.modules:
         mod = sys.modules[module_name]
     else:
         mod = __import__(module_name)
     if dotted_path is None:
         result = mod
@@ -676,14 +700,15 @@
         result = getattr(mod, parts.pop(0))
         for p in parts:
             result = getattr(result, p)
     return result
 
 
 class ExportEntry(object):
+
     def __init__(self, name, prefix, suffix, flags):
         self.name = name
         self.prefix = prefix
         self.suffix = suffix
         self.flags = flags
 
     @cached_property
@@ -694,28 +719,29 @@
         return '<ExportEntry %s = %s:%s %s>' % (self.name, self.prefix,
                                                 self.suffix, self.flags)
 
     def __eq__(self, other):
         if not isinstance(other, ExportEntry):
             result = False
         else:
-            result = (self.name == other.name and
-                      self.prefix == other.prefix and
-                      self.suffix == other.suffix and
-                      self.flags == other.flags)
+            result = (self.name == other.name and self.prefix == other.prefix
+                      and self.suffix == other.suffix
+                      and self.flags == other.flags)
         return result
 
     __hash__ = object.__hash__
 
 
-ENTRY_RE = re.compile(r'''(?P<name>(\w|[-.+])+)
+ENTRY_RE = re.compile(
+    r'''(?P<name>([^\[]\S*))
                       \s*=\s*(?P<callable>(\w+)([:\.]\w+)*)
                       \s*(\[\s*(?P<flags>[\w-]+(=\w+)?(,\s*\w+(=\w+)?)*)\s*\])?
                       ''', re.VERBOSE)
 
+
 def get_export_entry(specification):
     m = ENTRY_RE.search(specification)
     if not m:
         result = None
         if '[' in specification or ']' in specification:
             raise DistlibException("Invalid specification "
                                    "'%s'" % specification)
@@ -823,26 +849,29 @@
 
 
 def get_process_umask():
     result = os.umask(0o22)
     os.umask(result)
     return result
 
+
 def is_string_sequence(seq):
     result = True
     i = None
     for i, s in enumerate(seq):
         if not isinstance(s, string_types):
             result = False
             break
     assert i is not None
     return result
 
-PROJECT_NAME_AND_VERSION = re.compile('([a-z0-9_]+([.-][a-z_][a-z0-9_]*)*)-'
-                                      '([a-z0-9_.+-]+)', re.I)
+
+PROJECT_NAME_AND_VERSION = re.compile(
+    '([a-z0-9_]+([.-][a-z_][a-z0-9_]*)*)-'
+    '([a-z0-9_.+-]+)', re.I)
 PYTHON_VERSION = re.compile(r'-py(\d\.?\d?)')
 
 
 def split_filename(filename, project_name=None):
     """
     Extract name, version, python version from a filename (no extension)
 
@@ -862,18 +891,20 @@
             result = filename[:n], filename[n + 1:], pyver
     if result is None:
         m = PROJECT_NAME_AND_VERSION.match(filename)
         if m:
             result = m.group(1), m.group(3), pyver
     return result
 
+
 # Allow spaces in name because of legacy dists like "Twisted Core"
 NAME_VERSION_RE = re.compile(r'(?P<name>[\w .-]+)\s*'
                              r'\(\s*(?P<ver>[^\s)]+)\)$')
 
+
 def parse_name_and_version(p):
     """
     A utility method used to get name and version from a string.
 
     From e.g. a Provides-Dist value.
 
     :param p: A value in a form 'foo (1.0)'
@@ -881,14 +912,15 @@
     """
     m = NAME_VERSION_RE.match(p)
     if not m:
         raise DistlibException('Ill-formed name/version string: \'%s\'' % p)
     d = m.groupdict()
     return d['name'].strip().lower(), d['ver']
 
+
 def get_extras(requested, available):
     result = set()
     requested = set(requested or [])
     available = set(available or [])
     if '*' in requested:
         requested.remove('*')
         result |= available
@@ -902,46 +934,52 @@
             if unwanted in result:
                 result.remove(unwanted)
         else:
             if r not in available:
                 logger.warning('undeclared extra: %s' % r)
             result.add(r)
     return result
+
+
 #
 # Extended metadata functionality
 #
 
+
 def _get_external_data(url):
     result = {}
     try:
         # urlopen might fail if it runs into redirections,
         # because of Python issue #13696. Fixed in locators
         # using a custom redirect handler.
         resp = urlopen(url)
         headers = resp.info()
         ct = headers.get('Content-Type')
         if not ct.startswith('application/json'):
             logger.debug('Unexpected response for JSON request: %s', ct)
         else:
             reader = codecs.getreader('utf-8')(resp)
-            #data = reader.read().decode('utf-8')
-            #result = json.loads(data)
+            # data = reader.read().decode('utf-8')
+            # result = json.loads(data)
             result = json.load(reader)
     except Exception as e:
         logger.exception('Failed to get external data for %s: %s', url, e)
     return result
 
+
 _external_data_base_url = 'https://www.red-dove.com/pypi/projects/'
 
+
 def get_project_data(name):
     url = '%s/%s/project.json' % (name[0].upper(), name)
     url = urljoin(_external_data_base_url, url)
     result = _get_external_data(url)
     return result
 
+
 def get_package_data(name, version):
     url = '%s/%s/package-%s.json' % (name[0].upper(), name, version)
     url = urljoin(_external_data_base_url, url)
     return _get_external_data(url)
 
 
 class Cache(object):
@@ -988,14 +1026,15 @@
         return not_removed
 
 
 class EventMixin(object):
     """
     A very simple publish/subscribe system.
     """
+
     def __init__(self):
         self._subscribers = {}
 
     def add(self, event, subscriber, append=True):
         """
         Add a subscriber for an event.
 
@@ -1049,26 +1088,28 @@
         for subscriber in self.get_subscribers(event):
             try:
                 value = subscriber(event, *args, **kwargs)
             except Exception:
                 logger.exception('Exception during event publication')
                 value = None
             result.append(value)
-        logger.debug('publish %s: args = %s, kwargs = %s, result = %s',
-                     event, args, kwargs, result)
+        logger.debug('publish %s: args = %s, kwargs = %s, result = %s', event,
+                     args, kwargs, result)
         return result
 
+
 #
 # Simple sequencing
 #
 class Sequencer(object):
+
     def __init__(self):
         self._preds = {}
         self._succs = {}
-        self._nodes = set()     # nodes with no preds/succs
+        self._nodes = set()  # nodes with no preds/succs
 
     def add_node(self, node):
         self._nodes.add(node)
 
     def remove_node(self, node, edges=False):
         if node in self._nodes:
             self._nodes.remove(node)
@@ -1100,16 +1141,16 @@
         try:
             preds.remove(pred)
             succs.remove(succ)
         except KeyError:  # pragma: no cover
             raise ValueError('%r not a successor of %r' % (succ, pred))
 
     def is_step(self, step):
-        return (step in self._preds or step in self._succs or
-                step in self._nodes)
+        return (step in self._preds or step in self._succs
+                or step in self._nodes)
 
     def get_steps(self, final):
         if not self.is_step(final):
             raise ValueError('Unknown: %r' % final)
         result = []
         todo = []
         seen = set()
@@ -1130,15 +1171,15 @@
                 result.append(step)
                 preds = self._preds.get(step, ())
                 todo.extend(preds)
         return reversed(result)
 
     @property
     def strong_connections(self):
-        #http://en.wikipedia.org/wiki/Tarjan%27s_strongly_connected_components_algorithm
+        # http://en.wikipedia.org/wiki/Tarjan%27s_strongly_connected_components_algorithm
         index_counter = [0]
         stack = []
         lowlinks = {}
         index = {}
         result = []
 
         graph = self._succs
@@ -1155,28 +1196,29 @@
                 successors = graph[node]
             except Exception:
                 successors = []
             for successor in successors:
                 if successor not in lowlinks:
                     # Successor has not yet been visited
                     strongconnect(successor)
-                    lowlinks[node] = min(lowlinks[node],lowlinks[successor])
+                    lowlinks[node] = min(lowlinks[node], lowlinks[successor])
                 elif successor in stack:
                     # the successor is in the stack and hence in the current
                     # strongly connected component (SCC)
-                    lowlinks[node] = min(lowlinks[node],index[successor])
+                    lowlinks[node] = min(lowlinks[node], index[successor])
 
             # If `node` is a root node, pop the stack and generate an SCC
             if lowlinks[node] == index[node]:
                 connected_component = []
 
                 while True:
                     successor = stack.pop()
                     connected_component.append(successor)
-                    if successor == node: break
+                    if successor == node:
+                        break
                 component = tuple(connected_component)
                 # storing the result
                 result.append(component)
 
         for node in graph:
             if node not in lowlinks:
                 strongconnect(node)
@@ -1191,20 +1233,22 @@
             for pred in preds:
                 result.append('  %s -> %s;' % (pred, succ))
         for node in self._nodes:
             result.append('  %s;' % node)
         result.append('}')
         return '\n'.join(result)
 
+
 #
 # Unarchiving functionality for zip, tar, tgz, tbz, whl
 #
 
-ARCHIVE_EXTENSIONS = ('.tar.gz', '.tar.bz2', '.tar', '.zip',
-                      '.tgz', '.tbz', '.whl')
+ARCHIVE_EXTENSIONS = ('.tar.gz', '.tar.bz2', '.tar', '.zip', '.tgz', '.tbz',
+                      '.whl')
+
 
 def unarchive(archive_filename, dest_dir, format=None, check=True):
 
     def check_path(path):
         if not isinstance(path, text_type):
             path = path.decode('utf-8')
         p = os.path.abspath(os.path.join(dest_dir, path))
@@ -1245,14 +1289,28 @@
             # See Python issue 17153. If the dest path contains Unicode,
             # tarfile extraction fails on Python 2.x if a member path name
             # contains non-ASCII characters - it leads to an implicit
             # bytes -> unicode conversion using ASCII to decode.
             for tarinfo in archive.getmembers():
                 if not isinstance(tarinfo.name, text_type):
                     tarinfo.name = tarinfo.name.decode('utf-8')
+
+        # Limit extraction of dangerous items, if this Python
+        # allows it easily. If not, just trust the input.
+        # See: https://docs.python.org/3/library/tarfile.html#extraction-filters
+        def extraction_filter(member, path):
+            """Run tarfile.tar_filter, but raise the expected ValueError"""
+            # This is only called if the current Python has tarfile filters
+            try:
+                return tarfile.tar_filter(member, path)
+            except tarfile.FilterError as exc:
+                raise ValueError(str(exc))
+
+        archive.extraction_filter = extraction_filter
+
         archive.extractall(dest_dir)
 
     finally:
         if archive:
             archive.close()
 
 
@@ -1265,19 +1323,20 @@
             for name in files:
                 full = os.path.join(root, name)
                 rel = root[dlen:]
                 dest = os.path.join(rel, name)
                 zf.write(full, dest)
     return result
 
+
 #
 # Simple progress bar
 #
 
-UNITS = ('', 'K', 'M', 'G','T','P')
+UNITS = ('', 'K', 'M', 'G', 'T', 'P')
 
 
 class Progress(object):
     unknown = 'UNKNOWN'
 
     def __init__(self, minval=0, maxval=100):
         assert maxval is None or maxval >= minval
@@ -1324,34 +1383,34 @@
             v = 100.0 * (self.cur - self.min) / (self.max - self.min)
             result = '%3d %%' % v
         return result
 
     def format_duration(self, duration):
         if (duration <= 0) and self.max is None or self.cur == self.min:
             result = '??:??:??'
-        #elif duration < 1:
-        #    result = '--:--:--'
+        # elif duration < 1:
+        #     result = '--:--:--'
         else:
             result = time.strftime('%H:%M:%S', time.gmtime(duration))
         return result
 
     @property
     def ETA(self):
         if self.done:
             prefix = 'Done'
             t = self.elapsed
-            #import pdb; pdb.set_trace()
+            # import pdb; pdb.set_trace()
         else:
             prefix = 'ETA '
             if self.max is None:
                 t = -1
             elif self.elapsed == 0 or (self.cur == self.min):
                 t = 0
             else:
-                #import pdb; pdb.set_trace()
+                # import pdb; pdb.set_trace()
                 t = float(self.max - self.min)
                 t /= self.cur - self.min
                 t = (t - 1) * self.elapsed
         return '%s: %s' % (prefix, self.format_duration(t))
 
     @property
     def speed(self):
@@ -1361,14 +1420,15 @@
             result = (self.cur - self.min) / self.elapsed
         for unit in UNITS:
             if result < 1000:
                 break
             result /= 1000.0
         return '%d %sB/s' % (result, unit)
 
+
 #
 # Glob functionality
 #
 
 RICH_GLOB = re.compile(r'\{([^}]*)\}')
 _CHECK_RECURSIVE_GLOB = re.compile(r'[^/\\,{]\*\*|\*\*[^/\\,}]')
 _CHECK_MISMATCH_SET = re.compile(r'^[^{]*\}|\{[^}]*$')
@@ -1408,38 +1468,39 @@
                 radical = radical.lstrip('/')
                 radical = radical.lstrip('\\')
             for path, dir, files in os.walk(prefix):
                 path = os.path.normpath(path)
                 for fn in _iglob(os.path.join(path, radical)):
                     yield fn
 
+
 if ssl:
     from .compat import (HTTPSHandler as BaseHTTPSHandler, match_hostname,
                          CertificateError)
 
-
-#
-# HTTPSConnection which verifies certificates/matches domains
-#
+    #
+    # HTTPSConnection which verifies certificates/matches domains
+    #
 
     class HTTPSConnection(httplib.HTTPSConnection):
-        ca_certs = None # set this to the path to the certs file (.pem)
-        check_domain = True # only used if ca_certs is not None
+        ca_certs = None  # set this to the path to the certs file (.pem)
+        check_domain = True  # only used if ca_certs is not None
 
         # noinspection PyPropertyAccess
         def connect(self):
-            sock = socket.create_connection((self.host, self.port), self.timeout)
+            sock = socket.create_connection((self.host, self.port),
+                                            self.timeout)
             if getattr(self, '_tunnel_host', False):
                 self.sock = sock
                 self._tunnel()
 
             context = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
             if hasattr(ssl, 'OP_NO_SSLv2'):
                 context.options |= ssl.OP_NO_SSLv2
-            if self.cert_file:
+            if getattr(self, 'cert_file', None):
                 context.load_cert_chain(self.cert_file, self.key_file)
             kwargs = {}
             if self.ca_certs:
                 context.verify_mode = ssl.CERT_REQUIRED
                 context.load_verify_locations(cafile=self.ca_certs)
                 if getattr(ssl, 'HAS_SNI', False):
                     kwargs['server_hostname'] = self.host
@@ -1451,14 +1512,15 @@
                     logger.debug('Host verified: %s', self.host)
                 except CertificateError:  # pragma: no cover
                     self.sock.shutdown(socket.SHUT_RDWR)
                     self.sock.close()
                     raise
 
     class HTTPSHandler(BaseHTTPSHandler):
+
         def __init__(self, ca_certs, check_domain=True):
             BaseHTTPSHandler.__init__(self)
             self.ca_certs = ca_certs
             self.check_domain = check_domain
 
         def _conn_maker(self, *args, **kwargs):
             """
@@ -1477,67 +1539,76 @@
             return result
 
         def https_open(self, req):
             try:
                 return self.do_open(self._conn_maker, req)
             except URLError as e:
                 if 'certificate verify failed' in str(e.reason):
-                    raise CertificateError('Unable to verify server certificate '
-                                           'for %s' % req.host)
+                    raise CertificateError(
+                        'Unable to verify server certificate '
+                        'for %s' % req.host)
                 else:
                     raise
 
     #
     # To prevent against mixing HTTP traffic with HTTPS (examples: A Man-In-The-
     # Middle proxy using HTTP listens on port 443, or an index mistakenly serves
     # HTML containing a http://xyz link when it should be https://xyz),
     # you can use the following handler class, which does not allow HTTP traffic.
     #
     # It works by inheriting from HTTPHandler - so build_opener won't add a
     # handler for HTTP itself.
     #
     class HTTPSOnlyHandler(HTTPSHandler, HTTPHandler):
+
         def http_open(self, req):
-            raise URLError('Unexpected HTTP request on what should be a secure '
-                           'connection: %s' % req)
+            raise URLError(
+                'Unexpected HTTP request on what should be a secure '
+                'connection: %s' % req)
+
 
 #
 # XML-RPC with timeouts
 #
 class Transport(xmlrpclib.Transport):
+
     def __init__(self, timeout, use_datetime=0):
         self.timeout = timeout
         xmlrpclib.Transport.__init__(self, use_datetime)
 
     def make_connection(self, host):
         h, eh, x509 = self.get_host_info(host)
         if not self._connection or host != self._connection[0]:
             self._extra_headers = eh
             self._connection = host, httplib.HTTPConnection(h)
         return self._connection[1]
 
+
 if ssl:
+
     class SafeTransport(xmlrpclib.SafeTransport):
+
         def __init__(self, timeout, use_datetime=0):
             self.timeout = timeout
             xmlrpclib.SafeTransport.__init__(self, use_datetime)
 
         def make_connection(self, host):
             h, eh, kwargs = self.get_host_info(host)
             if not kwargs:
                 kwargs = {}
             kwargs['timeout'] = self.timeout
             if not self._connection or host != self._connection[0]:
                 self._extra_headers = eh
-                self._connection = host, httplib.HTTPSConnection(h, None,
-                                                                 **kwargs)
+                self._connection = host, httplib.HTTPSConnection(
+                    h, None, **kwargs)
             return self._connection[1]
 
 
 class ServerProxy(xmlrpclib.ServerProxy):
+
     def __init__(self, uri, **kwargs):
         self.timeout = timeout = kwargs.pop('timeout', None)
         # The above classes only come into play if a timeout
         # is specified
         if timeout is not None:
             # scheme = splittype(uri)  # deprecated as of Python 3.8
             scheme = urlparse(uri)[0]
@@ -1546,45 +1617,48 @@
                 tcls = SafeTransport
             else:
                 tcls = Transport
             kwargs['transport'] = t = tcls(timeout, use_datetime=use_datetime)
             self.transport = t
         xmlrpclib.ServerProxy.__init__(self, uri, **kwargs)
 
+
 #
 # CSV functionality. This is provided because on 2.x, the csv module can't
 # handle Unicode. However, we need to deal with Unicode in e.g. RECORD files.
 #
 
+
 def _csv_open(fn, mode, **kwargs):
     if sys.version_info[0] < 3:
         mode += 'b'
     else:
         kwargs['newline'] = ''
         # Python 3 determines encoding from locale. Force 'utf-8'
         # file encoding to match other forced utf-8 encoding
         kwargs['encoding'] = 'utf-8'
     return open(fn, mode, **kwargs)
 
 
 class CSVBase(object):
     defaults = {
-        'delimiter': str(','),      # The strs are used because we need native
-        'quotechar': str('"'),      # str in the csv API (2.x won't take
-        'lineterminator': str('\n') # Unicode)
+        'delimiter': str(','),  # The strs are used because we need native
+        'quotechar': str('"'),  # str in the csv API (2.x won't take
+        'lineterminator': str('\n')  # Unicode)
     }
 
     def __enter__(self):
         return self
 
     def __exit__(self, *exc_info):
         self.stream.close()
 
 
 class CSVReader(CSVBase):
+
     def __init__(self, **kwargs):
         if 'stream' in kwargs:
             stream = kwargs['stream']
             if sys.version_info[0] >= 3:
                 # needs to be a text stream
                 stream = codecs.getreader('utf-8')(stream)
             self.stream = stream
@@ -1601,43 +1675,48 @@
             for i, item in enumerate(result):
                 if not isinstance(item, text_type):
                     result[i] = item.decode('utf-8')
         return result
 
     __next__ = next
 
+
 class CSVWriter(CSVBase):
+
     def __init__(self, fn, **kwargs):
         self.stream = _csv_open(fn, 'w')
         self.writer = csv.writer(self.stream, **self.defaults)
 
     def writerow(self, row):
         if sys.version_info[0] < 3:
             r = []
             for item in row:
                 if isinstance(item, text_type):
                     item = item.encode('utf-8')
                 r.append(item)
             row = r
         self.writer.writerow(row)
 
+
 #
 #   Configurator functionality
 #
 
+
 class Configurator(BaseConfigurator):
 
     value_converters = dict(BaseConfigurator.value_converters)
     value_converters['inc'] = 'inc_convert'
 
     def __init__(self, config, base=None):
         super(Configurator, self).__init__(config)
         self.base = base or os.getcwd()
 
     def configure_custom(self, config):
+
         def convert(o):
             if isinstance(o, (list, tuple)):
                 result = type(o)([convert(i) for i in o])
             elif isinstance(o, dict):
                 if '()' in o:
                     result = self.configure_custom(o)
                 else:
@@ -1679,14 +1758,15 @@
         return result
 
 
 class SubprocessMixin(object):
     """
     Mixin for running subprocesses and capturing their output
     """
+
     def __init__(self, verbose=False, progress=None):
         self.verbose = verbose
         self.progress = progress
 
     def reader(self, stream, context):
         """
         Read lines from a subprocess' output stream and either pass to a progress
@@ -1705,16 +1785,18 @@
                     sys.stderr.write('.')
                 else:
                     sys.stderr.write(s.decode('utf-8'))
                 sys.stderr.flush()
         stream.close()
 
     def run_command(self, cmd, **kwargs):
-        p = subprocess.Popen(cmd, stdout=subprocess.PIPE,
-                             stderr=subprocess.PIPE, **kwargs)
+        p = subprocess.Popen(cmd,
+                             stdout=subprocess.PIPE,
+                             stderr=subprocess.PIPE,
+                             **kwargs)
         t1 = threading.Thread(target=self.reader, args=(p.stdout, 'stdout'))
         t1.start()
         t2 = threading.Thread(target=self.reader, args=(p.stderr, 'stderr'))
         t2.start()
         p.wait()
         t1.join()
         t2.join()
@@ -1726,23 +1808,25 @@
 
 
 def normalize_name(name):
     """Normalize a python package name a la PEP 503"""
     # https://www.python.org/dev/peps/pep-0503/#normalized-names
     return re.sub('[-_.]+', '-', name).lower()
 
+
 # def _get_pypirc_command():
-    # """
-    # Get the distutils command for interacting with PyPI configurations.
-    # :return: the command.
-    # """
-    # from distutils.core import Distribution
-    # from distutils.config import PyPIRCCommand
-    # d = Distribution()
-    # return PyPIRCCommand(d)
+# """
+# Get the distutils command for interacting with PyPI configurations.
+# :return: the command.
+# """
+# from distutils.core import Distribution
+# from distutils.config import PyPIRCCommand
+# d = Distribution()
+# return PyPIRCCommand(d)
+
 
 class PyPIRCFile(object):
 
     DEFAULT_REPOSITORY = 'https://upload.pypi.org/legacy/'
     DEFAULT_REALM = 'pypi'
 
     def __init__(self, fn=None, url=None):
@@ -1759,43 +1843,45 @@
 
             config = configparser.RawConfigParser()
             config.read(self.filename)
             sections = config.sections()
             if 'distutils' in sections:
                 # let's get the list of servers
                 index_servers = config.get('distutils', 'index-servers')
-                _servers = [server.strip() for server in
-                            index_servers.split('\n')
-                            if server.strip() != '']
+                _servers = [
+                    server.strip() for server in index_servers.split('\n')
+                    if server.strip() != ''
+                ]
                 if _servers == []:
                     # nothing set, let's try to get the default pypi
                     if 'pypi' in sections:
                         _servers = ['pypi']
                 else:
                     for server in _servers:
                         result = {'server': server}
                         result['username'] = config.get(server, 'username')
 
                         # optional params
-                        for key, default in (('repository', self.DEFAULT_REPOSITORY),
+                        for key, default in (('repository',
+                                              self.DEFAULT_REPOSITORY),
                                              ('realm', self.DEFAULT_REALM),
                                              ('password', None)):
                             if config.has_option(server, key):
                                 result[key] = config.get(server, key)
                             else:
                                 result[key] = default
 
                         # work around people having "repository" for the "pypi"
                         # section of their config set to the HTTP (rather than
                         # HTTPS) URL
-                        if (server == 'pypi' and
-                            repository in (self.DEFAULT_REPOSITORY, 'pypi')):
+                        if (server == 'pypi' and repository
+                                in (self.DEFAULT_REPOSITORY, 'pypi')):
                             result['repository'] = self.DEFAULT_REPOSITORY
-                        elif (result['server'] != repository and
-                              result['repository'] != repository):
+                        elif (result['server'] != repository
+                              and result['repository'] != repository):
                             result = {}
             elif 'server-login' in sections:
                 # old format
                 server = 'server-login'
                 if config.has_option(server, 'repository'):
                     repository = config.get(server, 'repository')
                 else:
@@ -1817,28 +1903,32 @@
         if not config.has_section('pypi'):
             config.add_section('pypi')
         config.set('pypi', 'username', username)
         config.set('pypi', 'password', password)
         with open(fn, 'w') as f:
             config.write(f)
 
+
 def _load_pypirc(index):
     """
     Read the PyPI access configuration as supported by distutils.
     """
     return PyPIRCFile(url=index.url).read()
 
+
 def _store_pypirc(index):
     PyPIRCFile().update(index.username, index.password)
 
+
 #
 # get_platform()/get_host_platform() copied from Python 3.10.a0 source, with some minor
 # tweaks
 #
 
+
 def get_host_platform():
     """Return a string that identifies the current platform.  This is used mainly to
     distinguish platform-specific build directories and platform-specific built
     distributions.  Typically includes the OS name and version and the
     architecture (as supplied by 'os.uname()'), although the exact information
     included depends on the OS; eg. on Linux, the kernel version isn't
     particularly important.
@@ -1882,48 +1972,51 @@
     osname = osname.lower().replace('/', '')
     machine = machine.replace(' ', '_').replace('/', '-')
 
     if osname[:5] == 'linux':
         # At least on Linux/Intel, 'machine' is the processor --
         # i386, etc.
         # XXX what about Alpha, SPARC, etc?
-        return  "%s-%s" % (osname, machine)
+        return "%s-%s" % (osname, machine)
 
     elif osname[:5] == 'sunos':
-        if release[0] >= '5':           # SunOS 5 == Solaris 2
+        if release[0] >= '5':  # SunOS 5 == Solaris 2
             osname = 'solaris'
             release = '%d.%s' % (int(release[0]) - 3, release[2:])
             # We can't use 'platform.architecture()[0]' because a
             # bootstrap problem. We use a dict to get an error
             # if some suspicious happens.
-            bitness = {2147483647:'32bit', 9223372036854775807:'64bit'}
+            bitness = {2147483647: '32bit', 9223372036854775807: '64bit'}
             machine += '.%s' % bitness[sys.maxsize]
         # fall through to standard osname-release-machine representation
     elif osname[:3] == 'aix':
         from _aix_support import aix_platform
         return aix_platform()
     elif osname[:6] == 'cygwin':
         osname = 'cygwin'
-        rel_re = re.compile (r'[\d.]+', re.ASCII)
+        rel_re = re.compile(r'[\d.]+', re.ASCII)
         m = rel_re.match(release)
         if m:
             release = m.group()
     elif osname[:6] == 'darwin':
-        import _osx_support, distutils.sysconfig
+        import _osx_support
+        try:
+            from distutils import sysconfig
+        except ImportError:
+            import sysconfig
         osname, release, machine = _osx_support.get_platform_osx(
-                                        distutils.sysconfig.get_config_vars(),
-                                        osname, release, machine)
+            sysconfig.get_config_vars(), osname, release, machine)
 
     return '%s-%s-%s' % (osname, release, machine)
 
 
 _TARGET_TO_PLAT = {
-    'x86' : 'win32',
-    'x64' : 'win-amd64',
-    'arm' : 'win-arm32',
+    'x86': 'win32',
+    'x64': 'win-amd64',
+    'arm': 'win-arm32',
 }
 
 
 def get_platform():
     if os.name != 'nt':
         return get_host_platform()
     cross_compilation_target = os.environ.get('VSCMD_ARG_TGT_ARCH')
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/version.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2012-2017 The Python Software Foundation.
+# Copyright (C) 2012-2023 The Python Software Foundation.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 """
 Implementation of a flexible versioning scheme providing support for PEP-440,
 setuptools-compatible and semantic versioning.
 """
 
@@ -172,17 +172,17 @@
     def __repr__(self):
         return "%s(%r)" % (self.__class__.__name__, self._string)
 
     def __str__(self):
         return self._string
 
 
-PEP440_VERSION_RE = re.compile(r'^v?(\d+!)?(\d+(\.\d+)*)((a|b|c|rc)(\d+))?'
-                               r'(\.(post)(\d+))?(\.(dev)(\d+))?'
-                               r'(\+([a-zA-Z\d]+(\.[a-zA-Z\d]+)?))?$')
+PEP440_VERSION_RE = re.compile(r'^v?(\d+!)?(\d+(\.\d+)*)((a|alpha|b|beta|c|rc|pre|preview)(\d+)?)?'
+                               r'(\.(post|r|rev)(\d+)?)?([._-]?(dev)(\d+)?)?'
+                               r'(\+([a-zA-Z\d]+(\.[a-zA-Z\d]+)?))?$', re.I)
 
 
 def _pep_440_key(s):
     s = s.strip()
     m = PEP440_VERSION_RE.match(s)
     if not m:
         raise UnsupportedVersionError('Not a valid version: %s' % s)
@@ -198,23 +198,32 @@
     pre = groups[4:6]
     post = groups[7:9]
     dev = groups[10:12]
     local = groups[13]
     if pre == (None, None):
         pre = ()
     else:
-        pre = pre[0], int(pre[1])
+        if pre[1] is None:
+            pre = pre[0], 0
+        else:
+            pre = pre[0], int(pre[1])
     if post == (None, None):
         post = ()
     else:
-        post = post[0], int(post[1])
+        if post[1] is None:
+            post = post[0], 0
+        else:
+            post = post[0], int(post[1])
     if dev == (None, None):
         dev = ()
     else:
-        dev = dev[0], int(dev[1])
+        if dev[1] is None:
+            dev = dev[0], 0
+        else:
+            dev = dev[0], int(dev[1])
     if local is None:
         local = ()
     else:
         parts = []
         for part in local.split('.'):
             # to ensure that numeric compares as > lexicographic, avoid
             # comparing them directly, but encode a tuple which ensures
@@ -234,15 +243,14 @@
             pre = ('z',)        # to sort after all pre-releases
     # now look at the state of post and dev.
     if not post:
         post = ('_',)   # sort before 'a'
     if not dev:
         dev = ('final',)
 
-    #print('%s -> %s' % (s, m.groups()))
     return epoch, nums, pre, post, dev, local
 
 
 _normalized_key = _pep_440_key
 
 
 class NormalizedVersion(Version):
@@ -374,25 +382,26 @@
 #            return True
         release_clause = constraint._release_clause
         if len(release_clause) > 1:
             release_clause = release_clause[:-1]
         pfx = '.'.join([str(i) for i in release_clause])
         return _match_prefix(version, pfx)
 
+
 _REPLACEMENTS = (
     (re.compile('[.+-]$'), ''),                     # remove trailing puncts
     (re.compile(r'^[.](\d)'), r'0.\1'),             # .N -> 0.N at start
     (re.compile('^[.-]'), ''),                      # remove leading puncts
     (re.compile(r'^\((.*)\)$'), r'\1'),             # remove parentheses
     (re.compile(r'^v(ersion)?\s*(\d+)'), r'\2'),    # remove leading v(ersion)
     (re.compile(r'^r(ev)?\s*(\d+)'), r'\2'),        # remove leading v(ersion)
     (re.compile('[.]{2,}'), '.'),                   # multiple runs of '.'
     (re.compile(r'\b(alfa|apha)\b'), 'alpha'),      # misspelt alpha
     (re.compile(r'\b(pre-alpha|prealpha)\b'),
-                'pre.alpha'),                       # standardise
+        'pre.alpha'),                               # standardise
     (re.compile(r'\(beta\)$'), 'beta'),             # remove parentheses
 )
 
 _SUFFIX_REPLACEMENTS = (
     (re.compile('^[:~._+-]+'), ''),                   # remove leading puncts
     (re.compile('[,*")([\\]]'), ''),                  # remove unwanted chars
     (re.compile('[~:+_ -]'), '.'),                    # replace illegal chars
@@ -412,15 +421,15 @@
     for pat, repl in _REPLACEMENTS:
         result = pat.sub(repl, result)
     if not result:
         result = '0.0.0'
 
     # Now look for numeric prefix, and separate it out from
     # the rest.
-    #import pdb; pdb.set_trace()
+    # import pdb; pdb.set_trace()
     m = _NUMERIC_PREFIX.match(result)
     if not m:
         prefix = '0.0.0'
         suffix = result
     else:
         prefix = m.groups()[0].split('.')
         prefix = [int(i) for i in prefix]
@@ -430,15 +439,15 @@
             suffix = result[m.end():]
         else:
             suffix = '.'.join([str(i) for i in prefix[3:]]) + result[m.end():]
             prefix = prefix[:3]
         prefix = '.'.join([str(i) for i in prefix])
         suffix = suffix.strip()
     if suffix:
-        #import pdb; pdb.set_trace()
+        # import pdb; pdb.set_trace()
         # massage the suffix.
         for pat, repl in _SUFFIX_REPLACEMENTS:
             suffix = pat.sub(repl, suffix)
 
     if not suffix:
         result = prefix
     else:
@@ -500,15 +509,15 @@
     rs = re.sub(r"[.~]?([abc])\.?", r"\1", rs)
 
     # Clean: v0.3, v1.0
     if rs.startswith('v'):
         rs = rs[1:]
 
     # Clean leading '0's on numbers.
-    #TODO: unintended side-effect on, e.g., "2003.05.09"
+    # TODO: unintended side-effect on, e.g., "2003.05.09"
     # PyPI stats: 77 (~2%) better
     rs = re.sub(r"\b0+(\d+)(?!\d)", r"\1", rs)
 
     # Clean a/b/c with no version. E.g. "1.0a" -> "1.0a0". Setuptools infers
     # zero.
     # PyPI stats: 245 (7.56%) better
     rs = re.sub(r"(\d+[abc])$", r"\g<1>0", rs)
@@ -559,14 +568,15 @@
         rs = None
     return rs
 
 #
 #   Legacy version processing (distribute-compatible)
 #
 
+
 _VERSION_PART = re.compile(r'([a-z]+|\d+|[\.-])', re.I)
 _VERSION_REPLACE = {
     'pre': 'c',
     'preview': 'c',
     '-': 'final-',
     'rc': 'c',
     'dev': '@',
@@ -606,15 +616,15 @@
         return _legacy_key(s)
 
     @property
     def is_prerelease(self):
         result = False
         for x in self._parts:
             if (isinstance(x, string_types) and x.startswith('*') and
-                x < '*final'):
+                    x < '*final'):
                 result = True
                 break
         return result
 
 
 class LegacyMatcher(Matcher):
     version_class = LegacyVersion
@@ -637,14 +647,15 @@
             s = s.rsplit('.', 1)[0]
         return _match_prefix(version, s)
 
 #
 #   Semantic versioning
 #
 
+
 _SEMVER_RE = re.compile(r'^(\d+)\.(\d+)\.(\d+)'
                         r'(-[a-z0-9]+(\.[a-z0-9-]+)*)?'
                         r'(\+[a-z0-9]+(\.[a-z0-9-]+)*)?$', re.I)
 
 
 def is_semver(s):
     return _SEMVER_RE.match(s)
@@ -718,14 +729,15 @@
     def suggest(self, s):
         if self.suggester is None:
             result = None
         else:
             result = self.suggester(s)
         return result
 
+
 _SCHEMES = {
     'normalized': VersionScheme(_normalized_key, NormalizedMatcher,
                                 _suggest_normalized_version),
     'legacy': VersionScheme(_legacy_key, LegacyMatcher, lambda self, s: s),
     'semantic': VersionScheme(_semantic_key, SemanticMatcher,
                               _suggest_semantic_version),
 }
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/w32.exe` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/w64.exe` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distlib/wheel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2013-2020 Vinay Sajip.
+# Copyright (C) 2013-2023 Vinay Sajip.
 # Licensed to the Python Software Foundation under a contributor agreement.
 # See LICENSE.txt and CONTRIBUTORS.txt.
 #
 from __future__ import unicode_literals
 
 import base64
 import codecs
@@ -20,46 +20,46 @@
 import sys
 import tempfile
 import zipfile
 
 from . import __version__, DistlibException
 from .compat import sysconfig, ZipFile, fsdecode, text_type, filter
 from .database import InstalledDistribution
-from .metadata import (Metadata, METADATA_FILENAME, WHEEL_METADATA_FILENAME,
-                       LEGACY_METADATA_FILENAME)
+from .metadata import Metadata, WHEEL_METADATA_FILENAME, LEGACY_METADATA_FILENAME
 from .util import (FileOperator, convert_path, CSVReader, CSVWriter, Cache,
                    cached_property, get_cache_base, read_exports, tempdir,
                    get_platform)
 from .version import NormalizedVersion, UnsupportedVersionError
 
 logger = logging.getLogger(__name__)
 
-cache = None    # created when needed
+cache = None  # created when needed
 
 if hasattr(sys, 'pypy_version_info'):  # pragma: no cover
     IMP_PREFIX = 'pp'
 elif sys.platform.startswith('java'):  # pragma: no cover
     IMP_PREFIX = 'jy'
 elif sys.platform == 'cli':  # pragma: no cover
     IMP_PREFIX = 'ip'
 else:
     IMP_PREFIX = 'cp'
 
 VER_SUFFIX = sysconfig.get_config_var('py_version_nodot')
-if not VER_SUFFIX:   # pragma: no cover
+if not VER_SUFFIX:  # pragma: no cover
     VER_SUFFIX = '%s%s' % sys.version_info[:2]
 PYVER = 'py' + VER_SUFFIX
 IMPVER = IMP_PREFIX + VER_SUFFIX
 
 ARCH = get_platform().replace('-', '_').replace('.', '_')
 
 ABI = sysconfig.get_config_var('SOABI')
 if ABI and ABI.startswith('cpython-'):
     ABI = ABI.replace('cpython-', 'cp').split('-')[0]
 else:
+
     def _derive_abi():
         parts = ['cp', VER_SUFFIX]
         if sysconfig.get_config_var('Py_DEBUG'):
             parts.append('d')
         if IMP_PREFIX == 'cp':
             vi = sys.version_info[:2]
             if vi < (3, 8):
@@ -69,28 +69,31 @@
                 if wpm:
                     parts.append('m')
                 if vi < (3, 3):
                     us = sysconfig.get_config_var('Py_UNICODE_SIZE')
                     if us == 4 or (us is None and sys.maxunicode == 0x10FFFF):
                         parts.append('u')
         return ''.join(parts)
+
     ABI = _derive_abi()
     del _derive_abi
 
-FILENAME_RE = re.compile(r'''
+FILENAME_RE = re.compile(
+    r'''
 (?P<nm>[^-]+)
 -(?P<vn>\d+[^-]*)
 (-(?P<bn>\d+[^-]*))?
 -(?P<py>\w+\d+(\.\w+\d+)*)
 -(?P<bi>\w+)
 -(?P<ar>\w+(\.\w+)*)
 \.whl$
 ''', re.IGNORECASE | re.VERBOSE)
 
-NAME_VERSION_RE = re.compile(r'''
+NAME_VERSION_RE = re.compile(
+    r'''
 (?P<nm>[^-]+)
 -(?P<vn>\d+[^-]*)
 (-(?P<bn>\d+[^-]*))?$
 ''', re.IGNORECASE | re.VERBOSE)
 
 SHEBANG_RE = re.compile(br'\s*#![^\r\n]*')
 SHEBANG_DETAIL_RE = re.compile(br'^(\s*#!("[^"]+"|\S+))\s+(.*)$')
@@ -105,32 +108,36 @@
 if sys.version_info[0] < 3:
     import imp
 else:
     imp = None
     import importlib.machinery
     import importlib.util
 
+
 def _get_suffixes():
     if imp:
         return [s[0] for s in imp.get_suffixes()]
     else:
         return importlib.machinery.EXTENSION_SUFFIXES
 
+
 def _load_dynamic(name, path):
     # https://docs.python.org/3/library/importlib.html#importing-a-source-file-directly
     if imp:
         return imp.load_dynamic(name, path)
     else:
         spec = importlib.util.spec_from_file_location(name, path)
         module = importlib.util.module_from_spec(spec)
         sys.modules[name] = module
         spec.loader.exec_module(module)
         return module
 
+
 class Mounter(object):
+
     def __init__(self):
         self.impure_wheels = {}
         self.libs = {}
 
     def add(self, pathname, extensions):
         self.impure_wheels[pathname] = extensions
         self.libs.update(extensions)
@@ -157,14 +164,15 @@
             result = _load_dynamic(fullname, self.libs[fullname])
             result.__loader__ = self
             parts = fullname.rsplit('.', 1)
             if len(parts) > 1:
                 result.__package__ = parts[0]
         return result
 
+
 _hook = Mounter()
 
 
 class Wheel(object):
     """
     Class to build and install from Wheel files (PEP 427).
     """
@@ -223,16 +231,16 @@
         else:
             buildver = ''
         pyver = '.'.join(self.pyver)
         abi = '.'.join(self.abi)
         arch = '.'.join(self.arch)
         # replace - with _ as a local version separator
         version = self.version.replace('-', '_')
-        return '%s-%s%s-%s-%s-%s.whl' % (self.name, version, buildver,
-                                         pyver, abi, arch)
+        return '%s-%s%s-%s-%s-%s.whl' % (self.name, version, buildver, pyver,
+                                         abi, arch)
 
     @property
     def exists(self):
         path = os.path.join(self.dirname, self.filename)
         return os.path.isfile(path)
 
     @property
@@ -245,22 +253,22 @@
     @cached_property
     def metadata(self):
         pathname = os.path.join(self.dirname, self.filename)
         name_ver = '%s-%s' % (self.name, self.version)
         info_dir = '%s.dist-info' % name_ver
         wrapper = codecs.getreader('utf-8')
         with ZipFile(pathname, 'r') as zf:
-            wheel_metadata = self.get_wheel_metadata(zf)
-            wv = wheel_metadata['Wheel-Version'].split('.', 1)
-            file_version = tuple([int(i) for i in wv])
+            self.get_wheel_metadata(zf)
+            # wv = wheel_metadata['Wheel-Version'].split('.', 1)
+            # file_version = tuple([int(i) for i in wv])
             # if file_version < (1, 1):
-                # fns = [WHEEL_METADATA_FILENAME, METADATA_FILENAME,
-                       # LEGACY_METADATA_FILENAME]
+            # fns = [WHEEL_METADATA_FILENAME, METADATA_FILENAME,
+            # LEGACY_METADATA_FILENAME]
             # else:
-                # fns = [WHEEL_METADATA_FILENAME, METADATA_FILENAME]
+            # fns = [WHEEL_METADATA_FILENAME, METADATA_FILENAME]
             fns = [WHEEL_METADATA_FILENAME, LEGACY_METADATA_FILENAME]
             result = None
             for fn in fns:
                 try:
                     metadata_filename = posixpath.join(info_dir, fn)
                     with zf.open(metadata_filename) as bf:
                         wf = wrapper(bf)
@@ -322,30 +330,31 @@
 
     def get_hash(self, data, hash_kind=None):
         if hash_kind is None:
             hash_kind = self.hash_kind
         try:
             hasher = getattr(hashlib, hash_kind)
         except AttributeError:
-            raise DistlibException('Unsupported hash algorithm: %r' % hash_kind)
+            raise DistlibException('Unsupported hash algorithm: %r' %
+                                   hash_kind)
         result = hasher(data).digest()
         result = base64.urlsafe_b64encode(result).rstrip(b'=').decode('ascii')
         return hash_kind, result
 
     def write_record(self, records, record_path, archive_record_path):
-        records = list(records) # make a copy, as mutated
+        records = list(records)  # make a copy, as mutated
         records.append((archive_record_path, '', ''))
         with CSVWriter(record_path) as writer:
             for row in records:
                 writer.writerow(row)
 
     def write_records(self, info, libdir, archive_paths):
         records = []
         distinfo, info_dir = info
-        hasher = getattr(hashlib, self.hash_kind)
+        # hasher = getattr(hashlib, self.hash_kind)
         for ap, p in archive_paths:
             with open(p, 'rb') as f:
                 data = f.read()
             digest = '%s=%s' % self.get_hash(data)
             size = os.path.getsize(p)
             records.append((ap, digest, size))
 
@@ -462,14 +471,15 @@
         # and keep the dist-info stuff at the end.
         def sorter(t):
             ap = t[0]
             n = ap.count('/')
             if '.dist-info' in ap:
                 n += 10000
             return (n, ap)
+
         archive_paths = sorted(archive_paths, key=sorter)
 
         # Now, at last, RECORD.
         # Paths in here are archive paths - nothing else makes sense.
         self.write_records((distinfo, info_dir), libdir, archive_paths)
         # Now, ready to build the zip file
         pathname = os.path.join(self.dirname, self.filename)
@@ -508,15 +518,16 @@
         The return value is a :class:`InstalledDistribution` instance unless
         ``options.lib_only`` is True, in which case the return value is ``None``.
         """
 
         dry_run = maker.dry_run
         warner = kwargs.get('warner')
         lib_only = kwargs.get('lib_only', False)
-        bc_hashed_invalidation = kwargs.get('bytecode_hashed_invalidation', False)
+        bc_hashed_invalidation = kwargs.get('bytecode_hashed_invalidation',
+                                            False)
 
         pathname = os.path.join(self.dirname, self.filename)
         name_ver = '%s-%s' % (self.name, self.version)
         data_dir = '%s.data' % name_ver
         info_dir = '%s.dist-info' % name_ver
 
         metadata_name = posixpath.join(info_dir, LEGACY_METADATA_FILENAME)
@@ -549,19 +560,19 @@
             data_pfx = posixpath.join(data_dir, '')
             info_pfx = posixpath.join(info_dir, '')
             script_pfx = posixpath.join(data_dir, 'scripts', '')
 
             # make a new instance rather than a copy of maker's,
             # as we mutate it
             fileop = FileOperator(dry_run=dry_run)
-            fileop.record = True    # so we can rollback if needed
+            fileop.record = True  # so we can rollback if needed
 
-            bc = not sys.dont_write_bytecode    # Double negatives. Lovely!
+            bc = not sys.dont_write_bytecode  # Double negatives. Lovely!
 
-            outfiles = []   # for RECORD writing
+            outfiles = []  # for RECORD writing
 
             # for script copying/shebang processing
             workdir = tempfile.mkdtemp()
             # set target dir later
             # we default add_launchers to False, as the
             # Python Launcher should be used instead
             maker.source_dir = workdir
@@ -607,29 +618,31 @@
                             fileop.copy_stream(bf, outfile)
                         # Issue #147: permission bits aren't preserved. Using
                         # zf.extract(zinfo, libdir) should have worked, but didn't,
                         # see https://www.thetopsites.net/article/53834422.shtml
                         # So ... manually preserve permission bits as given in zinfo
                         if os.name == 'posix':
                             # just set the normal permission bits
-                            os.chmod(outfile, (zinfo.external_attr >> 16) & 0x1FF)
+                            os.chmod(outfile,
+                                     (zinfo.external_attr >> 16) & 0x1FF)
                         outfiles.append(outfile)
                         # Double check the digest of the written file
                         if not dry_run and row[1]:
                             with open(outfile, 'rb') as bf:
                                 data = bf.read()
                                 _, newdigest = self.get_hash(data, kind)
                                 if newdigest != digest:
                                     raise DistlibException('digest mismatch '
                                                            'on write for '
                                                            '%s' % outfile)
                         if bc and outfile.endswith('.py'):
                             try:
-                                pyc = fileop.byte_compile(outfile,
-                                                          hashed_invalidation=bc_hashed_invalidation)
+                                pyc = fileop.byte_compile(
+                                    outfile,
+                                    hashed_invalidation=bc_hashed_invalidation)
                                 outfiles.append(pyc)
                             except Exception:
                                 # Don't give up if byte-compilation fails,
                                 # but log it and perhaps warn the user
                                 logger.warning('Byte-compilation failed',
                                                exc_info=True)
                     else:
@@ -696,25 +709,25 @@
                             maker.target_dir = script_dir
                             for k, v in console_scripts.items():
                                 script = '%s = %s' % (k, v)
                                 filenames = maker.make(script)
                                 fileop.set_executable_mode(filenames)
 
                             if gui_scripts:
-                                options = {'gui': True }
+                                options = {'gui': True}
                                 for k, v in gui_scripts.items():
                                     script = '%s = %s' % (k, v)
                                     filenames = maker.make(script, options)
                                     fileop.set_executable_mode(filenames)
 
                     p = os.path.join(libdir, info_dir)
                     dist = InstalledDistribution(p)
 
                     # Write SHARED
-                    paths = dict(paths)     # don't change passed in dict
+                    paths = dict(paths)  # don't change passed in dict
                     del paths['purelib']
                     del paths['platlib']
                     paths['lib'] = libdir
                     p = dist.write_shared_locations(paths, dry_run)
                     if p:
                         outfiles.append(p)
 
@@ -757,15 +770,16 @@
                         os.makedirs(cache_base)
                     for name, relpath in extensions.items():
                         dest = os.path.join(cache_base, convert_path(relpath))
                         if not os.path.exists(dest):
                             extract = True
                         else:
                             file_time = os.stat(dest).st_mtime
-                            file_time = datetime.datetime.fromtimestamp(file_time)
+                            file_time = datetime.datetime.fromtimestamp(
+                                file_time)
                             info = zf.getinfo(relpath)
                             wheel_time = datetime.datetime(*info.date_time)
                             extract = wheel_time > file_time
                         if extract:
                             zf.extract(relpath, cache_base)
                         result.append((name, dest))
             except KeyError:
@@ -778,15 +792,15 @@
         """
         return is_compatible(self)
 
     def is_mountable(self):
         """
         Determine if a wheel is asserted as mountable by its metadata.
         """
-        return True # for now - metadata details TBD
+        return True  # for now - metadata details TBD
 
     def mount(self, append=False):
         pathname = os.path.abspath(os.path.join(self.dirname, self.filename))
         if not self.is_compatible():
             msg = 'Wheel %s not compatible with this Python.' % pathname
             raise DistlibException(msg)
         if not self.is_mountable():
@@ -816,29 +830,29 @@
             if not _hook.impure_wheels:
                 if _hook in sys.meta_path:
                     sys.meta_path.remove(_hook)
 
     def verify(self):
         pathname = os.path.join(self.dirname, self.filename)
         name_ver = '%s-%s' % (self.name, self.version)
-        data_dir = '%s.data' % name_ver
+        # data_dir = '%s.data' % name_ver
         info_dir = '%s.dist-info' % name_ver
 
-        metadata_name = posixpath.join(info_dir, LEGACY_METADATA_FILENAME)
+        # metadata_name = posixpath.join(info_dir, LEGACY_METADATA_FILENAME)
         wheel_metadata_name = posixpath.join(info_dir, 'WHEEL')
         record_name = posixpath.join(info_dir, 'RECORD')
 
         wrapper = codecs.getreader('utf-8')
 
         with ZipFile(pathname, 'r') as zf:
             with zf.open(wheel_metadata_name) as bwf:
                 wf = wrapper(bwf)
-                message = message_from_file(wf)
-            wv = message['Wheel-Version'].split('.', 1)
-            file_version = tuple([int(i) for i in wv])
+                message_from_file(wf)
+            # wv = message['Wheel-Version'].split('.', 1)
+            # file_version = tuple([int(i) for i in wv])
             # TODO version verification
 
             records = {}
             with zf.open(record_name) as bf:
                 with CSVReader(stream=bf) as reader:
                     for row in reader:
                         p = row[0]
@@ -899,33 +913,33 @@
                 path = path_map[key]
                 version = Metadata(path=path).version
             return version, path
 
         def update_version(version, path):
             updated = None
             try:
-                v = NormalizedVersion(version)
+                NormalizedVersion(version)
                 i = version.find('-')
                 if i < 0:
                     updated = '%s+1' % version
                 else:
                     parts = [int(s) for s in version[i + 1:].split('.')]
                     parts[-1] += 1
-                    updated = '%s+%s' % (version[:i],
-                                         '.'.join(str(i) for i in parts))
+                    updated = '%s+%s' % (version[:i], '.'.join(
+                        str(i) for i in parts))
             except UnsupportedVersionError:
-                logger.debug('Cannot update non-compliant (PEP-440) '
-                             'version %r', version)
+                logger.debug(
+                    'Cannot update non-compliant (PEP-440) '
+                    'version %r', version)
             if updated:
                 md = Metadata(path=path)
                 md.version = updated
                 legacy = path.endswith(LEGACY_METADATA_FILENAME)
                 md.write(path=path, legacy=legacy)
-                logger.debug('Version updated from %r to %r', version,
-                             updated)
+                logger.debug('Version updated from %r to %r', version, updated)
 
         pathname = os.path.join(self.dirname, self.filename)
         name_ver = '%s-%s' % (self.name, self.version)
         info_dir = '%s.dist-info' % name_ver
         record_name = posixpath.join(info_dir, 'RECORD')
         with tempdir() as workdir:
             with ZipFile(pathname, 'r') as zf:
@@ -959,42 +973,45 @@
                 if dest_dir is None:
                     fd, newpath = tempfile.mkstemp(suffix='.whl',
                                                    prefix='wheel-update-',
                                                    dir=workdir)
                     os.close(fd)
                 else:
                     if not os.path.isdir(dest_dir):
-                        raise DistlibException('Not a directory: %r' % dest_dir)
+                        raise DistlibException('Not a directory: %r' %
+                                               dest_dir)
                     newpath = os.path.join(dest_dir, self.filename)
                 archive_paths = list(path_map.items())
                 distinfo = os.path.join(workdir, info_dir)
                 info = distinfo, info_dir
                 self.write_records(info, workdir, archive_paths)
                 self.build_zip(newpath, archive_paths)
                 if dest_dir is None:
                     shutil.copyfile(newpath, pathname)
         return modified
 
+
 def _get_glibc_version():
     import platform
     ver = platform.libc_ver()
     result = []
     if ver[0] == 'glibc':
         for s in ver[1].split('.'):
             result.append(int(s) if s.isdigit() else 0)
         result = tuple(result)
     return result
 
+
 def compatible_tags():
     """
     Return (pyver, abi, arch) tuples compatible with this Python.
     """
     versions = [VER_SUFFIX]
     major = VER_SUFFIX[0]
-    for minor in range(sys.version_info[1] - 1, - 1, -1):
+    for minor in range(sys.version_info[1] - 1, -1, -1):
         versions.append(''.join([major, str(minor)]))
 
     abis = []
     for suffix in _get_suffixes():
         if suffix.startswith('.abi'):
             abis.append(suffix.split('.', 2)[1])
     abis.sort()
@@ -1019,15 +1036,15 @@
             if arch in ('i386', 'x86_64'):
                 matches.append('intel')
             if arch in ('i386', 'x86_64', 'intel', 'ppc', 'ppc64'):
                 matches.append('universal')
             while minor >= 0:
                 for match in matches:
                     s = '%s_%s_%s_%s' % (name, major, minor, match)
-                    if s != ARCH:   # already there
+                    if s != ARCH:  # already there
                         arches.append(s)
                 minor -= 1
 
     # Most specific - our Python version, ABI and arch
     for abi in abis:
         for arch in arches:
             result.append((''.join((IMP_PREFIX, versions[0])), abi, arch))
@@ -1041,17 +1058,17 @@
                                        'manylinux1_%s' % arch))
                     if parts >= (2, 12):
                         result.append((''.join((IMP_PREFIX, versions[0])), abi,
                                        'manylinux2010_%s' % arch))
                     if parts >= (2, 17):
                         result.append((''.join((IMP_PREFIX, versions[0])), abi,
                                        'manylinux2014_%s' % arch))
-                    result.append((''.join((IMP_PREFIX, versions[0])), abi,
-                                   'manylinux_%s_%s_%s' % (parts[0], parts[1],
-                                                           arch)))
+                    result.append(
+                        (''.join((IMP_PREFIX, versions[0])), abi,
+                         'manylinux_%s_%s_%s' % (parts[0], parts[1], arch)))
 
     # where no ABI / arch dependency, but IMP_PREFIX dependency
     for i, version in enumerate(versions):
         result.append((''.join((IMP_PREFIX, version)), 'none', 'any'))
         if i == 0:
             result.append((''.join((IMP_PREFIX, version[0])), 'none', 'any'))
 
@@ -1067,15 +1084,15 @@
 COMPATIBLE_TAGS = compatible_tags()
 
 del compatible_tags
 
 
 def is_compatible(wheel, tags=None):
     if not isinstance(wheel, Wheel):
-        wheel = Wheel(wheel)    # assume it's a filename
+        wheel = Wheel(wheel)  # assume it's a filename
     result = False
     if tags is None:
         tags = COMPATIBLE_TAGS
     for ver, abi, arch in tags:
         if ver in wheel.pyver and abi in wheel.abi and arch in wheel.arch:
             result = True
             break
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distro/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/distro/distro.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/codec.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/core.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/idnadata.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/intranges.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/idna/uts46data.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/msgpack/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/msgpack/ext.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/msgpack/fallback.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/__about__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/_structures.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/markers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/requirements.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/specifiers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/tags.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/packaging/version.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/android.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/api.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/macos.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/unix.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/windows.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/cmdline.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/console.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/filter.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatter.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexer.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/modeline.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/plugin.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/regexopt.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/scanner.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/style.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/token.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/unistring.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/util.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/actions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/common.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/core.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/results.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/testing.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/util.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/adapters.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/api.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/auth.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/certs.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/compat.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/cookies.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/exceptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/help.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/hooks.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/models.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/packages.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/sessions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/status_codes.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/structures.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/requests/utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/providers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/structs.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/__main__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_export_format.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_fileno.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_inspect.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_log_render.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_loop.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_null_file.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_palettes.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_ratio.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_spinners.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_win32_console.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_windows.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/_wrap.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/abc.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/align.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/ansi.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/bar.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/box.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/cells.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/color.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/color_triplet.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/columns.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/console.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/constrain.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/containers.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/control.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/default_styles.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/diagnose.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/emoji.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/errors.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/file_proxy.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/filesize.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/highlighter.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/json.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/jupyter.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/layout.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/live.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/live_render.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/logging.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/markup.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/measure.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/padding.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/pager.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/palette.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/panel.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/pretty.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/progress.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/progress_bar.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/prompt.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/protocol.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/repr.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/rule.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/scope.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/screen.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/segment.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/spinner.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/status.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/style.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/styled.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/syntax.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/table.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/text.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/theme.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/traceback.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/rich/tree.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/_utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/after.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/before.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/nap.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/retry.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/stop.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tenacity/wait.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tomli/_parser.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/tomli/_re.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_api.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_api.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_macos.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_macos.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_openssl.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_openssl.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/truststore/_windows.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/truststore/_windows.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/_collections.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/connection.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/fields.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/filepost.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/request.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/response.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/request.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/response.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/url.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/labels.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/tests.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/AUTHORS.txt` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/AUTHORS.txt`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
 Craig Kerstiens
 Cristian Sorinel
 Cristina
 Cristina Muñoz
 Curtis Doty
 cytolentino
 Daan De Meyer
+Dale
 Damian
 Damian Quiroga
 Damian Shaw
 Dan Black
 Dan Savilonis
 Dan Sully
 Dane Hillard
@@ -222,15 +223,18 @@
 Dos Moonen
 Douglas Thor
 DrFeathers
 Dustin Ingram
 Dwayne Bailey
 Ed Morley
 Edgar Ramírez
+Edgar Ramírez Mondragón
 Ee Durbin
+Efflam Lemaillet
+efflamlemaillet
 Eitan Adler
 ekristina
 elainechan
 Eli Schwartz
 Elisha Hollander
 Ellen Marie Dash
 Emil Burzo
@@ -252,14 +256,15 @@
 Felipe Peter
 Felix Yan
 fiber-space
 Filip Kokosiński
 Filipe Laíns
 Finn Womack
 finnagin
+Flavio Amurrio
 Florian Briand
 Florian Rathgeber
 Francesco
 Francesco Montesano
 Frost Ming
 Gabriel Curio
 Gabriel de Perthuis
@@ -314,14 +319,15 @@
 Illia Volochii
 Ilya Baryshev
 Inada Naoki
 Ionel Cristian Mărieș
 Ionel Maries Cristian
 Itamar Turner-Trauring
 Ivan Pozdeev
+J. Nick Koston
 Jacob Kim
 Jacob Walls
 Jaime Sanz
 jakirkham
 Jakub Kuczys
 Jakub Stasiak
 Jakub Vysoky
@@ -336,14 +342,15 @@
 Jarek Potiuk
 jarondl
 Jason Curtis
 Jason R. Coombs
 JasonMo
 JasonMo1
 Jay Graves
+Jean Abou Samra
 Jean-Christophe Fillion-Robin
 Jeff Barber
 Jeff Dairiki
 Jeff Widman
 Jelmer Vernooĳ
 jenix21
 Jeremy Stanley
@@ -575,14 +582,15 @@
 pre-commit-ci[bot]
 Preet Thakkar
 Preston Holmes
 Przemek Wrzos
 Pulkit Goyal
 q0w
 Qiangning Hong
+Qiming Xu
 Quentin Lee
 Quentin Pradet
 R. David Murray
 Rafael Caricio
 Ralf Schmitt
 Razzi Abuissa
 rdb
@@ -713,14 +721,15 @@
 Viktor Szépe
 Ville Skyttä
 Vinay Sajip
 Vincent Philippon
 Vinicyus Macedo
 Vipul Kumar
 Vitaly Babiy
+Vladimir Fokow
 Vladimir Rutsky
 W. Trevor King
 Wil Tan
 Wilfred Hughes
 William Edwards
 William ML Leslie
 William T Olson
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/LICENSE.txt` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: pip
-Version: 23.3.1
+Version: 24.0
 Summary: The PyPA recommended tool for installing Python packages.
-Home-page: https://pip.pypa.io/
-Author: The pip developers
-Author-email: distutils-sig@python.org
+Author-email: The pip developers <distutils-sig@python.org>
 License: MIT
+Project-URL: Homepage, https://pip.pypa.io/
 Project-URL: Documentation, https://pip.pypa.io
 Project-URL: Source, https://github.com/pypa/pip
 Project-URL: Changelog, https://pip.pypa.io/en/stable/news/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Build Tools
@@ -21,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 pip - The Python Package Installer
 ==================================
 
 .. image:: https://img.shields.io/pypi/v/pip.svg
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pip-23.3.1.dist-info/RECORD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pip-24.0.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,178 +1,180 @@
-pip/__init__.py,sha256=MSbZQYwV5U4mAXP2fBQh70QhM71N-1vh7T4CRREqVog,357
+pip/__init__.py,sha256=oAk1nFpLmUVS5Ln7NxvNoGUn5Vkn6FGQjPaNDf8Q8pk,355
 pip/__main__.py,sha256=WzbhHXTbSE6gBY19mNN9m4s5o_365LOvTYSgqgbdBhE,854
 pip/__pip-runner__.py,sha256=EnrfKmKMzWAdqg_JicLCOP9Y95Ux7zHh4ObvqLtQcjo,1444
 pip/py.typed,sha256=EBVvvPRTn_eIpz5e5QztSCdrMX7Qwd7VP93RSoIlZ2I,286
 pip/_internal/__init__.py,sha256=iqZ5-YQsQV08tkUc7L806Reop6tguLFWf70ySF6be0Y,515
 pip/_internal/build_env.py,sha256=1ESpqw0iupS_K7phZK5zshVE5Czy9BtGLFU4W6Enva8,10243
 pip/_internal/cache.py,sha256=uiYD-9F0Bv1C8ZyWE85lpzDmQf7hcUkgL99GmI8I41Q,10370
-pip/_internal/configuration.py,sha256=i_dePJKndPAy7hf48Sl6ZuPyl3tFPCE67z0SNatwuwE,13839
-pip/_internal/exceptions.py,sha256=LyTVY2dANx-i_TEk5Yr9YcwUtiy0HOEFCAQq1F_46co,23737
+pip/_internal/configuration.py,sha256=XkAiBS0hpzsM-LF0Qu5hvPWO_Bs67-oQKRYFBuMbESs,14006
+pip/_internal/exceptions.py,sha256=TmF1iNFEneSWaemwlg6a5bpPuq2cMHK7d1-SvjsQHb0,23634
 pip/_internal/main.py,sha256=r-UnUe8HLo5XFJz8inTcOOTiu_sxNhgHb6VwlGUllOI,340
-pip/_internal/pyproject.py,sha256=ltmrXWaMXjiJHbYyzWplTdBvPYPdKk99GjKuQVypGZU,7161
+pip/_internal/pyproject.py,sha256=4Xszp11xgr126yzG6BbJA0oaQ9WXuhb0jyUb-y_6lPQ,7152
 pip/_internal/self_outdated_check.py,sha256=saxQLB8UzIFtMScquytG10TOTsYVFJQ_mkW1NY-46wE,8378
-pip/_internal/wheel_builder.py,sha256=3UlHfxQi7_AAXI7ur8aPpPbmqHhecCsubmkHEl-00KU,11842
+pip/_internal/wheel_builder.py,sha256=qTTzQV8F6b1jNsFCda1TRQC8J7gK-m7iuRNgKo7Dj68,11801
 pip/_internal/cli/__init__.py,sha256=FkHBgpxxb-_gd6r1FjnNhfMOzAUYyXoXKJ6abijfcFU,132
 pip/_internal/cli/autocompletion.py,sha256=_br_5NgSxSuvPjMF0MLHzS5s6BpSkQAQHKrLK89VauM,6690
 pip/_internal/cli/base_command.py,sha256=iuVWGa2oTq7gBReo0er3Z0tXJ2oqBIC6QjDHcnDhKXY,8733
-pip/_internal/cli/cmdoptions.py,sha256=fAi5GzWuM9mKUesJZO56LcPCVMDtm64c2tC_YUpI1qs,30117
+pip/_internal/cli/cmdoptions.py,sha256=1EIm8yMixQMELO4QzogdIoWkvIlQqlAW0YnPeOmnvEA,30064
 pip/_internal/cli/command_context.py,sha256=RHgIPwtObh5KhMrd3YZTkl8zbVG-6Okml7YbFX4Ehg0,774
 pip/_internal/cli/main.py,sha256=Uzxt_YD1hIvB1AW5mxt6IVcht5G712AtMqdo51UMhmQ,2816
 pip/_internal/cli/main_parser.py,sha256=laDpsuBDl6kyfywp9eMMA9s84jfH2TJJn-vmL0GG90w,4338
-pip/_internal/cli/parser.py,sha256=o4esYgG-rvPsf6FBpF3fSLGHa4ndDvJtwxBgeckGyfI,10801
+pip/_internal/cli/parser.py,sha256=KW6C3-7-4ErTNB0TfLTKwOdHcd-qefCeGnrOoE2r0RQ,10781
 pip/_internal/cli/progress_bars.py,sha256=So4mPoSjXkXiSHiTzzquH3VVyVD_njXlHJSExYPXAow,1968
 pip/_internal/cli/req_command.py,sha256=c7_XHABnXmD3_qlK9-r37KqdKBAcgmVKvQ2WcTrNLfc,18369
 pip/_internal/cli/spinners.py,sha256=hIJ83GerdFgFCdobIA23Jggetegl_uC4Sp586nzFbPE,5118
 pip/_internal/cli/status_codes.py,sha256=sEFHUaUJbqv8iArL3HAtcztWZmGOFX01hTesSytDEh0,116
 pip/_internal/commands/__init__.py,sha256=5oRO9O3dM2vGuh0bFw4HOVletryrz5HHMmmPWwJrH9U,3882
-pip/_internal/commands/cache.py,sha256=LfPA8wNcgZtjiI5faeFFCR2Zp-ugaj7XX--FmKxx4_4,7952
+pip/_internal/commands/cache.py,sha256=xg76_ZFEBC6zoQ3gXLRfMZJft4z2a0RwH4GEFZC6nnU,7944
 pip/_internal/commands/check.py,sha256=Rb13Q28yoLh0j1gpx5SU0jlResNct21eQCRsnaO9xKA,1782
 pip/_internal/commands/completion.py,sha256=HT4lD0bgsflHq2IDgYfiEdp7IGGtE7s6MgI3xn0VQEw,4287
-pip/_internal/commands/configuration.py,sha256=NB5uf8HIX8-li95YLoZO09nALIWlLCHDF5aifSKcBn8,9815
-pip/_internal/commands/debug.py,sha256=L15rfN8DwORQln-QW3ihBaVdCfV7Iba-lwlcyw1f_Vk,6854
+pip/_internal/commands/configuration.py,sha256=n98enwp6y0b5G6fiRQjaZo43FlJKYve_daMhN-4BRNc,9766
+pip/_internal/commands/debug.py,sha256=63972uUCeMIGOdMMVeIUGrOjTOqTVWplFC82a-hcKyA,6777
 pip/_internal/commands/download.py,sha256=e4hw088zGo26WmJaMIRvCniLlLmoOjqolGyfHjsCkCQ,5335
 pip/_internal/commands/freeze.py,sha256=2qjQrH9KWi5Roav0CuR7vc7hWm4uOi_0l6tp3ESKDHM,3172
 pip/_internal/commands/hash.py,sha256=EVVOuvGtoPEdFi8SNnmdqlCQrhCxV-kJsdwtdcCnXGQ,1703
 pip/_internal/commands/help.py,sha256=gcc6QDkcgHMOuAn5UxaZwAStsRBrnGSn_yxjS57JIoM,1132
-pip/_internal/commands/index.py,sha256=cGQVSA5dAs7caQ9sz4kllYvaI4ZpGiq1WhCgaImXNSA,4793
+pip/_internal/commands/index.py,sha256=CNXQer_PeZKSJooURcCFCBEKGfwyNoUWYP_MWczAcOM,4775
 pip/_internal/commands/inspect.py,sha256=2wSPt9yfr3r6g-s2S5L6PvRtaHNVyb4TuodMStJ39cw,3188
-pip/_internal/commands/install.py,sha256=KTHT8EASlPfbNx428tcvnGhN8D9jlfBwcRa5lxEhFsA,28920
+pip/_internal/commands/install.py,sha256=VxDd-BD3a27ApeE2OK34rfBXS6Zo2wtemK9-HCwPqxM,28782
 pip/_internal/commands/list.py,sha256=7wRUUmdyyOknl-WZYbO_LtFQxHlWod3pjOY9yYH435o,12450
 pip/_internal/commands/search.py,sha256=sbBZiARRc050QquOKcCvOr2K3XLsoYebLKZGRi__iUI,5697
 pip/_internal/commands/show.py,sha256=t5jia4zcYJRJZy4U_Von7zMl03hJmmcofj6oDNTnj7Y,6419
 pip/_internal/commands/uninstall.py,sha256=OIqO9tqadY8kM4HwhFf1Q62fUIp7v8KDrTRo8yWMz7Y,3886
 pip/_internal/commands/wheel.py,sha256=CSnX8Pmf1oPCnd7j7bn1_f58G9KHNiAblvVJ5zykN-A,6476
 pip/_internal/distributions/__init__.py,sha256=Hq6kt6gXBgjNit5hTTWLAzeCNOKoB-N0pGYSqehrli8,858
 pip/_internal/distributions/base.py,sha256=oRSEvnv2ZjBnargamnv2fcJa1n6gUDKaW0g6CWSEpWs,1743
 pip/_internal/distributions/installed.py,sha256=QinHFbWAQ8oE0pbD8MFZWkwlnfU1QYTccA1vnhrlYOU,842
 pip/_internal/distributions/sdist.py,sha256=4K3V0VNMllHbBzCJibjwd_tylUKpmIdu2AQyhplvCQo,6709
 pip/_internal/distributions/wheel.py,sha256=-ma3sOtUQj0AxXCEb6_Fhmjl3nh4k3A0HC2taAb2N-4,1277
 pip/_internal/index/__init__.py,sha256=vpt-JeTZefh8a-FC22ZeBSXFVbuBcXSGiILhQZJaNpQ,30
-pip/_internal/index/collector.py,sha256=3OmYZ3tCoRPGOrELSgQWG-03M-bQHa2-VCA3R_nJAaU,16504
-pip/_internal/index/package_finder.py,sha256=uA354-mHjHvTwxDmk9HvpAkq_7KyGvEd7_9aZFqu0HY,37889
-pip/_internal/index/sources.py,sha256=7jw9XSeeQA5K-H4I5a5034Ks2gkQqm4zPXjrhwnP1S4,6556
+pip/_internal/index/collector.py,sha256=sH0tL_cOoCk6pLLfCSGVjFM4rPEJtllF-VobvAvLSH4,16590
+pip/_internal/index/package_finder.py,sha256=S_nC8gzVIMY6ikWfKoSOzRtoesUqnfNhAPl_BwSOusA,37843
+pip/_internal/index/sources.py,sha256=dJegiR9f86kslaAHcv9-R5L_XBf5Rzm_FkyPteDuPxI,8688
 pip/_internal/locations/__init__.py,sha256=Dh8LJWG8LRlDK4JIj9sfRF96TREzE--N_AIlx7Tqoe4,15365
-pip/_internal/locations/_distutils.py,sha256=DXL6H3xERLF76BjcYanV4j-4Sw-qcPdO2qeZhLN30WQ,6102
+pip/_internal/locations/_distutils.py,sha256=H9ZHK_35rdDV1Qsmi4QeaBULjFT4Mbu6QuoVGkJ6QHI,6009
 pip/_internal/locations/_sysconfig.py,sha256=jyNVtUfMIf0mtyY-Xp1m9yQ8iwECozSVVFmjkN9a2yw,7680
 pip/_internal/locations/base.py,sha256=RQiPi1d4FVM2Bxk04dQhXZ2PqkeljEL2fZZ9SYqIQ78,2556
 pip/_internal/metadata/__init__.py,sha256=9pU3W3s-6HtjFuYhWcLTYVmSaziklPv7k2x8p7X1GmA,4339
-pip/_internal/metadata/_json.py,sha256=BTkWfFDrWFwuSodImjtbAh8wCL3isecbnjTb5E6UUDI,2595
+pip/_internal/metadata/_json.py,sha256=Rz5M5ciSNvITwaTQR6NfN8TgKgM5WfTws4D6CFknovE,2627
 pip/_internal/metadata/base.py,sha256=l3Wgku4xlgr8s4p6fS-3qQ4QKOpPbWLRwi5d9omEFG4,25907
 pip/_internal/metadata/pkg_resources.py,sha256=opjw4IBSqHvie6sXJ_cbT42meygoPEUfNURJuWZY7sk,10035
 pip/_internal/metadata/importlib/__init__.py,sha256=jUUidoxnHcfITHHaAWG1G2i5fdBYklv_uJcjo2x7VYE,135
 pip/_internal/metadata/importlib/_compat.py,sha256=GAe_prIfCE4iUylrnr_2dJRlkkBVRUbOidEoID7LPoE,1882
 pip/_internal/metadata/importlib/_dists.py,sha256=UPl1wUujFqiwiltRJ1tMF42WRINO1sSpNNlYQ2mX0mk,8297
 pip/_internal/metadata/importlib/_envs.py,sha256=XTaFIYERP2JF0QUZuPx2ETiugXbPEcZ8q8ZKeht6Lpc,7456
 pip/_internal/models/__init__.py,sha256=3DHUd_qxpPozfzouoqa9g9ts1Czr5qaHfFxbnxriepM,63
-pip/_internal/models/candidate.py,sha256=6pcABsaR7CfIHlbJbr2_kMkVJFL_yrYjTx6SVWUnCPQ,990
-pip/_internal/models/direct_url.py,sha256=EepBxI97j7wSZ3AmRETYyVTmR9NoTas15vc8popxVTg,6931
-pip/_internal/models/format_control.py,sha256=DJpMYjxeYKKQdwNcML2_F0vtAh-qnKTYe-CpTxQe-4g,2520
+pip/_internal/models/candidate.py,sha256=hEPu8VdGE5qVASv6vLz-R-Rgh5-7LMbai1jgthMCd8M,931
+pip/_internal/models/direct_url.py,sha256=FwouYBKcqckh7B-k2H3HVgRhhFTukFwqiS3kfvtFLSk,6889
+pip/_internal/models/format_control.py,sha256=wtsQqSK9HaUiNxQEuB-C62eVimw6G4_VQFxV9-_KDBE,2486
 pip/_internal/models/index.py,sha256=tYnL8oxGi4aSNWur0mG8DAP7rC6yuha_MwJO8xw0crI,1030
 pip/_internal/models/installation_report.py,sha256=zRVZoaz-2vsrezj_H3hLOhMZCK9c7TbzWgC-jOalD00,2818
-pip/_internal/models/link.py,sha256=6OEk3bt41WU7QZoiyuoVPGsKOU-J_BbDDhouKbIXm0Y,20819
+pip/_internal/models/link.py,sha256=XirOAGv1jgMu7vu87kuPbohGj7VHpwVrd2q3KUgVQNg,20777
 pip/_internal/models/scheme.py,sha256=3EFQp_ICu_shH1-TBqhl0QAusKCPDFOlgHFeN4XowWs,738
 pip/_internal/models/search_scope.py,sha256=ASVyyZxiJILw7bTIVVpJx8J293M3Hk5F33ilGn0e80c,4643
 pip/_internal/models/selection_prefs.py,sha256=KZdi66gsR-_RUXUr9uejssk3rmTHrQVJWeNA2sV-VSY,1907
 pip/_internal/models/target_python.py,sha256=34EkorrMuRvRp-bjqHKJ-bOO71m9xdjN2b8WWFEC2HU,4272
 pip/_internal/models/wheel.py,sha256=YqazoIZyma_Q1ejFa1C7NHKQRRWlvWkdK96VRKmDBeI,3600
 pip/_internal/network/__init__.py,sha256=jf6Tt5nV_7zkARBrKojIXItgejvoegVJVKUbhAa5Ioc,50
 pip/_internal/network/auth.py,sha256=TC-OcW2KU4W6R1hU4qPgQXvVH54adACpZz6sWq-R9NA,20541
 pip/_internal/network/cache.py,sha256=48A971qCzKNFvkb57uGEk7-0xaqPS0HWj2711QNTxkU,3935
-pip/_internal/network/download.py,sha256=HvDDq9bVqaN3jcS3DyVJHP7uTqFzbShdkf7NFSoHfkw,6096
+pip/_internal/network/download.py,sha256=i0Tn55CD5D7XYEFY3TxiYaCf0OaaTQ6SScNgCsSeV14,6086
 pip/_internal/network/lazy_wheel.py,sha256=2PXVduYZPCPZkkQFe1J1GbfHJWeCU--FXonGyIfw9eU,7638
-pip/_internal/network/session.py,sha256=uhovd4J7abd0Yr2g426yC4aC6Uw1VKrQfpzalsEBEMw,18607
+pip/_internal/network/session.py,sha256=9tqEDD8JiVaFdplOEXJxNo9cjRfBZ6RIa0yQQ_qBNiM,18698
 pip/_internal/network/utils.py,sha256=6A5SrUJEEUHxbGtbscwU2NpCyz-3ztiDlGWHpRRhsJ8,4073
-pip/_internal/network/xmlrpc.py,sha256=AzQgG4GgS152_cqmGr_Oz2MIXsCal-xfsis7fA7nmU0,1791
+pip/_internal/network/xmlrpc.py,sha256=sAxzOacJ-N1NXGPvap9jC3zuYWSnnv3GXtgR2-E2APA,1838
 pip/_internal/operations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_internal/operations/check.py,sha256=Hgz0wQJ4fGi8aAVfmdShviNc7XM_2j8oMQJUsVv6AqY,6806
+pip/_internal/operations/check.py,sha256=fsqA88iGaqftCr2tlP3sSU202CSkoODRtW0O-JU9M4Y,6806
 pip/_internal/operations/freeze.py,sha256=uqoeTAf6HOYVMR2UgAT8N85UZoGEVEoQdan_Ao6SOfk,9816
-pip/_internal/operations/prepare.py,sha256=NWkGkNOjrnnUbHgJPTms_5usKF0M8JlaHL3nyIHABMk,28155
+pip/_internal/operations/prepare.py,sha256=57Oq87HfunX3Rbqp47FdaJr9cHbAKUm_3gv7WhBAqbE,28128
 pip/_internal/operations/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_internal/operations/build/build_tracker.py,sha256=z-H5DOknZdBa3dh2Vq6VBMY5qLYIKmlj2p6CGZK5Lc8,4832
 pip/_internal/operations/build/metadata.py,sha256=9S0CUD8U3QqZeXp-Zyt8HxwU90lE4QrnYDgrqZDzBnc,1422
 pip/_internal/operations/build/metadata_editable.py,sha256=VLL7LvntKE8qxdhUdEJhcotFzUsOSI8NNS043xULKew,1474
 pip/_internal/operations/build/metadata_legacy.py,sha256=o-eU21As175hDC7dluM1fJJ_FqokTIShyWpjKaIpHZw,2198
 pip/_internal/operations/build/wheel.py,sha256=sT12FBLAxDC6wyrDorh8kvcZ1jG5qInCRWzzP-UkJiQ,1075
 pip/_internal/operations/build/wheel_editable.py,sha256=yOtoH6zpAkoKYEUtr8FhzrYnkNHQaQBjWQ2HYae1MQg,1417
 pip/_internal/operations/build/wheel_legacy.py,sha256=C9j6rukgQI1n_JeQLoZGuDdfUwzCXShyIdPTp6edbMQ,3064
 pip/_internal/operations/install/__init__.py,sha256=mX7hyD2GNBO2mFGokDQ30r_GXv7Y_PLdtxcUv144e-s,51
 pip/_internal/operations/install/editable_legacy.py,sha256=YeR0KadWXw_ZheC1NtAG1qVIEkOgRGHc23x-YtGW7NU,1282
-pip/_internal/operations/install/wheel.py,sha256=a5KnguJ9uQRo7Ikq4YJEno0fFltXYlud-0DpRj3zLr0,27457
+pip/_internal/operations/install/wheel.py,sha256=9hGb1c4bRnPIb2FG7CtUSPfPxqprmHQBtwIAlWPNTtE,27311
 pip/_internal/req/__init__.py,sha256=TELFgZOof3lhMmaICVWL9U7PlhXo9OufokbMAJ6J2GI,2738
-pip/_internal/req/constructors.py,sha256=PgLoQlsZ_ErZORw5M1mgnxW5V4mKZC0-gyj_3k4hCe0,19028
-pip/_internal/req/req_file.py,sha256=5PCO4GnDEnUENiFj4vD_1QmAMjHNtvN6HXbETZ9UGok,17872
-pip/_internal/req/req_install.py,sha256=XvoTWTF7STk9EUqIphdOI0ZtQOplw44PIl9TCb-HtXw,35130
-pip/_internal/req/req_set.py,sha256=nM-CetUtESEH31fdugrOl20GV5-pCUYAvu65FwYDJeI,4704
-pip/_internal/req/req_uninstall.py,sha256=m9GlbQ3rzLORTSa6NPFFCmONmC5zTw2lY_0fLOkLYCk,24676
+pip/_internal/req/constructors.py,sha256=8hlY56imEthLORRwmloyKz3YOyXymIaKsNB6P9ewvNI,19018
+pip/_internal/req/req_file.py,sha256=M8ttOZL-PwAj7scPElhW3ZD2hiD9mm_6FJAGIbwAzEI,17790
+pip/_internal/req/req_install.py,sha256=wtOPxkyRSM8comTks8oL1Gp2oyGqbH7JwIDRci2QiPk,35460
+pip/_internal/req/req_set.py,sha256=iMYDUToSgkxFyrP_OrTtPSgw4dwjRyGRDpGooTqeA4Y,4704
+pip/_internal/req/req_uninstall.py,sha256=nmvTQaRCC0iu-5Tw0djlXJhSj6WmqHRvT3qkkEdC35E,24551
 pip/_internal/resolution/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_internal/resolution/base.py,sha256=qlmh325SBVfvG6Me9gc5Nsh5sdwHBwzHBq6aEXtKsLA,583
 pip/_internal/resolution/legacy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_internal/resolution/legacy/resolver.py,sha256=th-eTPIvbecfJaUsdrbH1aHQvDV2yCE-RhrrpsJhKbE,24128
+pip/_internal/resolution/legacy/resolver.py,sha256=Xk24jQ62GvLr4Mc7IjN_qiO88qp0BImzVmPIFz9QLOE,24025
 pip/_internal/resolution/resolvelib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_internal/resolution/resolvelib/base.py,sha256=jg5COmHLhmBIKOR-4spdJD3jyULYa1BdsqiBu2YJnJ4,5173
-pip/_internal/resolution/resolvelib/candidates.py,sha256=IAcXcBj-LLzJwwfBXFGyhpxir42CMBW64oCc4zEgLYo,21320
-pip/_internal/resolution/resolvelib/factory.py,sha256=FIOXvrdEGo6DMtLF9gqhUd4IQphPUkAYUe8ZIQ0ThMY,31317
+pip/_internal/resolution/resolvelib/candidates.py,sha256=19Ki91Po-MSxBknGIfOGkaWkFdOznN0W_nKv7jL28L0,21052
+pip/_internal/resolution/resolvelib/factory.py,sha256=vqqk-hjchdhShwWVdeW2_A-5ZblLhE_nC_v3Mhz4Svc,32292
 pip/_internal/resolution/resolvelib/found_candidates.py,sha256=hvL3Hoa9VaYo-qEOZkBi2Iqw251UDxPz-uMHVaWmLpE,5705
 pip/_internal/resolution/resolvelib/provider.py,sha256=4t23ivjruqM6hKBX1KpGiTt-M4HGhRcZnGLV0c01K7U,9824
 pip/_internal/resolution/resolvelib/reporter.py,sha256=YFm9hQvz4DFCbjZeFTQ56hTz3Ac-mDBnHkeNRVvMHLY,3100
-pip/_internal/resolution/resolvelib/requirements.py,sha256=SZh98hbSVbHiHBkgjrSLtdrrZB1zqRIUqFdXptS-aVY,6030
+pip/_internal/resolution/resolvelib/requirements.py,sha256=-kJONP0WjDfdTvBAs2vUXPgAnOyNIBEAXY4b72ogtPE,5696
 pip/_internal/resolution/resolvelib/resolver.py,sha256=nLJOsVMEVi2gQUVJoUFKMZAeu2f7GRMjGMvNSWyz0Bc,12592
 pip/_internal/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_internal/utils/_jaraco_text.py,sha256=yvDGelTVugRayPaOF2k4ab0Ky4d3uOkAfuOQjASjImY,3351
 pip/_internal/utils/_log.py,sha256=-jHLOE_THaZz5BFcCnoSL9EYAtJ0nXem49s9of4jvKw,1015
 pip/_internal/utils/appdirs.py,sha256=swgcTKOm3daLeXTW6v5BUS2Ti2RvEnGRQYH_yDXklAo,1665
 pip/_internal/utils/compat.py,sha256=ACyBfLgj3_XG-iA5omEDrXqDM0cQKzi8h8HRBInzG6Q,1884
 pip/_internal/utils/compatibility_tags.py,sha256=ydin8QG8BHqYRsPY4OL6cmb44CbqXl1T0xxS97VhHkk,5377
 pip/_internal/utils/datetime.py,sha256=m21Y3wAtQc-ji6Veb6k_M5g6A0ZyFI4egchTdnwh-pQ,242
 pip/_internal/utils/deprecation.py,sha256=NKo8VqLioJ4nnXXGmW4KdasxF90EFHkZaHeX1fT08C8,3627
 pip/_internal/utils/direct_url_helpers.py,sha256=6F1tc2rcKaCZmgfVwsE6ObIe_Pux23mUVYA-2D9wCFc,3206
-pip/_internal/utils/egg_link.py,sha256=ZryCchR_yQSCsdsMkCpxQjjLbQxObA5GDtLG0RR5mGc,2118
+pip/_internal/utils/egg_link.py,sha256=0FePZoUYKv4RGQ2t6x7w5Z427wbA_Uo3WZnAkrgsuqo,2463
 pip/_internal/utils/encoding.py,sha256=qqsXDtiwMIjXMEiIVSaOjwH5YmirCaK-dIzb6-XJsL0,1169
 pip/_internal/utils/entrypoints.py,sha256=YlhLTRl2oHBAuqhc-zmL7USS67TPWVHImjeAQHreZTQ,3064
 pip/_internal/utils/filesystem.py,sha256=RhMIXUaNVMGjc3rhsDahWQ4MavvEQDdqXqgq-F6fpw8,5122
 pip/_internal/utils/filetypes.py,sha256=i8XAQ0eFCog26Fw9yV0Yb1ygAqKYB1w9Cz9n0fj8gZU,716
 pip/_internal/utils/glibc.py,sha256=Mesxxgg3BLxheLZx-dSf30b6gKpOgdVXw6W--uHSszQ,3113
 pip/_internal/utils/hashes.py,sha256=MjOigC75z6qoRMkgHiHqot7eqxfwDZSrEflJMPm-bHE,5118
 pip/_internal/utils/logging.py,sha256=fdtuZJ-AKkqwDTANDvGcBEpssL8el7T1jnwk1CnZl3Y,11603
-pip/_internal/utils/misc.py,sha256=96DVNJQIeMi0vWrNp0C0v3xjk2r7Zcay5yDoruIm_Js,23739
+pip/_internal/utils/misc.py,sha256=fNXwaeeikvnUt4CPMFIL4-IQbZDxxjj4jDpzCi4ZsOw,23623
 pip/_internal/utils/models.py,sha256=5GoYU586SrxURMvDn_jBMJInitviJg4O5-iOU-6I0WY,1193
 pip/_internal/utils/packaging.py,sha256=5Wm6_x7lKrlqVjPI5MBN_RurcRHwVYoQ7Ksrs84de7s,2108
 pip/_internal/utils/setuptools_build.py,sha256=ouXpud-jeS8xPyTPsXJ-m34NPvK5os45otAzdSV_IJE,4435
 pip/_internal/utils/subprocess.py,sha256=zzdimb75jVLE1GU4WlTZ055gczhD7n1y1xTcNc7vNZQ,9207
 pip/_internal/utils/temp_dir.py,sha256=DUAw22uFruQdK43i2L2K53C-CDjRCPeAsBKJpu-rHQ4,9312
 pip/_internal/utils/unpacking.py,sha256=SBb2iV1crb89MDRTEKY86R4A_UOWApTQn9VQVcMDOlE,8821
 pip/_internal/utils/urls.py,sha256=AhaesUGl-9it6uvG6fsFPOr9ynFpGaTMk4t5XTX7Z_Q,1759
 pip/_internal/utils/virtualenv.py,sha256=S6f7csYorRpiD6cvn3jISZYc3I8PJC43H5iMFpRAEDU,3456
-pip/_internal/utils/wheel.py,sha256=lXOgZyTlOm5HmK8tw5iw0A3_5A6wRzsXHOaQkIvvloU,4549
+pip/_internal/utils/wheel.py,sha256=i4BwUNHattzN0ixy3HBAF04tZPRh2CcxaT6t86viwkE,4499
 pip/_internal/vcs/__init__.py,sha256=UAqvzpbi0VbZo3Ub6skEeZAw-ooIZR-zX_WpCbxyCoU,596
 pip/_internal/vcs/bazaar.py,sha256=j0oin0fpGRHcCFCxEcpPCQoFEvA-DMLULKdGP8Nv76o,3519
 pip/_internal/vcs/git.py,sha256=CeKBGJnl6uskvvjkAUXrJVxbHJrpS_B_pyfFdjL3CRc,18121
-pip/_internal/vcs/mercurial.py,sha256=ytRnzmP5CkLM2RfdiS4mVJx4jQcmB3FjXeLOPPFEjG8,5246
+pip/_internal/vcs/mercurial.py,sha256=oULOhzJ2Uie-06d1omkL-_Gc6meGaUkyogvqG9ZCyPs,5249
 pip/_internal/vcs/subversion.py,sha256=vhZs8L-TNggXqM1bbhl-FpbxE3TrIB6Tgnx8fh3S2HE,11729
-pip/_internal/vcs/versioncontrol.py,sha256=KUOc-hN51em9jrqxKwUR3JnkgSE-xSOqMiiJcSaL6B8,22811
+pip/_internal/vcs/versioncontrol.py,sha256=3eIjtOMYvOY5qP6BMYIYDZ375CSuec6kSEB0bOo1cSs,22787
 pip/_vendor/__init__.py,sha256=U51NPwXdA-wXOiANIQncYjcMp6txgeOL5nHxksJeyas,4993
 pip/_vendor/six.py,sha256=TOOfQi7nFGfMrIvtdr6wX4wyHH8M7aknmuLfo2cBBrM,34549
 pip/_vendor/typing_extensions.py,sha256=EWpcpyQnVmc48E9fSyPGs-vXgHcAk9tQABQIxmMsCGk,111130
-pip/_vendor/vendor.txt,sha256=epuLpe-n1shCqP5BzC97iMIAIeOeDHdtNKFgcxax-9A,493
+pip/_vendor/vendor.txt,sha256=4NKk7fQhVsZw0U-0zmm9Q2LgGyaPXacFbnJAaS0Q6EY,493
 pip/_vendor/cachecontrol/__init__.py,sha256=ctHagMhQXuvQDdm4TirZrwDOT5H8oBNAJqzdKI6sovk,676
 pip/_vendor/cachecontrol/_cmd.py,sha256=iist2EpzJvDVIhMAxXq8iFnTBsiZAd6iplxfmNboNyk,1737
 pip/_vendor/cachecontrol/adapter.py,sha256=_CcWvUP9048qAZjsNqViaHbdcLs9mmFNixVfpO7oebE,6392
 pip/_vendor/cachecontrol/cache.py,sha256=OTQj72tUf8C1uEgczdl3Gc8vkldSzsTITKtDGKMx4z8,1952
 pip/_vendor/cachecontrol/controller.py,sha256=keCFA3ZaNVaWTwHd6F1zqWhb4vyvNx_UvZuo5iIYMfo,18384
 pip/_vendor/cachecontrol/filewrapper.py,sha256=STttGmIPBvZzt2b51dUOwoWX5crcMCpKZOisM3f5BNc,4292
 pip/_vendor/cachecontrol/heuristics.py,sha256=fdFbk9W8IeLrjteIz_fK4mj2HD_Y7COXF2Uc8TgjT1c,4828
+pip/_vendor/cachecontrol/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/cachecontrol/serialize.py,sha256=0dHeMaDwysVAAnGVlhMOP4tDliohgNK0Jxk_zsOiWxw,7173
 pip/_vendor/cachecontrol/wrapper.py,sha256=hsGc7g8QGQTT-4f8tgz3AM5qwScg6FO0BSdLSRdEvpU,1417
 pip/_vendor/cachecontrol/caches/__init__.py,sha256=dtrrroK5BnADR1GWjCZ19aZ0tFsMfvFBtLQQU1sp_ag,303
 pip/_vendor/cachecontrol/caches/file_cache.py,sha256=3z8AWKD-vfKeiJqIzLmJyIYtR2yd6Tsh3u1TyLRQoIQ,5352
 pip/_vendor/cachecontrol/caches/redis_cache.py,sha256=9rmqwtYu_ljVkW6_oLqbC7EaX_a8YT_yLuna-eS0dgo,1386
 pip/_vendor/certifi/__init__.py,sha256=L_j-d0kYuA_MzA2_2hraF1ovf6KT6DTquRdV3paQwOk,94
 pip/_vendor/certifi/__main__.py,sha256=1k3Cr95vCxxGRGDljrW3wMdpZdL3Nhf0u1n-k2qdsCY,255
 pip/_vendor/certifi/cacert.pem,sha256=eU0Dn_3yd8BH4m8sfVj4Glhl2KDrcCSg-sEWT-pNJ88,281617
 pip/_vendor/certifi/core.py,sha256=ZwiOsv-sD_ouU1ft8wy_xZ3LQ7UbcVzyqj2XNyrsZis,4279
+pip/_vendor/certifi/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/chardet/__init__.py,sha256=57R-HSxj0PWmILMN0GFmUNqEMfrEVSamXyjD-W6_fbs,4797
 pip/_vendor/chardet/big5freq.py,sha256=ltcfP-3PjlNHCoo5e4a7C4z-2DhBTXRfY6jbMbB7P30,31274
 pip/_vendor/chardet/big5prober.py,sha256=lPMfwCX6v2AaPgvFh_cSWZcgLDbWiFCHLZ_p9RQ9uxE,1763
 pip/_vendor/chardet/chardistribution.py,sha256=13B8XUG4oXDuLdXvfbIWwLFeR-ZU21AqTS1zcdON8bU,10032
 pip/_vendor/chardet/charsetgroupprober.py,sha256=UKK3SaIZB2PCdKSIS0gnvMtLR9JJX62M-fZJu3OlWyg,3915
 pip/_vendor/chardet/charsetprober.py,sha256=L3t8_wIOov8em-vZWOcbkdsrwe43N6_gqNh5pH7WPd4,5420
 pip/_vendor/chardet/codingstatemachine.py,sha256=K7k69sw3jY5DmTXoSJQVsUtFIQKYPQVOSJJhBuGv_yE,3732
@@ -201,14 +203,15 @@
 pip/_vendor/chardet/langthaimodel.py,sha256=7bJlQitRpTnVGABmbSznHnJwOHDy3InkTvtFUx13WQI,102774
 pip/_vendor/chardet/langturkishmodel.py,sha256=XY0eGdTIy4eQ9Xg1LVPZacb-UBhHBR-cq0IpPVHowKc,95372
 pip/_vendor/chardet/latin1prober.py,sha256=p15EEmFbmQUwbKLC7lOJVGHEZwcG45ubEZYTGu01J5g,5380
 pip/_vendor/chardet/macromanprober.py,sha256=9anfzmY6TBfUPDyBDOdY07kqmTHpZ1tK0jL-p1JWcOY,6077
 pip/_vendor/chardet/mbcharsetprober.py,sha256=Wr04WNI4F3X_VxEverNG-H25g7u-MDDKlNt-JGj-_uU,3715
 pip/_vendor/chardet/mbcsgroupprober.py,sha256=iRpaNBjV0DNwYPu_z6TiHgRpwYahiM7ztI_4kZ4Uz9A,2131
 pip/_vendor/chardet/mbcssm.py,sha256=hUtPvDYgWDaA2dWdgLsshbwRfm3Q5YRlRogdmeRUNQw,30391
+pip/_vendor/chardet/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/chardet/resultdict.py,sha256=ez4FRvN5KaSosJeJ2WzUyKdDdg35HDy_SSLPXKCdt5M,402
 pip/_vendor/chardet/sbcharsetprober.py,sha256=-nd3F90i7GpXLjehLVHqVBE0KlWzGvQUPETLBNn4o6U,6400
 pip/_vendor/chardet/sbcsgroupprober.py,sha256=gcgI0fOfgw_3YTClpbra_MNxwyEyJ3eUXraoLHYb59E,4137
 pip/_vendor/chardet/sjisprober.py,sha256=aqQufMzRw46ZpFlzmYaYeT2-nzmKb-hmcrApppJ862k,4007
 pip/_vendor/chardet/universaldetector.py,sha256=xYBrg4x0dd9WnT8qclfADVD9ondrUNkqPmvte1pa520,14848
 pip/_vendor/chardet/utf1632prober.py,sha256=pw1epGdMj1hDGiCu1AHqqzOEfjX8MVdiW7O1BlT8-eQ,8505
 pip/_vendor/chardet/utf8prober.py,sha256=8m08Ub5490H4jQ6LYXvFysGtgKoKsHUd2zH_i8_TnVw,2812
@@ -226,65 +229,69 @@
 pip/_vendor/colorama/tests/__init__.py,sha256=MkgPAEzGQd-Rq0w0PZXSX2LadRWhUECcisJY8lSrm4Q,75
 pip/_vendor/colorama/tests/ansi_test.py,sha256=FeViDrUINIZcr505PAxvU4AjXz1asEiALs9GXMhwRaE,2839
 pip/_vendor/colorama/tests/ansitowin32_test.py,sha256=RN7AIhMJ5EqDsYaCjVo-o4u8JzDD4ukJbmevWKS70rY,10678
 pip/_vendor/colorama/tests/initialise_test.py,sha256=BbPy-XfyHwJ6zKozuQOvNvQZzsx9vdb_0bYXn7hsBTc,6741
 pip/_vendor/colorama/tests/isatty_test.py,sha256=Pg26LRpv0yQDB5Ac-sxgVXG7hsA1NYvapFgApZfYzZg,1866
 pip/_vendor/colorama/tests/utils.py,sha256=1IIRylG39z5-dzq09R_ngufxyPZxgldNbrxKxUGwGKE,1079
 pip/_vendor/colorama/tests/winterm_test.py,sha256=qoWFPEjym5gm2RuMwpf3pOis3a5r_PJZFCzK254JL8A,3709
-pip/_vendor/distlib/__init__.py,sha256=acgfseOC55dNrVAzaBKpUiH3Z6V7Q1CaxsiQ3K7pC-E,581
-pip/_vendor/distlib/compat.py,sha256=tfoMrj6tujk7G4UC2owL6ArgDuCKabgBxuJRGZSmpko,41259
-pip/_vendor/distlib/database.py,sha256=o_mw0fAr93NDAHHHfqG54Y1Hi9Rkfrp2BX15XWZYK50,51697
-pip/_vendor/distlib/index.py,sha256=HFiDG7LMoaBs829WuotrfIwcErOOExUOR_AeBtw_TCU,20834
-pip/_vendor/distlib/locators.py,sha256=wNzG-zERzS_XGls-nBPVVyLRHa2skUlkn0-5n0trMWA,51991
-pip/_vendor/distlib/manifest.py,sha256=nQEhYmgoreaBZzyFzwYsXxJARu3fo4EkunU163U16iE,14811
-pip/_vendor/distlib/markers.py,sha256=TpHHHLgkzyT7YHbwj-2i6weRaq-Ivy2-MUnrDkjau-U,5058
-pip/_vendor/distlib/metadata.py,sha256=g_DIiu8nBXRzA-mWPRpatHGbmFZqaFoss7z9TG7QSUU,39801
+pip/_vendor/distlib/__init__.py,sha256=hJKF7FHoqbmGckncDuEINWo_OYkDNiHODtYXSMcvjcc,625
+pip/_vendor/distlib/compat.py,sha256=Un-uIBvy02w-D267OG4VEhuddqWgKj9nNkxVltAb75w,41487
+pip/_vendor/distlib/database.py,sha256=0V9Qvs0Vrxa2F_-hLWitIyVyRifJ0pCxyOI-kEOBwsA,51965
+pip/_vendor/distlib/index.py,sha256=lTbw268rRhj8dw1sib3VZ_0EhSGgoJO3FKJzSFMOaeA,20797
+pip/_vendor/distlib/locators.py,sha256=o1r_M86_bRLafSpetmyfX8KRtFu-_Q58abvQrnOSnbA,51767
+pip/_vendor/distlib/manifest.py,sha256=3qfmAmVwxRqU1o23AlfXrQGZzh6g_GGzTAP_Hb9C5zQ,14168
+pip/_vendor/distlib/markers.py,sha256=n3DfOh1yvZ_8EW7atMyoYeZFXjYla0Nz0itQlojCd0A,5268
+pip/_vendor/distlib/metadata.py,sha256=pB9WZ9mBfmQxc9OVIldLS5CjOoQRvKAvUwwQyKwKQtQ,39693
 pip/_vendor/distlib/resources.py,sha256=LwbPksc0A1JMbi6XnuPdMBUn83X7BPuFNWqPGEKI698,10820
-pip/_vendor/distlib/scripts.py,sha256=BmkTKmiTk4m2cj-iueliatwz3ut_9SsABBW51vnQnZU,18102
+pip/_vendor/distlib/scripts.py,sha256=nQFXN6G7nOWNDUyxirUep-3WOlJhB7McvCs9zOnkGTI,18315
 pip/_vendor/distlib/t32.exe,sha256=a0GV5kCoWsMutvliiCKmIgV98eRZ33wXoS-XrqvJQVs,97792
 pip/_vendor/distlib/t64-arm.exe,sha256=68TAa32V504xVBnufojh0PcenpR3U4wAqTqf-MZqbPw,182784
 pip/_vendor/distlib/t64.exe,sha256=gaYY8hy4fbkHYTTnA4i26ct8IQZzkBG2pRdy0iyuBrc,108032
-pip/_vendor/distlib/util.py,sha256=31dPXn3Rfat0xZLeVoFpuniyhe6vsbl9_QN-qd9Lhlk,66262
-pip/_vendor/distlib/version.py,sha256=WG__LyAa2GwmA6qSoEJtvJE8REA1LZpbSizy8WvhJLk,23513
+pip/_vendor/distlib/util.py,sha256=XSznxEi_i3T20UJuaVc0qXHz5ksGUCW1khYlBprN_QE,67530
+pip/_vendor/distlib/version.py,sha256=9pXkduchve_aN7JG6iL9VTYV_kqNSGoc2Dwl8JuySnQ,23747
 pip/_vendor/distlib/w32.exe,sha256=R4csx3-OGM9kL4aPIzQKRo5TfmRSHZo6QWyLhDhNBks,91648
 pip/_vendor/distlib/w64-arm.exe,sha256=xdyYhKj0WDcVUOCb05blQYvzdYIKMbmJn2SZvzkcey4,168448
 pip/_vendor/distlib/w64.exe,sha256=ejGf-rojoBfXseGLpya6bFTFPWRG21X5KvU8J5iU-K0,101888
-pip/_vendor/distlib/wheel.py,sha256=Rgqs658VsJ3R2845qwnZD8XQryV2CzWw2mghwLvxxsI,43898
+pip/_vendor/distlib/wheel.py,sha256=FVQCve8u-L0QYk5-YTZc7s4WmNQdvjRWTK08KXzZVX4,43958
 pip/_vendor/distro/__init__.py,sha256=2fHjF-SfgPvjyNZ1iHh_wjqWdR_Yo5ODHwZC0jLBPhc,981
 pip/_vendor/distro/__main__.py,sha256=bu9d3TifoKciZFcqRBuygV3GSuThnVD_m2IK4cz96Vs,64
 pip/_vendor/distro/distro.py,sha256=UZO1LjIhtFCMdlbiz39gj3raV-Amf3SBwzGzfApiMHw,49330
+pip/_vendor/distro/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/idna/__init__.py,sha256=KJQN1eQBr8iIK5SKrJ47lXvxG0BJ7Lm38W4zT0v_8lk,849
 pip/_vendor/idna/codec.py,sha256=6ly5odKfqrytKT9_7UrlGklHnf1DSK2r9C6cSM4sa28,3374
 pip/_vendor/idna/compat.py,sha256=0_sOEUMT4CVw9doD3vyRhX80X19PwqFoUBs7gWsFME4,321
 pip/_vendor/idna/core.py,sha256=1JxchwKzkxBSn7R_oCE12oBu3eVux0VzdxolmIad24M,12950
 pip/_vendor/idna/idnadata.py,sha256=xUjqKqiJV8Ho_XzBpAtv5JFoVPSupK-SUXvtjygUHqw,44375
 pip/_vendor/idna/intranges.py,sha256=YBr4fRYuWH7kTKS2tXlFjM24ZF1Pdvcir-aywniInqg,1881
 pip/_vendor/idna/package_data.py,sha256=C_jHJzmX8PI4xq0jpzmcTMxpb5lDsq4o5VyxQzlVrZE,21
+pip/_vendor/idna/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/idna/uts46data.py,sha256=zvjZU24s58_uAS850Mcd0NnD0X7_gCMAMjzWNIeUJdc,206539
 pip/_vendor/msgpack/__init__.py,sha256=hyGhlnmcJkxryJBKC3X5FnEph375kQoL_mG8LZUuXgY,1132
 pip/_vendor/msgpack/exceptions.py,sha256=dCTWei8dpkrMsQDcjQk74ATl9HsIBH0ybt8zOPNqMYc,1081
 pip/_vendor/msgpack/ext.py,sha256=C5MK8JhVYGYFWPvxsORsqZAnvOXefYQ57m1Ym0luW5M,6079
 pip/_vendor/msgpack/fallback.py,sha256=tvNBHyxxFbuVlC8GZShETClJxjLiDMOja4XwwyvNm2g,34544
 pip/_vendor/packaging/__about__.py,sha256=ugASIO2w1oUyH8_COqQ2X_s0rDhjbhQC3yJocD03h2c,661
 pip/_vendor/packaging/__init__.py,sha256=b9Kk5MF7KxhhLgcDmiUWukN-LatWFxPdNug0joPhHSk,497
 pip/_vendor/packaging/_manylinux.py,sha256=XcbiXB-qcjv3bcohp6N98TMpOP4_j3m-iOA8ptK2GWY,11488
 pip/_vendor/packaging/_musllinux.py,sha256=_KGgY_qc7vhMGpoqss25n2hiLCNKRtvz9mCrS7gkqyc,4378
 pip/_vendor/packaging/_structures.py,sha256=q3eVNmbWJGG_S0Dit_S3Ao8qQqz_5PYTXFAKBZe5yr4,1431
 pip/_vendor/packaging/markers.py,sha256=AJBOcY8Oq0kYc570KuuPTkvuqjAlhufaE2c9sCUbm64,8487
+pip/_vendor/packaging/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/packaging/requirements.py,sha256=NtDlPBtojpn1IUC85iMjPNsUmufjpSlwnNA-Xb4m5NA,4676
 pip/_vendor/packaging/specifiers.py,sha256=LRQ0kFsHrl5qfcFNEEJrIFYsnIHQUJXY9fIsakTrrqE,30110
 pip/_vendor/packaging/tags.py,sha256=lmsnGNiJ8C4D_Pf9PbM0qgbZvD9kmB9lpZBQUZa3R_Y,15699
 pip/_vendor/packaging/utils.py,sha256=dJjeat3BS-TYn1RrUFVwufUMasbtzLfYRoy_HXENeFQ,4200
 pip/_vendor/packaging/version.py,sha256=_fLRNrFrxYcHVfyo8vk9j8s6JM8N_xsSxVFr6RJyco8,14665
 pip/_vendor/pkg_resources/__init__.py,sha256=hTAeJCNYb7dJseIDVsYK3mPQep_gphj4tQh-bspX8bg,109364
 pip/_vendor/platformdirs/__init__.py,sha256=SkhEYVyC_HUHC6KX7n4M_6coyRMtEB38QMyOYIAX6Yk,20155
 pip/_vendor/platformdirs/__main__.py,sha256=fVvSiTzr2-RM6IsjWjj4fkaOtDOgDhUWv6sA99do4CQ,1476
 pip/_vendor/platformdirs/android.py,sha256=y_EEMKwYl2-bzYBDovksSn8m76on0Lda8eyJksVQE9U,7211
 pip/_vendor/platformdirs/api.py,sha256=jWtX06jAJytYrkJDOqEls97mCkyHRSZkoqUlbMK5Qew,7132
 pip/_vendor/platformdirs/macos.py,sha256=LueVOoVgGWDBwQb8OFwXkVKfVn33CM1Lkwf1-A86tRQ,3678
+pip/_vendor/platformdirs/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/platformdirs/unix.py,sha256=22JhR8ZY0aLxSVCFnKrc6f1iz6Gv42K24Daj7aTjfSg,8809
 pip/_vendor/platformdirs/version.py,sha256=mavZTQIJIXfdewEaSTn7EWrNfPZWeRofb-74xqW5f2M,160
 pip/_vendor/platformdirs/windows.py,sha256=4TtbPGoWG2PRgI11uquDa7eRk8TcxvnUNuuMGZItnXc,9573
 pip/_vendor/pygments/__init__.py,sha256=6AuDljQtvf89DTNUyWM7k3oUlP_lq70NU-INKKteOBY,2983
 pip/_vendor/pygments/__main__.py,sha256=es8EKMvXj5yToIfQ-pf3Dv5TnIeeM6sME0LW-n4ecHo,353
 pip/_vendor/pygments/cmdline.py,sha256=byxYJp9gnjVeyhRlZ3UTMgo_LhkXh1afvN8wJBtAcc8,23685
 pip/_vendor/pygments/console.py,sha256=2wZ5W-U6TudJD1_NLUwjclMpbomFM91lNv11_60sfGY,1697
@@ -321,14 +328,15 @@
 pip/_vendor/pygments/styles/__init__.py,sha256=he7HjQx7sC0d2kfTVLjUs0J15mtToJM6M1brwIm9--Q,3700
 pip/_vendor/pyparsing/__init__.py,sha256=9m1JbE2JTLdBG0Mb6B0lEaZj181Wx5cuPXZpsbHEYgE,9116
 pip/_vendor/pyparsing/actions.py,sha256=05uaIPOznJPQ7VgRdmGCmG4sDnUPtwgv5qOYIqbL2UY,6567
 pip/_vendor/pyparsing/common.py,sha256=p-3c83E5-DjlkF35G0O9-kjQRpoejP-2_z0hxZ-eol4,13387
 pip/_vendor/pyparsing/core.py,sha256=yvuRlLpXSF8mgk-QhiW3OVLqD9T0rsj9tbibhRH4Yaw,224445
 pip/_vendor/pyparsing/exceptions.py,sha256=6Jc6W1eDZBzyFu1J0YrcdNFVBC-RINujZmveSnB8Rxw,9523
 pip/_vendor/pyparsing/helpers.py,sha256=BZJHCA8SS0pYio30KGQTc9w2qMOaK4YpZ7hcvHbnTgk,38646
+pip/_vendor/pyparsing/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/pyparsing/results.py,sha256=9dyqQ-w3MjfmxWbFt8KEPU6IfXeyRdoWp2Og802rUQY,26692
 pip/_vendor/pyparsing/testing.py,sha256=eJncg0p83zm1FTPvM9auNT6oavIvXaibmRFDf1qmwkY,13488
 pip/_vendor/pyparsing/unicode.py,sha256=fAPdsJiARFbkPAih6NkYry0dpj4jPqelGVMlE4wWFW8,10646
 pip/_vendor/pyparsing/util.py,sha256=vTMzTdwSDyV8d_dSgquUTdWgBFoA_W30nfxEJDsshRQ,8670
 pip/_vendor/pyparsing/diagram/__init__.py,sha256=nxmDOoYF9NXuLaGYy01tKFjkNReWJlrGFuJNWEiTo84,24215
 pip/_vendor/pyproject_hooks/__init__.py,sha256=kCehmy0UaBa9oVMD7ZIZrnswfnP3LXZ5lvnNJAL5JBM,491
 pip/_vendor/pyproject_hooks/_compat.py,sha256=by6evrYnqkisiM-MQcvOKs5bgDMzlOSgZqRHNqf04zE,138
@@ -351,14 +359,15 @@
 pip/_vendor/requests/packages.py,sha256=njJmVifY4aSctuW3PP5EFRCxjEwMRDO6J_feG2dKWsI,695
 pip/_vendor/requests/sessions.py,sha256=-LvTzrPtetSTrR3buxu4XhdgMrJFLB1q5D7P--L2Xhw,30373
 pip/_vendor/requests/status_codes.py,sha256=FvHmT5uH-_uimtRz5hH9VCbt7VV-Nei2J9upbej6j8g,4235
 pip/_vendor/requests/structures.py,sha256=-IbmhVz06S-5aPSZuUthZ6-6D9XOjRuTXHOabY041XM,2912
 pip/_vendor/requests/utils.py,sha256=kOPn0qYD6xRTzaxbqTdYiSInBZHl6379AJsyIgzYGLY,33460
 pip/_vendor/resolvelib/__init__.py,sha256=h509TdEcpb5-44JonaU3ex2TM15GVBLjM9CNCPwnTTs,537
 pip/_vendor/resolvelib/providers.py,sha256=fuuvVrCetu5gsxPB43ERyjfO8aReS3rFQHpDgiItbs4,5871
+pip/_vendor/resolvelib/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/resolvelib/reporters.py,sha256=TSbRmWzTc26w0ggsV1bxVpeWDB8QNIre6twYl7GIZBE,1601
 pip/_vendor/resolvelib/resolvers.py,sha256=G8rsLZSq64g5VmIq-lB7UcIJ1gjAxIQJmTF4REZleQ0,20511
 pip/_vendor/resolvelib/structs.py,sha256=0_1_XO8z_CLhegP3Vpf9VJ3zJcfLm0NOHRM-i0Ykz3o,4963
 pip/_vendor/resolvelib/compat/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/resolvelib/compat/collections_abc.py,sha256=uy8xUZ-NDEw916tugUXm8HgwCGiMO0f-RcdnpkfXfOs,156
 pip/_vendor/rich/__init__.py,sha256=dRxjIL-SbFVY0q3IjSMrfgBTHrm1LZDgLOygVBwiYZc,6090
 pip/_vendor/rich/__main__.py,sha256=TT8sb9PTnsnKhhrGuHkLN0jdN0dtKhtPkEr9CidDbPM,8478
@@ -415,14 +424,15 @@
 pip/_vendor/rich/palette.py,sha256=lInvR1ODDT2f3UZMfL1grq7dY_pDdKHw4bdUgOGaM4Y,3396
 pip/_vendor/rich/panel.py,sha256=wGMe40J8KCGgQoM0LyjRErmGIkv2bsYA71RCXThD0xE,10574
 pip/_vendor/rich/pretty.py,sha256=eLEYN9xVaMNuA6EJVYm4li7HdOHxCqmVKvnOqJpyFt0,35852
 pip/_vendor/rich/progress.py,sha256=n4KF9vky8_5iYeXcyZPEvzyLplWlDvFLkM5JI0Bs08A,59706
 pip/_vendor/rich/progress_bar.py,sha256=cEoBfkc3lLwqba4XKsUpy4vSQKDh2QQ5J2J94-ACFoo,8165
 pip/_vendor/rich/prompt.py,sha256=x0mW-pIPodJM4ry6grgmmLrl8VZp99kqcmdnBe70YYA,11303
 pip/_vendor/rich/protocol.py,sha256=5hHHDDNHckdk8iWH5zEbi-zuIVSF5hbU2jIo47R7lTE,1391
+pip/_vendor/rich/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/rich/region.py,sha256=rNT9xZrVZTYIXZC0NYn41CJQwYNbR-KecPOxTgQvB8Y,166
 pip/_vendor/rich/repr.py,sha256=9Z8otOmM-tyxnyTodvXlectP60lwahjGiDTrbrxPSTg,4431
 pip/_vendor/rich/rule.py,sha256=0fNaS_aERa3UMRc3T5WMpN_sumtDxfaor2y3of1ftBk,4602
 pip/_vendor/rich/scope.py,sha256=TMUU8qo17thyqQCPqjDLYpg_UU1k5qVd-WwiJvnJVas,2843
 pip/_vendor/rich/screen.py,sha256=YoeReESUhx74grqb0mSSb9lghhysWmFHYhsbMVQjXO8,1591
 pip/_vendor/rich/segment.py,sha256=XLnJEFvcV3bjaVzMNUJiem3n8lvvI9TJ5PTu-IG2uTg,24247
 pip/_vendor/rich/spinner.py,sha256=15koCmF0DQeD8-k28Lpt6X_zJQUlzEhgo_6A6uy47lc,4339
@@ -440,28 +450,31 @@
 pip/_vendor/tenacity/__init__.py,sha256=3kvAL6KClq8GFo2KFhmOzskRKSDQI-ubrlfZ8AQEEI0,20493
 pip/_vendor/tenacity/_asyncio.py,sha256=Qi6wgQsGa9MQibYRy3OXqcDQswIZZ00dLOoSUGN-6o8,3551
 pip/_vendor/tenacity/_utils.py,sha256=ubs6a7sxj3JDNRKWCyCU2j5r1CB7rgyONgZzYZq6D_4,2179
 pip/_vendor/tenacity/after.py,sha256=S5NCISScPeIrKwIeXRwdJl3kV9Q4nqZfnNPDx6Hf__g,1682
 pip/_vendor/tenacity/before.py,sha256=dIZE9gmBTffisfwNkK0F1xFwGPV41u5GK70UY4Pi5Kc,1562
 pip/_vendor/tenacity/before_sleep.py,sha256=YmpgN9Y7HGlH97U24vvq_YWb5deaK4_DbiD8ZuFmy-E,2372
 pip/_vendor/tenacity/nap.py,sha256=fRWvnz1aIzbIq9Ap3gAkAZgDH6oo5zxMrU6ZOVByq0I,1383
+pip/_vendor/tenacity/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/tenacity/retry.py,sha256=jrzD_mxA5mSTUEdiYB7SHpxltjhPSYZSnSRATb-ggRc,8746
 pip/_vendor/tenacity/stop.py,sha256=YMJs7ZgZfND65PRLqlGB_agpfGXlemx_5Hm4PKnBqpQ,3086
 pip/_vendor/tenacity/tornadoweb.py,sha256=po29_F1Mt8qZpsFjX7EVwAT0ydC_NbVia9gVi7R_wXA,2142
 pip/_vendor/tenacity/wait.py,sha256=3FcBJoCDgym12_dN6xfK8C1gROY0Hn4NSI2u8xv50uE,8024
 pip/_vendor/tomli/__init__.py,sha256=JhUwV66DB1g4Hvt1UQCVMdfCu-IgAV8FXmvDU9onxd4,396
 pip/_vendor/tomli/_parser.py,sha256=g9-ENaALS-B8dokYpCuzUFalWlog7T-SIYMjLZSWrtM,22633
 pip/_vendor/tomli/_re.py,sha256=dbjg5ChZT23Ka9z9DHOXfdtSpPwUfdgMXnj8NOoly-w,2943
 pip/_vendor/tomli/_types.py,sha256=-GTG2VUqkpxwMqzmVO4F7ybKddIbAnuAHXfmWQcTi3Q,254
+pip/_vendor/tomli/py.typed,sha256=8PjyZ1aVoQpRVvt71muvuq5qE-jTFZkK-GLHkhdebmc,26
 pip/_vendor/truststore/__init__.py,sha256=qzTLSH8PvAkY1fr6QQ2vV-KwE_M83wdXugtpJaP_AbM,403
 pip/_vendor/truststore/_api.py,sha256=xjuEu_rlH4hcdJTROImEyOEqdw-F8t5vO2H2BToY0Ro,9893
 pip/_vendor/truststore/_macos.py,sha256=BjvAKoAjXhdIPuxpY124HJIFswDb0pq8DjynzJOVwqc,17694
 pip/_vendor/truststore/_openssl.py,sha256=LLUZ7ZGaio-i5dpKKjKCSeSufmn6T8pi9lDcFnvSyq0,2324
 pip/_vendor/truststore/_ssl_constants.py,sha256=NUD4fVKdSD02ri7-db0tnO0VqLP9aHuzmStcW7tAl08,1130
 pip/_vendor/truststore/_windows.py,sha256=1x_EhROeJ9QK1sMAjfnZC7awYI8UnBJYL-TjACUYI4A,17468
+pip/_vendor/truststore/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip/_vendor/urllib3/__init__.py,sha256=iXLcYiJySn0GNbWOOZDDApgBL1JgP44EZ8i1760S8Mc,3333
 pip/_vendor/urllib3/_collections.py,sha256=Rp1mVyBgc_UlAcp6M3at1skJBXR5J43NawRTvW2g_XY,10811
 pip/_vendor/urllib3/_version.py,sha256=azoM7M7BUADl2kBhMVR6PPf2GhBDI90me1fcnzTwdcw,64
 pip/_vendor/urllib3/connection.py,sha256=92k9td_y4PEiTIjNufCUa1NzMB3J3w0LEdyokYgXnW8,20300
 pip/_vendor/urllib3/connectionpool.py,sha256=ItVDasDnPRPP9R8bNxY7tPBlC724nJ9nlxVgXG_SLbI,39990
 pip/_vendor/urllib3/exceptions.py,sha256=0Mnno3KHTNfXRfY7638NufOPkUb6mXOm-Lqj-4x2w8A,8217
 pip/_vendor/urllib3/fields.py,sha256=kvLDCg_JmH1lLjUUEY_FLS8UhY7hBvDPuVETbY8mdrM,8579
@@ -498,575 +511,575 @@
 pip/_vendor/urllib3/util/url.py,sha256=lCAE7M5myA8EDdW0sJuyyZhVB9K_j38ljWhHAnFaWoE,14296
 pip/_vendor/urllib3/util/wait.py,sha256=fOX0_faozG2P7iVojQoE1mbydweNyTcm-hXEfFrTtLI,5403
 pip/_vendor/webencodings/__init__.py,sha256=qOBJIuPy_4ByYH6W_bNgJF-qYQ2DoU-dKsDu5yRWCXg,10579
 pip/_vendor/webencodings/labels.py,sha256=4AO_KxTddqGtrL9ns7kAPjb0CcN6xsCIxbK37HY9r3E,8979
 pip/_vendor/webencodings/mklabels.py,sha256=GYIeywnpaLnP0GSic8LFWgd0UVvO_l1Nc6YoF-87R_4,1305
 pip/_vendor/webencodings/tests.py,sha256=OtGLyjhNY1fvkW1GvLJ_FV9ZoqC9Anyjr7q3kxTbzNs,6563
 pip/_vendor/webencodings/x_user_defined.py,sha256=yOqWSdmpytGfUgh_Z6JYgDNhoc-BAHyyeeT15Fr42tM,4307
-pip-23.3.1.dist-info/AUTHORS.txt,sha256=HOVK0m4Fk7uZrqt9MhiBlBTdmUbMIxXJziTWeMc_Jxc,10253
-pip-23.3.1.dist-info/LICENSE.txt,sha256=Y0MApmnUmurmWxLGxIySTFGkzfPR_whtw0VtyLyqIQQ,1093
-pip-23.3.1.dist-info/METADATA,sha256=ePd4oJwtCOg7e5hjeRczRRgaxHUSasxlmRPNHMtKToE,3540
-pip-23.3.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-pip-23.3.1.dist-info/entry_points.txt,sha256=xg35gOct0aY8S3ftLtweJ0uw3KBAIVyW4k-0Jx1rkNE,125
-pip-23.3.1.dist-info/top_level.txt,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
-pip-23.3.1.dist-info/RECORD,,
-pip/_internal/locations/__init__.cpython-312.pyc,,
-pip/_internal/cli/status_codes.cpython-312.pyc,,
-pip/_internal/resolution/legacy/__pycache__,,
-pip/_vendor/cachecontrol/serialize.cpython-312.pyc,,
-pip/_vendor/requests/hooks.cpython-312.pyc,,
-pip/_internal/utils/compat.cpython-312.pyc,,
-pip/_internal/operations/install/wheel.cpython-312.pyc,,
-pip/_vendor/chardet/universaldetector.cpython-312.pyc,,
-pip/_vendor/colorama/ansi.cpython-312.pyc,,
-pip/_vendor/resolvelib/reporters.cpython-312.pyc,,
-pip/_vendor/distro/__pycache__,,
-pip/_vendor/pygments/formatters/pangomarkup.cpython-312.pyc,,
-pip/_vendor/chardet/charsetgroupprober.cpython-312.pyc,,
-pip/_vendor/urllib3/util/retry.cpython-312.pyc,,
-pip/_vendor/urllib3/util/proxy.cpython-312.pyc,,
-pip/_internal/index/package_finder.cpython-312.pyc,,
-pip/_vendor/chardet/langturkishmodel.cpython-312.pyc,,
-pip/_internal/models/selection_prefs.cpython-312.pyc,,
-pip/_vendor/rich/filesize.cpython-312.pyc,,
-pip/_vendor/six.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/other.cpython-312.pyc,,
-pip/_vendor/pygments/lexer.cpython-312.pyc,,
-pip/_internal/index/sources.cpython-312.pyc,,
-pip/_vendor/rich/_palettes.cpython-312.pyc,,
+pip-24.0.dist-info/AUTHORS.txt,sha256=SwXm4nkwRkmtnO1ZY-dLy7EPeoQNXMNLby5CN3GlNhY,10388
+pip-24.0.dist-info/LICENSE.txt,sha256=Y0MApmnUmurmWxLGxIySTFGkzfPR_whtw0VtyLyqIQQ,1093
+pip-24.0.dist-info/METADATA,sha256=kNEfJ3_Vho2mee4lfJdlbd5RHIqsfQJSMUB-bOkIOeI,3581
+pip-24.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+pip-24.0.dist-info/entry_points.txt,sha256=ynZN1_707_L23Oa8_O5LOxEoccj1nDa4xHT5galfN7o,125
+pip-24.0.dist-info/top_level.txt,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
+pip-24.0.dist-info/RECORD,,
+pip/_internal/metadata/importlib/__pycache__,,
+pip/_vendor/pygments/formatters/img.cpython-312.pyc,,
+pip/_vendor/rich/color_triplet.cpython-312.pyc,,
+pip/_vendor/chardet/version.cpython-312.pyc,,
+pip/_internal/commands/show.cpython-312.pyc,,
+pip/_internal/utils/packaging.cpython-312.pyc,,
 pip/_vendor/cachecontrol/heuristics.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/_appengine_environ.cpython-312.pyc,,
-pip/_vendor/packaging/version.cpython-312.pyc,,
-pip/_vendor/pygments/styles/__init__.cpython-312.pyc,,
-pip/_vendor/tenacity/__init__.cpython-312.pyc,,
-pip/_internal/models/format_control.cpython-312.pyc,,
-pip/_vendor/rich/_export_format.cpython-312.pyc,,
-pip/_vendor/urllib3/__init__.cpython-312.pyc,,
-pip/_vendor/chardet/charsetprober.cpython-312.pyc,,
-pip/_internal/utils/datetime.cpython-312.pyc,,
-pip/_internal/operations/build/wheel_editable.cpython-312.pyc,,
-pip/_vendor/cachecontrol/cache.cpython-312.pyc,,
-pip/_vendor/rich/_win32_console.cpython-312.pyc,,
+pip/_internal/utils/setuptools_build.cpython-312.pyc,,
+pip/_internal/utils/filesystem.cpython-312.pyc,,
+pip/_internal/req/req_set.cpython-312.pyc,,
+pip/_vendor/chardet/utf8prober.cpython-312.pyc,,
+pip/_vendor/requests/__version__.cpython-312.pyc,,
+pip/_internal/utils/__pycache__,,
+pip/_internal/commands/download.cpython-312.pyc,,
+pip/_vendor/pyparsing/results.cpython-312.pyc,,
+pip/_vendor/rich/color.cpython-312.pyc,,
+pip/_internal/network/lazy_wheel.cpython-312.pyc,,
 pip/_vendor/colorama/tests/winterm_test.cpython-312.pyc,,
-pip/_internal/operations/__init__.cpython-312.pyc,,
-pip/_vendor/webencodings/mklabels.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/__pycache__,,
-pip/_vendor/colorama/tests/ansi_test.cpython-312.pyc,,
-pip/_vendor/urllib3/util/__init__.cpython-312.pyc,,
-pip/_vendor/requests/models.cpython-312.pyc,,
-pip/_vendor/__init__.cpython-312.pyc,,
-pip/_internal/models/wheel.cpython-312.pyc,,
-pip/_vendor/rich/diagnose.cpython-312.pyc,,
-pip/_vendor/urllib3/util/url.cpython-312.pyc,,
-pip/_internal/commands/check.cpython-312.pyc,,
-pip/_vendor/urllib3/connection.cpython-312.pyc,,
-pip/_vendor/urllib3/util/ssl_.cpython-312.pyc,,
-pip/_vendor/colorama/__pycache__,,
-pip/_vendor/chardet/mbcharsetprober.cpython-312.pyc,,
-pip/_vendor/requests/auth.cpython-312.pyc,,
-pip/_vendor/pygments/token.cpython-312.pyc,,
-pip/_internal/utils/subprocess.cpython-312.pyc,,
-pip/_vendor/distlib/compat.cpython-312.pyc,,
-pip/_internal/utils/filetypes.cpython-312.pyc,,
-pip/_vendor/distlib/resources.cpython-312.pyc,,
-pip/_vendor/colorama/tests/ansitowin32_test.cpython-312.pyc,,
-pip/_vendor/rich/palette.cpython-312.pyc,,
-pip/_vendor/rich/text.cpython-312.pyc,,
+pip/_vendor/rich/panel.cpython-312.pyc,,
+pip/_vendor/tomli/_parser.cpython-312.pyc,,
+pip/_internal/utils/virtualenv.cpython-312.pyc,,
+pip/_vendor/webencodings/labels.cpython-312.pyc,,
+pip/_internal/operations/build/__pycache__,,
+pip/_vendor/distro/__pycache__,,
+pip/_internal/utils/deprecation.cpython-312.pyc,,
+pip/_vendor/packaging/_structures.cpython-312.pyc,,
+pip/_vendor/rich/file_proxy.cpython-312.pyc,,
+pip/_internal/cli/command_context.cpython-312.pyc,,
+pip/_internal/utils/wheel.cpython-312.pyc,,
 pip/_internal/main.cpython-312.pyc,,
-pip/_vendor/rich/_stack.cpython-312.pyc,,
-pip/_vendor/colorama/win32.cpython-312.pyc,,
-pip/_vendor/distlib/version.cpython-312.pyc,,
-pip/_vendor/pyproject_hooks/_in_process/__pycache__,,
-pip/_internal/utils/_jaraco_text.cpython-312.pyc,,
-pip/_internal/cli/main_parser.cpython-312.pyc,,
-pip/_vendor/resolvelib/resolvers.cpython-312.pyc,,
-pip/_vendor/chardet/big5prober.cpython-312.pyc,,
-pip/_vendor/distlib/__init__.cpython-312.pyc,,
+pip/_vendor/requests/status_codes.cpython-312.pyc,,
+pip/_vendor/rich/themes.cpython-312.pyc,,
+pip/_internal/metadata/importlib/_compat.cpython-312.pyc,,
+../../../bin/pip3.12,,
+pip/_internal/resolution/resolvelib/found_candidates.cpython-312.pyc,,
+pip/_vendor/rich/rule.cpython-312.pyc,,
+pip/_vendor/chardet/escsm.cpython-312.pyc,,
+pip/_vendor/urllib3/exceptions.cpython-312.pyc,,
+pip/_internal/utils/__init__.cpython-312.pyc,,
+pip/_vendor/pkg_resources/__init__.cpython-312.pyc,,
+pip/_vendor/requests/help.cpython-312.pyc,,
+pip/_vendor/rich/default_styles.cpython-312.pyc,,
+pip/_vendor/requests/exceptions.cpython-312.pyc,,
+pip/_vendor/pygments/token.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/__init__.cpython-312.pyc,,
+pip/_vendor/urllib3/util/wait.cpython-312.pyc,,
+pip/_vendor/chardet/macromanprober.cpython-312.pyc,,
+pip/_internal/models/scheme.cpython-312.pyc,,
+pip/_vendor/chardet/langthaimodel.cpython-312.pyc,,
+pip/__init__.cpython-312.pyc,,
+pip/_vendor/colorama/ansitowin32.cpython-312.pyc,,
+pip/_vendor/requests/__pycache__,,
+pip/_vendor/pyproject_hooks/_in_process/_in_process.cpython-312.pyc,,
+pip/_internal/utils/encoding.cpython-312.pyc,,
+pip/_internal/metadata/importlib/_envs.cpython-312.pyc,,
+pip/_internal/network/cache.cpython-312.pyc,,
+pip/_internal/models/search_scope.cpython-312.pyc,,
+pip/_vendor/pygments/style.cpython-312.pyc,,
+pip/_internal/resolution/resolvelib/base.cpython-312.pyc,,
 pip/_vendor/cachecontrol/__pycache__,,
-pip/_vendor/chardet/hebrewprober.cpython-312.pyc,,
-pip/_vendor/chardet/big5freq.cpython-312.pyc,,
-pip/_internal/utils/entrypoints.cpython-312.pyc,,
+pip/_vendor/truststore/_ssl_constants.cpython-312.pyc,,
+pip/_internal/cli/main.cpython-312.pyc,,
+pip/_internal/commands/check.cpython-312.pyc,,
+pip/_vendor/urllib3/util/connection.cpython-312.pyc,,
+pip/_vendor/chardet/johabprober.cpython-312.pyc,,
+pip/_vendor/rich/segment.cpython-312.pyc,,
+pip/_vendor/rich/highlighter.cpython-312.pyc,,
+pip/_internal/network/session.cpython-312.pyc,,
+pip/_internal/commands/debug.cpython-312.pyc,,
+pip/__main__.cpython-312.pyc,,
+pip/_vendor/cachecontrol/caches/redis_cache.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/svg.cpython-312.pyc,,
+pip/_vendor/urllib3/packages/__init__.cpython-312.pyc,,
+pip/_vendor/resolvelib/compat/collections_abc.cpython-312.pyc,,
+pip/_internal/resolution/legacy/resolver.cpython-312.pyc,,
+pip/_vendor/pygments/util.cpython-312.pyc,,
+pip/_vendor/distlib/util.cpython-312.pyc,,
+pip/_vendor/colorama/win32.cpython-312.pyc,,
 pip/_vendor/resolvelib/providers.cpython-312.pyc,,
-pip/_vendor/rich/_fileno.cpython-312.pyc,,
+pip/_vendor/rich/ansi.cpython-312.pyc,,
+pip/_vendor/rich/_log_render.cpython-312.pyc,,
+pip/_vendor/pygments/filter.cpython-312.pyc,,
 pip/_vendor/rich/__init__.cpython-312.pyc,,
-pip/_vendor/msgpack/exceptions.cpython-312.pyc,,
-pip/_vendor/pygments/style.cpython-312.pyc,,
-pip/_internal/operations/build/__pycache__,,
-pip/_internal/distributions/installed.cpython-312.pyc,,
-pip/_vendor/requests/certs.cpython-312.pyc,,
-pip/__init__.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__,,
-pip/_vendor/urllib3/poolmanager.cpython-312.pyc,,
-pip/_vendor/rich/_pick.cpython-312.pyc,,
-pip/_vendor/rich/containers.cpython-312.pyc,,
-pip/_vendor/requests/adapters.cpython-312.pyc,,
-pip/_internal/utils/temp_dir.cpython-312.pyc,,
-pip/_internal/operations/build/build_tracker.cpython-312.pyc,,
-pip/_vendor/idna/uts46data.cpython-312.pyc,,
-pip/_vendor/rich/_windows.cpython-312.pyc,,
-pip/_vendor/requests/__init__.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/candidates.cpython-312.pyc,,
-pip/_internal/locations/_distutils.cpython-312.pyc,,
-pip/_vendor/platformdirs/android.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/terminal.cpython-312.pyc,,
-pip/_vendor/rich/columns.cpython-312.pyc,,
-pip/_vendor/urllib3/_collections.cpython-312.pyc,,
-pip/_internal/exceptions.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/resolver.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/latex.cpython-312.pyc,,
-pip/_vendor/chardet/langrussianmodel.cpython-312.pyc,,
-pip/_vendor/urllib3/packages/backports/weakref_finalize.cpython-312.pyc,,
-pip/_vendor/rich/highlighter.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/html.cpython-312.pyc,,
-pip/_vendor/distro/__init__.cpython-312.pyc,,
-pip/_vendor/requests/structures.cpython-312.pyc,,
-pip/_vendor/colorama/initialise.cpython-312.pyc,,
-pip/_internal/cli/progress_bars.cpython-312.pyc,,
+pip/_vendor/platformdirs/__main__.cpython-312.pyc,,
 pip/_internal/cli/cmdoptions.cpython-312.pyc,,
-pip/_internal/network/session.cpython-312.pyc,,
-pip/_internal/metadata/__init__.cpython-312.pyc,,
-pip/_vendor/chardet/macromanprober.cpython-312.pyc,,
-pip/_vendor/requests/_internal_utils.cpython-312.pyc,,
-pip/_vendor/distlib/scripts.cpython-312.pyc,,
-pip/_vendor/pygments/lexers/__pycache__,,
-pip/_internal/operations/install/__pycache__,,
-pip/_vendor/tomli/_re.cpython-312.pyc,,
-pip/_internal/locations/__pycache__,,
-pip/_internal/models/index.cpython-312.pyc,,
-pip/_internal/__init__.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/__init__.cpython-312.pyc,,
+pip/_vendor/rich/styled.cpython-312.pyc,,
+pip/_internal/metadata/__pycache__,,
+pip/_internal/commands/list.cpython-312.pyc,,
+pip/_vendor/colorama/tests/utils.cpython-312.pyc,,
+pip/_vendor/chardet/euctwfreq.cpython-312.pyc,,
 pip/_internal/network/__pycache__,,
-pip/_internal/req/req_install.cpython-312.pyc,,
-pip/_vendor/urllib3/packages/__pycache__,,
-pip/_vendor/idna/intranges.cpython-312.pyc,,
-pip/_vendor/rich/pretty.cpython-312.pyc,,
-pip/_internal/req/__pycache__,,
-pip/_vendor/chardet/eucjpprober.cpython-312.pyc,,
-pip/_vendor/colorama/winterm.cpython-312.pyc,,
-pip/_vendor/rich/__main__.cpython-312.pyc,,
-pip/_internal/utils/filesystem.cpython-312.pyc,,
-pip/_vendor/rich/themes.cpython-312.pyc,,
-pip/_internal/index/__pycache__,,
-pip/_internal/vcs/mercurial.cpython-312.pyc,,
-pip/_vendor/platformdirs/macos.cpython-312.pyc,,
-pip/_vendor/pygments/__main__.cpython-312.pyc,,
-pip/_vendor/chardet/version.cpython-312.pyc,,
-pip/__main__.cpython-312.pyc,,
-pip/_vendor/chardet/jpcntx.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/appengine.cpython-312.pyc,,
-pip/_vendor/requests/exceptions.cpython-312.pyc,,
-pip/_vendor/tenacity/before.cpython-312.pyc,,
-pip/_internal/distributions/sdist.cpython-312.pyc,,
-pip/_vendor/cachecontrol/caches/__init__.cpython-312.pyc,,
+pip/_internal/models/direct_url.cpython-312.pyc,,
+pip/_internal/locations/_distutils.cpython-312.pyc,,
+pip/_vendor/urllib3/fields.cpython-312.pyc,,
+pip/_vendor/pyproject_hooks/_compat.cpython-312.pyc,,
+pip/_vendor/requests/api.cpython-312.pyc,,
+pip/_vendor/colorama/tests/ansi_test.cpython-312.pyc,,
+pip/_vendor/requests/sessions.cpython-312.pyc,,
+pip/_vendor/pygments/formatter.cpython-312.pyc,,
+pip/_vendor/pygments/lexers/_mapping.cpython-312.pyc,,
+pip/_vendor/chardet/escprober.cpython-312.pyc,,
+pip/_vendor/distro/__main__.cpython-312.pyc,,
+pip/_internal/network/download.cpython-312.pyc,,
 pip/_vendor/chardet/mbcssm.cpython-312.pyc,,
-pip/_vendor/chardet/gb2312freq.cpython-312.pyc,,
-pip/_vendor/pygments/__pycache__,,
-pip/_internal/models/installation_report.cpython-312.pyc,,
-pip/_internal/metadata/pkg_resources.cpython-312.pyc,,
-pip/_vendor/chardet/johabprober.cpython-312.pyc,,
-pip/_vendor/colorama/__init__.cpython-312.pyc,,
-pip/_vendor/rich/_windows_renderer.cpython-312.pyc,,
+pip/_vendor/chardet/metadata/languages.cpython-312.pyc,,
+pip/_vendor/tenacity/after.cpython-312.pyc,,
+pip/_vendor/rich/box.cpython-312.pyc,,
+pip/_vendor/rich/logging.cpython-312.pyc,,
+pip/_internal/utils/compatibility_tags.cpython-312.pyc,,
+pip/_vendor/cachecontrol/cache.cpython-312.pyc,,
 pip/_vendor/chardet/codingstatemachinedict.cpython-312.pyc,,
-pip/_internal/utils/glibc.cpython-312.pyc,,
-pip/_vendor/rich/__pycache__,,
+pip/_vendor/cachecontrol/caches/file_cache.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/rtf.cpython-312.pyc,,
+pip/_vendor/colorama/tests/__init__.cpython-312.pyc,,
+pip/_internal/operations/build/wheel.cpython-312.pyc,,
+pip/_internal/commands/hash.cpython-312.pyc,,
+pip/_internal/models/link.cpython-312.pyc,,
+pip/_internal/metadata/importlib/__init__.cpython-312.pyc,,
+pip/_internal/resolution/resolvelib/factory.cpython-312.pyc,,
 pip/_vendor/webencodings/x_user_defined.cpython-312.pyc,,
-pip/_vendor/rich/file_proxy.cpython-312.pyc,,
-pip/_internal/commands/help.cpython-312.pyc,,
+pip/_vendor/distlib/__init__.cpython-312.pyc,,
+pip/_vendor/platformdirs/version.cpython-312.pyc,,
+pip/_vendor/rich/traceback.cpython-312.pyc,,
+pip-24.0.dist-info/INSTALLER,,
+pip/_vendor/tenacity/_utils.cpython-312.pyc,,
+pip/_internal/cli/spinners.cpython-312.pyc,,
+pip/_internal/cache.cpython-312.pyc,,
+pip/_internal/commands/inspect.cpython-312.pyc,,
+pip/_vendor/colorama/tests/__pycache__,,
 pip/_vendor/urllib3/contrib/_securetransport/low_level.cpython-312.pyc,,
-pip/_vendor/rich/panel.cpython-312.pyc,,
-pip/_internal/utils/compatibility_tags.cpython-312.pyc,,
-pip/_internal/cli/main.cpython-312.pyc,,
-pip/_vendor/pkg_resources/__init__.cpython-312.pyc,,
-pip/_vendor/urllib3/util/queue.cpython-312.pyc,,
-pip/_vendor/distlib/util.cpython-312.pyc,,
-pip/_vendor/chardet/langthaimodel.cpython-312.pyc,,
-pip/_internal/utils/_log.cpython-312.pyc,,
-pip/_vendor/platformdirs/windows.cpython-312.pyc,,
-pip/_vendor/pygments/lexers/__init__.cpython-312.pyc,,
-pip/_vendor/pyparsing/unicode.cpython-312.pyc,,
-pip/_vendor/requests/__pycache__,,
-pip/_vendor/truststore/__init__.cpython-312.pyc,,
-pip/_vendor/chardet/euckrprober.cpython-312.pyc,,
-pip/_vendor/chardet/jisfreq.cpython-312.pyc,,
-pip/_internal/cli/req_command.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/_mapping.cpython-312.pyc,,
-pip/_vendor/truststore/__pycache__,,
-pip/_vendor/rich/theme.cpython-312.pyc,,
-pip/_internal/metadata/__pycache__,,
-pip/_vendor/truststore/_ssl_constants.cpython-312.pyc,,
-pip/_vendor/distlib/wheel.cpython-312.pyc,,
-pip/_vendor/cachecontrol/_cmd.cpython-312.pyc,,
-../../../bin/pip,,
-pip/_internal/operations/build/metadata.cpython-312.pyc,,
-pip/_internal/resolution/__pycache__,,
-pip/_internal/utils/logging.cpython-312.pyc,,
-pip/_vendor/urllib3/packages/backports/makefile.cpython-312.pyc,,
-pip/_vendor/cachecontrol/caches/file_cache.cpython-312.pyc,,
-pip/_vendor/packaging/requirements.cpython-312.pyc,,
-pip/_vendor/tenacity/after.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/groff.cpython-312.pyc,,
-pip/_internal/network/auth.cpython-312.pyc,,
-pip/_vendor/pyparsing/diagram/__init__.cpython-312.pyc,,
-pip/_internal/commands/download.cpython-312.pyc,,
-pip/_vendor/chardet/langbulgarianmodel.cpython-312.pyc,,
-pip/_vendor/platformdirs/__init__.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/__init__.cpython-312.pyc,,
-pip/_vendor/idna/__pycache__,,
-pip/_vendor/rich/progress_bar.cpython-312.pyc,,
-pip/_vendor/requests/help.cpython-312.pyc,,
-pip/_internal/build_env.cpython-312.pyc,,
-pip/_vendor/chardet/metadata/__pycache__,,
-pip/_internal/operations/__pycache__,,
-pip/_vendor/pyproject_hooks/_impl.cpython-312.pyc,,
-pip/_vendor/typing_extensions.cpython-312.pyc,,
-pip/_internal/utils/deprecation.cpython-312.pyc,,
-pip/_vendor/rich/console.cpython-312.pyc,,
-pip/_vendor/tenacity/nap.cpython-312.pyc,,
-pip/_vendor/tomli/_types.cpython-312.pyc,,
-pip/_vendor/pygments/styles/__pycache__,,
-pip/_internal/operations/install/__init__.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/__pycache__,,
-pip/_internal/network/utils.cpython-312.pyc,,
-pip/_vendor/chardet/metadata/languages.cpython-312.pyc,,
-pip/_internal/utils/packaging.cpython-312.pyc,,
-pip/_vendor/tenacity/wait.cpython-312.pyc,,
-pip/_vendor/pygments/regexopt.cpython-312.pyc,,
-pip/_vendor/tenacity/before_sleep.cpython-312.pyc,,
-pip/_internal/metadata/importlib/_envs.cpython-312.pyc,,
-pip/_vendor/idna/package_data.cpython-312.pyc,,
-pip/_internal/cli/__init__.cpython-312.pyc,,
-pip/_vendor/rich/terminal_theme.cpython-312.pyc,,
-pip/_vendor/urllib3/util/wait.cpython-312.pyc,,
-pip/_vendor/__pycache__,,
-pip/_vendor/pyproject_hooks/_in_process/_in_process.cpython-312.pyc,,
-pip/_internal/commands/debug.cpython-312.pyc,,
-pip/_vendor/rich/prompt.cpython-312.pyc,,
-pip/_vendor/msgpack/fallback.cpython-312.pyc,,
-pip/_internal/commands/configuration.cpython-312.pyc,,
+pip/_vendor/distlib/database.cpython-312.pyc,,
+pip/_vendor/rich/_win32_console.cpython-312.pyc,,
 pip/_internal/req/req_file.cpython-312.pyc,,
-pip/_vendor/requests/utils.cpython-312.pyc,,
-pip/_internal/cli/base_command.cpython-312.pyc,,
-pip/_vendor/rich/measure.cpython-312.pyc,,
-pip/_internal/commands/list.cpython-312.pyc,,
-pip/_vendor/urllib3/util/timeout.cpython-312.pyc,,
-pip/__pip-runner__.cpython-312.pyc,,
-pip/_internal/operations/build/metadata_legacy.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/provider.cpython-312.pyc,,
-pip/_vendor/chardet/enums.cpython-312.pyc,,
-pip/_vendor/pygments/lexers/python.cpython-312.pyc,,
-pip/_vendor/cachecontrol/adapter.cpython-312.pyc,,
-pip/_vendor/pyproject_hooks/_compat.cpython-312.pyc,,
+pip/_internal/utils/datetime.cpython-312.pyc,,
+pip/_vendor/urllib3/util/response.cpython-312.pyc,,
 pip/_vendor/truststore/_api.cpython-312.pyc,,
-pip/_vendor/rich/rule.cpython-312.pyc,,
-pip/_internal/utils/__init__.cpython-312.pyc,,
-pip/_internal/utils/unpacking.cpython-312.pyc,,
-pip/_vendor/rich/control.cpython-312.pyc,,
-pip/_vendor/cachecontrol/caches/__pycache__,,
+pip/_vendor/rich/_stack.cpython-312.pyc,,
+pip/_internal/operations/build/metadata.cpython-312.pyc,,
+pip/_vendor/idna/idnadata.cpython-312.pyc,,
+pip/_vendor/urllib3/_collections.cpython-312.pyc,,
+../../../bin/pip-3.12,,
+pip/_vendor/colorama/__pycache__,,
+pip/_vendor/certifi/__pycache__,,
+pip/_vendor/distlib/scripts.cpython-312.pyc,,
+pip/_vendor/distlib/markers.cpython-312.pyc,,
+pip/_vendor/pyparsing/common.cpython-312.pyc,,
+pip/_vendor/tenacity/retry.cpython-312.pyc,,
+pip/_vendor/rich/pager.cpython-312.pyc,,
+pip/_internal/resolution/base.cpython-312.pyc,,
+pip/_vendor/chardet/langrussianmodel.cpython-312.pyc,,
+pip/_vendor/idna/package_data.cpython-312.pyc,,
+pip/_vendor/pygments/console.cpython-312.pyc,,
+pip/_vendor/pygments/styles/__pycache__,,
+pip/_vendor/requests/__init__.cpython-312.pyc,,
+pip/_internal/vcs/__pycache__,,
+pip/_vendor/chardet/metadata/__init__.cpython-312.pyc,,
+pip/_internal/network/__init__.cpython-312.pyc,,
+pip/_vendor/pygments/filters/__pycache__,,
 pip/_vendor/urllib3/util/request.cpython-312.pyc,,
-pip/_internal/vcs/versioncontrol.cpython-312.pyc,,
-pip/_internal/operations/prepare.cpython-312.pyc,,
+pip/_vendor/pygments/lexers/python.cpython-312.pyc,,
+pip/_internal/utils/urls.cpython-312.pyc,,
+pip/_internal/metadata/__init__.cpython-312.pyc,,
+pip/_internal/operations/freeze.cpython-312.pyc,,
+pip/_internal/index/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/big5prober.cpython-312.pyc,,
+pip/_internal/utils/entrypoints.cpython-312.pyc,,
+pip/_internal/operations/install/wheel.cpython-312.pyc,,
+pip/_internal/models/__pycache__,,
+pip/_internal/req/req_install.cpython-312.pyc,,
+pip/_vendor/urllib3/connectionpool.cpython-312.pyc,,
+pip/_internal/utils/glibc.cpython-312.pyc,,
+pip/_internal/vcs/__init__.cpython-312.pyc,,
 pip/_vendor/chardet/resultdict.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/_securetransport/bindings.cpython-312.pyc,,
-pip/_internal/__pycache__,,
-pip/_vendor/pygments/lexers/_mapping.cpython-312.pyc,,
-pip/_vendor/platformdirs/api.cpython-312.pyc,,
-pip/_internal/metadata/importlib/_dists.cpython-312.pyc,,
-pip/_internal/distributions/__init__.cpython-312.pyc,,
-pip/_vendor/platformdirs/__main__.cpython-312.pyc,,
+pip/_internal/commands/wheel.cpython-312.pyc,,
+pip/_vendor/rich/syntax.cpython-312.pyc,,
+pip/_internal/req/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/charsetprober.cpython-312.pyc,,
+pip/_vendor/requests/auth.cpython-312.pyc,,
+pip/_vendor/packaging/requirements.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/_appengine_environ.cpython-312.pyc,,
 pip/_vendor/urllib3/packages/backports/__pycache__,,
-pip/_vendor/tenacity/__pycache__,,
-pip/_vendor/resolvelib/__pycache__,,
-pip/_vendor/chardet/sjisprober.cpython-312.pyc,,
-pip/_vendor/chardet/cli/__init__.cpython-312.pyc,,
-pip/_vendor/packaging/__pycache__,,
-pip/_vendor/tenacity/_utils.cpython-312.pyc,,
-pip/_internal/utils/urls.cpython-312.pyc,,
-pip/_vendor/webencodings/tests.cpython-312.pyc,,
-pip/_internal/models/scheme.cpython-312.pyc,,
-pip/_internal/utils/encoding.cpython-312.pyc,,
 pip/_vendor/cachecontrol/wrapper.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/base.cpython-312.pyc,,
-pip/_internal/commands/completion.cpython-312.pyc,,
-pip/_vendor/rich/_extension.cpython-312.pyc,,
-pip/_vendor/requests/api.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/_securetransport/__pycache__,,
-pip/_vendor/rich/table.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/pyopenssl.cpython-312.pyc,,
-pip/_vendor/cachecontrol/__init__.cpython-312.pyc,,
-pip/_vendor/rich/emoji.cpython-312.pyc,,
-pip/_vendor/resolvelib/compat/__pycache__,,
-pip/_vendor/pygments/formatters/img.cpython-312.pyc,,
-pip/_vendor/packaging/__init__.cpython-312.pyc,,
-pip/_vendor/pyparsing/helpers.cpython-312.pyc,,
-pip/_internal/self_outdated_check.cpython-312.pyc,,
-pip/_vendor/pygments/sphinxext.cpython-312.pyc,,
-pip/_vendor/truststore/_openssl.cpython-312.pyc,,
-pip/_vendor/chardet/cli/__pycache__,,
-pip/_vendor/cachecontrol/controller.cpython-312.pyc,,
-pip/_internal/utils/appdirs.cpython-312.pyc,,
-pip/_internal/locations/base.cpython-312.pyc,,
-pip/_vendor/packaging/__about__.cpython-312.pyc,,
-pip/_internal/network/xmlrpc.cpython-312.pyc,,
-pip/_vendor/chardet/utf1632prober.cpython-312.pyc,,
+pip/_vendor/urllib3/util/__init__.cpython-312.pyc,,
+pip/_vendor/packaging/specifiers.cpython-312.pyc,,
+pip/_vendor/chardet/charsetgroupprober.cpython-312.pyc,,
+pip/_internal/resolution/legacy/__pycache__,,
+pip/_vendor/rich/align.cpython-312.pyc,,
+pip/_vendor/pyproject_hooks/__pycache__,,
+pip/_internal/utils/logging.cpython-312.pyc,,
+pip/_vendor/requests/_internal_utils.cpython-312.pyc,,
+pip/_vendor/chardet/langgreekmodel.cpython-312.pyc,,
+pip/_vendor/requests/structures.cpython-312.pyc,,
+pip/_internal/distributions/__init__.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/pangomarkup.cpython-312.pyc,,
 pip/_vendor/pyparsing/exceptions.cpython-312.pyc,,
-pip/_vendor/pyproject_hooks/__init__.cpython-312.pyc,,
-pip/_internal/utils/models.cpython-312.pyc,,
-pip/_vendor/rich/json.cpython-312.pyc,,
-pip/_vendor/rich/pager.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/svg.cpython-312.pyc,,
-pip/_vendor/colorama/tests/utils.cpython-312.pyc,,
-pip/_vendor/rich/color.cpython-312.pyc,,
-pip/_internal/operations/freeze.cpython-312.pyc,,
-pip/_vendor/chardet/__init__.cpython-312.pyc,,
-pip/_vendor/rich/color_triplet.cpython-312.pyc,,
-pip/_vendor/chardet/mbcsgroupprober.cpython-312.pyc,,
-pip/_vendor/packaging/_manylinux.cpython-312.pyc,,
-pip/_internal/req/req_uninstall.cpython-312.pyc,,
-pip/_vendor/pyparsing/core.cpython-312.pyc,,
-pip/_internal/vcs/bazaar.cpython-312.pyc,,
-pip/_vendor/chardet/langhebrewmodel.cpython-312.pyc,,
-pip/_vendor/pygments/console.cpython-312.pyc,,
-pip/_internal/commands/hash.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/ntlmpool.cpython-312.pyc,,
-pip/_vendor/rich/style.cpython-312.pyc,,
-pip/_vendor/urllib3/util/__pycache__,,
-pip/_vendor/pyparsing/actions.cpython-312.pyc,,
-pip/_vendor/urllib3/packages/six.cpython-312.pyc,,
-pip/_internal/req/constructors.cpython-312.pyc,,
-pip/_internal/resolution/legacy/resolver.cpython-312.pyc,,
-pip/_vendor/rich/live.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/rtf.cpython-312.pyc,,
-pip/_vendor/rich/segment.cpython-312.pyc,,
-pip/_vendor/rich/jupyter.cpython-312.pyc,,
-pip/_internal/utils/virtualenv.cpython-312.pyc,,
-pip/_vendor/pygments/modeline.cpython-312.pyc,,
-pip/_vendor/chardet/gb2312prober.cpython-312.pyc,,
-pip/_vendor/chardet/latin1prober.cpython-312.pyc,,
-pip/_internal/commands/search.cpython-312.pyc,,
-pip/_internal/models/direct_url.cpython-312.pyc,,
-pip/_internal/metadata/importlib/_compat.cpython-312.pyc,,
-pip/_vendor/chardet/euctwfreq.cpython-312.pyc,,
-pip/_internal/vcs/__init__.cpython-312.pyc,,
-pip/_vendor/platformdirs/unix.cpython-312.pyc,,
-pip/_internal/operations/build/metadata_editable.cpython-312.pyc,,
-pip/_vendor/chardet/langhungarianmodel.cpython-312.pyc,,
-pip/_vendor/idna/compat.cpython-312.pyc,,
+pip/_vendor/rich/pretty.cpython-312.pyc,,
+pip/_vendor/pygments/cmdline.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/__pycache__,,
+pip/_vendor/pygments/lexers/__pycache__,,
+pip/_vendor/rich/filesize.cpython-312.pyc,,
 pip/_vendor/tenacity/stop.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/_securetransport/__init__.cpython-312.pyc,,
-pip/_internal/operations/install/editable_legacy.cpython-312.pyc,,
-pip/_vendor/tomli/_parser.cpython-312.pyc,,
-pip/_vendor/colorama/tests/initialise_test.cpython-312.pyc,,
-pip/_vendor/platformdirs/version.cpython-312.pyc,,
-pip/_vendor/pygments/plugin.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/reporter.cpython-312.pyc,,
-pip/_internal/wheel_builder.cpython-312.pyc,,
-pip/_vendor/distlib/metadata.cpython-312.pyc,,
-pip/_vendor/chardet/johabfreq.cpython-312.pyc,,
-pip/_vendor/webencodings/labels.cpython-312.pyc,,
-pip/_internal/commands/__pycache__,,
-pip/_internal/network/lazy_wheel.cpython-312.pyc,,
-pip/_vendor/rich/spinner.cpython-312.pyc,,
-pip/_vendor/rich/region.cpython-312.pyc,,
-pip/_vendor/pygments/formatter.cpython-312.pyc,,
-pip/_vendor/webencodings/__pycache__,,
+pip/_internal/commands/install.cpython-312.pyc,,
+pip/_vendor/requests/packages.cpython-312.pyc,,
+pip/_vendor/packaging/_manylinux.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/irc.cpython-312.pyc,,
+pip/_internal/vcs/subversion.cpython-312.pyc,,
+pip/_internal/resolution/resolvelib/requirements.cpython-312.pyc,,
+pip/_vendor/tomli/_re.cpython-312.pyc,,
+pip/_vendor/pyparsing/diagram/__pycache__,,
+pip/_internal/exceptions.cpython-312.pyc,,
+pip/_internal/metadata/pkg_resources.cpython-312.pyc,,
 pip/_vendor/pygments/formatters/terminal256.cpython-312.pyc,,
-pip/_vendor/rich/traceback.cpython-312.pyc,,
-../../../bin/pip3,,
-pip/_vendor/rich/_ratio.cpython-312.pyc,,
-pip/_vendor/pygments/filter.cpython-312.pyc,,
-pip/_vendor/rich/_spinners.cpython-312.pyc,,
-pip/_internal/metadata/importlib/__pycache__,,
+pip/_vendor/distlib/__pycache__,,
+pip/_vendor/platformdirs/__init__.cpython-312.pyc,,
+pip/_vendor/msgpack/ext.cpython-312.pyc,,
+pip/_internal/utils/models.cpython-312.pyc,,
+pip/_vendor/rich/_null_file.cpython-312.pyc,,
+pip/_vendor/chardet/cp949prober.cpython-312.pyc,,
+pip/_internal/cli/__pycache__,,
+pip/_vendor/six.cpython-312.pyc,,
+pip/_vendor/requests/certs.cpython-312.pyc,,
+pip/_vendor/rich/palette.cpython-312.pyc,,
+pip/_vendor/chardet/universaldetector.cpython-312.pyc,,
+pip/_internal/operations/build/wheel_legacy.cpython-312.pyc,,
+pip/_vendor/distlib/version.cpython-312.pyc,,
+pip/_vendor/webencodings/__pycache__,,
+pip/_internal/models/candidate.cpython-312.pyc,,
+pip/_vendor/cachecontrol/serialize.cpython-312.pyc,,
+pip/_internal/locations/base.cpython-312.pyc,,
+pip/_vendor/packaging/utils.cpython-312.pyc,,
+pip/_vendor/cachecontrol/caches/__pycache__,,
+pip/_internal/resolution/resolvelib/resolver.cpython-312.pyc,,
+pip/_vendor/urllib3/filepost.cpython-312.pyc,,
+pip/_vendor/chardet/chardistribution.cpython-312.pyc,,
+pip/_vendor/pygments/scanner.cpython-312.pyc,,
+pip/_vendor/rich/live_render.cpython-312.pyc,,
 pip/_vendor/rich/_emoji_replace.cpython-312.pyc,,
-pip/_vendor/urllib3/packages/backports/__init__.cpython-312.pyc,,
-pip/_vendor/msgpack/__pycache__,,
-pip/_vendor/rich/progress.cpython-312.pyc,,
-pip/_vendor/tomli/__pycache__,,
-pip/_vendor/rich/ansi.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/_securetransport/bindings.cpython-312.pyc,,
+pip/_internal/utils/appdirs.cpython-312.pyc,,
+pip/_internal/network/utils.cpython-312.pyc,,
+pip/_vendor/rich/containers.cpython-312.pyc,,
 pip/_internal/utils/direct_url_helpers.cpython-312.pyc,,
-pip/_vendor/rich/padding.cpython-312.pyc,,
-pip/_vendor/distro/distro.cpython-312.pyc,,
-pip/_internal/utils/misc.cpython-312.pyc,,
-pip/_vendor/distro/__main__.cpython-312.pyc,,
-pip/_vendor/truststore/_windows.cpython-312.pyc,,
-pip/_vendor/pygments/__init__.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/irc.cpython-312.pyc,,
-pip/_internal/vcs/__pycache__,,
-pip/_vendor/rich/live_render.cpython-312.pyc,,
-pip/_vendor/colorama/tests/__pycache__,,
-pip/_internal/cli/__pycache__,,
-pip/_vendor/urllib3/__pycache__,,
-pip/_vendor/rich/default_styles.cpython-312.pyc,,
-pip/_vendor/cachecontrol/caches/redis_cache.cpython-312.pyc,,
-pip/_internal/cli/parser.cpython-312.pyc,,
-pip/_vendor/requests/__version__.cpython-312.pyc,,
-pip/_vendor/rich/_null_file.cpython-312.pyc,,
-pip/_internal/models/search_scope.cpython-312.pyc,,
 pip/_vendor/msgpack/__init__.cpython-312.pyc,,
-pip/_vendor/rich/_loop.cpython-312.pyc,,
+pip/_internal/vcs/versioncontrol.cpython-312.pyc,,
+pip/_vendor/rich/region.cpython-312.pyc,,
+pip/_vendor/colorama/tests/ansitowin32_test.cpython-312.pyc,,
+pip/_vendor/rich/columns.cpython-312.pyc,,
+pip/_vendor/packaging/version.cpython-312.pyc,,
+pip/_vendor/resolvelib/structs.cpython-312.pyc,,
+pip/_internal/models/__init__.cpython-312.pyc,,
+pip/_vendor/rich/padding.cpython-312.pyc,,
+pip/_internal/commands/configuration.cpython-312.pyc,,
+pip/_vendor/chardet/big5freq.cpython-312.pyc,,
+pip/_internal/cli/main_parser.cpython-312.pyc,,
+pip/_vendor/pygments/unistring.cpython-312.pyc,,
+pip/_vendor/distlib/manifest.cpython-312.pyc,,
+pip/_vendor/urllib3/packages/six.cpython-312.pyc,,
+pip/_internal/operations/build/metadata_legacy.cpython-312.pyc,,
+pip/_vendor/urllib3/packages/backports/makefile.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/groff.cpython-312.pyc,,
+pip/_vendor/colorama/initialise.cpython-312.pyc,,
+pip/_vendor/rich/text.cpython-312.pyc,,
+pip/_vendor/pyproject_hooks/_in_process/__pycache__,,
+pip/_vendor/packaging/__pycache__,,
+pip/_vendor/chardet/mbcharsetprober.cpython-312.pyc,,
+pip/_vendor/resolvelib/__init__.cpython-312.pyc,,
 pip/_vendor/colorama/tests/isatty_test.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/found_candidates.cpython-312.pyc,,
-pip/_vendor/pkg_resources/__pycache__,,
-pip/_internal/commands/cache.cpython-312.pyc,,
-pip/_vendor/pyproject_hooks/__pycache__,,
-pip/_internal/locations/_sysconfig.cpython-312.pyc,,
-pip/_internal/cache.cpython-312.pyc,,
-pip/_internal/cli/autocompletion.cpython-312.pyc,,
-pip/_internal/commands/__init__.cpython-312.pyc,,
-pip/_vendor/chardet/utf8prober.cpython-312.pyc,,
-pip/_vendor/distlib/markers.cpython-312.pyc,,
-pip/_vendor/pygments/util.cpython-312.pyc,,
-pip/_internal/operations/build/wheel.cpython-312.pyc,,
-pip/_vendor/rich/abc.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/factory.cpython-312.pyc,,
-pip/_vendor/chardet/sbcsgroupprober.cpython-312.pyc,,
+pip/_internal/operations/install/__pycache__,,
+pip/_vendor/cachecontrol/controller.cpython-312.pyc,,
+pip/_vendor/chardet/johabfreq.cpython-312.pyc,,
 pip/_internal/metadata/base.cpython-312.pyc,,
-pip/_internal/utils/hashes.cpython-312.pyc,,
-pip/_vendor/pyparsing/testing.cpython-312.pyc,,
-pip/_internal/commands/freeze.cpython-312.pyc,,
-pip/_vendor/tenacity/retry.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/securetransport.cpython-312.pyc,,
-pip/_vendor/urllib3/_version.cpython-312.pyc,,
-pip/_vendor/distlib/__pycache__,,
-pip/_vendor/urllib3/util/ssl_match_hostname.cpython-312.pyc,,
-pip/_vendor/rich/_cell_widths.cpython-312.pyc,,
-pip/_vendor/chardet/codingstatemachine.cpython-312.pyc,,
-pip-23.3.1.virtualenv,,
-pip/_vendor/rich/protocol.cpython-312.pyc,,
-pip/_vendor/pyparsing/common.cpython-312.pyc,,
-pip/_vendor/urllib3/contrib/socks.cpython-312.pyc,,
-pip/_vendor/distlib/manifest.cpython-312.pyc,,
-pip/_internal/resolution/base.cpython-312.pyc,,
-pip/_vendor/rich/styled.cpython-312.pyc,,
-pip/_vendor/urllib3/connectionpool.cpython-312.pyc,,
-pip/_internal/models/candidate.cpython-312.pyc,,
-pip/_vendor/chardet/langgreekmodel.cpython-312.pyc,,
+pip/_vendor/rich/jupyter.cpython-312.pyc,,
+pip/_vendor/cachecontrol/__init__.cpython-312.pyc,,
+pip/_vendor/idna/uts46data.cpython-312.pyc,,
+pip/_vendor/chardet/langbulgarianmodel.cpython-312.pyc,,
 pip/_vendor/distlib/index.cpython-312.pyc,,
-pip/_internal/resolution/resolvelib/requirements.cpython-312.pyc,,
-pip/_vendor/requests/packages.cpython-312.pyc,,
-pip/_vendor/rich/scope.cpython-312.pyc,,
-pip-23.3.1.dist-info/INSTALLER,,
-pip/_vendor/chardet/escsm.cpython-312.pyc,,
-pip/_vendor/truststore/_macos.cpython-312.pyc,,
-pip/_internal/operations/build/wheel_legacy.cpython-312.pyc,,
-pip/_vendor/idna/idnadata.cpython-312.pyc,,
-pip/_vendor/pyparsing/__pycache__,,
-pip/_internal/operations/check.cpython-312.pyc,,
-pip/_vendor/urllib3/packages/__init__.cpython-312.pyc,,
-pip-23.3.1.dist-info/__pycache__,,
-pip/_vendor/rich/_emoji_codes.cpython-312.pyc,,
-pip/_internal/vcs/git.cpython-312.pyc,,
-pip/_vendor/packaging/_structures.cpython-312.pyc,,
-pip/_vendor/urllib3/util/response.cpython-312.pyc,,
-pip/__pycache__,,
+pip/_vendor/rich/theme.cpython-312.pyc,,
+pip/_vendor/tomli/_types.cpython-312.pyc,,
+pip/_vendor/cachecontrol/adapter.cpython-312.pyc,,
+pip/_vendor/resolvelib/compat/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/euckrfreq.cpython-312.pyc,,
+pip/_vendor/tenacity/_asyncio.cpython-312.pyc,,
+pip/_internal/distributions/sdist.cpython-312.pyc,,
+pip/_vendor/pyparsing/helpers.cpython-312.pyc,,
+pip/_vendor/rich/_fileno.cpython-312.pyc,,
+pip/_vendor/platformdirs/unix.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/bbcode.cpython-312.pyc,,
+pip/_internal/__pycache__,,
+pip/_vendor/pyparsing/diagram/__init__.cpython-312.pyc,,
+pip/_internal/req/req_uninstall.cpython-312.pyc,,
+pip/_internal/operations/build/__init__.cpython-312.pyc,,
+pip/_vendor/tenacity/wait.cpython-312.pyc,,
+pip/_internal/distributions/wheel.cpython-312.pyc,,
+pip/_vendor/colorama/winterm.cpython-312.pyc,,
+pip/_vendor/resolvelib/compat/__pycache__,,
+pip/_vendor/urllib3/request.cpython-312.pyc,,
+pip/_vendor/rich/constrain.cpython-312.pyc,,
+pip/_internal/cli/__init__.cpython-312.pyc,,
+pip/_internal/commands/index.cpython-312.pyc,,
+pip/_vendor/rich/measure.cpython-312.pyc,,
+pip/_vendor/cachecontrol/filewrapper.cpython-312.pyc,,
+pip/_internal/operations/build/build_tracker.cpython-312.pyc,,
+pip/_internal/self_outdated_check.cpython-312.pyc,,
+pip/_internal/locations/__pycache__,,
+pip/_vendor/rich/console.cpython-312.pyc,,
+pip/_vendor/rich/abc.cpython-312.pyc,,
+pip/_vendor/urllib3/util/__pycache__,,
+pip/_vendor/chardet/sbcsgroupprober.cpython-312.pyc,,
+pip/_vendor/urllib3/__init__.cpython-312.pyc,,
+pip/_vendor/distlib/wheel.cpython-312.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__,,
+pip/_vendor/distlib/resources.cpython-312.pyc,,
+pip/_internal/operations/prepare.cpython-312.pyc,,
+pip/_vendor/rich/progress_bar.cpython-312.pyc,,
+pip/_internal/cli/status_codes.cpython-312.pyc,,
+pip/_vendor/pygments/filters/__init__.cpython-312.pyc,,
+pip/_vendor/packaging/tags.cpython-312.pyc,,
+pip/_vendor/truststore/_windows.cpython-312.pyc,,
+pip/_vendor/tenacity/before.cpython-312.pyc,,
+pip/_vendor/packaging/markers.cpython-312.pyc,,
+pip/_vendor/chardet/langhungarianmodel.cpython-312.pyc,,
+pip/_vendor/urllib3/util/ssltransport.cpython-312.pyc,,
+pip/_vendor/urllib3/packages/backports/__init__.cpython-312.pyc,,
+pip/_vendor/rich/prompt.cpython-312.pyc,,
+pip/_vendor/chardet/sbcharsetprober.cpython-312.pyc,,
 pip/_vendor/chardet/cli/chardetect.cpython-312.pyc,,
-pip/_internal/utils/egg_link.cpython-312.pyc,,
-pip/_internal/commands/wheel.cpython-312.pyc,,
-pip/_internal/metadata/importlib/__init__.cpython-312.pyc,,
-pip/_internal/utils/setuptools_build.cpython-312.pyc,,
-pip/_vendor/pyproject_hooks/_in_process/__init__.cpython-312.pyc,,
+pip/_internal/commands/__init__.cpython-312.pyc,,
 pip/_internal/resolution/legacy/__init__.cpython-312.pyc,,
-pip/_vendor/pygments/filters/__pycache__,,
+pip/_vendor/rich/terminal_theme.cpython-312.pyc,,
+pip/_vendor/urllib3/util/timeout.cpython-312.pyc,,
+pip/_vendor/pyparsing/core.cpython-312.pyc,,
+pip/_vendor/urllib3/response.cpython-312.pyc,,
+pip/_vendor/chardet/eucjpprober.cpython-312.pyc,,
+pip/_vendor/cachecontrol/_cmd.cpython-312.pyc,,
+pip/_vendor/distro/distro.cpython-312.pyc,,
+pip/_vendor/packaging/__about__.cpython-312.pyc,,
 pip/_vendor/rich/errors.cpython-312.pyc,,
-pip/_vendor/urllib3/util/connection.cpython-312.pyc,,
-pip/_vendor/resolvelib/structs.cpython-312.pyc,,
-pip/_vendor/pyparsing/results.cpython-312.pyc,,
-pip/_vendor/rich/constrain.cpython-312.pyc,,
-pip/_vendor/distlib/database.cpython-312.pyc,,
-pip/_vendor/cachecontrol/filewrapper.cpython-312.pyc,,
-pip/_internal/network/cache.cpython-312.pyc,,
-pip/_internal/vcs/subversion.cpython-312.pyc,,
+pip/_internal/commands/completion.cpython-312.pyc,,
+pip/_vendor/chardet/metadata/__pycache__,,
+pip/_vendor/cachecontrol/caches/__init__.cpython-312.pyc,,
+pip/_internal/utils/compat.cpython-312.pyc,,
+pip/_vendor/pyparsing/__pycache__,,
+pip/_vendor/resolvelib/__pycache__,,
+pip/_vendor/rich/json.cpython-312.pyc,,
+pip/_vendor/chardet/sjisprober.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/securetransport.cpython-312.pyc,,
+pip/_internal/models/format_control.cpython-312.pyc,,
+pip/_vendor/resolvelib/resolvers.cpython-312.pyc,,
 pip/_vendor/requests/compat.cpython-312.pyc,,
-pip/_internal/commands/uninstall.cpython-312.pyc,,
+pip/_internal/utils/unpacking.cpython-312.pyc,,
+pip/_vendor/rich/live.cpython-312.pyc,,
+pip/_vendor/chardet/euckrprober.cpython-312.pyc,,
+pip/_vendor/rich/_wrap.cpython-312.pyc,,
+pip/_internal/utils/_log.cpython-312.pyc,,
+pip/_internal/cli/req_command.cpython-312.pyc,,
+pip/_vendor/platformdirs/__pycache__,,
+pip/_vendor/pyparsing/testing.cpython-312.pyc,,
+pip/_vendor/platformdirs/android.cpython-312.pyc,,
+pip/_vendor/rich/_extension.cpython-312.pyc,,
+pip-24.0.virtualenv,,
+pip/_internal/vcs/git.cpython-312.pyc,,
+pip/_internal/network/xmlrpc.cpython-312.pyc,,
+pip/_internal/operations/build/metadata_editable.cpython-312.pyc,,
+pip/_vendor/platformdirs/api.cpython-312.pyc,,
+pip/_internal/utils/_jaraco_text.cpython-312.pyc,,
+pip/_vendor/tenacity/nap.cpython-312.pyc,,
+pip/_vendor/urllib3/packages/__pycache__,,
+pip/_internal/pyproject.cpython-312.pyc,,
+pip/_vendor/idna/__init__.cpython-312.pyc,,
+pip/_vendor/rich/layout.cpython-312.pyc,,
+pip/_vendor/idna/codec.cpython-312.pyc,,
+../../../bin/pip,,
+pip/_vendor/webencodings/mklabels.cpython-312.pyc,,
+pip/_vendor/resolvelib/reporters.cpython-312.pyc,,
+pip/_vendor/pkg_resources/__pycache__,,
 pip/_internal/metadata/_json.cpython-312.pyc,,
-pip/_internal/distributions/__pycache__,,
-pip/_vendor/chardet/chardistribution.cpython-312.pyc,,
-pip/_vendor/colorama/ansitowin32.cpython-312.pyc,,
-pip/_vendor/rich/logging.cpython-312.pyc,,
-pip/_internal/models/link.cpython-312.pyc,,
-pip/_vendor/requests/cookies.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/bbcode.cpython-312.pyc,,
-pip/_internal/models/__pycache__,,
-pip/_internal/req/req_set.cpython-312.pyc,,
-pip/_internal/cli/command_context.cpython-312.pyc,,
-pip/_internal/cli/spinners.cpython-312.pyc,,
-pip/_internal/operations/build/__init__.cpython-312.pyc,,
-pip/_vendor/urllib3/util/ssltransport.cpython-312.pyc,,
-pip/_vendor/chardet/cp949prober.cpython-312.pyc,,
+pip/_vendor/chardet/euctwprober.cpython-312.pyc,,
+pip/_internal/commands/help.cpython-312.pyc,,
+pip/_vendor/pyparsing/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/__init__.cpython-312.pyc,,
+pip/_vendor/rich/table.cpython-312.pyc,,
+pip/_vendor/urllib3/util/ssl_.cpython-312.pyc,,
+pip/_vendor/certifi/__init__.cpython-312.pyc,,
+pip/_vendor/rich/_cell_widths.cpython-312.pyc,,
+pip/_vendor/colorama/__init__.cpython-312.pyc,,
+pip/_internal/resolution/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/cli/__pycache__,,
+pip/_vendor/urllib3/packages/backports/weakref_finalize.cpython-312.pyc,,
+pip/_internal/cli/autocompletion.cpython-312.pyc,,
+pip/_vendor/tomli/__init__.cpython-312.pyc,,
+pip/_vendor/__init__.cpython-312.pyc,,
+pip/_vendor/tenacity/before_sleep.cpython-312.pyc,,
+pip/_internal/locations/__init__.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/_mapping.cpython-312.pyc,,
+pip/_vendor/chardet/latin1prober.cpython-312.pyc,,
+pip/_vendor/distlib/metadata.cpython-312.pyc,,
+pip/_vendor/rich/_ratio.cpython-312.pyc,,
+pip/_vendor/requests/models.cpython-312.pyc,,
+pip/_vendor/truststore/_openssl.cpython-312.pyc,,
 pip/_vendor/rich/repr.cpython-312.pyc,,
-pip/_internal/models/__init__.cpython-312.pyc,,
-pip/_vendor/packaging/markers.cpython-312.pyc,,
+pip/_vendor/pygments/lexer.cpython-312.pyc,,
+pip/_vendor/urllib3/util/ssl_match_hostname.cpython-312.pyc,,
+pip/_vendor/tenacity/__init__.cpython-312.pyc,,
+pip/_internal/operations/build/wheel_editable.cpython-312.pyc,,
+pip/_vendor/pygments/__pycache__,,
 pip/_vendor/rich/markup.cpython-312.pyc,,
-pip/_vendor/certifi/core.cpython-312.pyc,,
-pip/_vendor/certifi/__main__.cpython-312.pyc,,
+pip/_vendor/truststore/_macos.cpython-312.pyc,,
+pip/_internal/operations/install/editable_legacy.cpython-312.pyc,,
+pip/_internal/resolution/resolvelib/reporter.cpython-312.pyc,,
+pip/_vendor/truststore/__init__.cpython-312.pyc,,
+pip/_vendor/rich/style.cpython-312.pyc,,
+pip/_internal/req/__pycache__,,
+pip/_vendor/pyproject_hooks/_impl.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/_securetransport/__init__.cpython-312.pyc,,
+pip/_vendor/typing_extensions.cpython-312.pyc,,
+pip/_vendor/tenacity/tornadoweb.cpython-312.pyc,,
 pip/_vendor/rich/bar.cpython-312.pyc,,
-pip/_vendor/rich/status.cpython-312.pyc,,
-pip/_internal/commands/install.cpython-312.pyc,,
-pip/_vendor/packaging/tags.cpython-312.pyc,,
-pip/_vendor/pygments/cmdline.cpython-312.pyc,,
-pip/_vendor/platformdirs/__pycache__,,
-pip/_vendor/certifi/__init__.cpython-312.pyc,,
-pip/_internal/index/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/cli/__init__.cpython-312.pyc,,
+pip/_vendor/colorama/ansi.cpython-312.pyc,,
+pip/_vendor/rich/_inspect.cpython-312.pyc,,
+pip/_internal/vcs/mercurial.cpython-312.pyc,,
+pip/_vendor/certifi/__main__.cpython-312.pyc,,
+pip/_vendor/platformdirs/windows.cpython-312.pyc,,
+pip/_vendor/webencodings/tests.cpython-312.pyc,,
+pip/_internal/utils/filetypes.cpython-312.pyc,,
+pip/_vendor/urllib3/util/url.cpython-312.pyc,,
+pip/_vendor/rich/_palettes.cpython-312.pyc,,
+pip/_internal/wheel_builder.cpython-312.pyc,,
+pip/_vendor/idna/intranges.cpython-312.pyc,,
+pip/_internal/configuration.cpython-312.pyc,,
+pip/_vendor/distro/__init__.cpython-312.pyc,,
+pip/_internal/operations/check.cpython-312.pyc,,
+pip/_vendor/truststore/__pycache__,,
+pip/_vendor/distlib/compat.cpython-312.pyc,,
+pip/_vendor/rich/emoji.cpython-312.pyc,,
+pip/_vendor/pyparsing/actions.cpython-312.pyc,,
+pip/_vendor/urllib3/util/retry.cpython-312.pyc,,
+pip/_internal/resolution/resolvelib/candidates.cpython-312.pyc,,
+pip/_internal/commands/cache.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/_securetransport/__pycache__,,
+pip/_vendor/requests/cookies.cpython-312.pyc,,
+pip/_internal/vcs/bazaar.cpython-312.pyc,,
+pip/_internal/operations/__pycache__,,
+pip/_internal/models/wheel.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/appengine.cpython-312.pyc,,
+pip/_internal/utils/egg_link.cpython-312.pyc,,
+pip/_vendor/chardet/langturkishmodel.cpython-312.pyc,,
+pip/_vendor/rich/_timer.cpython-312.pyc,,
+pip/_internal/models/target_python.cpython-312.pyc,,
+pip/_vendor/pygments/styles/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/enums.cpython-312.pyc,,
+pip/_vendor/rich/_pick.cpython-312.pyc,,
+pip/_internal/models/installation_report.cpython-312.pyc,,
+pip/_vendor/urllib3/connection.cpython-312.pyc,,
+pip/_vendor/msgpack/__pycache__,,
+pip/_vendor/pygments/lexers/__init__.cpython-312.pyc,,
+pip/_vendor/__pycache__,,
+pip/_vendor/chardet/utf1632prober.cpython-312.pyc,,
+pip/_vendor/rich/_emoji_codes.cpython-312.pyc,,
+pip/_internal/resolution/resolvelib/provider.cpython-312.pyc,,
+pip/_vendor/pyparsing/unicode.cpython-312.pyc,,
+pip/_internal/cli/base_command.cpython-312.pyc,,
+pip/_internal/commands/search.cpython-312.pyc,,
+pip/_vendor/pygments/regexopt.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/ntlmpool.cpython-312.pyc,,
+pip/_vendor/rich/_spinners.cpython-312.pyc,,
+pip/_internal/utils/temp_dir.cpython-312.pyc,,
+pip/_internal/distributions/base.cpython-312.pyc,,
+pip/_vendor/chardet/hebrewprober.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/latex.cpython-312.pyc,,
+pip/_vendor/pyproject_hooks/_in_process/__init__.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/terminal.cpython-312.pyc,,
+pip/_vendor/pygments/plugin.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/pyopenssl.cpython-312.pyc,,
+pip/_internal/distributions/installed.cpython-312.pyc,,
+pip/_internal/index/__pycache__,,
+pip/_vendor/requests/adapters.cpython-312.pyc,,
+pip/_vendor/urllib3/util/proxy.cpython-312.pyc,,
+pip/_internal/utils/hashes.cpython-312.pyc,,
+pip/_vendor/rich/diagnose.cpython-312.pyc,,
+pip/_vendor/chardet/__pycache__,,
+pip/__pycache__,,
+pip/_vendor/tenacity/__pycache__,,
+pip/_internal/commands/__pycache__,,
 pip/_vendor/rich/cells.cpython-312.pyc,,
-pip/_vendor/packaging/utils.cpython-312.pyc,,
+pip/_vendor/pygments/modeline.cpython-312.pyc,,
+../../../bin/pip3,,
+pip/_vendor/rich/scope.cpython-312.pyc,,
+pip/_vendor/rich/_windows_renderer.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/other.cpython-312.pyc,,
+pip/_vendor/pyproject_hooks/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/mbcsgroupprober.cpython-312.pyc,,
+pip/_vendor/pygments/__main__.cpython-312.pyc,,
 pip/_vendor/distlib/locators.cpython-312.pyc,,
-../../../bin/pip-3.12,,
-pip/_vendor/rich/syntax.cpython-312.pyc,,
-pip/_internal/resolution/__init__.cpython-312.pyc,,
-pip/_vendor/chardet/euckrfreq.cpython-312.pyc,,
+pip/_vendor/pygments/formatters/html.cpython-312.pyc,,
+pip/_internal/models/selection_prefs.cpython-312.pyc,,
+pip/_internal/index/collector.cpython-312.pyc,,
+pip/_internal/metadata/importlib/_dists.cpython-312.pyc,,
+pip/_internal/index/sources.cpython-312.pyc,,
+pip/_vendor/rich/protocol.cpython-312.pyc,,
+pip/_internal/resolution/__pycache__,,
+pip/_vendor/requests/utils.cpython-312.pyc,,
+pip/_internal/locations/_sysconfig.cpython-312.pyc,,
 pip/_vendor/pyparsing/util.cpython-312.pyc,,
-pip/_vendor/chardet/sbcharsetprober.cpython-312.pyc,,
-pip/_vendor/tenacity/_asyncio.cpython-312.pyc,,
-pip/_vendor/urllib3/request.cpython-312.pyc,,
-pip/_internal/models/target_python.cpython-312.pyc,,
-pip/_vendor/msgpack/ext.cpython-312.pyc,,
-pip/_vendor/pyparsing/diagram/__pycache__,,
-pip/_vendor/chardet/__pycache__,,
-pip/_vendor/resolvelib/compat/collections_abc.cpython-312.pyc,,
-pip/_internal/commands/show.cpython-312.pyc,,
-pip/_vendor/webencodings/__init__.cpython-312.pyc,,
-pip/_vendor/packaging/specifiers.cpython-312.pyc,,
+pip/_vendor/rich/spinner.cpython-312.pyc,,
+pip/_internal/models/index.cpython-312.pyc,,
 pip/_vendor/packaging/_musllinux.cpython-312.pyc,,
-pip/_vendor/rich/_timer.cpython-312.pyc,,
-pip/_vendor/rich/tree.cpython-312.pyc,,
-pip/_vendor/colorama/tests/__init__.cpython-312.pyc,,
-pip/_vendor/tenacity/tornadoweb.cpython-312.pyc,,
-pip/_internal/commands/index.cpython-312.pyc,,
-pip/_internal/pyproject.cpython-312.pyc,,
-pip/_vendor/urllib3/response.cpython-312.pyc,,
-pip/_vendor/pyparsing/__init__.cpython-312.pyc,,
-pip/_internal/network/__init__.cpython-312.pyc,,
-pip/_vendor/requests/status_codes.cpython-312.pyc,,
-pip/_internal/commands/inspect.cpython-312.pyc,,
-pip/_vendor/resolvelib/compat/__init__.cpython-312.pyc,,
-pip/_internal/distributions/base.cpython-312.pyc,,
-pip/_vendor/requests/sessions.cpython-312.pyc,,
-pip/_vendor/idna/__init__.cpython-312.pyc,,
-pip/_vendor/urllib3/filepost.cpython-312.pyc,,
-pip/_vendor/chardet/metadata/__init__.cpython-312.pyc,,
-pip/_internal/index/collector.cpython-312.pyc,,
-pip/_vendor/pygments/filters/__init__.cpython-312.pyc,,
-pip/_vendor/resolvelib/__init__.cpython-312.pyc,,
-pip/_vendor/rich/_log_render.cpython-312.pyc,,
-pip/_vendor/rich/screen.cpython-312.pyc,,
-pip/_vendor/rich/align.cpython-312.pyc,,
-pip/_internal/utils/wheel.cpython-312.pyc,,
-pip/_internal/distributions/wheel.cpython-312.pyc,,
+pip/_vendor/urllib3/poolmanager.cpython-312.pyc,,
+pip/_internal/utils/subprocess.cpython-312.pyc,,
+pip/_internal/req/constructors.cpython-312.pyc,,
+pip/_vendor/rich/progress.cpython-312.pyc,,
+pip/_internal/__init__.cpython-312.pyc,,
+pip/_vendor/urllib3/_version.cpython-312.pyc,,
+pip/_internal/build_env.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/socks.cpython-312.pyc,,
+pip/_vendor/urllib3/contrib/__pycache__,,
 pip/_internal/resolution/resolvelib/__init__.cpython-312.pyc,,
-pip/_vendor/chardet/euctwprober.cpython-312.pyc,,
-pip/_vendor/rich/_inspect.cpython-312.pyc,,
-pip/_internal/configuration.cpython-312.pyc,,
-pip/_vendor/pygments/scanner.cpython-312.pyc,,
-pip/_vendor/urllib3/exceptions.cpython-312.pyc,,
-pip/_internal/req/__init__.cpython-312.pyc,,
-pip/_vendor/rich/_wrap.cpython-312.pyc,,
-../../../bin/pip3.12,,
-pip/_internal/network/download.cpython-312.pyc,,
-pip/_vendor/rich/box.cpython-312.pyc,,
-pip/_vendor/urllib3/fields.cpython-312.pyc,,
-pip/_vendor/tomli/__init__.cpython-312.pyc,,
-pip/_vendor/chardet/escprober.cpython-312.pyc,,
-pip/_vendor/certifi/__pycache__,,
-pip/_vendor/rich/layout.cpython-312.pyc,,
-pip/_internal/utils/__pycache__,,
+pip/_vendor/msgpack/exceptions.cpython-312.pyc,,
+pip/_vendor/certifi/core.cpython-312.pyc,,
+pip/_vendor/rich/tree.cpython-312.pyc,,
+pip/_vendor/pygments/sphinxext.cpython-312.pyc,,
+pip/_vendor/chardet/gb2312prober.cpython-312.pyc,,
+pip/_vendor/packaging/__init__.cpython-312.pyc,,
+pip/_vendor/rich/__pycache__,,
+pip/_internal/cli/progress_bars.cpython-312.pyc,,
+pip/_vendor/idna/compat.cpython-312.pyc,,
+pip/_vendor/urllib3/util/queue.cpython-312.pyc,,
+pip/_vendor/platformdirs/macos.cpython-312.pyc,,
+pip/_vendor/rich/control.cpython-312.pyc,,
+pip/_internal/distributions/__pycache__,,
+pip/_internal/operations/install/__init__.cpython-312.pyc,,
+pip/_internal/index/package_finder.cpython-312.pyc,,
+pip/_vendor/urllib3/__pycache__,,
+pip/_vendor/msgpack/fallback.cpython-312.pyc,,
 pip/_vendor/idna/core.cpython-312.pyc,,
-pip/_vendor/idna/codec.cpython-312.pyc,,
-pip/_vendor/pygments/formatters/__init__.cpython-312.pyc,,
-pip/_vendor/pygments/unistring.cpython-312.pyc,,
+pip/_vendor/chardet/jpcntx.cpython-312.pyc,,
+pip/_vendor/rich/_windows.cpython-312.pyc,,
+pip/_vendor/pygments/__init__.cpython-312.pyc,,
+pip/__pip-runner__.cpython-312.pyc,,
+pip/_vendor/colorama/tests/initialise_test.cpython-312.pyc,,
+pip/_internal/commands/uninstall.cpython-312.pyc,,
+pip/_internal/network/auth.cpython-312.pyc,,
+pip/_vendor/chardet/codingstatemachine.cpython-312.pyc,,
+pip/_vendor/idna/__pycache__,,
+pip/_vendor/tomli/__pycache__,,
+pip/_vendor/chardet/gb2312freq.cpython-312.pyc,,
+pip/_internal/commands/freeze.cpython-312.pyc,,
+pip/_vendor/webencodings/__init__.cpython-312.pyc,,
+pip/_vendor/chardet/jisfreq.cpython-312.pyc,,
+pip/_vendor/rich/screen.cpython-312.pyc,,
+pip/_internal/cli/parser.cpython-312.pyc,,
+pip/_internal/operations/__init__.cpython-312.pyc,,
+pip-24.0.dist-info/__pycache__,,
+pip/_internal/utils/misc.cpython-312.pyc,,
+pip/_vendor/requests/hooks.cpython-312.pyc,,
+pip/_vendor/rich/status.cpython-312.pyc,,
+pip/_vendor/rich/_export_format.cpython-312.pyc,,
+pip/_vendor/chardet/langhebrewmodel.cpython-312.pyc,,
+pip/_vendor/rich/_loop.cpython-312.pyc,,
+pip/_vendor/rich/__main__.cpython-312.pyc,,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks/_in_process/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks/_in_process/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,12 +7,15 @@
 import importlib.resources as resources
 
 try:
     resources.files
 except AttributeError:
     # Python 3.8 compatibility
     def _in_proc_script_path():
-        return resources.path(__package__, '_in_process.py')
+        return resources.path(__package__, "_in_process.py")
+
 else:
+
     def _in_proc_script_path():
         return resources.as_file(
-            resources.files(__package__).joinpath('_in_process.py'))
+            resources.files(__package__).joinpath("_in_process.py")
+        )
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks/_in_process/_in_process.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks/_in_process/_in_process.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This is invoked in a subprocess to call the build backend hooks.
 
 It expects:
 - Command line args: hook_name, control_dir
 - Environment variables:
-      PEP517_BUILD_BACKEND=entry.point:spec
-      PEP517_BACKEND_PATH=paths (separated with os.pathsep)
+      _PYPROJECT_HOOKS_BUILD_BACKEND=entry.point:spec
+      _PYPROJECT_HOOKS_BACKEND_PATH=paths (separated with os.pathsep)
 - control_dir/input.json:
   - {"kwargs": {...}}
 
 Results:
 - control_dir/output.json
   - {"return_val": ...}
 """
@@ -17,84 +17,100 @@
 import os.path
 import re
 import shutil
 import sys
 import traceback
 from glob import glob
 from importlib import import_module
+from importlib.machinery import PathFinder
 from os.path import join as pjoin
 
 # This file is run as a script, and `import wrappers` is not zip-safe, so we
 # include write_json() and read_json() from wrappers.py.
 
 
 def write_json(obj, path, **kwargs):
-    with open(path, 'w', encoding='utf-8') as f:
+    with open(path, "w", encoding="utf-8") as f:
         json.dump(obj, f, **kwargs)
 
 
 def read_json(path):
-    with open(path, encoding='utf-8') as f:
+    with open(path, encoding="utf-8") as f:
         return json.load(f)
 
 
 class BackendUnavailable(Exception):
     """Raised if we cannot import the backend"""
-    def __init__(self, traceback):
-        self.traceback = traceback
-
 
-class BackendInvalid(Exception):
-    """Raised if the backend is invalid"""
-    def __init__(self, message):
+    def __init__(self, message, traceback=None):
+        super().__init__(message)
         self.message = message
+        self.traceback = traceback
 
 
 class HookMissing(Exception):
     """Raised if a hook is missing and we are not executing the fallback"""
+
     def __init__(self, hook_name=None):
         super().__init__(hook_name)
         self.hook_name = hook_name
 
 
-def contained_in(filename, directory):
-    """Test if a file is located within the given directory."""
-    filename = os.path.normcase(os.path.abspath(filename))
-    directory = os.path.normcase(os.path.abspath(directory))
-    return os.path.commonprefix([filename, directory]) == directory
-
-
 def _build_backend():
     """Find and load the build backend"""
-    # Add in-tree backend directories to the front of sys.path.
-    backend_path = os.environ.get('PEP517_BACKEND_PATH')
+    backend_path = os.environ.get("_PYPROJECT_HOOKS_BACKEND_PATH")
+    ep = os.environ["_PYPROJECT_HOOKS_BUILD_BACKEND"]
+    mod_path, _, obj_path = ep.partition(":")
+
     if backend_path:
+        # Ensure in-tree backend directories have the highest priority when importing.
         extra_pathitems = backend_path.split(os.pathsep)
-        sys.path[:0] = extra_pathitems
+        sys.meta_path.insert(0, _BackendPathFinder(extra_pathitems, mod_path))
 
-    ep = os.environ['PEP517_BUILD_BACKEND']
-    mod_path, _, obj_path = ep.partition(':')
     try:
         obj = import_module(mod_path)
     except ImportError:
-        raise BackendUnavailable(traceback.format_exc())
-
-    if backend_path:
-        if not any(
-            contained_in(obj.__file__, path)
-            for path in extra_pathitems
-        ):
-            raise BackendInvalid("Backend was not loaded from backend-path")
+        msg = f"Cannot import {mod_path!r}"
+        raise BackendUnavailable(msg, traceback.format_exc())
 
     if obj_path:
-        for path_part in obj_path.split('.'):
+        for path_part in obj_path.split("."):
             obj = getattr(obj, path_part)
     return obj
 
 
+class _BackendPathFinder:
+    """Implements the MetaPathFinder interface to locate modules in ``backend-path``.
+
+    Since the environment provided by the frontend can contain all sorts of
+    MetaPathFinders, the only way to ensure the backend is loaded from the
+    right place is to prepend our own.
+    """
+
+    def __init__(self, backend_path, backend_module):
+        self.backend_path = backend_path
+        self.backend_module = backend_module
+        self.backend_parent, _, _ = backend_module.partition(".")
+
+    def find_spec(self, fullname, _path, _target=None):
+        if "." in fullname:
+            # Rely on importlib to find nested modules based on parent's path
+            return None
+
+        # Ignore other items in _path or sys.path and use backend_path instead:
+        spec = PathFinder.find_spec(fullname, path=self.backend_path)
+        if spec is None and fullname == self.backend_parent:
+            # According to the spec, the backend MUST be loaded from backend-path.
+            # Therefore, we can halt the import machinery and raise a clean error.
+            msg = f"Cannot find module {self.backend_module!r} in {self.backend_path!r}"
+            raise BackendUnavailable(msg)
+
+        return spec
+
+
 def _supported_features():
     """Return the list of options features supported by the backend.
 
     Returns a list of strings.
     The only possible value is 'build_editable'.
     """
     backend = _build_backend()
@@ -129,15 +145,16 @@
     except AttributeError:
         return []
     else:
         return hook(config_settings)
 
 
 def prepare_metadata_for_build_wheel(
-        metadata_directory, config_settings, _allow_fallback):
+    metadata_directory, config_settings, _allow_fallback
+):
     """Invoke optional prepare_metadata_for_build_wheel
 
     Implements a fallback by building a wheel if the hook isn't defined,
     unless _allow_fallback is False in which case HookMissing is raised.
     """
     backend = _build_backend()
     try:
@@ -146,20 +163,22 @@
         if not _allow_fallback:
             raise HookMissing()
     else:
         return hook(metadata_directory, config_settings)
     # fallback to build_wheel outside the try block to avoid exception chaining
     # which can be confusing to users and is not relevant
     whl_basename = backend.build_wheel(metadata_directory, config_settings)
-    return _get_wheel_metadata_from_wheel(whl_basename, metadata_directory,
-                                          config_settings)
+    return _get_wheel_metadata_from_wheel(
+        whl_basename, metadata_directory, config_settings
+    )
 
 
 def prepare_metadata_for_build_editable(
-        metadata_directory, config_settings, _allow_fallback):
+    metadata_directory, config_settings, _allow_fallback
+):
     """Invoke optional prepare_metadata_for_build_editable
 
     Implements a fallback by building an editable wheel if the hook isn't
     defined, unless _allow_fallback is False in which case HookMissing is
     raised.
     """
     backend = _build_backend()
@@ -167,73 +186,74 @@
         hook = backend.prepare_metadata_for_build_editable
     except AttributeError:
         if not _allow_fallback:
             raise HookMissing()
         try:
             build_hook = backend.build_editable
         except AttributeError:
-            raise HookMissing(hook_name='build_editable')
+            raise HookMissing(hook_name="build_editable")
         else:
             whl_basename = build_hook(metadata_directory, config_settings)
-            return _get_wheel_metadata_from_wheel(whl_basename,
-                                                  metadata_directory,
-                                                  config_settings)
+            return _get_wheel_metadata_from_wheel(
+                whl_basename, metadata_directory, config_settings
+            )
     else:
         return hook(metadata_directory, config_settings)
 
 
-WHEEL_BUILT_MARKER = 'PEP517_ALREADY_BUILT_WHEEL'
+WHEEL_BUILT_MARKER = "PYPROJECT_HOOKS_ALREADY_BUILT_WHEEL"
 
 
 def _dist_info_files(whl_zip):
     """Identify the .dist-info folder inside a wheel ZipFile."""
     res = []
     for path in whl_zip.namelist():
-        m = re.match(r'[^/\\]+-[^/\\]+\.dist-info/', path)
+        m = re.match(r"[^/\\]+-[^/\\]+\.dist-info/", path)
         if m:
             res.append(path)
     if res:
         return res
     raise Exception("No .dist-info folder found in wheel")
 
 
-def _get_wheel_metadata_from_wheel(
-        whl_basename, metadata_directory, config_settings):
+def _get_wheel_metadata_from_wheel(whl_basename, metadata_directory, config_settings):
     """Extract the metadata from a wheel.
 
     Fallback for when the build backend does not
     define the 'get_wheel_metadata' hook.
     """
     from zipfile import ZipFile
-    with open(os.path.join(metadata_directory, WHEEL_BUILT_MARKER), 'wb'):
+
+    with open(os.path.join(metadata_directory, WHEEL_BUILT_MARKER), "wb"):
         pass  # Touch marker file
 
     whl_file = os.path.join(metadata_directory, whl_basename)
     with ZipFile(whl_file) as zipf:
         dist_info = _dist_info_files(zipf)
         zipf.extractall(path=metadata_directory, members=dist_info)
-    return dist_info[0].split('/')[0]
+    return dist_info[0].split("/")[0]
 
 
 def _find_already_built_wheel(metadata_directory):
-    """Check for a wheel already built during the get_wheel_metadata hook.
-    """
+    """Check for a wheel already built during the get_wheel_metadata hook."""
     if not metadata_directory:
         return None
     metadata_parent = os.path.dirname(metadata_directory)
     if not os.path.isfile(pjoin(metadata_parent, WHEEL_BUILT_MARKER)):
         return None
 
-    whl_files = glob(os.path.join(metadata_parent, '*.whl'))
+    whl_files = glob(os.path.join(metadata_parent, "*.whl"))
     if not whl_files:
-        print('Found wheel built marker, but no .whl files')
+        print("Found wheel built marker, but no .whl files")
         return None
     if len(whl_files) > 1:
-        print('Found multiple .whl files; unspecified behaviour. '
-              'Will call build_wheel.')
+        print(
+            "Found multiple .whl files; unspecified behaviour. "
+            "Will call build_wheel."
+        )
         return None
 
     # Exactly one .whl file
     return whl_files[0]
 
 
 def build_wheel(wheel_directory, config_settings, metadata_directory=None):
@@ -244,16 +264,17 @@
     will copy it rather than rebuilding the wheel.
     """
     prebuilt_whl = _find_already_built_wheel(metadata_directory)
     if prebuilt_whl:
         shutil.copy2(prebuilt_whl, wheel_directory)
         return os.path.basename(prebuilt_whl)
 
-    return _build_backend().build_wheel(wheel_directory, config_settings,
-                                        metadata_directory)
+    return _build_backend().build_wheel(
+        wheel_directory, config_settings, metadata_directory
+    )
 
 
 def build_editable(wheel_directory, config_settings, metadata_directory=None):
     """Invoke the optional build_editable hook.
 
     If a wheel was already built in the
     prepare_metadata_for_build_editable fallback, this
@@ -289,65 +310,64 @@
 
 class _DummyException(Exception):
     """Nothing should ever raise this exception"""
 
 
 class GotUnsupportedOperation(Exception):
     """For internal use when backend raises UnsupportedOperation"""
+
     def __init__(self, traceback):
         self.traceback = traceback
 
 
 def build_sdist(sdist_directory, config_settings):
     """Invoke the mandatory build_sdist hook."""
     backend = _build_backend()
     try:
         return backend.build_sdist(sdist_directory, config_settings)
-    except getattr(backend, 'UnsupportedOperation', _DummyException):
+    except getattr(backend, "UnsupportedOperation", _DummyException):
         raise GotUnsupportedOperation(traceback.format_exc())
 
 
 HOOK_NAMES = {
-    'get_requires_for_build_wheel',
-    'prepare_metadata_for_build_wheel',
-    'build_wheel',
-    'get_requires_for_build_editable',
-    'prepare_metadata_for_build_editable',
-    'build_editable',
-    'get_requires_for_build_sdist',
-    'build_sdist',
-    '_supported_features',
+    "get_requires_for_build_wheel",
+    "prepare_metadata_for_build_wheel",
+    "build_wheel",
+    "get_requires_for_build_editable",
+    "prepare_metadata_for_build_editable",
+    "build_editable",
+    "get_requires_for_build_sdist",
+    "build_sdist",
+    "_supported_features",
 }
 
 
 def main():
     if len(sys.argv) < 3:
         sys.exit("Needs args: hook_name, control_dir")
     hook_name = sys.argv[1]
     control_dir = sys.argv[2]
     if hook_name not in HOOK_NAMES:
         sys.exit("Unknown hook: %s" % hook_name)
     hook = globals()[hook_name]
 
-    hook_input = read_json(pjoin(control_dir, 'input.json'))
+    hook_input = read_json(pjoin(control_dir, "input.json"))
 
-    json_out = {'unsupported': False, 'return_val': None}
+    json_out = {"unsupported": False, "return_val": None}
     try:
-        json_out['return_val'] = hook(**hook_input['kwargs'])
+        json_out["return_val"] = hook(**hook_input["kwargs"])
     except BackendUnavailable as e:
-        json_out['no_backend'] = True
-        json_out['traceback'] = e.traceback
-    except BackendInvalid as e:
-        json_out['backend_invalid'] = True
-        json_out['backend_error'] = e.message
+        json_out["no_backend"] = True
+        json_out["traceback"] = e.traceback
+        json_out["backend_error"] = e.message
     except GotUnsupportedOperation as e:
-        json_out['unsupported'] = True
-        json_out['traceback'] = e.traceback
+        json_out["unsupported"] = True
+        json_out["traceback"] = e.traceback
     except HookMissing as e:
-        json_out['hook_missing'] = True
-        json_out['missing_hook_name'] = e.hook_name or hook_name
+        json_out["hook_missing"] = True
+        json_out["missing_hook_name"] = e.hook_name or hook_name
 
-    write_json(json_out, pjoin(control_dir, 'output.json'), indent=2)
+    write_json(json_out, pjoin(control_dir, "output.json"), indent=2)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-The MIT License (MIT)
-
-Copyright (c) 2017 Thomas Kluyver
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in
 all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks-1.1.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyproject_hooks
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wrappers to call pyproject.toml-based build backend hooks.
 Author-email: Thomas Kluyver <thomas@kluyver.me.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: tomli >=1.1.0 ; python_version<'3.11'
 Project-URL: Changelog, https://pyproject-hooks.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://pyproject-hooks.readthedocs.io/
 Project-URL: Source, https://github.com/pypa/pyproject-hooks
 
 ``pyproject-hooks``
 ===================
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/pyproject_hooks-1.1.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-pyproject_hooks-1.0.0.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
-pyproject_hooks-1.0.0.dist-info/LICENSE,sha256=GyKwSbUmfW38I6Z79KhNjsBLn9-xpR02DkK0NCyLQVQ,1081
-pyproject_hooks-1.0.0.dist-info/METADATA,sha256=W-kbDJ885CyP_Lx_lSzn_1t6zejS3U4d5C2uUPvPbOk,1341
-pyproject_hooks-1.0.0.dist-info/RECORD,,
-pyproject_hooks-1.0.0.dist-info/WHEEL,sha256=rSgq_JpHF9fHR1lx53qwg_1-2LypZE_qmcuXbVUq948,81
-pyproject_hooks/__init__.py,sha256=kCehmy0UaBa9oVMD7ZIZrnswfnP3LXZ5lvnNJAL5JBM,491
+pyproject_hooks-1.1.0.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
+pyproject_hooks-1.1.0.dist-info/METADATA,sha256=GFtikAHRG7IjGgWt23nz6orimbdlMY_K5M5Tq1FSu9o,1288
+pyproject_hooks-1.1.0.dist-info/RECORD,,
+pyproject_hooks-1.1.0.dist-info/WHEEL,sha256=EZbGkh7Ie4PoZfRQ8I0ZuP9VklN_TvcZ6DSE5Uar4z4,81
+pyproject_hooks/__init__.py,sha256=lTZh3ElUBYq9sDir1jjP8exNT7GxD0KHyTsbP7-C4uo,691
 pyproject_hooks/__pycache__/__init__.cpython-312.pyc,,
-pyproject_hooks/__pycache__/_compat.cpython-312.pyc,,
 pyproject_hooks/__pycache__/_impl.cpython-312.pyc,,
-pyproject_hooks/_compat.py,sha256=qn8v6Suythkg002Jg4OxCTpRdT_5Xdazf_JDwEzMLj8,121
-pyproject_hooks/_impl.py,sha256=61GJxzQip0IInhuO69ZI5GbNQ82XEDUB_1Gg5_KtUoc,11920
-pyproject_hooks/_in_process/__init__.py,sha256=9gQATptbFkelkIy0OfWFEACzqxXJMQDWCH9rBOAZVwQ,546
+pyproject_hooks/_impl.py,sha256=jY-raxnmyRyB57ruAitrJRUzEexuAhGTpgMygqx67Z4,14936
+pyproject_hooks/_in_process/__init__.py,sha256=MJNPpfIxcO-FghxpBbxkG1rFiQf6HOUbV4U5mq0HFns,557
 pyproject_hooks/_in_process/__pycache__/__init__.cpython-312.pyc,,
 pyproject_hooks/_in_process/__pycache__/_in_process.cpython-312.pyc,,
-pyproject_hooks/_in_process/_in_process.py,sha256=m2b34c917IW5o-Q_6TYIHlsK9lSUlNiyrITTUH_zwew,10927
+pyproject_hooks/_in_process/_in_process.py,sha256=n_KTwipnsls5dWtJr1Jm2h18u5U5D_OVubKqtEu2UNQ,11603
+pyproject_hooks/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/_internal_utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/adapters.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/api.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/auth.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/compat.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/cookies.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/exceptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/help.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/hooks.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/models.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/packages.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/sessions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/status_codes.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/structures.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests/utils.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/LICENSE` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/RECORD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/requests-2.31.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/_base_connection.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/_collections.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/_request_methods.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/connection.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/connectionpool.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/exceptions.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/fields.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/filepost.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/http2.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/http2.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/poolmanager.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/response.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/pyopenssl.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/socks.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/connection.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/connection.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/fetch.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/fetch.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/request.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/request.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/response.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/contrib/emscripten/response.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/__init__.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/connection.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/proxy.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/request.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/response.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/retry.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/ssl_.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/ssl_match_hostname.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/ssltransport.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/timeout.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/url.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/util.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3/util/wait.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/METADATA` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/RECORD` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 urllib3-2.2.1.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
 urllib3-2.2.1.dist-info/METADATA,sha256=uROmjQwfAbwRYjV9PMdc5JF5NA3kRkpoKafPkNzybfc,6434
 urllib3-2.2.1.dist-info/RECORD,,
+urllib3-2.2.1.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 urllib3-2.2.1.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
 urllib3-2.2.1.dist-info/licenses/LICENSE.txt,sha256=Ew46ZNX91dCWp1JpRjSn2d8oRGnehuVzIQAmgEHj1oY,1093
 urllib3/__init__.py,sha256=JMo1tg1nIV1AeJ2vENC_Txfl0e5h6Gzl9DGVk1rWRbo,6979
 urllib3/__pycache__/__init__.cpython-312.pyc,,
 urllib3/__pycache__/_base_connection.cpython-312.pyc,,
 urllib3/__pycache__/_collections.cpython-312.pyc,,
 urllib3/__pycache__/_request_methods.cpython-312.pyc,,
```

### Comparing `franklinwh-0.0.2/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/franklinwh/client.py` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import hashlib
 from dataclasses import dataclass
+import typing
 
 DEFAULT_URL_BASE = "https://energy.franklinwh.com/";
 
 @dataclass
 class Current:
     solar_production: float
     generator_production: float
@@ -51,14 +52,25 @@
     def _get_smart_switch_state(self):
         url = self.url_base + "hes-gateway/manage/getCommunicationOptimization"
         params = { "gatewayId": self.gateway, "lang": "en_US" }
         headers = { "loginToken": self.token }
         res = requests.get(url, params=params, headers=headers)
         return res.json()
 
+    def _set_smart_switch_state(self):
+        """This method uses the same payload format as _get_smart_switch_state returns.
+
+        Who absolutely knows what happens if you tangle stuff up in here, so in
+        the spirit of hoping for the best the only way I'm willing to attempt
+        this is by manipulating that blob and sending it back, hopefully
+        quickly enough that nothing else can race it
+
+
+        """
+
     def get_smart_switch_state(self):
         # TODO(richo) This API is super in flux, both because of how vague the
         # underlying API is and also trying to figure out what to do with
         # inconsistency.
         data = self._get_smart_switch_state()
         def state(swmode, swproload):
             if swmode == 1 and swproload == 1:
@@ -71,25 +83,38 @@
         result = data["result"]
         sw1 = state(result["Sw1Mode"], result["Sw1ProLoad"])
         sw2 = state(result["Sw2Mode"], result["Sw2ProLoad"])
         sw3 = state(result["Sw3Mode"], result["Sw3ProLoad"])
 
         return [sw1, sw2, sw3]
 
+    def set_smart_switch_state(self, state: (typing.Optional[bool], typing.Optional[bool], typing.Optional[bool])):
+        """Set the state of the smart circuits
+
+        Setting a value in the state tuple to True will turn on that circuit,
+        setting to False will turn it off. Setting to None will make it
+        unchanged.
+        """
+
+
+        initial = self.get_smart_switch_state()
+        payload = initial["result"]
+
+        def set_value(keys, value):
+            for k in keys:
+                payload[k] = value
 
 
-    def set_smart_switch_state(self):
+        for i, ks in enumerate(("Sw1Mode", "Sw1ProLoad"), ("Sw2Mode", "Sw2ProLoad"), ("Sw3Mode", "Sw3ProLoad")):
+            if state[i] == True:
+                set_value(ks, 1)
+            elif state[i] == False:
+                set_value(ks, 0)
 
-        pass
-        # TODO(richo)
-        # Set all of these to 1.
-        # Sw1Mode
-        # Sw2Mode
-        # Sw1ProLoad
-        # Sw2ProLoad
+        self._set_smart_switch_state(payload)
 
     def get_stats(self) -> dict:
         """Get current statistics for the FHP.
 
         This includes instantaneous measurements for current power, as well as totals for today (in local time)
         """
         url = self.url_base + "hes-gateway/terminal/selectIotUserRuntimeDataLog"
```

### Comparing `franklinwh-0.0.2/LICENSE` & `franklinwh-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `franklinwh-0.0.2/PKG-INFO` & `franklinwh-0.0.3/env/lib/python3.12/site-packages/franklinwh-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: franklinwh
 Version: 0.0.2
 Summary: Python wrapper for FranklinWH
 Project-URL: Homepage, https://github.com/richo/franklinwh-python
 Project-URL: Issues, https://github.com/richo/franklinwh-python/issues
 Author-email: Richo Butts <richo@psych0tik.net>
 License-File: LICENSE
```

