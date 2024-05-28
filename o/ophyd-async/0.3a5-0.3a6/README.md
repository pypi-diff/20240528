# Comparing `tmp/ophyd_async-0.3a5.tar.gz` & `tmp/ophyd_async-0.3a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_async-0.3a5.tar", last modified: Mon May 20 11:36:47 2024, max compression
+gzip compressed data, was "ophyd_async-0.3a6.tar", last modified: Tue May 28 15:21:27 2024, max compression
```

## Comparing `ophyd_async-0.3a5.tar` & `ophyd_async-0.3a6.tar`

### file list

```diff
@@ -1,249 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.821964 ophyd_async-0.3a5/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.781963 ophyd_async-0.3a5/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.781963 ophyd_async-0.3a5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.773963 ophyd_async-0.3a5/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.781963 ophyd_async-0.3a5/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.781963 ophyd_async-0.3a5/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-20 11:36:47.821964 ophyd_async-0.3a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/_templates/README
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/examples/epics_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/examples/foo_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0003-ophyd-async-migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0004-repository-structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0005-respect-black-line-length.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0006-procedural-device-definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/design-goals.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/event-loop-choice.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/flyscanning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/choose-interfaces-for-devices.md
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/compound-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/make-a-simple-device.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/make-a-standard-detector.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/write-tests-for-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/bluesky_ophyd_epics_devices_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/bluesky_ophyd_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   253748 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/hardware-triggered-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/ophyd_favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    89951 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/outer-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)   128990 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/simple-hardware-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/tutorials/using-existing-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:36:47.821964 ophyd_async-0.3a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.777963 ophyd_async-0.3a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/src/ophyd_async/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.793963 ophyd_async-0.3a5/src/ophyd_async/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/mock_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/mock_signal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/soft_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.793963 ophyd_async-0.3a5/src/ophyd_async/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.793963 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/_aioca.py
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/_p4p.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.797963 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/aravis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.797963 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.797963 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/ad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/kinetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/vimba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.797963 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/_hdffile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/demo/mover.db
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/demo/sensor.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/motion/motor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/epics/pvi/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/pvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/pvi/pvi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/epics/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/signal/_epics_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/signal/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/panda/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_common_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/panda/writers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/writers/_hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/writers/_panda_hdf_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/planstubs/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/planstubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/planstubs/ensure_connected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/planstubs/prepare_trigger_and_dets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.805963 ophyd_async-0.3a5/src/ophyd_async/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.805963 ophyd_async-0.3a5/src/ophyd_async/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/demo/sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_detector_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_detector_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/src/ophyd_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.805963 ophyd_async-0.3a5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.805963 ophyd_async-0.3a5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_device_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_mock_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_soft_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_watchable_async_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/_backend/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_aravis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_kinetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_vimba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/demo/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/demo/test_demo_ad_sim_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/motion/test_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/test_pvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/test_records.db
--rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/test_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/panda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/panda/db/
--rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/db/panda.db
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_panda_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_panda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/protocols/test_protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/sim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/demo/test_sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/test_pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/test_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/test_sim_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/test_streaming_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/test_flyer_with_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.627468 ophyd_async-0.3a6/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.595468 ophyd_async-0.3a6/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.595468 ophyd_async-0.3a6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.591468 ophyd_async-0.3a6/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.595468 ophyd_async-0.3a6/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.595468 ophyd_async-0.3a6/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-28 15:21:27.627468 ophyd_async-0.3a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/_templates/README
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/examples/epics_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/examples/foo_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.599468 ophyd_async-0.3a6/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0003-ophyd-async-migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0004-repository-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0005-respect-black-line-length.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/0006-procedural-device-definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/design-goals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/event-loop-choice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations/flyscanning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/choose-interfaces-for-devices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/compound-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/make-a-simple-device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/make-a-standard-detector.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to/write-tests-for-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/images/bluesky_ophyd_epics_devices_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/images/bluesky_ophyd_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/images/ophyd_favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/tutorials/using-existing-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:21:27.627468 ophyd_async-0.3a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.591468 ophyd_async-0.3a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.603468 ophyd_async-0.3a6/src/ophyd_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.607468 ophyd_async-0.3a6/src/ophyd_async/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/mock_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/mock_signal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16456 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/soft_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.607468 ophyd_async-0.3a6/src/ophyd_async/epics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.607468 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/_aioca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/_p4p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/_backend/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.607468 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/aravis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/ad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/vimba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/_hdffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/demo/mover.db
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/demo/sensor.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/motion/motor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/pvi/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/pvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/pvi/pvi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.611468 ophyd_async-0.3a6/src/ophyd_async/epics/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/signal/_epics_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/epics/signal/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_common_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/panda/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/writers/_hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/panda/writers/_panda_hdf_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/plan_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/plan_stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/plan_stubs/ensure_connected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/plan_stubs/fly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/src/ophyd_async/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/demo/sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_detector_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_detector_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/src/ophyd_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 15:21:27.000000 ophyd_async-0.3a6/src/ophyd_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.615468 ophyd_async-0.3a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_device_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_mock_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_soft_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/core/test_watchable_async_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/_backend/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_aravis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_vimba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/areadetector/test_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/demo/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/demo/test_demo_ad_sim_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.619468 ophyd_async-0.3a6/tests/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/motion/test_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/test_pvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/test_records.db
+-rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/epics/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/panda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/panda/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/db/panda.db
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_panda_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_panda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/panda/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/plan_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/plan_stubs/test_fly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/protocols/test_protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:27.623468 ophyd_async-0.3a6/tests/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/demo/test_sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/test_pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/test_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/test_sim_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/sim/test_streaming_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-28 15:21:22.000000 ophyd_async-0.3a6/tests/test_log.py
```

### Comparing `ophyd_async-0.3a5/.devcontainer/devcontainer.json` & `ophyd_async-0.3a6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/CONTRIBUTING.md` & `ophyd_async-0.3a6/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/actions/install_requirements/action.yml` & `ophyd_async-0.3a6/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/dependabot.yml` & `ophyd_async-0.3a6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/pages/make_switcher.py` & `ophyd_async-0.3a6/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/workflows/_check.yml` & `ophyd_async-0.3a6/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/workflows/_dist.yml` & `ophyd_async-0.3a6/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/workflows/_docs.yml` & `ophyd_async-0.3a6/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/workflows/_release.yml` & `ophyd_async-0.3a6/.github/workflows/_release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,14 @@
             zip -r docs.zip $GITHUB_REF_NAME
             rm -rf $GITHUB_REF_NAME
           fi
 
       - name: Create GitHub Release
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564 # v2.0.4
+        uses: softprops/action-gh-release@69320dbe05506a9a39fc8ae11030b214ec2d1f87 # v2.0.5
         with:
           prerelease: ${{ contains(github.ref_name, 'a') || contains(github.ref_name, 'b') || contains(github.ref_name, 'rc') }}
           files: "*"
           generate_release_notes: true
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `ophyd_async-0.3a5/.github/workflows/_test.yml` & `ophyd_async-0.3a6/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.github/workflows/ci.yml` & `ophyd_async-0.3a6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.gitignore` & `ophyd_async-0.3a6/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.mailmap` & `ophyd_async-0.3a6/.mailmap`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/.pre-commit-config.yaml` & `ophyd_async-0.3a6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/Dockerfile` & `ophyd_async-0.3a6/Dockerfile`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/LICENSE` & `ophyd_async-0.3a6/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/PKG-INFO` & `ophyd_async-0.3a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a5
+Version: 0.3a6
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ophyd_async-0.3a5/README.md` & `ophyd_async-0.3a6/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/_templates/custom-class-template.rst` & `ophyd_async-0.3a6/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/_templates/custom-module-template.rst` & `ophyd_async-0.3a6/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/conf.py` & `ophyd_async-0.3a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/examples/epics_demo.py` & `ophyd_async-0.3a6/docs/examples/epics_demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/examples/foo_detector.py` & `ophyd_async-0.3a6/docs/examples/foo_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `ophyd_async-0.3a6/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/explanations/decisions/0003-ophyd-async-migration.rst` & `ophyd_async-0.3a6/docs/explanations/decisions/0003-ophyd-async-migration.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/explanations/decisions/0004-repository-structure.rst` & `ophyd_async-0.3a6/docs/explanations/decisions/0004-repository-structure.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/explanations/decisions/0005-respect-black-line-length.rst` & `ophyd_async-0.3a6/docs/explanations/decisions/0005-respect-black-line-length.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/explanations/decisions/0006-procedural-device-definitions.rst` & `ophyd_async-0.3a6/docs/explanations/decisions/0006-procedural-device-definitions.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/explanations/design-goals.rst` & `ophyd_async-0.3a6/docs/explanations/design-goals.rst`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 Parity with Malcolm
 -------------------
 
 .. seealso:: `./flyscanning`
 
 Ophyd-async should provide the same building blocks for defining flyscans scans as malcolm_. It should support PandA and Zebra as timing masters by default, but also provide easy helpers for developers to write support for their own devices.
 
-It should enable `motor trajectory scanning <motortraj_>` and `multiple triggering rates<detectorsync_>` based around a base rate, and pausing/resuming scans. Scans should be modelled using scanspec_, which serves as a universal language for defining trajectory and time-resolved scans, and converted to the underlying format of the given motion controller. It should also be possible to define an `outer scan <outerscan_>`.
+It should enable motor trajectory scanning and multiple triggering rates based around a base rate, and pausing/resuming scans. Scans should be modelled using scanspec_, which serves as a universal language for defining trajectory and time-resolved scans, and converted to the underlying format of the given motion controller. It should also be possible to define an outer scan .
 
 
 Improved Trajectory Calculation
 -------------------------------
 
 Ophyd-async will provide and improve upon the algorithms that malcolm_ uses to calculate trajectories for supported hardware.
```

### Comparing `ophyd_async-0.3a5/docs/explanations/event-loop-choice.rst` & `ophyd_async-0.3a6/docs/explanations/event-loop-choice.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/how-to/choose-interfaces-for-devices.md` & `ophyd_async-0.3a6/docs/how-to/choose-interfaces-for-devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/how-to/compound-devices.rst` & `ophyd_async-0.3a6/docs/how-to/compound-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/how-to/make-a-simple-device.rst` & `ophyd_async-0.3a6/docs/how-to/make-a-simple-device.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/how-to/make-a-standard-detector.rst` & `ophyd_async-0.3a6/docs/how-to/make-a-standard-detector.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/how-to/write-tests-for-devices.rst` & `ophyd_async-0.3a6/docs/how-to/write-tests-for-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/images/bluesky_ophyd_epics_devices_logo.svg` & `ophyd_async-0.3a6/docs/images/bluesky_ophyd_epics_devices_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/images/bluesky_ophyd_logo.svg` & `ophyd_async-0.3a6/docs/images/bluesky_ophyd_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/images/ophyd_favicon.svg` & `ophyd_async-0.3a6/docs/images/ophyd_favicon.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/index.md` & `ophyd_async-0.3a6/docs/index.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/reference/api.rst` & `ophyd_async-0.3a6/docs/reference/api.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/tutorials/installation.md` & `ophyd_async-0.3a6/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/docs/tutorials/using-existing-devices.rst` & `ophyd_async-0.3a6/docs/tutorials/using-existing-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/pyproject.toml` & `ophyd_async-0.3a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/__init__.py` & `ophyd_async-0.3a6/src/ophyd_async/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     wait_for_value,
 )
 from .signal_backend import SignalBackend
 from .soft_signal_backend import SoftSignalBackend
 from .standard_readable import ConfigSignal, HintedSignal, StandardReadable
 from .utils import (
     DEFAULT_TIMEOUT,
+    CalculatableTimeout,
+    CalculateTimeout,
     Callback,
     NotConnected,
     ReadingValueCallback,
     T,
     get_dtype,
     get_unique,
     merge_gathered_dicts,
@@ -104,14 +106,16 @@
     "StaticDirectoryProvider",
     "StandardReadable",
     "ConfigSignal",
     "HintedSignal",
     "TriggerInfo",
     "TriggerLogic",
     "HardwareTriggeredFlyable",
+    "CalculateTimeout",
+    "CalculatableTimeout",
     "DEFAULT_TIMEOUT",
     "Callback",
     "NotConnected",
     "ReadingValueCallback",
     "T",
     "get_dtype",
     "get_unique",
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/_providers.py` & `ophyd_async-0.3a6/src/ophyd_async/core/_providers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/async_status.py` & `ophyd_async-0.3a6/src/ophyd_async/core/async_status.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import time
 from dataclasses import asdict, replace
 from typing import (
     AsyncIterator,
     Awaitable,
     Callable,
     Generic,
-    SupportsFloat,
     Type,
     TypeVar,
     cast,
 )
 
 from bluesky.protocols import Status
 
@@ -23,39 +22,34 @@
 AS = TypeVar("AS", bound="AsyncStatus")
 WAS = TypeVar("WAS", bound="WatchableAsyncStatus")
 
 
 class AsyncStatusBase(Status):
     """Convert asyncio awaitable to bluesky Status interface"""
 
-    def __init__(self, awaitable: Awaitable, timeout: SupportsFloat | None = None):
-        if isinstance(timeout, SupportsFloat):
-            timeout = float(timeout)
+    def __init__(self, awaitable: Awaitable):
         if isinstance(awaitable, asyncio.Task):
             self.task = awaitable
         else:
-            self.task = asyncio.create_task(
-                asyncio.wait_for(awaitable, timeout=timeout)
-            )
+            self.task = asyncio.create_task(awaitable)
         self.task.add_done_callback(self._run_callbacks)
         self._callbacks: list[Callback[Status]] = []
 
     def __await__(self):
         return self.task.__await__()
 
     def add_callback(self, callback: Callback[Status]):
         if self.done:
             callback(self)
         else:
             self._callbacks.append(callback)
 
     def _run_callbacks(self, task: asyncio.Task):
-        if not task.cancelled():
-            for callback in self._callbacks:
-                callback(self)
+        for callback in self._callbacks:
+            callback(self)
 
     def exception(self, timeout: float | None = 0.0) -> BaseException | None:
         if timeout != 0.0:
             raise ValueError(
                 "cannot honour any timeout other than 0 in an asynchronous function"
             )
         if self.task.done():
@@ -89,40 +83,33 @@
 
     __str__ = __repr__
 
 
 class AsyncStatus(AsyncStatusBase):
     @classmethod
     def wrap(cls: Type[AS], f: Callable[P, Awaitable]) -> Callable[P, AS]:
+        """Wrap an async function in an AsyncStatus."""
+
         @functools.wraps(f)
         def wrap_f(*args: P.args, **kwargs: P.kwargs) -> AS:
-            # We can't type this more properly because Concatenate/ParamSpec doesn't
-            # yet support keywords
-            # https://peps.python.org/pep-0612/#concatenating-keyword-parameters
-            timeout = kwargs.get("timeout")
-            assert isinstance(timeout, SupportsFloat) or timeout is None
-            return cls(f(*args, **kwargs), timeout=timeout)
+            return cls(f(*args, **kwargs))
 
         # type is actually functools._Wrapped[P, Awaitable, P, AS]
         # but functools._Wrapped is not necessarily available
         return cast(Callable[P, AS], wrap_f)
 
 
 class WatchableAsyncStatus(AsyncStatusBase, Generic[T]):
     """Convert AsyncIterator of WatcherUpdates to bluesky Status interface."""
 
-    def __init__(
-        self,
-        iterator: AsyncIterator[WatcherUpdate[T]],
-        timeout: SupportsFloat | None = None,
-    ):
+    def __init__(self, iterator: AsyncIterator[WatcherUpdate[T]]):
         self._watchers: list[Watcher] = []
         self._start = time.monotonic()
         self._last_update: WatcherUpdate[T] | None = None
-        super().__init__(self._notify_watchers_from(iterator), timeout)
+        super().__init__(self._notify_watchers_from(iterator))
 
     async def _notify_watchers_from(self, iterator: AsyncIterator[WatcherUpdate[T]]):
         async for update in iterator:
             self._last_update = (
                 update
                 if update.time_elapsed is not None
                 else replace(update, time_elapsed=time.monotonic() - self._start)
@@ -142,18 +129,14 @@
             self._update_watcher(watcher, self._last_update)
 
     @classmethod
     def wrap(
         cls: Type[WAS],
         f: Callable[P, AsyncIterator[WatcherUpdate[T]]],
     ) -> Callable[P, WAS]:
-        """Wrap an AsyncIterator in a WatchableAsyncStatus. If it takes
-        'timeout' as an argument, this must be a float or None, and it
-        will be propagated to the status."""
+        """Wrap an AsyncIterator in a WatchableAsyncStatus."""
 
         @functools.wraps(f)
         def wrap_f(*args: P.args, **kwargs: P.kwargs) -> WAS:
-            timeout = kwargs.get("timeout")
-            assert isinstance(timeout, SupportsFloat) or timeout is None
-            return cls(f(*args, **kwargs), timeout=timeout)
+            return cls(f(*args, **kwargs))
 
         return cast(Callable[P, WAS], wrap_f)
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/detector.py` & `ophyd_async-0.3a6/src/ophyd_async/core/detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,14 +328,14 @@
 
     async def collect_asset_docs(
         self, index: Optional[int] = None
     ) -> AsyncIterator[StreamAsset]:
         # Collect stream datum documents for all indices written.
         # The index is optional, and provided for fly scans, however this needs to be
         # retrieved for step scans.
-        if not index:
+        if index is None:
             index = await self.writer.get_indices_written()
         async for doc in self.writer.collect_stream_docs(index):
             yield doc
 
     async def get_index(self) -> int:
         return await self.writer.get_indices_written()
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/device.py` & `ophyd_async-0.3a6/src/ophyd_async/core/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Base device"""
 
-from __future__ import annotations
-
 import asyncio
 import sys
 from functools import cached_property
 from logging import LoggerAdapter, getLogger
 from typing import (
     Any,
     Coroutine,
@@ -28,15 +26,15 @@
     """Common base class for all Ophyd Async Devices.
 
     By default, names and connects all Device children.
     """
 
     _name: str = ""
     #: The parent Device if it exists
-    parent: Optional[Device] = None
+    parent: Optional["Device"] = None
     # None if connect hasn't started, a Task if it has
     _connect_task: Optional[asyncio.Task] = None
     _connect_mock_arg: bool = False
 
     def __init__(self, name: str = "") -> None:
         self.set_name(name)
 
@@ -47,15 +45,15 @@
 
     @cached_property
     def log(self):
         return LoggerAdapter(
             getLogger("ophyd_async.devices"), {"ophyd_async_device_name": self.name}
         )
 
-    def children(self) -> Iterator[Tuple[str, Device]]:
+    def children(self) -> Iterator[Tuple[str, "Device"]]:
         for attr_name, attr in self.__dict__.items():
             if attr_name != "parent" and isinstance(attr, Device):
                 yield attr_name, attr
 
     def set_name(self, name: str):
         """Set ``self.name=name`` and each ``self.child.name=name+"-child"``.
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/device_save_loader.py` & `ophyd_async-0.3a6/src/ophyd_async/core/device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/flyer.py` & `ophyd_async-0.3a6/src/ophyd_async/core/flyer.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Preparable,
     Flyable,
     Generic[T],
 ):
     def __init__(
         self,
         trigger_logic: TriggerLogic[T],
-        configuration_signals: Sequence[SignalR],
+        configuration_signals: Sequence[SignalR] = (),
         name: str = "",
     ):
         self._trigger_logic = trigger_logic
         self._configuration_signals = tuple(configuration_signals)
         super().__init__(name=name)
 
     @property
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/mock_signal_backend.py` & `ophyd_async-0.3a6/src/ophyd_async/core/mock_signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/mock_signal_utils.py` & `ophyd_async-0.3a6/src/ophyd_async/core/mock_signal_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from contextlib import asynccontextmanager, contextmanager
-from typing import Any, Callable, Generator, Iterable, Iterator, List
+from typing import Any, Callable, Iterable, Iterator, List
 from unittest.mock import ANY, Mock
 
 from ophyd_async.core.signal import Signal
 from ophyd_async.core.utils import T
 
 from .mock_signal_backend import MockSignalBackend
 
@@ -123,19 +123,15 @@
 
 @contextmanager
 def _unset_side_effect_cm(put_mock: Mock):
     yield
     put_mock.side_effect = None
 
 
-# linting isn't smart enought to realize @contextmanager will give use a
-# ContextManager[None]
-def callback_on_mock_put(
-    signal: Signal, callback: Callable[[T], None]
-) -> Generator[None, None, None]:
+def callback_on_mock_put(signal: Signal, callback: Callable[[T], None]):
     """For setting a callback when a backend is put to.
 
     Can either be used in a context, with the callback being
     unset on exit, or as an ordinary function.
 
     Parameters
     ----------
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/signal.py` & `ophyd_async-0.3a6/src/ophyd_async/core/signal.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from ophyd_async.core.mock_signal_backend import MockSignalBackend
 from ophyd_async.protocols import AsyncConfigurable, AsyncReadable, AsyncStageable
 
 from .async_status import AsyncStatus
 from .device import Device
 from .signal_backend import SignalBackend
 from .soft_signal_backend import SoftSignalBackend
-from .utils import DEFAULT_TIMEOUT, Callback, T
+from .utils import DEFAULT_TIMEOUT, CalculatableTimeout, CalculateTimeout, Callback, T
 
 
 def _add_timeout(func):
     @functools.wraps(func)
     async def wrapper(self: Signal, *args, **kwargs):
         return await asyncio.wait_for(func(self, *args, **kwargs), self._timeout)
 
@@ -209,23 +209,22 @@
 
     @AsyncStatus.wrap
     async def unstage(self) -> None:
         """Stop caching this signal"""
         self._del_cache(self._get_cache().set_staged(False))
 
 
-USE_DEFAULT_TIMEOUT = "USE_DEFAULT_TIMEOUT"
-
-
 class SignalW(Signal[T], Movable):
     """Signal that can be set"""
 
-    def set(self, value: T, wait=True, timeout=USE_DEFAULT_TIMEOUT) -> AsyncStatus:
+    def set(
+        self, value: T, wait=True, timeout: CalculatableTimeout = CalculateTimeout
+    ) -> AsyncStatus:
         """Set the value and return a status saying when it's done"""
-        if timeout is USE_DEFAULT_TIMEOUT:
+        if timeout is CalculateTimeout:
             timeout = self._timeout
 
         async def do_set():
             self.log.debug(f"Putting value {value} to backend at source {self.source}")
             await self._backend.put(value, wait=wait, timeout=timeout)
             self.log.debug(
                 f"Successfully put value {value} to backend at source {self.source}"
@@ -244,17 +243,19 @@
         }
         return location
 
 
 class SignalX(Signal):
     """Signal that puts the default value"""
 
-    def trigger(self, wait=True, timeout=USE_DEFAULT_TIMEOUT) -> AsyncStatus:
+    def trigger(
+        self, wait=True, timeout: CalculatableTimeout = CalculateTimeout
+    ) -> AsyncStatus:
         """Trigger the action and return a status saying when it's done"""
-        if timeout is USE_DEFAULT_TIMEOUT:
+        if timeout is CalculateTimeout:
             timeout = self._timeout
         coro = self._backend.put(None, wait=wait, timeout=timeout)
         return AsyncStatus(coro)
 
 
 def soft_signal_rw(
     datatype: Optional[Type[T]] = None,
@@ -266,15 +267,15 @@
     return signal
 
 
 def soft_signal_r_and_setter(
     datatype: Optional[Type[T]] = None,
     initial_value: Optional[T] = None,
     name: str = "",
-) -> Tuple[SignalR[T], Callable[[T]]]:
+) -> Tuple[SignalR[T], Callable[[T], None]]:
     """Returns a tuple of a read-only Signal and a callable through
     which the signal can be internally modified within the device. Use
     soft_signal_rw if you want a device that is externally modifiable
     """
     backend = SoftSignalBackend(datatype, initial_value)
     signal = SignalR(backend, name=name)
 
@@ -390,55 +391,60 @@
     actual_numbers = {name: len(d) for name, d in docs.items()}
     assert actual_numbers == numbers, _generate_assert_error_msg(
         "emitted", numbers, actual_numbers
     )
 
 
 async def observe_value(
-    signal: SignalR[T], timeout=None, done_status: Status | None = None
+    signal: SignalR[T], timeout: float | None = None, done_status: Status | None = None
 ) -> AsyncGenerator[T, None]:
     """Subscribe to the value of a signal so it can be iterated from.
 
     Parameters
     ----------
     signal:
         Call subscribe_value on this at the start, and clear_sub on it at the
         end
+    timeout:
+        If given, how long to wait for each updated value in seconds. If an update
+        is not produced in this time then raise asyncio.TimeoutError
     done_status:
         If this status is complete, stop observing and make the iterator return.
+        If it raises an exception then this exception will be raised by the iterator.
 
     Notes
     -----
     Example usage::
 
         async for value in observe_value(sig):
             do_something_with(value)
     """
 
-    class StatusIsDone: ...
-
-    q: asyncio.Queue[T | StatusIsDone] = asyncio.Queue()
+    q: asyncio.Queue[T | Status] = asyncio.Queue()
     if timeout is None:
         get_value = q.get
     else:
 
         async def get_value():
             return await asyncio.wait_for(q.get(), timeout)
 
     if done_status is not None:
-        done_status.add_callback(lambda _: q.put_nowait(StatusIsDone()))
+        done_status.add_callback(q.put_nowait)
 
     signal.subscribe_value(q.put_nowait)
     try:
         while True:
             item = await get_value()
-            if not isinstance(item, StatusIsDone):
-                yield item
+            if done_status and item is done_status:
+                if exc := done_status.exception():
+                    raise exc
+                else:
+                    break
             else:
-                break
+                yield item
     finally:
         signal.clear_sub(q.put_nowait)
 
 
 class _ValueChecker(Generic[T]):
     def __init__(self, matcher: Callable[[T], bool], matcher_name: str):
         self._last_value: Optional[T] = None
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/signal_backend.py` & `ophyd_async-0.3a6/src/ophyd_async/core/signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/soft_signal_backend.py` & `ophyd_async-0.3a6/src/ophyd_async/core/soft_signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/standard_readable.py` & `ophyd_async-0.3a6/src/ophyd_async/core/standard_readable.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/core/utils.py` & `ophyd_async-0.3a6/src/ophyd_async/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,25 @@
 #: A function that will be called with the Reading and value when the
 #: monitor updates
 ReadingValueCallback = Callable[[Reading, T], None]
 DEFAULT_TIMEOUT = 10.0
 ErrorText = Union[str, Dict[str, Exception]]
 
 
+class CalculateTimeout:
+    """Sentinel class used to implement ``myfunc(timeout=CalculateTimeout)``
+
+    This signifies that the function should calculate a suitable non-zero
+    timeout itself
+    """
+
+
+CalculatableTimeout = float | None | Type[CalculateTimeout]
+
+
 class NotConnected(Exception):
     """Exception to be raised if a `Device.connect` is cancelled"""
 
     _indent_width = "    "
 
     def __init__(self, errors: ErrorText):
         """
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/_backend/_aioca.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/_backend/_aioca.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/_backend/_p4p.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/_backend/_p4p.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/_backend/common.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/_backend/common.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/aravis.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/aravis.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/ad_base.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/ad_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     AsyncStatus,
     ShapeProvider,
     set_and_wait_for_value,
 )
 
-from ...signal.signal import epics_signal_r, epics_signal_rw, epics_signal_rw_rbv
+from ...signal.signal import epics_signal_r, epics_signal_rw_rbv
 from ..utils import ImageMode
 from ..writers.nd_plugin import NDArrayBase
 
 
 class DetectorState(str, Enum):
     """
     Default set of states of an AreaDetector driver.
@@ -39,26 +39,20 @@
     [DetectorState.Idle, DetectorState.Aborted]
 )
 
 
 class ADBase(NDArrayBase):
     def __init__(self, prefix: str, name: str = "") -> None:
         # Define some signals
-        self.acquire = epics_signal_rw_rbv(bool, prefix + "Acquire")
         self.acquire_time = epics_signal_rw_rbv(float, prefix + "AcquireTime")
         self.num_images = epics_signal_rw_rbv(int, prefix + "NumImages")
         self.image_mode = epics_signal_rw_rbv(ImageMode, prefix + "ImageMode")
-        self.array_counter = epics_signal_rw_rbv(int, prefix + "ArrayCounter")
-        self.array_size_x = epics_signal_r(int, prefix + "ArraySizeX_RBV")
-        self.array_size_y = epics_signal_r(int, prefix + "ArraySizeY_RBV")
         self.detector_state = epics_signal_r(
             DetectorState, prefix + "DetectorState_RBV"
         )
-        # There is no _RBV for this one
-        self.wait_for_plugins = epics_signal_rw(bool, prefix + "WaitForPlugins")
         super().__init__(prefix, name=name)
 
 
 async def start_acquiring_driver_and_ensure_status(
     driver: ADBase,
     good_states: Set[DetectorState] = set(DEFAULT_GOOD_STATES),
     timeout: float = DEFAULT_TIMEOUT,
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/kinetix.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/kinetix.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/pilatus.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/pilatus.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/single_trigger_det.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/utils.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/vimba.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/vimba.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/_hdffile.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/_hdffile.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/hdf_writer.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/hdf_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,31 +39,32 @@
         self._datasets: List[_HDFDataset] = []
         self._file: Optional[_HDFFile] = None
         self._multiplier = 1
 
     async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
         self._file = None
         info = self._directory_provider()
+        file_path = str(info.root / info.resource_dir)
         await asyncio.gather(
             self.hdf.num_extra_dims.set(0),
             self.hdf.lazy_open.set(True),
             self.hdf.swmr_mode.set(True),
             # See https://github.com/bluesky/ophyd-async/issues/122
-            self.hdf.file_path.set(str(info.root / info.resource_dir)),
+            self.hdf.file_path.set(file_path),
             self.hdf.file_name.set(f"{info.prefix}{self.hdf.name}{info.suffix}"),
             self.hdf.file_template.set("%s/%s.h5"),
             self.hdf.file_write_mode.set(FileWriteMode.stream),
             # Never use custom xml layout file but use the one defined
             # in the source code file NDFileHDF5LayoutXML.cpp
             self.hdf.xml_file_name.set(""),
         )
 
         assert (
             await self.hdf.file_path_exists.get_value()
-        ), f"File path {self.hdf.file_path.get_value()} for hdf plugin does not exist"
+        ), f"File path {file_path} for hdf plugin does not exist"
 
         # Overwrite num_capture to go forever
         await self.hdf.num_capture.set(0)
         # Wait for it to start, stashing the status that tells us when it finishes
         self._capture_status = await set_and_wait_for_value(self.hdf.capture, True)
         name = self._name_provider()
         detector_shape = tuple(await self._shape_provider())
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,11 +32,9 @@
         )
         self.num_capture = epics_signal_rw_rbv(int, prefix + "NumCapture")
         self.num_captured = epics_signal_r(int, prefix + "NumCaptured_RBV")
         self.swmr_mode = epics_signal_rw_rbv(bool, prefix + "SWMRMode")
         self.lazy_open = epics_signal_rw_rbv(bool, prefix + "LazyOpen")
         self.capture = epics_signal_rw_rbv(bool, prefix + "Capture")
         self.flush_now = epics_signal_rw(bool, prefix + "FlushNow")
-        self.array_size0 = epics_signal_r(int, prefix + "ArraySize0_RBV")
-        self.array_size1 = epics_signal_r(int, prefix + "ArraySize1_RBV")
         self.xml_file_name = epics_signal_rw_rbv(str, prefix + "XMLFileName")
         super().__init__(prefix, name)
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/demo/__init__.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/demo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import asyncio
 import atexit
 import random
 import string
 import subprocess
 import sys
-from dataclasses import replace
 from enum import Enum
 from pathlib import Path
 
 import numpy as np
 from bluesky.protocols import Movable, Stoppable
 
 from ophyd_async.core import (
@@ -18,15 +17,21 @@
     Device,
     DeviceVector,
     HintedSignal,
     StandardReadable,
     WatchableAsyncStatus,
     observe_value,
 )
-from ophyd_async.core.utils import WatcherUpdate
+from ophyd_async.core.async_status import AsyncStatus
+from ophyd_async.core.utils import (
+    DEFAULT_TIMEOUT,
+    CalculatableTimeout,
+    CalculateTimeout,
+    WatcherUpdate,
+)
 
 from ..signal.signal import epics_signal_r, epics_signal_rw, epics_signal_x
 
 
 class EnergyMode(str, Enum):
     """Energy mode for `Sensor`"""
 
@@ -62,68 +67,67 @@
 class Mover(StandardReadable, Movable, Stoppable):
     """A demo movable that moves based on velocity"""
 
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
         with self.add_children_as_readables(HintedSignal):
             self.readback = epics_signal_r(float, prefix + "Readback")
-
         with self.add_children_as_readables(ConfigSignal):
             self.velocity = epics_signal_rw(float, prefix + "Velocity")
             self.units = epics_signal_r(str, prefix + "Readback.EGU")
-
         self.setpoint = epics_signal_rw(float, prefix + "Setpoint")
         self.precision = epics_signal_r(int, prefix + "Readback.PREC")
         # Signals that collide with standard methods should have a trailing underscore
         self.stop_ = epics_signal_x(prefix + "Stop.PROC")
         # Whether set() should complete successfully or not
         self._set_success = True
 
         super().__init__(name=name)
 
     def set_name(self, name: str):
         super().set_name(name)
         # Readback should be named the same as its parent in read()
         self.readback.set_name(name)
 
-    async def _move(self, new_position: float):
+    @WatchableAsyncStatus.wrap
+    async def set(
+        self, new_position: float, timeout: CalculatableTimeout = CalculateTimeout
+    ):
         self._set_success = True
-        # time.monotonic won't go backwards in case of NTP corrections
-        old_position, units, precision = await asyncio.gather(
+        old_position, units, precision, velocity = await asyncio.gather(
             self.setpoint.get_value(),
             self.units.get_value(),
             self.precision.get_value(),
+            self.velocity.get_value(),
         )
+        if timeout is CalculateTimeout:
+            assert velocity > 0, "Mover has zero velocity"
+            timeout = abs(new_position - old_position) / velocity + DEFAULT_TIMEOUT
+        # Make an Event that will be set on completion, and a Status that will
+        # error if not done in time
+        done = asyncio.Event()
+        done_status = AsyncStatus(asyncio.wait_for(done.wait(), timeout))
         # Wait for the value to set, but don't wait for put completion callback
-        move_status = self.setpoint.set(new_position, wait=True)
-        if not self._set_success:
-            raise RuntimeError("Motor was stopped")
-        # return a template to set() which it can use to yield progress updates
-        return (
-            WatcherUpdate(
+        await self.setpoint.set(new_position, wait=False)
+        async for current_position in observe_value(
+            self.readback, done_status=done_status
+        ):
+            yield WatcherUpdate(
+                current=current_position,
                 initial=old_position,
-                current=old_position,
                 target=new_position,
+                name=self.name,
                 unit=units,
                 precision=precision,
-            ),
-            move_status,
-        )
-
-    @WatchableAsyncStatus.wrap  # uses the timeout argument from the function it wraps
-    async def set(self, new_position: float, timeout: float | None = None):
-        update, _ = await self._move(new_position)
-        async for current_position in observe_value(self.readback):
-            yield replace(
-                update,
-                name=self.name,
-                current=current_position,
             )
             if np.isclose(current_position, new_position):
+                done.set()
                 break
+        if not self._set_success:
+            raise RuntimeError("Motor was stopped")
 
     async def stop(self, success=True):
         self._set_success = success
         status = self.stop_.trigger()
         await status
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/demo/demo_ad_sim_detector.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/demo/demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/demo/mover.db` & `ophyd_async-0.3a6/src/ophyd_async/epics/demo/mover.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/demo/sensor.db` & `ophyd_async-0.3a6/src/ophyd_async/epics/demo/sensor.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/pvi/pvi.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/pvi/pvi.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/signal/_epics_transport.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/signal/_epics_transport.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/epics/signal/signal.py` & `ophyd_async-0.3a6/src/ophyd_async/epics/signal/signal.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/log.py` & `ophyd_async-0.3a6/src/ophyd_async/log.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/panda/__init__.py` & `ophyd_async-0.3a6/src/ophyd_async/panda/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ._table import (
     SeqTable,
     SeqTableRow,
     SeqTrigger,
     seq_table_from_arrays,
     seq_table_from_rows,
 )
+from ._trigger import StaticSeqTableTriggerLogic
 from ._utils import phase_sorter
 
 __all__ = [
     "CommonPandaBlocks",
     "HDFPanda",
     "PcapBlock",
     "PulseBlock",
@@ -29,8 +30,9 @@
     "SeqTableRow",
     "SeqTrigger",
     "phase_sorter",
     "PandaPcapController",
     "TimeUnits",
     "DataBlock",
     "CommonPandABlocks",
+    "StaticSeqTableTriggerLogic",
 ]
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/panda/_common_blocks.py` & `ophyd_async-0.3a6/src/ophyd_async/panda/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/panda/_hdf_panda.py` & `ophyd_async-0.3a6/src/ophyd_async/panda/_hdf_panda.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/panda/_panda_controller.py` & `ophyd_async-0.3a6/src/ophyd_async/panda/_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/panda/_table.py` & `ophyd_async-0.3a6/src/ophyd_async/panda/_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/panda/_trigger.py` & `ophyd_async-0.3a6/src/ophyd_async/panda/_trigger.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/panda/writers/_hdf_writer.py` & `ophyd_async-0.3a6/src/ophyd_async/panda/writers/_hdf_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,18 +75,18 @@
     ), "Length of read signals are different to length of signals"
 
     signals_to_capture: Dict[str, CaptureSignalWrapper] = {}
     for signal_path, signal_object, signal_value in zip(
         capture_signals.keys(), capture_signals.values(), signal_values
     ):
         signal_path = signal_path.replace("_capture", "")
-        if (signal_value.value in iter(Capture)) and (signal_value.value != Capture.No):
+        if (signal_value in iter(Capture)) and (signal_value != Capture.No):
             signals_to_capture[signal_path] = CaptureSignalWrapper(
                 signal_object,
-                signal_value.value,
+                signal_value,
             )
 
     return signals_to_capture
 
 
 class PandaHDFWriter(DetectorWriter):
     _ctxt: Optional[Context] = None
@@ -122,15 +122,15 @@
         info = self._directory_provider()
         # Set the initial values
         await asyncio.gather(
             self.panda_device.data.hdf_directory.set(
                 str(info.root / info.resource_dir)
             ),
             self.panda_device.data.hdf_file_name.set(
-                f"{info.prefix}{self.panda_device.name}{info.suffix}",
+                f"{info.prefix}{self.panda_device.name}{info.suffix}.h5",
             ),
             self.panda_device.data.num_capture.set(0),
         )
 
         # Wait for it to start, stashing the status that tells us when it finishes
         await self.panda_device.data.capture.set(True)
         name = self._name_provider()
@@ -145,15 +145,15 @@
             # Get block names from numbered blocks, eg INENC[1]
             block_name = (
                 f"{split_path[-3]}{split_path[-2]}"
                 if split_path[-2].isnumeric()
                 else split_path[-2]
             )
 
-            for suffix in str(capture_signal.capture_type).split(" "):
+            for suffix in capture_signal.capture_type.split(" "):
                 self._datasets.append(
                     _HDFDataset(
                         name,
                         block_name,
                         f"{name}-{block_name}-{signal_name}-{suffix}",
                         f"{block_name}-{signal_name}".upper() + f"-{suffix}",
                         [1],
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/panda/writers/_panda_hdf_file.py` & `ophyd_async-0.3a6/src/ophyd_async/panda/writers/_panda_hdf_file.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/planstubs/ensure_connected.py` & `ophyd_async-0.3a6/src/ophyd_async/plan_stubs/ensure_connected.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/protocols.py` & `ophyd_async-0.3a6/src/ophyd_async/protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/sim/demo/sim_motor.py` & `ophyd_async-0.3a6/src/ophyd_async/sim/demo/sim_motor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
+import contextlib
 import time
-from dataclasses import replace
 
 from bluesky.protocols import Movable, Stoppable
 
 from ophyd_async.core import StandardReadable
 from ophyd_async.core.async_status import AsyncStatus, WatchableAsyncStatus
 from ophyd_async.core.signal import (
     observe_value,
@@ -21,113 +21,83 @@
         Simulated motor device
 
         args:
         - prefix: str: Signal names prefix
         - name: str: name of device
         - instant: bool: whether to move instantly, or with a delay
         """
+        # Define some signals
         with self.add_children_as_readables(HintedSignal):
             self.user_readback, self._user_readback_set = soft_signal_r_and_setter(
                 float, 0
             )
-
         with self.add_children_as_readables(ConfigSignal):
-            self.velocity = soft_signal_rw(float, 1.0)
-            self.egu = soft_signal_rw(str, "mm")
-
-        self._instant = instant
-        self._move_status: AsyncStatus | None = None
-
-        # Define some signals
+            self.velocity = soft_signal_rw(float, 0 if instant else 1.0)
+            self.units = soft_signal_rw(str, "mm")
         self.user_setpoint = soft_signal_rw(float, 0)
 
-        super().__init__(name=name)
-
         # Whether set() should complete successfully or not
         self._set_success = True
+        self._move_status: AsyncStatus | None = None
 
-    def stop(self, success=False):
-        """
-        Stop the motor if it is moving
-        """
-        if self._move_status:
-            self._move_status.task.cancel()
-            self._move_status = None
+        super().__init__(name=name)
 
-        async def trigger_callbacks():
-            await self.user_readback._backend.put(
-                await self.user_readback._backend.get_value()
-            )
+    async def _move(self, old_position: float, new_position: float, move_time: float):
+        start = time.monotonic()
+        distance = abs(new_position - old_position)
+        while True:
+            time_elapsed = round(time.monotonic() - start, 2)
+
+            # update position based on time elapsed
+            if time_elapsed >= move_time:
+                # successfully reached our target position
+                self._user_readback_set(new_position)
+                break
+            else:
+                current_position = old_position + distance * time_elapsed / move_time
 
-        asyncio.create_task(trigger_callbacks())
+            self._user_readback_set(current_position)
 
-        self._set_success = success
+            # 10hz update loop
+            await asyncio.sleep(0.1)
 
     @WatchableAsyncStatus.wrap
-    async def set(self, new_position: float, timeout: float | None = None):
+    async def set(self, new_position: float):
         """
         Asynchronously move the motor to a new position.
         """
-        update, move_status = await self._move(new_position, timeout)
-        async for current_position in observe_value(
-            self.user_readback, done_status=move_status
-        ):
-            if not self._set_success:
-                raise RuntimeError("Motor was stopped")
-            yield replace(
-                update,
-                name=self.name,
-                current=current_position,
-            )
-
-    async def _move(self, new_position: float, timeout: float | None = None):
-        """
-        Start the motor moving to a new position.
-
-        If the motor is already moving, it will stop first.
-        If this is an instant motor the move will be instantaneous.
-        """
-        self.stop()
-        start = time.monotonic()
-        self._set_success = True
-
-        current_position = await self.user_readback.get_value()
-        distance = abs(new_position - current_position)
-        travel_time = 0 if self._instant else distance / await self.velocity.get_value()
-
-        old_position, units = await asyncio.gather(
+        # Make sure any existing move tasks are stopped
+        await self.stop()
+        old_position, units, velocity = await asyncio.gather(
             self.user_setpoint.get_value(),
-            self.egu.get_value(),
+            self.units.get_value(),
+            self.velocity.get_value(),
         )
-
-        async def update_position():
-            while True:
-                time_elapsed = round(time.monotonic() - start, 2)
-
-                # update position based on time elapsed
-                if time_elapsed >= travel_time:
-                    # successfully reached our target position
-                    self._user_readback_set(new_position)
-                    self._set_success = True
-                    break
-                else:
-                    current_position = (
-                        old_position + distance * time_elapsed / travel_time
-                    )
-
-                self._user_readback_set(current_position)
-
-                # 10hz update loop
-                await asyncio.sleep(0.1)
-
-        # set up a task that updates the motor position at ~10hz
-        self._move_status = AsyncStatus(asyncio.wait_for(update_position(), timeout))
-
-        return (
-            WatcherUpdate(
-                initial=old_position,
-                current=old_position,
-                target=new_position,
-                unit=units,
-            ),
-            self._move_status,
+        # If zero velocity, do instant move
+        move_time = abs(new_position - old_position) / velocity if velocity else 0
+        self._move_status = AsyncStatus(
+            self._move(old_position, new_position, move_time)
         )
+        # If stop is called then this will raise a CancelledError, ignore it
+        with contextlib.suppress(asyncio.CancelledError):
+            async for current_position in observe_value(
+                self.user_readback, done_status=self._move_status
+            ):
+                yield WatcherUpdate(
+                    current=current_position,
+                    initial=old_position,
+                    target=new_position,
+                    name=self.name,
+                    unit=units,
+                )
+        if not self._set_success:
+            raise RuntimeError("Motor was stopped")
+
+    async def stop(self, success=True):
+        """
+        Stop the motor if it is moving
+        """
+        self._set_success = success
+        if self._move_status:
+            self._move_status.task.cancel()
+            self._move_status = None
+        await self.user_setpoint.set(await self.user_readback.get_value())
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async/sim/pattern_generator.py` & `ophyd_async-0.3a6/src/ophyd_async/sim/pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_detector_control.py` & `ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_detector_control.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_detector_writer.py` & `ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_detector_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_generator.py` & `ophyd_async-0.3a6/src/ophyd_async/sim/sim_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/src/ophyd_async.egg-info/PKG-INFO` & `ophyd_async-0.3a6/src/ophyd_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a5
+Version: 0.3a6
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async.egg-info/SOURCES.txt` & `ophyd_async-0.3a6/src/ophyd_async.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,15 @@
 docs/how-to/compound-devices.rst
 docs/how-to/contribute.md
 docs/how-to/make-a-simple-device.rst
 docs/how-to/make-a-standard-detector.rst
 docs/how-to/write-tests-for-devices.rst
 docs/images/bluesky_ophyd_epics_devices_logo.svg
 docs/images/bluesky_ophyd_logo.svg
-docs/images/hardware-triggered-scan.png
 docs/images/ophyd_favicon.svg
-docs/images/outer-scan.png
-docs/images/simple-hardware-scan.png
 docs/reference/api.rst
 docs/tutorials/installation.md
 docs/tutorials/using-existing-devices.rst
 src/ophyd_async/__init__.py
 src/ophyd_async/__main__.py
 src/ophyd_async/_version.py
 src/ophyd_async/log.py
@@ -133,27 +130,26 @@
 src/ophyd_async/panda/_panda_controller.py
 src/ophyd_async/panda/_table.py
 src/ophyd_async/panda/_trigger.py
 src/ophyd_async/panda/_utils.py
 src/ophyd_async/panda/writers/__init__.py
 src/ophyd_async/panda/writers/_hdf_writer.py
 src/ophyd_async/panda/writers/_panda_hdf_file.py
-src/ophyd_async/planstubs/__init__.py
-src/ophyd_async/planstubs/ensure_connected.py
-src/ophyd_async/planstubs/prepare_trigger_and_dets.py
+src/ophyd_async/plan_stubs/__init__.py
+src/ophyd_async/plan_stubs/ensure_connected.py
+src/ophyd_async/plan_stubs/fly.py
 src/ophyd_async/sim/__init__.py
 src/ophyd_async/sim/pattern_generator.py
 src/ophyd_async/sim/sim_pattern_detector_control.py
 src/ophyd_async/sim/sim_pattern_detector_writer.py
 src/ophyd_async/sim/sim_pattern_generator.py
 src/ophyd_async/sim/demo/__init__.py
 src/ophyd_async/sim/demo/sim_motor.py
 tests/conftest.py
 tests/test_cli.py
-tests/test_flyer_with_panda.py
 tests/test_log.py
 tests/core/test_async_status.py
 tests/core/test_device.py
 tests/core/test_device_collector.py
 tests/core/test_device_save_loader.py
 tests/core/test_flyer.py
 tests/core/test_mock_signal_backend.py
@@ -185,14 +181,15 @@
 tests/panda/test_panda_connect.py
 tests/panda/test_panda_controller.py
 tests/panda/test_panda_utils.py
 tests/panda/test_table.py
 tests/panda/test_trigger.py
 tests/panda/test_writer.py
 tests/panda/db/panda.db
+tests/plan_stubs/test_fly.py
 tests/protocols/test_protocols.py
 tests/sim/__init__.py
 tests/sim/conftest.py
 tests/sim/test_pattern_generator.py
 tests/sim/test_sim_detector.py
 tests/sim/test_sim_writer.py
 tests/sim/test_streaming_plan.py
```

### Comparing `ophyd_async-0.3a5/src/ophyd_async.egg-info/requires.txt` & `ophyd_async-0.3a6/src/ophyd_async.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/conftest.py` & `ophyd_async-0.3a6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/core/test_async_status.py` & `ophyd_async-0.3a6/tests/core/test_async_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,25 +46,26 @@
 
     await status
 
     assert status.exception() is None
 
 
 async def test_async_status_success_if_cancelled(normal_coroutine):
+    cbs = []
     coro = normal_coroutine()
     status = AsyncStatus(coro)
+    status.add_callback(cbs.append)
     assert status.exception() is None
     status.task.cancel()
+    assert not cbs
     with pytest.raises(asyncio.CancelledError):
         await status
+    assert cbs == [status]
     assert status.success is False
     assert isinstance(status.exception(), asyncio.CancelledError)
-    # asyncio will RuntimeWarning us about this never being awaited if we don't.
-    # RunEngine handled this as a special case
-    await coro
 
 
 async def coroutine_to_wrap(time: float):
     await asyncio.sleep(time)
 
 
 async def test_async_status_wrap() -> None:
@@ -122,15 +123,15 @@
             self._fail()
 
     def set(self, value) -> AsyncStatus:
         return AsyncStatus(self._set(value))
 
 
 async def test_status_propogates_traceback_under_RE(RE) -> None:
-    expected_call_stack = ["wait_for", "_set", "_fail"]
+    expected_call_stack = ["_set", "_fail"]
     d = FailingMovable()
     with pytest.raises(FailedStatus) as ctx:
         RE(bps.mv(d, 3))
     # We get "The above exception was the direct cause of the following exception:",
     # so extract that first exception traceback and check
     assert ctx.value.__cause__
     assert expected_call_stack == [
```

### Comparing `ophyd_async-0.3a5/tests/core/test_device.py` & `ophyd_async-0.3a6/tests/core/test_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     DeviceVector,
     MockSignalBackend,
     NotConnected,
     wait_for_connection,
 )
 from ophyd_async.core.soft_signal_backend import SoftSignalBackend
 from ophyd_async.epics.motion import motor
-from ophyd_async.planstubs.ensure_connected import (
-    ensure_connected,
-)
+from ophyd_async.plan_stubs.ensure_connected import ensure_connected
 from ophyd_async.sim.demo.sim_motor import SimMotor
 
 
 class DummyBaseDevice(Device):
     def __init__(self) -> None:
         self.connected = False
 
@@ -145,18 +143,18 @@
     )
 
 
 async def test_device_mock_and_back_again(RE):
     motor = SimMotor("motor")
     assert not motor._connect_task
     await motor.connect(mock=False)
-    assert isinstance(motor.egu._backend, SoftSignalBackend)
+    assert isinstance(motor.units._backend, SoftSignalBackend)
     assert motor._connect_task
     await motor.connect(mock=True)
-    assert isinstance(motor.egu._backend, MockSignalBackend)
+    assert isinstance(motor.units._backend, MockSignalBackend)
 
 
 class MotorBundle(Device):
     def __init__(self, name: str) -> None:
         self.X = motor.Motor("BLxxI-MO-TABLE-01:X")
         self.Y = motor.Motor("BLxxI-MO-TABLE-01:Y")
         self.V: DeviceVector[motor.Motor] = DeviceVector(
```

### Comparing `ophyd_async-0.3a5/tests/core/test_device_collector.py` & `ophyd_async-0.3a6/tests/core/test_device_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pytest
 from bluesky import plan_stubs as bps
 from bluesky.run_engine import RunEngine
 from super_state_machine.errors import TransitionError
 
 from ophyd_async.core import DEFAULT_TIMEOUT, Device, DeviceCollector, NotConnected
+from ophyd_async.core.mock_signal_utils import set_mock_value
 from ophyd_async.epics.motion import motor
 
 
 class FailingDevice(Device):
     async def connect(self, mock: bool = False, timeout=DEFAULT_TIMEOUT):
         raise AttributeError()
 
@@ -82,14 +83,15 @@
     return RE
 
 
 def test_async_device_connector_run_engine_same_event_loop():
     async def set_up_device():
         async with DeviceCollector(mock=True):
             mock_motor = motor.Motor("BLxxI-MO-TABLE-01:X")
+        set_mock_value(mock_motor.velocity, 1)
         return mock_motor
 
     loop = asyncio.new_event_loop()
     checking_loop = asyncio.new_event_loop()
 
     try:
         mock_motor = loop.run_until_complete(set_up_device())
```

### Comparing `ophyd_async-0.3a5/tests/core/test_device_save_loader.py` & `ophyd_async-0.3a6/tests/core/test_device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/core/test_flyer.py` & `ophyd_async-0.3a6/tests/core/test_flyer.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 yield "stream_datum", self._file.compose_stream_datum(indices)
 
     async def close(self) -> None:
         self._file = None
 
 
 @pytest.fixture
-async def detector_list(RE: RunEngine) -> tuple[StandardDetector, StandardDetector]:
+async def detectors(RE: RunEngine) -> tuple[StandardDetector, StandardDetector]:
     writers = [DummyWriter("testa", (1, 1)), DummyWriter("testb", (1, 1))]
     await writers[0].dummy_signal.connect(mock=True)
     await writers[1].dummy_signal.connect(mock=True)
 
     async def dummy_arm_1(self=None, trigger=None, num=0, exposure=None):
         return writers[0].dummy_signal.set(1)
 
@@ -133,15 +133,15 @@
         writer_timeout=3,
     )
 
     return (detector_1, detector_2)
 
 
 async def test_hardware_triggered_flyable(
-    RE: RunEngine, detector_list: tuple[StandardDetector]
+    RE: RunEngine, detectors: tuple[StandardDetector]
 ):
     names = []
     docs = []
 
     def append_and_print(name, doc):
         names.append(name)
         docs.append(doc)
@@ -151,67 +151,67 @@
     trigger_logic = DummyTriggerLogic()
     flyer = HardwareTriggeredFlyable(trigger_logic, [], name="flyer")
     trigger_info = TriggerInfo(
         num=1, trigger=DetectorTrigger.constant_gate, deadtime=2, livetime=2
     )
 
     def flying_plan():
-        yield from bps.stage_all(*detector_list, flyer)
+        yield from bps.stage_all(*detectors, flyer)
         assert flyer._trigger_logic.state == TriggerState.stopping
 
         # move the flyer to the correct place, before fly scanning.
         # Prepare the flyer first to get the trigger info for the detectors
         yield from bps.prepare(flyer, 1, wait=True)
 
         # prepare detectors second.
-        for detector in detector_list:
+        for detector in detectors:
             yield from bps.prepare(
                 detector,
                 trigger_info,
                 wait=True,
             )
 
         assert flyer._trigger_logic.state == TriggerState.preparing
-        for detector in detector_list:
+        for detector in detectors:
             detector.controller.disarm.assert_called_once  # type: ignore
 
         yield from bps.open_run()
-        yield from bps.declare_stream(*detector_list, name="main_stream", collect=True)
+        yield from bps.declare_stream(*detectors, name="main_stream", collect=True)
 
         yield from bps.kickoff(flyer)
-        for detector in detector_list:
+        for detector in detectors:
             yield from bps.kickoff(detector)
 
         yield from bps.complete(flyer, wait=False, group="complete")
-        for detector in detector_list:
+        for detector in detectors:
             yield from bps.complete(detector, wait=False, group="complete")
         assert flyer._trigger_logic.state == TriggerState.null
 
         # Manually incremenet the index as if a frame was taken
-        for detector in detector_list:
+        for detector in detectors:
             detector.writer.index += 1
 
         done = False
         while not done:
             try:
                 yield from bps.wait(group="complete", timeout=0.5)
             except TimeoutError:
                 pass
             else:
                 done = True
             yield from bps.collect(
-                *detector_list,
+                *detectors,
                 return_payload=False,
                 name="main_stream",
             )
         yield from bps.wait(group="complete")
         yield from bps.close_run()
 
-        yield from bps.unstage_all(flyer, *detector_list)
-        for detector in detector_list:
+        yield from bps.unstage_all(flyer, *detectors)
+        for detector in detectors:
             assert detector.controller.disarm.called  # type: ignore
         assert trigger_logic.state == TriggerState.stopping
 
     # fly scan
     RE(flying_plan())
 
     assert names == [
```

### Comparing `ophyd_async-0.3a5/tests/core/test_mock_signal_backend.py` & `ophyd_async-0.3a6/tests/core/test_mock_signal_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,14 +227,29 @@
             "_args": (10.0,),
             "timeout": 10.0,
             "wait": True,
         }
     ]
 
 
+async def test_callback_on_mock_put_fails_if_args_are_not_correct():
+    mock_signal = SignalRW(SoftSignalBackend(float))
+    await mock_signal.connect(mock=True)
+
+    def some_function_without_kwargs(arg):
+        pass
+
+    callback_on_mock_put(mock_signal, some_function_without_kwargs)
+    with pytest.raises(TypeError) as exc:
+        await mock_signal.set(10.0)
+    assert str(exc.value).endswith(
+        "some_function_without_kwargs() got an unexpected keyword argument 'wait'"
+    )
+
+
 async def test_set_mock_values(mock_signals):
     signal1, signal2 = mock_signals
 
     await signal2.get_value() == "first_value"
     for value_set in set_mock_values(signal1, ["second_value", "third_value"]):
         assert await signal1.get_value() == value_set
```

### Comparing `ophyd_async-0.3a5/tests/core/test_signal.py` & `ophyd_async-0.3a6/tests/core/test_signal.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/core/test_soft_signal_backend.py` & `ophyd_async-0.3a6/tests/core/test_soft_signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/core/test_standard_readable.py` & `ophyd_async-0.3a6/tests/core/test_standard_readable.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/core/test_utils.py` & `ophyd_async-0.3a6/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/core/test_watchable_async_status.py` & `ophyd_async-0.3a6/tests/core/test_watchable_async_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,21 +82,17 @@
         await asyncio.sleep(0.01)
         self._sig_setter(val)  # type: ignore
 
 
 class ASTestDeviceTimeoutSet(ASTestDevice):
     @WatchableAsyncStatus.wrap
     async def set(self, val, timeout=0.01):
-        assert self._staged
-        await asyncio.sleep(0.01)
-        self._sig_setter(val - 1)  # type: ignore
-        await asyncio.sleep(0.01)
-        yield WatcherUpdate(1, 1, 1)
-        await asyncio.sleep(0.01)
+        await asyncio.sleep(timeout)
         yield WatcherUpdate(1, 1, 1)
+        raise asyncio.TimeoutError()
 
 
 class ASTestDeviceIteratorSet(ASTestDevice):
     def __init__(
         self, name: str = "", values=[1, 2, 3, 4, 5], complete_set: bool = True
     ) -> None:
         self.values = values
```

### Comparing `ophyd_async-0.3a5/tests/epics/_backend/test_common.py` & `ophyd_async-0.3a6/tests/epics/_backend/test_common.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_aravis.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_aravis.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_controllers.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_controllers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_drivers.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_drivers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_kinetix.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_kinetix.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_pilatus.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_pilatus.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_scans.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_single_trigger_det.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_utils.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_vimba.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_vimba.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/areadetector/test_writers.py` & `ophyd_async-0.3a6/tests/epics/areadetector/test_writers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/demo/test_demo.py` & `ophyd_async-0.3a6/tests/epics/demo/test_demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/demo/test_demo_ad_sim_detector.py` & `ophyd_async-0.3a6/tests/epics/demo/test_demo_ad_sim_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Integration tests for a StandardDetector using a HDFWriter and ADSimController."""
 
 import time
+from collections import defaultdict
 from pathlib import Path
 from typing import List, cast
 
 import bluesky.plan_stubs as bps
+import bluesky.preprocessors as bpp
 import pytest
 from bluesky import RunEngine
 from bluesky.utils import new_uid
 
 from ophyd_async.core import (
     AsyncStatus,
     DeviceCollector,
     StandardDetector,
     StaticDirectoryProvider,
     callback_on_mock_put,
     set_mock_value,
 )
+from ophyd_async.core.signal import assert_emitted
 from ophyd_async.epics.areadetector.controllers import ADSimController
 from ophyd_async.epics.areadetector.drivers import ADBase
 from ophyd_async.epics.areadetector.utils import FileWriteMode, ImageMode
 from ophyd_async.epics.areadetector.writers import HDFWriter, NDFileHDF
 from ophyd_async.epics.demo.demo_ad_sim_detector import DemoADSimDetector
 
 
@@ -98,19 +101,44 @@
         controller = det._controller
         writer = det._writer
 
         set_mock_value(controller.driver.acquire_time, 0.8 + i)
         set_mock_value(controller.driver.image_mode, ImageMode.continuous)
         set_mock_value(writer.hdf.num_capture, 1000)
         set_mock_value(writer.hdf.num_captured, 0)
+        set_mock_value(writer.hdf.file_path_exists, True)
         set_mock_value(controller.driver.array_size_x, 1024 + i)
         set_mock_value(controller.driver.array_size_y, 768 + i)
     yield deta, detb
 
 
+async def test_two_detectors_fly_different_rate(
+    two_detectors: List[DemoADSimDetector], RE: RunEngine
+):
+    docs = defaultdict(list)
+
+    @bpp.stage_decorator(two_detectors)
+    @bpp.run_decorator()
+    def fly_plan():
+        yield from bps.declare_stream(*two_detectors, name="primary")
+        # Make one produce some frames and collect
+        set_mock_value(two_detectors[0].hdf.num_captured, 15)
+        yield from bps.collect(*two_detectors)
+        # It shouldn't make anything as the other one is lagging
+        assert "stream_datum" not in docs
+        # Make the other one produce some frames
+        set_mock_value(two_detectors[1].hdf.num_captured, 15)
+        yield from bps.collect(*two_detectors)
+
+    RE(fly_plan(), lambda name, doc: docs[name].append(doc))
+    assert_emitted(
+        docs, start=1, descriptor=1, stream_resource=2, stream_datum=2, stop=1
+    )
+
+
 async def test_two_detectors_step(
     two_detectors: List[StandardDetector],
     RE: RunEngine,
 ):
     names = []
     docs = []
     RE.subscribe(lambda name, _: names.append(name))
```

### Comparing `ophyd_async-0.3a5/tests/epics/motion/test_motor.py` & `ophyd_async-0.3a6/tests/epics/motion/test_motor.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from bluesky.protocols import Reading
 
 from ophyd_async.core import (
     DeviceCollector,
     set_mock_put_proceeds,
     set_mock_value,
 )
+from ophyd_async.core.mock_signal_utils import callback_on_mock_put
 from ophyd_async.epics.motion import motor
 
 # Long enough for multiple asyncio event loop cycles to run so
 # all the tasks have a chance to run
 A_BIT = 0.001
 
 
@@ -114,14 +115,41 @@
     )
     set_mock_put_proceeds(sim_motor.user_setpoint, True)
     await asyncio.sleep(A_BIT)
     assert s.done
     done.assert_called_once_with(s)
 
 
+async def test_motor_move_timeout(sim_motor: motor.Motor):
+    class MyTimeout(Exception):
+        pass
+
+    def do_timeout(value, wait=False, timeout=None):
+        # Check we were given the right timeout of move_time + DEFAULT_TIMEOUT
+        assert timeout == 10.3
+        # Raise custom exception to be clear it bubbles up
+        raise MyTimeout()
+
+    callback_on_mock_put(sim_motor.user_setpoint, do_timeout)
+    s = sim_motor.set(0.3)
+    watcher = Mock()
+    s.watch(watcher)
+    with pytest.raises(MyTimeout):
+        await s
+    watcher.assert_called_once_with(
+        name="sim_motor",
+        current=0.0,
+        initial=0.0,
+        target=0.3,
+        unit="mm",
+        precision=3,
+        time_elapsed=pytest.approx(0.0, abs=0.05),
+    )
+
+
 async def test_motor_moving_stopped(sim_motor: motor.Motor):
     set_mock_value(sim_motor.motor_done_move, False)
     set_mock_put_proceeds(sim_motor.user_setpoint, False)
     s = sim_motor.set(1.5)
     s.add_callback(Mock())
     await asyncio.sleep(0.2)
     assert not s.done
```

### Comparing `ophyd_async-0.3a5/tests/epics/test_pvi.py` & `ophyd_async-0.3a6/tests/epics/test_pvi.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/test_records.db` & `ophyd_async-0.3a6/tests/epics/test_records.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/epics/test_signals.py` & `ophyd_async-0.3a6/tests/epics/test_signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/panda/db/panda.db` & `ophyd_async-0.3a6/tests/panda/db/panda.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/panda/test_hdf_panda.py` & `ophyd_async-0.3a6/tests/panda/test_hdf_panda.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 
 from ophyd_async.core import StaticDirectoryProvider, set_mock_value
 from ophyd_async.core.device import Device
 from ophyd_async.core.flyer import HardwareTriggeredFlyable
 from ophyd_async.core.mock_signal_utils import callback_on_mock_put
 from ophyd_async.core.signal import SignalR, assert_emitted
 from ophyd_async.epics.signal.signal import epics_signal_r
-from ophyd_async.panda import HDFPanda
-from ophyd_async.panda._trigger import StaticSeqTableTriggerLogic
+from ophyd_async.panda import HDFPanda, StaticSeqTableTriggerLogic
 from ophyd_async.panda.writers._hdf_writer import Capture
-from ophyd_async.planstubs.prepare_trigger_and_dets import (
+from ophyd_async.plan_stubs import (
     prepare_static_seq_table_flyer_and_detectors_with_same_trigger,
 )
 
 
 @pytest.fixture
 async def mock_hdf_panda(tmp_path):
     class CaptureBlock(Device):
@@ -76,20 +75,18 @@
 
     def flying_plan():
         yield from bps.stage_all(mock_hdf_panda, flyer)
 
         yield from prepare_static_seq_table_flyer_and_detectors_with_same_trigger(
             flyer,
             [mock_hdf_panda],
-            num=1,
-            width=exposure,
-            deadtime=mock_hdf_panda.controller.get_deadtime(1),
+            number_of_frames=1,
+            exposure=exposure,
             shutter_time=shutter_time,
         )
-        # mock_hdf_panda.controller.disarm.assert_called_once  # type: ignore
 
         yield from bps.open_run()
         yield from bps.declare_stream(mock_hdf_panda, name="main_stream", collect=True)
 
         set_mock_value(flyer.trigger_logic.seq.active, 1)
 
         yield from bps.kickoff(flyer, wait=True)
@@ -116,15 +113,14 @@
                 name="main_stream",
             )
         yield from bps.wait(group="complete")
         yield from bps.close_run()
 
         yield from bps.unstage_all(flyer, mock_hdf_panda)
         yield from bps.wait_for([lambda: mock_hdf_panda.controller.disarm()])
-        # assert mock_hdf_panda.controller.disarm.called  # type: ignore
 
     # fly scan
     RE(flying_plan())
 
     assert_emitted(
         docs, start=1, descriptor=1, stream_resource=2, stream_datum=2, stop=1
     )
```

### Comparing `ophyd_async-0.3a5/tests/panda/test_panda_connect.py` & `ophyd_async-0.3a6/tests/panda/test_panda_connect.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/panda/test_panda_controller.py` & `ophyd_async-0.3a6/tests/panda/test_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/panda/test_panda_utils.py` & `ophyd_async-0.3a6/tests/panda/test_panda_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/panda/test_table.py` & `ophyd_async-0.3a6/tests/panda/test_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/panda/test_trigger.py` & `ophyd_async-0.3a6/tests/panda/test_trigger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest
 
 from ophyd_async.core.device import DEFAULT_TIMEOUT, DeviceCollector
 from ophyd_async.epics.pvi.pvi import fill_pvi_entries
-from ophyd_async.panda import CommonPandaBlocks
-from ophyd_async.panda._trigger import StaticSeqTableTriggerLogic
+from ophyd_async.panda import CommonPandaBlocks, StaticSeqTableTriggerLogic
 
 
 @pytest.fixture
 async def panda():
     class Panda(CommonPandaBlocks):
         def __init__(self, prefix: str, name: str = ""):
             self._prefix = prefix
```

### Comparing `ophyd_async-0.3a5/tests/panda/test_writer.py` & `ophyd_async-0.3a6/tests/panda/test_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     return mock_panda
 
 
 @pytest.fixture
 async def mock_writer(tmp_path, mock_panda) -> PandaHDFWriter:
     dir_prov = StaticDirectoryProvider(
-        directory_path=str(tmp_path), filename_prefix="", filename_suffix="/data.h5"
+        directory_path=str(tmp_path), filename_prefix="", filename_suffix="/data"
     )
     async with DeviceCollector(mock=True):
         writer = PandaHDFWriter(
             prefix="TEST-PANDA",
             directory_provider=dir_prov,
             name_provider=lambda: "test-panda",
             panda_device=mock_panda,
@@ -201,8 +201,8 @@
             )
         }
 
     with patch(
         "ophyd_async.panda.writers._hdf_writer.get_signals_marked_for_capture",
         get_numeric_signal,
     ):
-        assert "test-panda-block-1-Capture.Value" in await mock_writer.open()
+        assert "test-panda-block-1-Value" in await mock_writer.open()
```

### Comparing `ophyd_async-0.3a5/tests/protocols/test_protocols.py` & `ophyd_async-0.3a6/tests/protocols/test_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/sim/test_pattern_generator.py` & `ophyd_async-0.3a6/tests/sim/test_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/sim/test_sim_detector.py` & `ophyd_async-0.3a6/tests/sim/test_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/sim/test_sim_writer.py` & `ophyd_async-0.3a6/tests/sim/test_sim_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/sim/test_streaming_plan.py` & `ophyd_async-0.3a6/tests/sim/test_streaming_plan.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a5/tests/test_flyer_with_panda.py` & `ophyd_async-0.3a6/tests/plan_stubs/test_fly.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,23 +12,28 @@
     DEFAULT_TIMEOUT,
     DetectorControl,
     DetectorWriter,
     HardwareTriggeredFlyable,
     observe_value,
     set_mock_value,
 )
+from ophyd_async.core.async_status import AsyncStatus, WatchableAsyncStatus
 from ophyd_async.core.detector import StandardDetector
 from ophyd_async.core.device import DeviceCollector
+from ophyd_async.core.flyer import TriggerLogic
+from ophyd_async.core.signal import SignalR
+from ophyd_async.core.utils import WatcherUpdate
 from ophyd_async.epics.pvi.pvi import fill_pvi_entries
 from ophyd_async.epics.signal.signal import epics_signal_rw
-from ophyd_async.panda import CommonPandaBlocks
-from ophyd_async.panda._trigger import StaticSeqTableTriggerLogic
-from ophyd_async.planstubs import (
+from ophyd_async.panda import CommonPandaBlocks, StaticSeqTableTriggerLogic
+from ophyd_async.plan_stubs import (
     prepare_static_seq_table_flyer_and_detectors_with_same_trigger,
+    time_resolved_fly_and_collect_with_static_seq_table,
 )
+from ophyd_async.protocols import AsyncReadable
 
 
 class DummyWriter(DetectorWriter):
     def __init__(self, name: str, shape: Sequence[int]):
         self.dummy_signal = epics_signal_rw(int, "pva://read_pv")
         self._shape = shape
         self._name = name
@@ -82,34 +87,69 @@
                 self._last_emitted = indices_written
                 self._last_flush = time.monotonic()
                 yield "stream_datum", self._file.compose_stream_datum(indices)
 
     async def close(self) -> None:
         self._file = None
 
+    def increment_index(self) -> None:
+        self.index += 1
+
+
+class MockDetector(StandardDetector):
+    def __init__(
+        self,
+        controller: DetectorControl,
+        writer: DetectorWriter,
+        config_sigs: Sequence[AsyncReadable] = [],
+        name: str = "",
+        writer_timeout: float = 1,
+    ) -> None:
+        super().__init__(controller, writer, config_sigs, name, writer_timeout)
+
+    @WatchableAsyncStatus.wrap
+    async def complete(self):
+        assert self._arm_status, "Prepare not run"
+        assert self._trigger_info
+        self.writer.increment_index()
+        async for index in self.writer.observe_indices_written(
+            self._frame_writing_timeout
+        ):
+            yield WatcherUpdate(
+                name=self.name,
+                current=index,
+                initial=self._initial_frame,
+                target=self._trigger_info.num,
+                unit="",
+                precision=0,
+                time_elapsed=time.monotonic() - self._fly_start,
+            )
+            if index >= self._trigger_info.num:
+                break
+
 
 @pytest.fixture
-async def detector_list(RE: RunEngine) -> tuple[StandardDetector, StandardDetector]:
+async def detectors(RE: RunEngine) -> tuple[MockDetector, MockDetector]:
     writers = [DummyWriter("testa", (1, 1)), DummyWriter("testb", (1, 1))]
     await writers[0].dummy_signal.connect(mock=True)
     await writers[1].dummy_signal.connect(mock=True)
 
     async def dummy_arm_1(self=None, trigger=None, num=0, exposure=None):
         return writers[0].dummy_signal.set(1)
 
     async def dummy_arm_2(self=None, trigger=None, num=0, exposure=None):
         return writers[1].dummy_signal.set(1)
 
-    detector_1: StandardDetector = StandardDetector(
+    detector_1 = MockDetector(
         Mock(spec=DetectorControl, get_deadtime=lambda num: num, arm=dummy_arm_1),
         writers[0],
         name="detector_1",
         writer_timeout=3,
     )
-    detector_2: StandardDetector = StandardDetector(
+    detector_2 = MockDetector(
         Mock(spec=DetectorControl, get_deadtime=lambda num: num, arm=dummy_arm_2),
         writers[1],
         name="detector_2",
         writer_timeout=3,
     )
     return (detector_1, detector_2)
 
@@ -130,53 +170,81 @@
     async with DeviceCollector(mock=True):
         mock_panda = Panda("PANDAQSRV:", "mock_panda")
 
     assert mock_panda.name == "mock_panda"
     yield mock_panda
 
 
+@pytest.fixture
+async def flyer(panda):
+    class MockFlyer(HardwareTriggeredFlyable):
+        def __init__(
+            self,
+            trigger_logic: TriggerLogic,
+            configuration_signals: Sequence[SignalR] = ...,
+            name: str = "",
+        ):
+            super().__init__(trigger_logic, configuration_signals, name)
+
+        @AsyncStatus.wrap
+        async def kickoff(self) -> None:
+            set_mock_value(self.trigger_logic.seq.active, 1)
+            await super().kickoff()
+
+        @AsyncStatus.wrap
+        async def complete(self) -> None:
+            set_mock_value(self.trigger_logic.seq.active, 0)
+            await self._trigger_logic.complete()
+
+    # Make flyer
+    trigger_logic = StaticSeqTableTriggerLogic(panda.seq[1])
+    flyer = MockFlyer(trigger_logic, [], name="flyer")
+
+    return flyer
+
+
 async def test_hardware_triggered_flyable_with_static_seq_table_logic(
     RE: RunEngine,
-    detector_list: tuple[StandardDetector],
+    detectors: tuple[StandardDetector],
     panda,
 ):
     """Run a dummy scan using a flyer with a prepare plan stub.
 
     This runs a dummy plan with two detectors and a flyer that uses
     StaticSeqTableTriggerLogic. The flyer and detectors are prepared with the
     prepare_static_seq_table_flyer_and_detectors_with_same_trigger plan stub.
     This stub creates trigger_info and a sequence table from given parameters
     and prepares the fly and both detectors with the same trigger info.
 
     """
     names = []
     docs = []
+    detector_list = list(detectors)
 
     def append_and_print(name, doc):
         names.append(name)
         docs.append(doc)
 
     RE.subscribe(append_and_print)
 
-    shutter_time = 0.004
+    number_of_frames = 1
     exposure = 1
-    deadtime = max(det.controller.get_deadtime(1) for det in detector_list)
+    shutter_time = 0.004
 
     trigger_logic = StaticSeqTableTriggerLogic(panda.seq[1])
     flyer = HardwareTriggeredFlyable(trigger_logic, [], name="flyer")
 
     def flying_plan():
         yield from bps.stage_all(*detector_list, flyer)
 
         yield from prepare_static_seq_table_flyer_and_detectors_with_same_trigger(
             flyer,
             detector_list,
-            num=1,
-            width=exposure,
-            deadtime=deadtime,
+            number_of_frames=number_of_frames,
+            exposure=exposure,
             shutter_time=shutter_time,
         )
 
         for detector in detector_list:
             detector.controller.disarm.assert_called_once  # type: ignore
 
         yield from bps.open_run()
@@ -190,15 +258,15 @@
 
         yield from bps.complete(flyer, wait=False, group="complete")
         for detector in detector_list:
             yield from bps.complete(detector, wait=False, group="complete")
 
         # Manually incremenet the index as if a frame was taken
         for detector in detector_list:
-            detector.writer.index += 1
+            detector.writer.increment_index()
 
         set_mock_value(flyer.trigger_logic.seq.active, 0)
 
         done = False
         while not done:
             try:
                 yield from bps.wait(group="complete", timeout=0.5)
@@ -226,7 +294,83 @@
         "descriptor",
         "stream_resource",
         "stream_datum",
         "stream_resource",
         "stream_datum",
         "stop",
     ]
+
+
+async def test_time_resolved_fly_and_collect_with_static_seq_table(
+    RE: RunEngine,
+    detectors: tuple[StandardDetector],
+    flyer,
+):
+    names = []
+    docs = []
+    detector_list = list(detectors)
+
+    def append_and_print(name, doc):
+        names.append(name)
+        docs.append(doc)
+
+    RE.subscribe(append_and_print)
+
+    # Trigger parameters
+    number_of_frames = 1
+    exposure = 1
+    shutter_time = 0.004
+
+    def fly():
+        yield from bps.stage_all(*detector_list, flyer)
+        yield from bps.open_run()
+        yield from time_resolved_fly_and_collect_with_static_seq_table(
+            stream_name="stream1",
+            flyer=flyer,
+            detectors=detector_list,
+            number_of_frames=number_of_frames,
+            exposure=exposure,
+            shutter_time=shutter_time,
+        )
+        yield from bps.close_run()
+        yield from bps.unstage_all(flyer, *detector_list)
+
+    # fly scan
+    RE(fly())
+
+    assert names == [
+        "start",
+        "descriptor",
+        "stream_resource",
+        "stream_datum",
+        "stream_resource",
+        "stream_datum",
+        "stop",
+    ]
+
+
+@pytest.mark.parametrize("detector_list", [[], None])
+async def test_at_least_one_detector_in_fly_plan(
+    RE: RunEngine,
+    flyer,
+    detector_list,
+):
+    # Trigger parameters
+    number_of_frames = 1
+    exposure = 1
+    shutter_time = 0.004
+
+    assert not detector_list
+
+    def fly():
+        yield from time_resolved_fly_and_collect_with_static_seq_table(
+            stream_name="stream1",
+            flyer=flyer,
+            detectors=detector_list,
+            number_of_frames=number_of_frames,
+            exposure=exposure,
+            shutter_time=shutter_time,
+        )
+
+    with pytest.raises(ValueError) as exc:
+        RE(fly())
+        assert str(exc) == "No detectors provided. There must be at least one."
```

### Comparing `ophyd_async-0.3a5/tests/test_log.py` & `ophyd_async-0.3a6/tests/test_log.py`

 * *Files identical despite different names*

