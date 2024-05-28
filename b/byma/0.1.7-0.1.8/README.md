# Comparing `tmp/byma-0.1.7.tar.gz` & `tmp/byma-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.1.7.tar", last modified: Mon May 27 20:30:35 2024, max compression
+gzip compressed data, was "byma-0.1.8.tar", last modified: Tue May 28 05:53:29 2024, max compression
```

## Comparing `byma-0.1.7.tar` & `byma-0.1.8.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.109779 byma-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-05-27 20:30:22.000000 byma-0.1.7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-27 20:30:22.000000 byma-0.1.7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-27 20:30:22.000000 byma-0.1.7/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-05-27 20:30:22.000000 byma-0.1.7/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-27 20:30:22.000000 byma-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3433 2024-05-27 20:30:35.108778 byma-0.1.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2538 2024-05-27 20:30:22.000000 byma-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.094776 byma-0.1.7/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1384 2024-05-27 20:30:22.000000 byma-0.1.7/byma/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-27 20:30:34.000000 byma-0.1.7/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.096776 byma-0.1.7/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     2612 2024-05-27 20:30:22.000000 byma-0.1.7/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-27 20:30:22.000000 byma-0.1.7/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2024-05-27 20:30:22.000000 byma-0.1.7/byma/interface/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-27 20:30:22.000000 byma-0.1.7/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.097777 byma-0.1.7/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)     8604 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/GradientDescent.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/Iteral.py
--rw-rw-rw-   0 root         (0) root         (0)     6420 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/NesterovMethod.py
--rw-rw-rw-   0 root         (0) root         (0)     5149 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)     4832 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.098777 byma-0.1.7/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-27 20:30:22.000000 byma-0.1.7/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     7951 2024-05-27 20:30:22.000000 byma-0.1.7/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-27 20:30:22.000000 byma-0.1.7/byma/nuby/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-27 20:30:22.000000 byma-0.1.7/byma/nuby/_nuby.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.099777 byma-0.1.7/byma/numy/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-27 20:30:22.000000 byma-0.1.7/byma/numy/Numy.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-27 20:30:22.000000 byma-0.1.7/byma/numy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-05-27 20:30:22.000000 byma-0.1.7/byma/numy/_numy.py
--rw-rw-rw-   0 root         (0) root         (0)     3576 2024-05-27 20:30:22.000000 byma-0.1.7/byma/numy/integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.100777 byma-0.1.7/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-27 20:30:22.000000 byma-0.1.7/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6292 2024-05-27 20:30:22.000000 byma-0.1.7/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.108778 byma-0.1.7/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3433 2024-05-27 20:30:35.000000 byma-0.1.7/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2143 2024-05-27 20:30:35.000000 byma-0.1.7/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 20:30:35.000000 byma-0.1.7/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-27 20:30:35.000000 byma-0.1.7/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.100777 byma-0.1.7/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-27 20:30:22.000000 byma-0.1.7/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-27 20:30:22.000000 byma-0.1.7/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-27 20:30:22.000000 byma-0.1.7/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.101777 byma-0.1.7/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.101777 byma-0.1.7/docs/source/autoapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.101777 byma-0.1.7/docs/source/autoapi/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/OrthogonalSubspace/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.101777 byma-0.1.7/docs/source/autoapi/byma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.102777 byma-0.1.7/docs/source/autoapi/byma/_version/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/_version/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      849 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.102777 byma-0.1.7/docs/source/autoapi/byma/interface/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.102777 byma-0.1.7/docs/source/autoapi/byma/interface/BaseInterface/
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/interface/BaseInterface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.102777 byma-0.1.7/docs/source/autoapi/byma/interface/NonlinearHeat/
--rw-rw-rw-   0 root         (0) root         (0)     2086 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.103778 byma-0.1.7/docs/source/autoapi/byma/interface/Time/
--rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/interface/Time/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     9459 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/interface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.103778 byma-0.1.7/docs/source/autoapi/byma/iteral/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.103778 byma-0.1.7/docs/source/autoapi/byma/iteral/GradientDescent/
--rw-rw-rw-   0 root         (0) root         (0)     3809 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/GradientDescent/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.103778 byma-0.1.7/docs/source/autoapi/byma/iteral/Iteral/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/Iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.104778 byma-0.1.7/docs/source/autoapi/byma/iteral/NesterovMethod/
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.104778 byma-0.1.7/docs/source/autoapi/byma/iteral/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.104778 byma-0.1.7/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     3588 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.104778 byma-0.1.7/docs/source/autoapi/byma/nuby/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/nuby/Bifurcation/
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/nuby/Continuation/
--rw-rw-rw-   0 root         (0) root         (0)     7798 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/nuby/Continuation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/nuby/_nuby/
--rw-rw-rw-   0 root         (0) root         (0)     4840 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/nuby/_nuby/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5104 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/nuby/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/numy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/numy/Numy/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/numy/Numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.106778 byma-0.1.7/docs/source/autoapi/byma/numy/_numy/
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/numy/_numy/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.106778 byma-0.1.7/docs/source/autoapi/byma/numy/integration/
--rw-rw-rw-   0 root         (0) root         (0)     4818 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/numy/integration/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.106778 byma-0.1.7/docs/source/autoapi/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     3579 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/pyplot/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.106778 byma-0.1.7/docs/source/autoapi/byma/pyplot/plots/
--rw-rw-rw-   0 root         (0) root         (0)     3522 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/pyplot/plots/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.107778 byma-0.1.7/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/user/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/user/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/user/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/user/whatisbyma.rst
--rwxrwxrwx   0 root         (0) root         (0)     1005 2024-05-27 20:30:22.000000 byma-0.1.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-27 20:30:22.000000 byma-0.1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 20:30:35.109779 byma-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-05-27 20:30:22.000000 byma-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.108778 byma-0.1.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 20:30:22.000000 byma-0.1.7/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.552209 byma-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-05-28 05:53:17.000000 byma-0.1.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-28 05:53:17.000000 byma-0.1.8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-28 05:53:17.000000 byma-0.1.8/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-05-28 05:53:17.000000 byma-0.1.8/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-28 05:53:17.000000 byma-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-28 05:53:29.552209 byma-0.1.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2409 2024-05-28 05:53:17.000000 byma-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.538209 byma-0.1.8/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2024-05-28 05:53:17.000000 byma-0.1.8/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-28 05:53:29.000000 byma-0.1.8/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.540209 byma-0.1.8/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-05-28 05:53:17.000000 byma-0.1.8/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-28 05:53:17.000000 byma-0.1.8/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2024-05-28 05:53:17.000000 byma-0.1.8/byma/interface/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-28 05:53:17.000000 byma-0.1.8/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.542209 byma-0.1.8/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)     8900 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/GradientDescent.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/Iteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     6420 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/NesterovMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)     4832 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.542209 byma-0.1.8/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-28 05:53:17.000000 byma-0.1.8/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2024-05-28 05:53:17.000000 byma-0.1.8/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-28 05:53:17.000000 byma-0.1.8/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-28 05:53:17.000000 byma-0.1.8/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.543209 byma-0.1.8/byma/numy/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-28 05:53:17.000000 byma-0.1.8/byma/numy/Numy.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-28 05:53:17.000000 byma-0.1.8/byma/numy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-05-28 05:53:17.000000 byma-0.1.8/byma/numy/_numy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-05-28 05:53:17.000000 byma-0.1.8/byma/numy/integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.544209 byma-0.1.8/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-28 05:53:17.000000 byma-0.1.8/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6292 2024-05-28 05:53:17.000000 byma-0.1.8/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.552209 byma-0.1.8/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-28 05:53:29.000000 byma-0.1.8/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2143 2024-05-28 05:53:29.000000 byma-0.1.8/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 05:53:29.000000 byma-0.1.8/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-28 05:53:29.000000 byma-0.1.8/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.544209 byma-0.1.8/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-28 05:53:17.000000 byma-0.1.8/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-28 05:53:17.000000 byma-0.1.8/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-28 05:53:17.000000 byma-0.1.8/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.545209 byma-0.1.8/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.545209 byma-0.1.8/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.545209 byma-0.1.8/docs/source/autoapi/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/OrthogonalSubspace/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.545209 byma-0.1.8/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.546209 byma-0.1.8/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.546209 byma-0.1.8/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.546209 byma-0.1.8/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.546209 byma-0.1.8/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/interface/Time/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/interface/Time/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9459 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/iteral/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/iteral/GradientDescent/
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/GradientDescent/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/iteral/Iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/Iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/iteral/NesterovMethod/
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.548209 byma-0.1.8/docs/source/autoapi/byma/iteral/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.548209 byma-0.1.8/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     3588 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.548209 byma-0.1.8/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.548209 byma-0.1.8/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     7798 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4840 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5104 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/numy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/numy/Numy/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/numy/Numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/numy/_numy/
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/numy/_numy/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.550209 byma-0.1.8/docs/source/autoapi/byma/numy/integration/
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/numy/integration/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.550209 byma-0.1.8/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.550209 byma-0.1.8/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.551209 byma-0.1.8/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/user/whatisbyma.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1005 2024-05-28 05:53:17.000000 byma-0.1.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-28 05:53:17.000000 byma-0.1.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 05:53:29.552209 byma-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-05-28 05:53:17.000000 byma-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.551209 byma-0.1.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 05:53:17.000000 byma-0.1.8/tests/__init__.py
```

### Comparing `byma-0.1.7/.gitlab-ci.yml` & `byma-0.1.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/CHANGELOG.txt` & `byma-0.1.8/CHANGELOG.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,12 +21,17 @@
 
 0.1.3 (10/04/2024)
 -------------------
 - Patch: Reoganization interal method
 - Major: 
     - New sub-package numy
 
-0.1.7 (10/04/2024)
+0.1.7 (27/05/2024)
 -------------------
 - Major: 
     - Nesterov Method
     - GradientDescent Method
+
+0.1.8 (28/05/2024)
+-------------------
+- Patch: 
+    - GradientDescent Method: adjust parameters
```

### Comparing `byma-0.1.7/LICENSE.md` & `byma-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/PKG-INFO` & `byma-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
@@ -18,15 +18,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ByMa
 ![PyPI - Version](https://img.shields.io/pypi/v/byma?style=plastic&label=ByMa&labelColor=green&color=blue&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/label=PyPI%20downloads)](
 https://pypi.org/project/byma/)
-[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/label=Conda%20downloads)](https://anaconda.org/conda-forge/byma)
 ![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/numpy/1.1.1?style=plastic&logo=numpy&label=NumPy&labelColor=blue&link=https%3A%2F%2Fnumpy.org%2F)
 ![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/scipy/1.0.0?style=plastic&logo=scipy&label=SciPy&labelColor=light%20blue&link=https%3A%2F%2Fscipy.org%2F)
 ![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/ByteMath%2Fpython%2FByMa?gitlab_url=https%3A%2F%2Fgitlab.com%2FByteMath%2Fpython%2FByMa&style=plastic)
 ![Static Badge](https://img.shields.io/badge/Docs-Read?style=plastic&label=Read&color=purple&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
```

### Comparing `byma-0.1.7/README.md` & `byma-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # ByMa
 ![PyPI - Version](https://img.shields.io/pypi/v/byma?style=plastic&label=ByMa&labelColor=green&color=blue&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/label=PyPI%20downloads)](
 https://pypi.org/project/byma/)
-[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/label=Conda%20downloads)](https://anaconda.org/conda-forge/byma)
 ![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/numpy/1.1.1?style=plastic&logo=numpy&label=NumPy&labelColor=blue&link=https%3A%2F%2Fnumpy.org%2F)
 ![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/scipy/1.0.0?style=plastic&logo=scipy&label=SciPy&labelColor=light%20blue&link=https%3A%2F%2Fscipy.org%2F)
 ![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/ByteMath%2Fpython%2FByMa?gitlab_url=https%3A%2F%2Fgitlab.com%2FByteMath%2Fpython%2FByMa&style=plastic)
 ![Static Badge](https://img.shields.io/badge/Docs-Read?style=plastic&label=Read&color=purple&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
```

### Comparing `byma-0.1.7/byma/__init__.py` & `byma-0.1.8/byma/__init__.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/interface/BaseInterface.py` & `byma-0.1.8/byma/interface/BaseInterface.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/interface/NonlinearHeat.py` & `byma-0.1.8/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/interface/Time.py` & `byma-0.1.8/byma/interface/Time.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/iteral/GradientDescent.py` & `byma-0.1.8/byma/iteral/GradientDescent.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     'mode': None, 
     'method': 'normal',
     'delta_x': 0.0005,
     "dim": 1,
     "step": 0,
     "beta": 1,
     "domain": None, 
-    "l": 1,
-    "alpha": 1,
+    "L": 1,
+    "gamma": 1,
     "sigma": 0.5,
-    "gamma": None,
+    "alpha": None,
     "c": 1,
     "p": 1
     }
 
 
 def _returns(x, fnorm, dxnorm, mode, method):
     """
@@ -65,40 +65,40 @@
 def calc_numerical_gradient(f, x, delta_x):
     """Function for computing gradient numerically."""
     val_at_x = f(x)
     val_at_next = f(x + delta_x)
     return (val_at_next - val_at_x) / delta_x
 
 ## Armijo stepsize
-def step_size_armijo(beta, sigma, alpha, x, d, f, df):
+def step_size_armijo(beta, sigma, gamma, x, d, f, df):
     """
     Armijo's Rule
     """
     i = 0
     inequality_satisfied = True
     while inequality_satisfied:
-        if df(x + np.power(beta, i)*alpha * d(x)) <= f(x) + alpha * np.power(beta, i) * sigma * df(x).dot(
+        if df(x + np.power(beta, i)*gamma * d(x)) <= f(x) + gamma * np.power(beta, i) * sigma * df(x).dot(
                 d(x)):
             break
 
         i += 1
 
     return np.power(beta, i)
 
-def _step(step, f, df, sigma, alpha, gamma, x, c, p, iter):
+def _step(step, f, df, sigma, alpha, gamma, x, c, p, iter, beta):
     """
     Check type of step
     """
     
     if step == 1:
         k = iter
-        gamma = c*(k**(-p))
+        alpha = c*(k**(-p))
         
     elif step == 2:
-        gamma = alpha*step_size_armijo(beta, sigma, alpha=alpha, x=x, d=d, f=f, df=df)
+        alpha = gamma*step_size_armijo(beta, sigma, gamma=gamma, x=x, d=d, f=f, df=df)
         
     elif step == 3:
         
         if iter != 0:
             g = df(x)
             beta = (npling.norm(g)/npling.norm(dxnorm))**2
             d = -g + beta*dk
@@ -109,21 +109,21 @@
             result = line_search(f=f, myfprime=df, xk=x, pk=dk)
 
         # Check for LineSearchWarning
         if any(isinstance(warn.message, warnings.WarningMessage) and 'The line search algorithm did not converge' in str(warn.message) for warn in w):
             raise ValueError('Line search did not converge.')      
 
         # Extract the step size from the result
-        gamma = result[0]
-        if gamma == None:
-            raise ValueError('Gamma is a NoneType => line search did not converge')
+        alpha = result[0]
+        if alpha == None:
+            raise ValueError('Alpha is a NoneType => line search did not converge')
 
         dxnorm = df(x)
         
-    return gamma
+    return alpha
             
         
 
 @bs.set_defaults(default_cls = Int, default_opts=_DEFAULT_OPTS)
 def gradient_descent(x, f, df, **kwargs):
     """
     Perform Gradient Descent iterations to find the minimizer of a given function.
@@ -156,15 +156,19 @@
                     1: vanishing method
                     2: armijo method
                     3: Fletcher-reeves method 
             
         stop :  int. Default 0. Default optimal 
                     0: ||grad(f)||<tol
         beta : float
-            parameter
+            armijo parameter. Defaul 1
+        gamma : float
+            2nd armijo parameter. Default 1/L
+        alpha : float
+            step size. Default 1/L
         L : float
             smooth constant
     
     Returns
     -------
     minimize, correction_norm, residuals_norm : tuple
         If mode is 'full'
@@ -188,28 +192,28 @@
     _opts = bs.opts(**kwargs)
     verbose = _opts['verbose']
     mode = _opts['mode']
     tol = _opts['tol']
     maxit = int(_opts['maxit'])
     stop = _opts['stop']
     step = _opts['step']
-    beta = _opts['beta']
     delta_x = _opts['delta_x']
     dim = _opts['dim']
     domain = _opts['domain'] 
-    L = _opts['l']
+    L = _opts['L']
     c = _opts['c']
     p = _opts['p']
-    gamma = _opts['gamma'] if _opts['gamma'] != None else 1/L
+    alpha = _opts['alpha'] if _opts['alpha'] != None else 1/L
     sigma = _opts['sigma']
-    alpha = _opts['alpha'] 
-    alpha = alpha if alpha != 0 else gamma
+    gamma = _opts['gamma']
+    beta = _opts['beta']  
+    gamma = gamma if gamma != 0 else alpha
     
     
-    iterative = lambda x, gamma, d: x + gamma * d(x) if callable(d) else x + gamma * d
+    iterative = lambda x, alpha, d: x + alpha * d(x) if callable(d) else x + alpha * d
     d = lambda x: - df(x)
 
     ##### Checking correctness parameters #####
     
     assert isinstance(dim, int), "dim must be an integer"
     
     if maxit <= 0 or not isinstance(maxit, int):
@@ -229,32 +233,37 @@
         print(f'tollerence: {tol}')
         print(f'maximum iter: {maxit}')
         print(f'stopping criteria: {stop}')
         print(f'starting guess: {x}')
         print(f'step size type: {step}')
         print(f'alpha: {alpha}')
         print(f'L: {L}')
-        print(f'gamma: {gamma}')
+        if step == 1:
+            print(f'p: {p}')
+            print(f'c: {c}')
+        if step == 2:
+            print(f'gamma: {gamma}')
+            print(f'beta: {beta}')
     
         print('------ Start iteration ------')
         
     # initialize solution lists
     f_value = f(x)
     df_value = df(x)
     normdx = []
     normf = []
     
     
     for iter in range(maxit):
         
         # Initialize the prescibe type of method 
-        gamma = _step(step, f, df, sigma, alpha, gamma, x, c, p, iter)
+        alpha = _step(step, f, df, sigma, alpha, gamma, x, c, p, iter, beta)
         
         # Iteration Step
-        x = iterative(x, gamma, d)
+        x = iterative(x, alpha, d)
         
         if sp.issparse(f_value) and sp.issparse(df_value):
             fnorm = sp.linalg.norm(f(x))
             dxnorm = sp.linalg.norm(df(x))
         else:
             fnorm = np.linalg.norm(f(x))
             dxnorm = np.linalg.norm(df(x))
```

### Comparing `byma-0.1.7/byma/iteral/NesterovMethod.py` & `byma-0.1.8/byma/iteral/NesterovMethod.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/iteral/Newton.py` & `byma-0.1.8/byma/iteral/Newton.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/iteral/OrthogonalSubspace.py` & `byma-0.1.8/byma/iteral/OrthogonalSubspace.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/nuby/Continuation.py` & `byma-0.1.8/byma/nuby/Continuation.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/numy/integration.py` & `byma-0.1.8/byma/numy/integration.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma/pyplot/plots.py` & `byma-0.1.8/byma/pyplot/plots.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/byma.egg-info/PKG-INFO` & `byma-0.1.8/byma.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
@@ -18,15 +18,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ByMa
 ![PyPI - Version](https://img.shields.io/pypi/v/byma?style=plastic&label=ByMa&labelColor=green&color=blue&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/label=PyPI%20downloads)](
 https://pypi.org/project/byma/)
-[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/label=Conda%20downloads)](https://anaconda.org/conda-forge/byma)
 ![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/numpy/1.1.1?style=plastic&logo=numpy&label=NumPy&labelColor=blue&link=https%3A%2F%2Fnumpy.org%2F)
 ![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/scipy/1.0.0?style=plastic&logo=scipy&label=SciPy&labelColor=light%20blue&link=https%3A%2F%2Fscipy.org%2F)
 ![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/ByteMath%2Fpython%2FByMa?gitlab_url=https%3A%2F%2Fgitlab.com%2FByteMath%2Fpython%2FByMa&style=plastic)
 ![Static Badge](https://img.shields.io/badge/Docs-Read?style=plastic&label=Read&color=purple&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
```

### Comparing `byma-0.1.7/byma.egg-info/SOURCES.txt` & `byma-0.1.8/byma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/Makefile` & `byma-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/make.bat` & `byma-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/interface/BaseInterface/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/interface/BaseInterface/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/interface/Time/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/interface/Time/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/interface/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/interface/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/iteral/GradientDescent/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/iteral/GradientDescent/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 
 .. py:function:: calc_numerical_gradient(f, x, delta_x)
 
    Function for computing gradient numerically.
 
 
-.. py:function:: step_size_armijo(beta, sigma, alpha, x, d, f, df)
+.. py:function:: step_size_armijo(beta, sigma, gamma, x, d, f, df)
 
    Armijo's Rule
 
 
 .. py:function:: gradient_descent(x, f, df, **kwargs)
 
    Perform Gradient Descent iterations to find the minimizer of a given function.
@@ -139,15 +139,19 @@
                    1: vanishing method
                    2: armijo method
                    3: Fletcher-reeves method 
            
        stop :  int. Default 0. Default optimal 
                    0: ||grad(f)||<tol
        beta : float
-           parameter
+           armijo parameter. Defaul 1
+       gamma : float
+           2nd armijo parameter. Default 1/L
+       alpha : float
+           step size. Default 1/L
        L : float
            smooth constant
 
    Returns
    -------
    minimize, correction_norm, residuals_norm : tuple
        If mode is 'full'
```

### Comparing `byma-0.1.7/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/iteral/Newton/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/iteral/Newton/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/nuby/Continuation/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/nuby/Continuation/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/nuby/_nuby/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/nuby/_nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/nuby/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/numy/_numy/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/numy/_numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/numy/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/numy/integration/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/numy/integration/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/pyplot/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/pyplot/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/autoapi/byma/pyplot/plots/index.rst` & `byma-0.1.8/docs/source/autoapi/byma/pyplot/plots/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/conf.py` & `byma-0.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/docs/source/index.rst` & `byma-0.1.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/pyproject.toml` & `byma-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byma-0.1.7/setup.py` & `byma-0.1.8/setup.py`

 * *Files identical despite different names*

