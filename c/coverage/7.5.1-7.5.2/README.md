# Comparing `tmp/coverage-7.5.1.tar.gz` & `tmp/coverage-7.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-7.5.1.tar", last modified: Sat May  4 14:44:36 2024, max compression
+gzip compressed data, was "coverage-7.5.2.tar", last modified: Sun May 26 11:05:30 2024, max compression
```

## Comparing `coverage-7.5.1.tar` & `coverage-7.5.2.tar`

### file list

```diff
@@ -1,462 +1,462 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-04 14:44:25.000000 coverage-7.5.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-04 14:44:25.000000 coverage-7.5.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.516669 coverage-7.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.516669 coverage-7.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/ISSUE_TEMPLATE/support.md
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.516669 coverage-7.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/kit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/python-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/quality.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/testsuite.yml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-04 14:44:25.000000 coverage-7.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    59054 2024-05-04 14:44:25.000000 coverage-7.5.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-04 14:44:25.000000 coverage-7.5.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-04 14:44:25.000000 coverage-7.5.1/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 14:44:25.000000 coverage-7.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-04 14:44:25.000000 coverage-7.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-04 14:44:25.000000 coverage-7.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-04 14:44:25.000000 coverage-7.5.1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-04 14:44:36.584669 coverage-7.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-04 14:44:25.000000 coverage-7.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-04 14:44:25.000000 coverage-7.5.1/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.520669 coverage-7.5.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/comment_on_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/download_gha_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/ghrel_template.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/parse_relnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/trigger_build_kits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.528669 coverage-7.5.1/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/bytecode.py
--rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21784 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    21955 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    51686 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.532669 coverage-7.5.1/coverage/ctracer/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/datastack.c
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/datastack.h
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/filedisp.c
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/filedisp.h
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/module.c
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/stats.h
--rw-r--r--   0 runner    (1001) docker     (127)    34412 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/tracer.c
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/tracer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/util.h
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20718 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/disposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/execfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    19370 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.532669 coverage-7.5.1/coverage/htmlfiles/
--rw-r--r--   0 runner    (1001) docker     (127)    24699 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/pyfile.html
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    18457 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/style.scss
--rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/inorout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/jsonreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/lcovreport.py
--rw-r--r--   0 runner    (1001) docker     (127)    11586 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/numbits.py
--rw-r--r--   0 runner    (1001) docker     (127)    54717 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/phystokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    21331 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/plugin_support.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    14680 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/pytracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/report_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    43636 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/sqldata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/sqlitedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/sysmon.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/templite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/tomlconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/tracer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/xmlreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.540669 coverage-7.5.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.540669 coverage-7.5.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/_static/coverage.css
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_coverage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_coveragedata.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/branch.rst
--rw-r--r--   0 runner    (1001) docker     (127)   112606 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    44589 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/cmd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/cog_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/dbschema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/dict.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/excluding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/howitworks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.540669 coverage-7.5.1/doc/media/
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png
--rw-r--r--   0 runner    (1001) docker     (127)   165210 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/media/sleepy-snake-600.png
--rw-r--r--   0 runner    (1001) docker     (127)    24168 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/media/sleepy-snake-circle-150.png
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/migrating.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/other.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/python-coverage.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/requirements.pip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.540669 coverage-7.5.1/doc/sample_html/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/sample_html/favicon_32_cb_58284776.png
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/sample_html/keybd_closed_cb_ce680311.png
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/sleepy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/source.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/subprocess.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/trouble.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/whatsnew5x.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-04 14:44:25.000000 coverage-7.5.1/howto.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16609 2024-05-04 14:44:25.000000 coverage-7.5.1/igor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.544669 coverage-7.5.1/lab/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.544669 coverage-7.5.1/lab/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)    23241 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/benchmark/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/benchmark/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/bpo_prelude.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/branch_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/branches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2066 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/compare_times.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/coverage-03.dtd
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/coverage-04.dtd
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/find_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/genpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/goals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/hack_pyc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/new-data.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.544669 coverage-7.5.1/lab/notes/
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/notes/bug1303.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/notes/pypy-738-decorated-functions.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/parse_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/pick.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/platform_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/run_sysmon.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/run_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/select_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/show_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/show_pyc.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/treetopy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-04 14:44:25.000000 coverage-7.5.1/metacov.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-04 14:44:25.000000 coverage-7.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.548669 coverage-7.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/dev.pip
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/kit.in
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/kit.pip
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/light-threads.in
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/light-threads.pip
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/mypy.pip
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pins.pip
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pip-tools.pip
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pip.pip
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pytest.in
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pytest.pip
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/tox.pip
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 14:44:36.584669 coverage-7.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-04 14:44:25.000000 coverage-7.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/balance_xdist_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/coveragetest.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/covmodzip1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.504670 coverage-7.5.1/tests/gold/annotate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/anno_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/multi.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/z_80084bf2fba02475___init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/z_80084bf2fba02475_a.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/z_b039179a8a4ce2c2___init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/z_b039179a8a4ce2c2_b.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/encodings/utf8.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/mae/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/mae/mae.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/multi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/multi/a/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/a/__init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/a/a.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/multi/b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/b/__init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/b/b.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/multi.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/white/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/white/white.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/html/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/html/a/
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/a/a_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/a/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/a/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/a/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/b_branch/
--rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/b_branch/b_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/b_branch/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/b_branch/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/b_branch/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/bom/
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/bom/bom_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/bom/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/bom/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/bom/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/contexts/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/contexts/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/contexts/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/contexts/two_tests_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/isolatin1/
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/isolatin1/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/isolatin1/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/isolatin1/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/isolatin1/isolatin1_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/omit_1/
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/m2_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.568669 coverage-7.5.1/tests/gold/html/omit_2/
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/m2_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.568669 coverage-7.5.1/tests/gold/html/omit_3/
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.568669 coverage-7.5.1/tests/gold/html/omit_4/
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.568669 coverage-7.5.1/tests/gold/html/omit_5/
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/other/
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/blah_blah_other_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/here_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/partial/
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial/partial_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/partial_626/
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial_626/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial_626/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial_626/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial_626/partial_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/styled/
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/a_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/index.html
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/myextra.css
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/support/
--rw-r--r--   0 runner    (1001) docker     (127)    24699 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/support/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/support/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/support/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/support/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/html/unicode/
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/unicode/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/unicode/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/unicode/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/unicode/unicode_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/gold/testing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/testing/getty/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/testing/getty/gettysburg.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/testing/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/testing/xml/output.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/gold/xml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/xml/x_xml/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/xml/x_xml/coverage.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/xml/y_xml_branch/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/xml/y_xml_branch/coverage.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/goldtest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/js/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/aa/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/afile.odd.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/afile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/aa/bb/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/bfile.odd.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/bfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/aa/bb/cc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/cc/cfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/aa/bb.odd/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb.odd/bfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/zfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/ambiguous/pkg1/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/ambiguous/pkg1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/ambiguous/pkg1/ambiguous.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/covmod1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/modules/namespace_420/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/namespace_420/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/namespace_420/sub1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/pkg1/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/p1a.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/p1b.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/p1c.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/runmod2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/pkg1/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/sub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/sub/ps1a.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/sub/runmod3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/pkg2/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg2/p2a.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg2/p2b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/plugins/a_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/plugins/another.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/process_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/process_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/process_test/try_execfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/runmod1.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/usepkgs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/moremodules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/moremodules/namespace_420/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/moremodules/namespace_420/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/namespace_420/sub2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/tests/moremodules/othermods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/othera.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/otherb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/tests/moremodules/othermods/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/sub/osa.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/sub/osb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/plugin1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/plugin2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/plugin_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/tests/qunit/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/qunit/jquery.tmpl.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/select_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/stress_phystoken.tok
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/stress_phystoken_dos.tok
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    55256 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    63291 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_arcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44715 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)    31725 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    38001 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16582 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10991 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_execfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_filereporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28110 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_goldtest.py
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_lcov.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_numbits.py
--rw-r--r--   0 runner    (1001) docker     (127)    22660 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_oddball.py
--rw-r--r--   0 runner    (1001) docker     (127)    32720 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_phystokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    44141 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    50581 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43130 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_report_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_report_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_sqlitedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_templite.py
--rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13664 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/testenv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.512669 coverage-7.5.1/tests/zipsrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/tests/zipsrc/zip1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/zipsrc/zip1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/zipsrc/zip1/zip1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-04 14:44:25.000000 coverage-7.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.041120 coverage-7.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-26 11:05:20.000000 coverage-7.5.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-26 11:05:20.000000 coverage-7.5.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.981119 coverage-7.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.981119 coverage-7.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/ISSUE_TEMPLATE/support.md
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.981119 coverage-7.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/workflows/kit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/workflows/python-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/workflows/quality.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-26 11:05:20.000000 coverage-7.5.2/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-26 11:05:20.000000 coverage-7.5.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    60289 2024-05-26 11:05:20.000000 coverage-7.5.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-26 11:05:20.000000 coverage-7.5.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-26 11:05:20.000000 coverage-7.5.2/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-26 11:05:20.000000 coverage-7.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-26 11:05:20.000000 coverage-7.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-26 11:05:20.000000 coverage-7.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-26 11:05:20.000000 coverage-7.5.2/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-26 11:05:30.041120 coverage-7.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-26 11:05:20.000000 coverage-7.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-26 11:05:20.000000 coverage-7.5.2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.985119 coverage-7.5.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 11:05:20.000000 coverage-7.5.2/ci/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-26 11:05:20.000000 coverage-7.5.2/ci/comment_on_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-26 11:05:20.000000 coverage-7.5.2/ci/download_gha_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-26 11:05:20.000000 coverage-7.5.2/ci/ghrel_template.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-26 11:05:20.000000 coverage-7.5.2/ci/parse_relnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-26 11:05:20.000000 coverage-7.5.2/ci/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-26 11:05:20.000000 coverage-7.5.2/ci/trigger_build_kits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.989119 coverage-7.5.2/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21784 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21955 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51686 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.993119 coverage-7.5.2/coverage/ctracer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/datastack.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/datastack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/filedisp.c
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/filedisp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/stats.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34412 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/tracer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/tracer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/ctracer/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20718 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/disposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/execfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19370 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29012 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.993119 coverage-7.5.2/coverage/htmlfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    25474 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/htmlfiles/coverage_html.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/htmlfiles/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/htmlfiles/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/htmlfiles/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/htmlfiles/pyfile.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/htmlfiles/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18457 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/htmlfiles/style.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/inorout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/jsonreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/lcovreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/numbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54315 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/phystokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21331 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/plugin_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/pytracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/report_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43636 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/sqldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/sqlitedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/sysmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/templite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/tomlconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/tracer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-26 11:05:20.000000 coverage-7.5.2/coverage/xmlreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.041120 coverage-7.5.2/coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-26 11:05:29.000000 coverage-7.5.2/coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-26 11:05:29.000000 coverage-7.5.2/coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:05:29.000000 coverage-7.5.2/coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-26 11:05:29.000000 coverage-7.5.2/coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:05:29.000000 coverage-7.5.2/coverage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-26 11:05:29.000000 coverage-7.5.2/coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 11:05:29.000000 coverage-7.5.2/coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.001119 coverage-7.5.2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.001119 coverage-7.5.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/_static/coverage.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/api_coverage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/api_coveragedata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/api_module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/api_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/branch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   112611 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    44589 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/cmd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/cog_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/dbschema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/excluding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/howitworks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.001119 coverage-7.5.2/doc/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165210 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/media/sleepy-snake-600.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24168 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/media/sleepy-snake-circle-150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/migrating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/other.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/python-coverage.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.001119 coverage-7.5.2/doc/sample_html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/sample_html/favicon_32_cb_58284776.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/sample_html/keybd_closed_cb_ce680311.png
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/sleepy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/source.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/subprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/trouble.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-26 11:05:20.000000 coverage-7.5.2/doc/whatsnew5x.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-26 11:05:20.000000 coverage-7.5.2/howto.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-26 11:05:20.000000 coverage-7.5.2/igor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.005119 coverage-7.5.2/lab/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.005119 coverage-7.5.2/lab/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)    23241 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/benchmark/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/benchmark/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/bpo_prelude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/branch_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2066 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/compare_times.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/coverage-03.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/coverage-04.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/find_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/genpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/goals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/hack_pyc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/new-data.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.005119 coverage-7.5.2/lab/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/notes/bug1303.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/notes/pypy-738-decorated-functions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/parse_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/pick.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/platform_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/run_sysmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/run_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/select_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/show_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/show_pyc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 11:05:20.000000 coverage-7.5.2/lab/treetopy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-26 11:05:20.000000 coverage-7.5.2/metacov.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-26 11:05:20.000000 coverage-7.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.009120 coverage-7.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/dev.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/kit.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/kit.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/light-threads.in
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/light-threads.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/mypy.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/pins.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/pip-tools.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/pip.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/pytest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/pytest.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-26 11:05:20.000000 coverage-7.5.2/requirements/tox.pip
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:05:30.041120 coverage-7.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-26 11:05:20.000000 coverage-7.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.017120 coverage-7.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/balance_xdist_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20653 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/coveragetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/covmodzip1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.017120 coverage-7.5.2/tests/gold/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.973119 coverage-7.5.2/tests/gold/annotate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.017120 coverage-7.5.2/tests/gold/annotate/anno_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/anno_dir/multi.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/anno_dir/z_80084bf2fba02475___init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/anno_dir/z_80084bf2fba02475_a.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/anno_dir/z_b039179a8a4ce2c2___init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/anno_dir/z_b039179a8a4ce2c2_b.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.017120 coverage-7.5.2/tests/gold/annotate/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/encodings/utf8.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.017120 coverage-7.5.2/tests/gold/annotate/mae/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/mae/mae.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.017120 coverage-7.5.2/tests/gold/annotate/multi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.021120 coverage-7.5.2/tests/gold/annotate/multi/a/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/multi/a/__init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/multi/a/a.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.021120 coverage-7.5.2/tests/gold/annotate/multi/b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/multi/b/__init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/multi/b/b.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/multi/multi.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.021120 coverage-7.5.2/tests/gold/annotate/white/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/annotate/white/white.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.021120 coverage-7.5.2/tests/gold/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.021120 coverage-7.5.2/tests/gold/html/a/
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/a/a_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/a/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/a/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/a/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.021120 coverage-7.5.2/tests/gold/html/b_branch/
+-rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/b_branch/b_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/b_branch/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/b_branch/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/b_branch/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.021120 coverage-7.5.2/tests/gold/html/bom/
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/bom/bom_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/bom/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/bom/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/bom/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.021120 coverage-7.5.2/tests/gold/html/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/contexts/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/contexts/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/contexts/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/contexts/two_tests_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.025120 coverage-7.5.2/tests/gold/html/isolatin1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/isolatin1/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/isolatin1/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/isolatin1/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/isolatin1/isolatin1_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.025120 coverage-7.5.2/tests/gold/html/omit_1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_1/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_1/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_1/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_1/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_1/m2_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_1/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_1/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.025120 coverage-7.5.2/tests/gold/html/omit_2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_2/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_2/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_2/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_2/m2_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_2/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_2/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.025120 coverage-7.5.2/tests/gold/html/omit_3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_3/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_3/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_3/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_3/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_3/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.029120 coverage-7.5.2/tests/gold/html/omit_4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_4/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_4/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_4/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_4/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_4/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_4/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.029120 coverage-7.5.2/tests/gold/html/omit_5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_5/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_5/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_5/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_5/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/omit_5/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.029120 coverage-7.5.2/tests/gold/html/other/
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/other/blah_blah_other_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/other/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/other/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/other/here_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/other/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.029120 coverage-7.5.2/tests/gold/html/partial/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/partial/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/partial/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/partial/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/partial/partial_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.029120 coverage-7.5.2/tests/gold/html/partial_626/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/partial_626/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/partial_626/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/partial_626/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/partial_626/partial_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/gold/html/styled/
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/styled/a_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/styled/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/styled/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/styled/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/styled/myextra.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/styled/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/gold/html/support/
+-rw-r--r--   0 runner    (1001) docker     (127)    25474 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/support/coverage_html.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/support/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/support/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/support/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/gold/html/unicode/
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/unicode/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/unicode/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/unicode/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/html/unicode/unicode_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.973119 coverage-7.5.2/tests/gold/testing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/gold/testing/getty/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/testing/getty/gettysburg.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/gold/testing/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/testing/xml/output.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.973119 coverage-7.5.2/tests/gold/xml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/gold/xml/x_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/xml/x_xml/coverage.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/gold/xml/y_xml_branch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/gold/xml/y_xml_branch/coverage.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/goldtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/js/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.033120 coverage-7.5.2/tests/modules/aa/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/afile.odd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/afile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/aa/bb/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/bb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/bb/bfile.odd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/bb/bfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/aa/bb/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/bb/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/bb/cc/cfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/aa/bb.odd/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/bb.odd/bfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/aa/zfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/ambiguous/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/ambiguous/pkg1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/ambiguous/pkg1/ambiguous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/covmod1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.977119 coverage-7.5.2/tests/modules/namespace_420/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/namespace_420/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/namespace_420/sub1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/p1a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/p1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/p1c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/runmod2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/pkg1/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/sub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/sub/ps1a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg1/sub/runmod3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/pkg2/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg2/p2a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/pkg2/p2b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/plugins/a_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/plugins/another.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.037120 coverage-7.5.2/tests/modules/process_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/process_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/process_test/try_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/runmod1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/modules/usepkgs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.977119 coverage-7.5.2/tests/moremodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.977119 coverage-7.5.2/tests/moremodules/namespace_420/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.041120 coverage-7.5.2/tests/moremodules/namespace_420/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/moremodules/namespace_420/sub2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.041120 coverage-7.5.2/tests/moremodules/othermods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/moremodules/othermods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/moremodules/othermods/othera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/moremodules/othermods/otherb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.041120 coverage-7.5.2/tests/moremodules/othermods/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/moremodules/othermods/sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/moremodules/othermods/sub/osa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/moremodules/othermods/sub/osb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/plugin1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/plugin2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/plugin_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.041120 coverage-7.5.2/tests/qunit/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/qunit/jquery.tmpl.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/select_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/stress_phystoken.tok
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/stress_phystoken_dos.tok
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55256 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63291 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_arcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44715 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31725 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42697 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38001 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16582 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10991 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_filereporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28110 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_goldtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_lcov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_numbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22660 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_oddball.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33617 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_phystokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44141 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50581 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44049 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_report_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_report_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_sqlitedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_templite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13664 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/test_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/testenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:29.977119 coverage-7.5.2/tests/zipsrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:30.041120 coverage-7.5.2/tests/zipsrc/zip1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/zipsrc/zip1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-26 11:05:20.000000 coverage-7.5.2/tests/zipsrc/zip1/zip1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-26 11:05:20.000000 coverage-7.5.2/tox.ini
```

### Comparing `coverage-7.5.1/.editorconfig` & `coverage-7.5.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.git-blame-ignore-revs` & `coverage-7.5.2/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `coverage-7.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/ISSUE_TEMPLATE/config.yml` & `coverage-7.5.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `coverage-7.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/ISSUE_TEMPLATE/support.md` & `coverage-7.5.2/.github/ISSUE_TEMPLATE/support.md`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/workflows/codeql-analysis.yml` & `coverage-7.5.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/workflows/coverage.yml` & `coverage-7.5.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/workflows/dependency-review.yml` & `coverage-7.5.2/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/workflows/kit.yml` & `coverage-7.5.2/.github/workflows/kit.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/workflows/python-nightly.yml` & `coverage-7.5.2/.github/workflows/python-nightly.yml`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         python-version:
           # When changing this list, be sure to check the [gh] list in
           # tox.ini so that tox will run properly. PYVERSIONS
           # Available versions:
           # https://launchpad.net/~deadsnakes/+archive/ubuntu/nightly/+packages
           - "3.12-dev"
           - "3.13-dev"
+          - "3.14-dev"
           # https://github.com/actions/setup-python#available-versions-of-pypy
           - "pypy-3.8-nightly"
           - "pypy-3.9-nightly"
           - "pypy-3.10-nightly"
         include:
             - python-version: "pypy-3.10-nightly"
               os: "windows-latest"
```

### Comparing `coverage-7.5.1/.github/workflows/quality.yml` & `coverage-7.5.2/.github/workflows/quality.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.github/workflows/testsuite.yml` & `coverage-7.5.2/.github/workflows/testsuite.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/.readthedocs.yaml` & `coverage-7.5.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/CHANGES.rst` & `coverage-7.5.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,44 @@
     ..  .. _changes_9-8-1:
     ..
     ..  Version 9.8.1 — 2027-07-27
     ..  --------------------------
 
 .. scriv-start-here
 
+.. _changes_7-5-2:
+
+Version 7.5.2 — 2024-05-24
+--------------------------
+
+- Fix: nested matches of exclude patterns could exclude too much code, as
+  reported in `issue 1779`_.  This is now fixed.
+
+- Changed: previously, coverage.py would consider a module docstring to be an
+  executable statement if it appeared after line 1 in the file, but not
+  executable if it was the first line.  Now module docstrings are never counted
+  as executable statements.  This can change coverage.py's count of the number
+  of statements in a file, which can slightly change the coverage percentage
+  reported.
+
+- In the HTML report, the filter term and "hide covered" checkbox settings are
+  remembered between viewings, thanks to `Daniel Diniz <pull 1776_>`_.
+
+- Python 3.13.0b1 is supported.
+
+- Fix: parsing error handling is improved to ensure bizarre source files are
+  handled gracefully, and to unblock oss-fuzz fuzzing, thanks to `Liam DeVoe
+  <pull 1788_>`_. Closes `issue 1787`_.
+
+.. _pull 1776: https://github.com/nedbat/coveragepy/pull/1776
+.. _issue 1779: https://github.com/nedbat/coveragepy/issues/1779
+.. _issue 1787: https://github.com/nedbat/coveragepy/issues/1787
+.. _pull 1788: https://github.com/nedbat/coveragepy/pull/1788
+
+
 .. _changes_7-5-1:
 
 Version 7.5.1 — 2024-05-04
 --------------------------
 
 - Fix: a pragma comment on the continuation lines of a multi-line statement
   now excludes the statement and its body, the same as if the pragma is
```

### Comparing `coverage-7.5.1/CITATION.cff` & `coverage-7.5.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/CONTRIBUTORS.txt` & `coverage-7.5.2/CONTRIBUTORS.txt`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 Krystian Kichewko
 Kyle Altendorf
 Lars Hupfeldt Nielsen
 Latrice Wilgus
 Leonardo Pistone
 Lewis Gaul
 Lex Berezhny
+Liam DeVoe
 Loïc Dachary
 Lorenzo Micò
 Louis Heredero
 Luis Nell
 Łukasz Stolcman
 Maciej Kowalczyk
 Manuel Jacob
```

### Comparing `coverage-7.5.1/LICENSE.txt` & `coverage-7.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/MANIFEST.in` & `coverage-7.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/Makefile` & `coverage-7.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/NOTICE.txt` & `coverage-7.5.2/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/PKG-INFO` & `coverage-7.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: coverage
-Version: 7.5.1
+Version: 7.5.2
 Summary: Code coverage measurement for Python
 Home-page: https://github.com/nedbat/coveragepy
-Author: Ned Batchelder and 226 others
+Author: Ned Batchelder and 227 others
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
-Project-URL: Documentation, https://coverage.readthedocs.io/en/7.5.1
+Project-URL: Documentation, https://coverage.readthedocs.io/en/7.5.2
 Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-coverage?utm_source=pypi-coverage&utm_medium=referral&utm_campaign=pypi
 Project-URL: Issues, https://github.com/nedbat/coveragepy/issues
 Project-URL: Mastodon, https://hachyderm.io/@coveragepy
 Project-URL: Mastodon (nedbat), https://hachyderm.io/@nedbat
 Keywords: code coverage testing
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -58,21 +58,21 @@
 the code analysis tools and tracing hooks provided in the Python standard
 library to determine which lines are executable, and which have been executed.
 
 Coverage.py runs on these versions of Python:
 
 .. PYVERSIONS
 
-* Python 3.8 through 3.12, and 3.13.0a6 and up.
+* Python 3.8 through 3.12, and 3.13.0b1 and up.
 * PyPy3 versions 3.8 through 3.10.
 
 Documentation is on `Read the Docs`_.  Code repository and issue tracker are on
 `GitHub`_.
 
-.. _Read the Docs: https://coverage.readthedocs.io/en/7.5.1/
+.. _Read the Docs: https://coverage.readthedocs.io/en/7.5.2/
 .. _GitHub: https://github.com/nedbat/coveragepy
 
 **New in 7.x:**
 initial function/class reporting;
 experimental support for sys.monitoring;
 dropped support for Python 3.7;
 added ``Coverage.collect()`` context manager;
@@ -108,23 +108,23 @@
 
 Getting Started
 ---------------
 
 Looking to run ``coverage`` on your test suite? See the `Quick Start section`_
 of the docs.
 
-.. _Quick Start section: https://coverage.readthedocs.io/en/7.5.1/#quick-start
+.. _Quick Start section: https://coverage.readthedocs.io/en/7.5.2/#quick-start
 
 
 Change history
 --------------
 
 The complete history of changes is on the `change history page`_.
 
-.. _change history page: https://coverage.readthedocs.io/en/7.5.1/changes.html
+.. _change history page: https://coverage.readthedocs.io/en/7.5.2/changes.html
 
 
 Code of Conduct
 ---------------
 
 Everyone participating in the coverage.py project is expected to treat other
 people with respect and to follow the guidelines articulated in the `Python
@@ -135,15 +135,15 @@
 
 Contributing
 ------------
 
 Found a bug? Want to help improve the code or documentation? See the
 `Contributing section`_ of the docs.
 
-.. _Contributing section: https://coverage.readthedocs.io/en/7.5.1/contributing.html
+.. _Contributing section: https://coverage.readthedocs.io/en/7.5.2/contributing.html
 
 
 Security
 --------
 
 To report a security vulnerability, please use the `Tidelift security
 contact`_.  Tidelift will coordinate the fix and disclosure.
@@ -163,15 +163,15 @@
 .. |test-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml
     :alt: Test suite status
 .. |quality-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml
     :alt: Quality check status
 .. |docs| image:: https://readthedocs.org/projects/coverage/badge/?version=latest&style=flat
-    :target: https://coverage.readthedocs.io/en/7.5.1/
+    :target: https://coverage.readthedocs.io/en/7.5.2/
     :alt: Documentation
 .. |kit| image:: https://img.shields.io/pypi/v/coverage
     :target: https://pypi.org/project/coverage/
     :alt: PyPI status
 .. |versions| image:: https://img.shields.io/pypi/pyversions/coverage.svg?logo=python&logoColor=FBE072
     :target: https://pypi.org/project/coverage/
     :alt: Python versions supported
```

### Comparing `coverage-7.5.1/README.rst` & `coverage-7.5.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 the code analysis tools and tracing hooks provided in the Python standard
 library to determine which lines are executable, and which have been executed.
 
 Coverage.py runs on these versions of Python:
 
 .. PYVERSIONS
 
-* Python 3.8 through 3.12, and 3.13.0a6 and up.
+* Python 3.8 through 3.12, and 3.13.0b1 and up.
 * PyPy3 versions 3.8 through 3.10.
 
 Documentation is on `Read the Docs`_.  Code repository and issue tracker are on
 `GitHub`_.
 
 .. _Read the Docs: https://coverage.readthedocs.io/
 .. _GitHub: https://github.com/nedbat/coveragepy
```

### Comparing `coverage-7.5.1/ci/comment_on_fixes.py` & `coverage-7.5.2/ci/comment_on_fixes.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/ci/download_gha_artifacts.py` & `coverage-7.5.2/ci/download_gha_artifacts.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/ci/parse_relnotes.py` & `coverage-7.5.2/ci/parse_relnotes.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/ci/session.py` & `coverage-7.5.2/ci/session.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/ci/trigger_build_kits.py` & `coverage-7.5.2/ci/trigger_build_kits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/__init__.py` & `coverage-7.5.2/coverage/__init__.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/annotate.py` & `coverage-7.5.2/coverage/annotate.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/bytecode.py` & `coverage-7.5.2/coverage/bytecode.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/cmdline.py` & `coverage-7.5.2/coverage/cmdline.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/collector.py` & `coverage-7.5.2/coverage/collector.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/config.py` & `coverage-7.5.2/coverage/config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/context.py` & `coverage-7.5.2/coverage/context.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/control.py` & `coverage-7.5.2/coverage/control.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/datastack.c` & `coverage-7.5.2/coverage/ctracer/datastack.c`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/datastack.h` & `coverage-7.5.2/coverage/ctracer/datastack.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/filedisp.c` & `coverage-7.5.2/coverage/ctracer/filedisp.c`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/filedisp.h` & `coverage-7.5.2/coverage/ctracer/filedisp.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/module.c` & `coverage-7.5.2/coverage/ctracer/module.c`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/stats.h` & `coverage-7.5.2/coverage/ctracer/stats.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/tracer.c` & `coverage-7.5.2/coverage/ctracer/tracer.c`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/tracer.h` & `coverage-7.5.2/coverage/ctracer/tracer.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/ctracer/util.h` & `coverage-7.5.2/coverage/ctracer/util.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/data.py` & `coverage-7.5.2/coverage/data.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/debug.py` & `coverage-7.5.2/coverage/debug.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/disposition.py` & `coverage-7.5.2/coverage/disposition.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/env.py` & `coverage-7.5.2/coverage/env.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/exceptions.py` & `coverage-7.5.2/coverage/exceptions.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/execfile.py` & `coverage-7.5.2/coverage/execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/files.py` & `coverage-7.5.2/coverage/files.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/html.py` & `coverage-7.5.2/coverage/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -593,15 +593,15 @@
             }
             for ip in self.index_pages.values()
         ]
         render_data = {
             "regions": index_page.summaries,
             "totals": index_page.totals,
             "noun": index_page.noun,
-            "column2": index_page.noun if index_page.noun != "file" else "",
+            "region_noun": index_page.noun if index_page.noun != "file" else "",
             "skip_covered": self.skip_covered,
             "skipped_covered_msg": skipped_covered_msg,
             "skipped_empty_msg": skipped_empty_msg,
             "first_html": "",
             "final_html": "",
             "index_buttons": index_buttons,
         }
```

### Comparing `coverage-7.5.1/coverage/htmlfiles/coverage_html.js` & `coverage-7.5.2/coverage/htmlfiles/coverage_html.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -123,14 +123,24 @@
             }
         });
     });
 };
 
 // Create the events for the filter box.
 coverage.wire_up_filter = function() {
+    // Populate the filter and hide100 inputs if there are saved values for them.
+    const saved_filter_value = localStorage.getItem(coverage.FILTER_STORAGE);
+    if (saved_filter_value) {
+        document.getElementById("filter").value = saved_filter_value;
+    }
+    const saved_hide100_value = localStorage.getItem(coverage.HIDE100_STORAGE);
+    if (saved_hide100_value) {
+        document.getElementById("hide100").checked = JSON.parse(saved_hide100_value);
+    }
+
     // Cache elements.
     const table = document.querySelector("table.index");
     const table_body_rows = table.querySelectorAll("tbody tr");
     const no_rows = document.getElementById("no_rows");
 
     // Observe filter keyevents.
     const filter_handler = (event => {
@@ -139,16 +149,20 @@
         // Accumulate the percentage as fraction
         totals[totals.length - 1] = {
             "numer": 0,
             "denom": 0
         }; // nosemgrep: eslint.detect-object-injection
 
         var text = document.getElementById("filter").value;
+        // Store filter value
+        localStorage.setItem(coverage.FILTER_STORAGE, text);
         const casefold = (text === text.toLowerCase());
         const hide100 = document.getElementById("hide100").checked;
+        // Store hide value.
+        localStorage.setItem(coverage.HIDE100_STORAGE, JSON.stringify(hide100));
 
         // Hide / show elements.
         table_body_rows.forEach(row => {
             var show = false;
             // Check the text filter.
             for (let column = 0; column < totals.length; column++) {
                 cell = row.cells[column];
@@ -242,14 +256,16 @@
     document.getElementById("hide100").addEventListener("input", debounce(filter_handler));
 
     // Trigger change event on setup, to force filter on page refresh
     // (filter value may still be present).
     document.getElementById("filter").dispatchEvent(new Event("input"));
     document.getElementById("hide100").dispatchEvent(new Event("input"));
 };
+coverage.FILTER_STORAGE = "COVERAGE_FILTER_VALUE";
+coverage.HIDE100_STORAGE = "COVERAGE_HIDE100_VALUE";
 
 // Set up the click-to-sort columns.
 coverage.wire_up_sorting = function() {
     document.querySelectorAll("[data-sortable] th[aria-sort]").forEach(
         th => th.addEventListener("click", e => sortColumn(e.target))
     );
```

### Comparing `coverage-7.5.1/coverage/htmlfiles/favicon_32.png` & `coverage-7.5.2/coverage/htmlfiles/favicon_32.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/htmlfiles/index.html` & `coverage-7.5.2/coverage/htmlfiles/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 <img id="keyboard_icon" src="{{ statics.keybd_closed_png }}" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
-                        {% if column2 %}
+                        {% if region_noun %}
                         <kbd>n</kbd>
                         {% endif %}
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         {% if has_arcs %}
                         <kbd>b</kbd>
@@ -79,16 +79,16 @@
 
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             {# The title="" attr doesn't work in Safari. #}
             <tr class="tablehead" title="Click to sort">
                 <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                {% if column2 %}
-                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">{{ column2 }}<span class="arrows"></span></th>
+                {% if region_noun %}
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">{{ region_noun }}<span class="arrows"></span></th>
                 {% endif %}
                 <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
                 <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
                 <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
                 {% if has_arcs %}
                 <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
                 <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
@@ -96,15 +96,15 @@
                 <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             {% for region in regions %}
             <tr class="region">
                 <td class="name left"><a href="{{region.url}}">{{region.file}}</a></td>
-                {% if column2 %}
+                {% if region_noun %}
                 <td class="name left"><a href="{{region.url}}">{{region.description}}</a></td>
                 {% endif %}
                 <td>{{region.nums.n_statements}}</td>
                 <td>{{region.nums.n_missing}}</td>
                 <td>{{region.nums.n_excluded}}</td>
                 {% if has_arcs %}
                 <td>{{region.nums.n_branches}}</td>
@@ -113,15 +113,15 @@
                 <td class="right" data-ratio="{{region.nums.ratio_covered|pair}}">{{region.nums.pc_covered_str}}%</td>
             </tr>
             {% endfor %}
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                {% if column2 %}
+                {% if region_noun %}
                 <td class="name left">&nbsp;</td>
                 {% endif %}
                 <td>{{totals.n_statements}}</td>
                 <td>{{totals.n_missing}}</td>
                 <td>{{totals.n_excluded}}</td>
                 {% if has_arcs %}
                 <td>{{totals.n_branches}}</td>
```

#### html2text {}

```diff
@@ -2,24 +2,24 @@
 2.0 #} {# For details: https://github.com/nedbat/coveragepy/blob/master/
 NOTICE.txt #}
 {% if extra_css %}
 {% endif %}
 ************ {{{{ ttiittllee||eessccaappee }}}}:: {{{{ttoottaallss..ppcc__ccoovveerreedd__ssttrr}}}}%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f {% if column2 %} n {% endif %} s m x {% if has_arcs %} b p {% endif %} c  
-change column sorting
+f {% if region_noun %} n {% endif %} s m x {% if has_arcs %} b p {% endif %} c
+  change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 % if skip_covered %}checked disabled {% endif %}> hide covered
 ********** {{%% ffoorr iibbttnn iinn iinnddeexx__bbuuttttoonnss %%}} %% iiff iibbttnn..uurrll %%}} hhrreeff==""{{{{ iibbttnn..uurrll }}}}""{{%%
 eennddiiff %%}}>>{{{{ iibbttnn..llaabbeell }}}}{{##--##}} {{%% eennddffoorr %%}} **********
 _c_o_v_e_r_a_g_e_._p_y_ _v_{_{_____v_e_r_s_i_o_n_____}_}, created at {{ time_stamp }}
-FFiillee           {{{{ ccoolluummnn22 }}}}         ssttaatteemmeennttss                  mmiissssiinngg                  eexxcclluuddeedd                  bbrraanncchheess                  ppaarrttiiaall                           ccoovveerraaggee
+FFiillee           {{{{ rreeggiioonn__nnoouunn }}}}     ssttaatteemmeennttss                  mmiissssiinngg                  eexxcclluuddeedd                  bbrraanncchheess                  ppaarrttiiaall                           ccoovveerraaggee
 _{              _{                     {                           {                        {                         {                         {                                 {
 _{_r_e_g_i_o_n_._f_i_l_e_}_} _{_r_e_g_i_o_n_._d_e_s_c_r_i_p_t_i_o_n_}_} {region.nums.n_statements}} {region.nums.n_missing}} {region.nums.n_excluded}} {region.nums.n_branches}} {region.nums.n_partial_branches}} {region.nums.pc_covered_str}}%
 Total                                {{totals.n_statements}}     {{totals.n_missing}}     {{totals.n_excluded}}     {{totals.n_branches}}     {{totals.n_partial_branches}}     {{totals.pc_covered_str}}%
 No items found using the specified filter.
 {% if skipped_covered_msg %}
 {{ skipped_covered_msg }}
 {% endif %} {% if skipped_empty_msg %}
```

### Comparing `coverage-7.5.1/coverage/htmlfiles/keybd_closed.png` & `coverage-7.5.2/coverage/htmlfiles/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/htmlfiles/pyfile.html` & `coverage-7.5.2/coverage/htmlfiles/pyfile.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/htmlfiles/style.css` & `coverage-7.5.2/coverage/htmlfiles/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/htmlfiles/style.scss` & `coverage-7.5.2/coverage/htmlfiles/style.scss`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/inorout.py` & `coverage-7.5.2/coverage/inorout.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/jsonreport.py` & `coverage-7.5.2/coverage/jsonreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/lcovreport.py` & `coverage-7.5.2/coverage/lcovreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/misc.py` & `coverage-7.5.2/coverage/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 import datetime
 import errno
 import functools
 import hashlib
 import importlib
 import importlib.util
 import inspect
-import locale
 import os
 import os.path
 import re
 import sys
 import types
 
 from types import ModuleType
 from typing import (
-    Any, IO, Iterable, Iterator, Mapping, NoReturn, Sequence, TypeVar,
+    Any, Iterable, Iterator, Mapping, NoReturn, Sequence, TypeVar,
 )
 
 from coverage.exceptions import CoverageException
 from coverage.types import TArc
 
 # In 6.0, the exceptions moved from misc.py to exceptions.py.  But a number of
 # other packages were importing the exceptions from misc, so import them here.
@@ -152,26 +151,14 @@
 
 
 def ensure_dir_for_file(path: str) -> None:
     """Make sure the directory for the path exists."""
     ensure_dir(os.path.dirname(path))
 
 
-def output_encoding(outfile: IO[str] | None = None) -> str:
-    """Determine the encoding to use for output written to `outfile` or stdout."""
-    if outfile is None:
-        outfile = sys.stdout
-    encoding = (
-        getattr(outfile, "encoding", None) or
-        getattr(sys.__stdout__, "encoding", None) or
-        locale.getpreferredencoding()
-    )
-    return encoding
-
-
 class Hasher:
     """Hashes Python data for fingerprinting."""
     def __init__(self) -> None:
         self.hash = hashlib.new("sha3_256")
 
     def update(self, v: Any) -> None:
         """Add `v` to the hash, recursively if needed."""
```

### Comparing `coverage-7.5.1/coverage/multiproc.py` & `coverage-7.5.2/coverage/multiproc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/numbits.py` & `coverage-7.5.2/coverage/numbits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/parser.py` & `coverage-7.5.2/coverage/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Set, Tuple,
 )
 
 from coverage import env
 from coverage.bytecode import code_objects
 from coverage.debug import short_stack
 from coverage.exceptions import NoSource, NotPython
-from coverage.misc import join_regex, nice_pair
+from coverage.misc import nice_pair
 from coverage.phystokens import generate_tokens
 from coverage.types import TArc, TLineNo
 
 
 class PythonParser:
     """Parse code to find executable lines, excluded lines, etc.
 
@@ -58,16 +58,16 @@
             try:
                 self.text = get_python_source(self.filename)
             except OSError as err:
                 raise NoSource(f"No source for code: '{self.filename}': {err}") from err
 
         self.exclude = exclude
 
-        # The text lines of the parsed code.
-        self.lines: list[str] = self.text.split("\n")
+        # The parsed AST of the text.
+        self._ast_root: ast.AST | None = None
 
         # The normalized line numbers of the statements in the code. Exclusions
         # are taken into account, and statements are adjusted to their first
         # lines.
         self.statements: set[TLineNo] = set()
 
         # The normalized line numbers of the excluded lines in the code,
@@ -97,60 +97,49 @@
         # multi-line statements.
         self._multiline: dict[TLineNo, TLineNo] = {}
 
         # Lazily-created arc data, and missing arc descriptions.
         self._all_arcs: set[TArc] | None = None
         self._missing_arc_fragments: TArcFragments | None = None
 
-    @functools.lru_cache()
-    def lines_matching(self, *regexes: str) -> set[TLineNo]:
-        """Find the lines matching one of a list of regexes.
+    def lines_matching(self, regex: str) -> set[TLineNo]:
+        """Find the lines matching a regex.
 
-        Returns a set of line numbers, the lines that contain a match for one
-        of the regexes in `regexes`.  The entire line needn't match, just a
-        part of it.
+        Returns a set of line numbers, the lines that contain a match for
+        `regex`.  The entire line needn't match, just a part of it.
 
         """
-        combined = join_regex(regexes)
-        regex_c = re.compile(combined)
+        regex_c = re.compile(regex)
         matches = set()
-        for i, ltext in enumerate(self.lines, start=1):
+        for i, ltext in enumerate(self.text.split("\n"), start=1):
             if regex_c.search(ltext):
                 matches.add(self._multiline.get(i, i))
         return matches
 
     def _raw_parse(self) -> None:
         """Parse the source to find the interesting facts about its lines.
 
         A handful of attributes are updated.
 
         """
         # Find lines which match an exclusion pattern.
         if self.exclude:
             self.raw_excluded = self.lines_matching(self.exclude)
+            self.excluded = set(self.raw_excluded)
 
-        # Tokenize, to find excluded suites, to find docstrings, and to find
-        # multi-line statements.
-
-        # The last token seen. Start with INDENT to get module docstrings
-        prev_toktype: int = token.INDENT
         # The current number of indents.
         indent: int = 0
         # An exclusion comment will exclude an entire clause at this indent.
         exclude_indent: int = 0
         # Are we currently excluding lines?
         excluding: bool = False
-        # Are we excluding decorators now?
-        excluding_decorators: bool = False
         # The line number of the first line in a multi-line statement.
         first_line: int = 0
         # Is the file empty?
         empty: bool = True
-        # Is this the first token on a line?
-        first_on_line: bool = True
         # Parenthesis (and bracket) nesting level.
         nesting: int = 0
 
         assert self.text is not None
         tokgen = generate_tokens(self.text)
         for toktype, ttext, (slineno, _), (elineno, _), ltext in tokgen:
             if self.show_tokens:                # pragma: debugging
@@ -158,86 +147,90 @@
                     tokenize.tok_name.get(toktype, toktype),
                     nice_pair((slineno, elineno)), ttext, ltext,
                 ))
             if toktype == token.INDENT:
                 indent += 1
             elif toktype == token.DEDENT:
                 indent -= 1
-            elif toktype == token.NAME:
-                if ttext == "class":
-                    # Class definitions look like branches in the bytecode, so
-                    # we need to exclude them.  The simplest way is to note the
-                    # lines with the "class" keyword.
-                    self.raw_classdefs.add(slineno)
             elif toktype == token.OP:
                 if ttext == ":" and nesting == 0:
                     should_exclude = (
-                        self.raw_excluded.intersection(range(first_line, elineno + 1))
-                        or excluding_decorators
+                        self.excluded.intersection(range(first_line, elineno + 1))
                     )
                     if not excluding and should_exclude:
                         # Start excluding a suite.  We trigger off of the colon
                         # token so that the #pragma comment will be recognized on
                         # the same line as the colon.
-                        self.raw_excluded.add(elineno)
+                        self.excluded.add(elineno)
                         exclude_indent = indent
                         excluding = True
-                        excluding_decorators = False
-                elif ttext == "@" and first_on_line:
-                    # A decorator.
-                    if elineno in self.raw_excluded:
-                        excluding_decorators = True
-                    if excluding_decorators:
-                        self.raw_excluded.add(elineno)
                 elif ttext in "([{":
                     nesting += 1
                 elif ttext in ")]}":
                     nesting -= 1
-            elif toktype == token.STRING:
-                if prev_toktype == token.INDENT:
-                    # Strings that are first on an indented line are docstrings.
-                    # (a trick from trace.py in the stdlib.) This works for
-                    # 99.9999% of cases.
-                    self.raw_docstrings.update(range(slineno, elineno+1))
             elif toktype == token.NEWLINE:
                 if first_line and elineno != first_line:
                     # We're at the end of a line, and we've ended on a
                     # different line than the first line of the statement,
                     # so record a multi-line range.
                     for l in range(first_line, elineno+1):
                         self._multiline[l] = first_line
                 first_line = 0
-                first_on_line = True
 
             if ttext.strip() and toktype != tokenize.COMMENT:
                 # A non-white-space token.
                 empty = False
                 if not first_line:
                     # The token is not white space, and is the first in a statement.
                     first_line = slineno
                     # Check whether to end an excluded suite.
                     if excluding and indent <= exclude_indent:
                         excluding = False
                     if excluding:
-                        self.raw_excluded.add(elineno)
-                    first_on_line = False
-
-            prev_toktype = toktype
+                        self.excluded.add(elineno)
 
         # Find the starts of the executable statements.
         if not empty:
             byte_parser = ByteParser(self.text, filename=self.filename)
             self.raw_statements.update(byte_parser._find_statements())
 
         # The first line of modules can lie and say 1 always, even if the first
         # line of code is later. If so, map 1 to the actual first line of the
         # module.
         if env.PYBEHAVIOR.module_firstline_1 and self._multiline:
             self._multiline[1] = min(self.raw_statements)
 
+        self.excluded = self.first_lines(self.excluded)
+
+        # AST lets us find classes, docstrings, and decorator-affected
+        # functions and classes.
+        assert self._ast_root is not None
+        for node in ast.walk(self._ast_root):
+            # Find class definitions.
+            if isinstance(node, ast.ClassDef):
+                self.raw_classdefs.add(node.lineno)
+            # Find docstrings.
+            if isinstance(node, (ast.ClassDef, ast.FunctionDef, ast.AsyncFunctionDef, ast.Module)):
+                if node.body:
+                    first = node.body[0]
+                    if (
+                        isinstance(first, ast.Expr)
+                        and isinstance(first.value, ast.Constant)
+                        and isinstance(first.value.value, str)
+                    ):
+                        self.raw_docstrings.update(
+                            range(first.lineno, cast(int, first.end_lineno) + 1)
+                        )
+            # Exclusions carry from decorators and signatures to the bodies of
+            # functions and classes.
+            if isinstance(node, (ast.ClassDef, ast.FunctionDef, ast.AsyncFunctionDef)):
+                first_line = min((d.lineno for d in node.decorator_list), default=node.lineno)
+                if self.excluded.intersection(range(first_line, node.lineno + 1)):
+                    self.excluded.update(range(first_line, cast(int, node.end_lineno) + 1))
+
     @functools.lru_cache(maxsize=1000)
     def first_line(self, lineno: TLineNo) -> TLineNo:
         """Return the first line number of the statement including `lineno`."""
         if lineno < 0:
             lineno = -self._multiline.get(-lineno, -lineno)
         else:
             lineno = self._multiline.get(lineno, lineno)
@@ -264,27 +257,26 @@
         """Parse source text to find executable lines, excluded lines, etc.
 
         Sets the .excluded and .statements attributes, normalized to the first
         line of multi-line statements.
 
         """
         try:
+            self._ast_root = ast.parse(self.text)
             self._raw_parse()
         except (tokenize.TokenError, IndentationError, SyntaxError) as err:
             if hasattr(err, "lineno"):
                 lineno = err.lineno         # IndentationError
             else:
                 lineno = err.args[1][0]     # TokenError
             raise NotPython(
                 f"Couldn't parse '{self.filename}' as Python source: " +
                 f"{err.args[0]!r} at line {lineno}",
             ) from err
 
-        self.excluded = self.first_lines(self.raw_excluded)
-
         ignore = self.excluded | self.raw_docstrings
         starts = self.raw_statements - ignore
         self.statements = self.first_lines(starts) - ignore
 
     def arcs(self) -> set[TArc]:
         """Get information about the arcs available in the code.
 
@@ -299,15 +291,16 @@
 
     def _analyze_ast(self) -> None:
         """Run the AstArcAnalyzer and save its results.
 
         `_all_arcs` is the set of arcs in the code.
 
         """
-        aaa = AstArcAnalyzer(self.text, self.raw_statements, self._multiline)
+        assert self._ast_root is not None
+        aaa = AstArcAnalyzer(self._ast_root, self.raw_statements, self._multiline)
         aaa.analyze()
 
         self._all_arcs = set()
         for l1, l2 in aaa.arcs:
             fl1 = self.first_line(l1)
             fl2 = self.first_line(l2)
             if fl1 != fl2:
@@ -399,22 +392,17 @@
         filename: str | None = None,
     ) -> None:
         self.text = text
         if code is not None:
             self.code = code
         else:
             assert filename is not None
-            try:
-                self.code = compile(text, filename, "exec", dont_inherit=True)
-            except SyntaxError as synerr:
-                raise NotPython(
-                    "Couldn't parse '%s' as Python source: '%s' at line %d" % (
-                        filename, synerr.msg, synerr.lineno or 0,
-                    ),
-                ) from synerr
+            # We only get here if earlier ast parsing succeeded, so no need to
+            # catch errors.
+            self.code = compile(text, filename, "exec", dont_inherit=True)
 
     def child_parsers(self) -> Iterable[ByteParser]:
         """Iterate over all the code objects nested within this one.
 
         The iteration includes `self` as its first value.
 
         """
@@ -681,19 +669,19 @@
 
 
 class AstArcAnalyzer:
     """Analyze source text with an AST to find executable code paths."""
 
     def __init__(
         self,
-        text: str,
+        root_node: ast.AST,
         statements: set[TLineNo],
         multiline: dict[TLineNo, TLineNo],
     ) -> None:
-        self.root_node = ast.parse(text)
+        self.root_node = root_node
         # TODO: I think this is happening in too many places.
         self.statements = {multiline.get(l, l) for l in statements}
         self.multiline = multiline
 
         # Turn on AST dumps with an environment variable.
         # $set_env.py: COVERAGE_AST_DUMP - Dump the AST nodes when parsing code.
         dump_ast = bool(int(os.getenv("COVERAGE_AST_DUMP", "0")))
```

### Comparing `coverage-7.5.1/coverage/phystokens.py` & `coverage-7.5.2/coverage/phystokens.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/plugin.py` & `coverage-7.5.2/coverage/plugin.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/plugin_support.py` & `coverage-7.5.2/coverage/plugin_support.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/python.py` & `coverage-7.5.2/coverage/python.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,16 +202,18 @@
 
     def translate_arcs(self, arcs: Iterable[TArc]) -> set[TArc]:
         return self.parser.translate_arcs(arcs)
 
     def no_branch_lines(self) -> set[TLineNo]:
         assert self.coverage is not None
         no_branch = self.parser.lines_matching(
-            join_regex(self.coverage.config.partial_list),
-            join_regex(self.coverage.config.partial_always_list),
+            join_regex(
+                self.coverage.config.partial_list
+                + self.coverage.config.partial_always_list
+            )
         )
         return no_branch
 
     def arcs(self) -> set[TArc]:
         return self.parser.arcs()
 
     def exit_counts(self) -> dict[TLineNo, int]:
```

### Comparing `coverage-7.5.1/coverage/pytracer.py` & `coverage-7.5.2/coverage/pytracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,20 +162,20 @@
 
         # if event != "call" and frame.f_code.co_filename != self.cur_file_name:
         #     self.log("---\n*", frame.f_code.co_filename, self.cur_file_name, frame.f_lineno)
 
         if event == "call":
             # Should we start a new context?
             if self.should_start_context and self.context is None:
-                context_maybe = self.should_start_context(frame)
+                context_maybe = self.should_start_context(frame)    # pylint: disable=not-callable
                 if context_maybe is not None:
                     self.context = context_maybe
                     started_context = True
                     assert self.switch_context is not None
-                    self.switch_context(self.context)
+                    self.switch_context(self.context)   # pylint: disable=not-callable
                 else:
                     started_context = False
             else:
                 started_context = False
             self.started_context = started_context
 
             # Entering a new frame.  Decide if we should trace in this file.
@@ -276,15 +276,15 @@
             self.cur_file_data, self.cur_file_name, self.last_line, self.started_context = (
                 self.data_stack.pop()
             )
             # Leaving a context?
             if self.started_context:
                 assert self.switch_context is not None
                 self.context = None
-                self.switch_context(None)
+                self.switch_context(None)   # pylint: disable=not-callable
         return self._cached_bound_method_trace
 
     def start(self) -> TTraceFn:
         """Start this Tracer.
 
         Return a Python function suitable for use with sys.settrace().
```

### Comparing `coverage-7.5.1/coverage/regions.py` & `coverage-7.5.2/coverage/regions.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/report.py` & `coverage-7.5.2/coverage/report.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/report_core.py` & `coverage-7.5.2/coverage/report_core.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/results.py` & `coverage-7.5.2/coverage/results.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/sqldata.py` & `coverage-7.5.2/coverage/sqldata.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/sqlitedb.py` & `coverage-7.5.2/coverage/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/sysmon.py` & `coverage-7.5.2/coverage/sysmon.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/templite.py` & `coverage-7.5.2/coverage/templite.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/tomlconfig.py` & `coverage-7.5.2/coverage/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/tracer.pyi` & `coverage-7.5.2/coverage/tracer.pyi`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/types.py` & `coverage-7.5.2/coverage/types.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage/version.py` & `coverage-7.5.2/coverage/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """The version and URL for coverage.py"""
 # This file is exec'ed in setup.py, don't import anything!
 
 from __future__ import annotations
 
 # version_info: same semantics as sys.version_info.
 # _dev: the .devN suffix if any.
-version_info = (7, 5, 1, "final", 0)
+version_info = (7, 5, 2, "final", 0)
 _dev = 0
 
 
 def _make_version(
     major: int,
     minor: int,
     micro: int,
```

### Comparing `coverage-7.5.1/coverage/xmlreport.py` & `coverage-7.5.2/coverage/xmlreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/coverage.egg-info/PKG-INFO` & `coverage-7.5.2/coverage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: coverage
-Version: 7.5.1
+Version: 7.5.2
 Summary: Code coverage measurement for Python
 Home-page: https://github.com/nedbat/coveragepy
-Author: Ned Batchelder and 226 others
+Author: Ned Batchelder and 227 others
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
-Project-URL: Documentation, https://coverage.readthedocs.io/en/7.5.1
+Project-URL: Documentation, https://coverage.readthedocs.io/en/7.5.2
 Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-coverage?utm_source=pypi-coverage&utm_medium=referral&utm_campaign=pypi
 Project-URL: Issues, https://github.com/nedbat/coveragepy/issues
 Project-URL: Mastodon, https://hachyderm.io/@coveragepy
 Project-URL: Mastodon (nedbat), https://hachyderm.io/@nedbat
 Keywords: code coverage testing
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -58,21 +58,21 @@
 the code analysis tools and tracing hooks provided in the Python standard
 library to determine which lines are executable, and which have been executed.
 
 Coverage.py runs on these versions of Python:
 
 .. PYVERSIONS
 
-* Python 3.8 through 3.12, and 3.13.0a6 and up.
+* Python 3.8 through 3.12, and 3.13.0b1 and up.
 * PyPy3 versions 3.8 through 3.10.
 
 Documentation is on `Read the Docs`_.  Code repository and issue tracker are on
 `GitHub`_.
 
-.. _Read the Docs: https://coverage.readthedocs.io/en/7.5.1/
+.. _Read the Docs: https://coverage.readthedocs.io/en/7.5.2/
 .. _GitHub: https://github.com/nedbat/coveragepy
 
 **New in 7.x:**
 initial function/class reporting;
 experimental support for sys.monitoring;
 dropped support for Python 3.7;
 added ``Coverage.collect()`` context manager;
@@ -108,23 +108,23 @@
 
 Getting Started
 ---------------
 
 Looking to run ``coverage`` on your test suite? See the `Quick Start section`_
 of the docs.
 
-.. _Quick Start section: https://coverage.readthedocs.io/en/7.5.1/#quick-start
+.. _Quick Start section: https://coverage.readthedocs.io/en/7.5.2/#quick-start
 
 
 Change history
 --------------
 
 The complete history of changes is on the `change history page`_.
 
-.. _change history page: https://coverage.readthedocs.io/en/7.5.1/changes.html
+.. _change history page: https://coverage.readthedocs.io/en/7.5.2/changes.html
 
 
 Code of Conduct
 ---------------
 
 Everyone participating in the coverage.py project is expected to treat other
 people with respect and to follow the guidelines articulated in the `Python
@@ -135,15 +135,15 @@
 
 Contributing
 ------------
 
 Found a bug? Want to help improve the code or documentation? See the
 `Contributing section`_ of the docs.
 
-.. _Contributing section: https://coverage.readthedocs.io/en/7.5.1/contributing.html
+.. _Contributing section: https://coverage.readthedocs.io/en/7.5.2/contributing.html
 
 
 Security
 --------
 
 To report a security vulnerability, please use the `Tidelift security
 contact`_.  Tidelift will coordinate the fix and disclosure.
@@ -163,15 +163,15 @@
 .. |test-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml
     :alt: Test suite status
 .. |quality-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml
     :alt: Quality check status
 .. |docs| image:: https://readthedocs.org/projects/coverage/badge/?version=latest&style=flat
-    :target: https://coverage.readthedocs.io/en/7.5.1/
+    :target: https://coverage.readthedocs.io/en/7.5.2/
     :alt: Documentation
 .. |kit| image:: https://img.shields.io/pypi/v/coverage
     :target: https://pypi.org/project/coverage/
     :alt: PyPI status
 .. |versions| image:: https://img.shields.io/pypi/pyversions/coverage.svg?logo=python&logoColor=FBE072
     :target: https://pypi.org/project/coverage/
     :alt: Python versions supported
```

### Comparing `coverage-7.5.1/coverage.egg-info/SOURCES.txt` & `coverage-7.5.2/coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/_static/coverage.css` & `coverage-7.5.2/doc/_static/coverage.css`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/api.rst` & `coverage-7.5.2/doc/api.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/api_module.rst` & `coverage-7.5.2/doc/api_module.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/api_plugin.rst` & `coverage-7.5.2/doc/api_plugin.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/branch.rst` & `coverage-7.5.2/doc/branch.rst`

 * *Files 9% similar despite different names*

```diff
@@ -112,7 +112,20 @@
         if eventually():
             break
 
 Here the while loop will never complete because the break will always be taken
 at some point.  Coverage.py can't work that out on its own, but the "no branch"
 pragma indicates that the branch is known to be partial, and the line is not
 flagged.
+
+Generator expressions
+=====================
+
+Generator expressions may also report partial branch coverage. Consider the
+following example::
+
+    value = next(i in range(1))
+
+While we might expect this line of code to be reported as covered, the
+generator did not iterate until ``StopIteration`` is raised, the indication
+that the loop is complete. This is another case
+where adding ``# pragma: no branch`` may be desirable.
```

### Comparing `coverage-7.5.1/doc/changes.rst` & `coverage-7.5.2/doc/changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -841,18 +841,18 @@
 Version 4.3.2 — 2017-01-16
 --------------------------
 
 - Using the ``--skip-covered`` option on an HTML report with 100% coverage
   would cause a "No data to report" error, as reported in `issue 549`_. This is
   now fixed; thanks, Loïc Dachary.
 
-- If-statements can be optimized away during compilation, for example, `if 0:`
-  or `if __debug__:`.  Coverage.py had problems properly understanding these
-  statements which existed in the source, but not in the compiled bytecode.
-  This problem, reported in `issue 522`_, is now fixed.
+- If-statements can be optimized away during compilation, for example,
+  ``if 0:`` or ``if __debug__:``.  Coverage.py had problems properly
+  understanding these statements which existed in the source, but not in the
+  compiled bytecode.  This problem, reported in `issue 522`_, is now fixed.
 
 - If you specified ``--source`` as a directory, then coverage.py would look for
   importable Python files in that directory, and could identify ones that had
   never been executed at all.  But if you specified it as a package name, that
   detection wasn't performed.  Now it is, closing `issue 426`_. Thanks to Loïc
   Dachary for the fix.
```

### Comparing `coverage-7.5.1/doc/cmd.rst` & `coverage-7.5.2/doc/cmd.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/cog_helpers.py` & `coverage-7.5.2/doc/cog_helpers.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/conf.py` & `coverage-7.5.2/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
 # @@@ editable
 copyright = "2009–2024, Ned Batchelder" # pylint: disable=redefined-builtin
 # The short X.Y.Z version.
-version = "7.5.1"
+version = "7.5.2"
 # The full version, including alpha/beta/rc tags.
-release = "7.5.1"
+release = "7.5.2"
 # The date of release, in "monthname day, year" format.
-release_date = "May 4, 2024"
+release_date = "May 24, 2024"
 # @@@ end
 
 rst_epilog = f"""
 .. |release_date| replace:: {release_date}
 .. |coverage-equals-release| replace:: coverage=={release}
 .. |doc-url| replace:: https://coverage.readthedocs.io/en/{release}
 .. |br| raw:: html
```

### Comparing `coverage-7.5.1/doc/config.rst` & `coverage-7.5.2/doc/config.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/contexts.rst` & `coverage-7.5.2/doc/contexts.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/contributing.rst` & `coverage-7.5.2/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/dbschema.rst` & `coverage-7.5.2/doc/dbschema.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/dict.txt` & `coverage-7.5.2/doc/dict.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/excluding.rst` & `coverage-7.5.2/doc/excluding.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/faq.rst` & `coverage-7.5.2/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/howitworks.rst` & `coverage-7.5.2/doc/howitworks.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/index.rst` & `coverage-7.5.2/doc/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 not.
 
 The latest version is coverage.py |release|, released |release_date|.  It is
 supported on:
 
 .. PYVERSIONS
 
-* Python 3.8 through 3.12, and 3.13.0a6 and up.
+* Python 3.8 through 3.12, and 3.13.0b1 and up.
 * PyPy3 versions 3.8 through 3.10.
 
 .. ifconfig:: prerelease
 
     **This is a pre-release build.  The usual warnings about possible bugs
     apply.** The latest stable version is coverage.py 6.5.0, `described here`_.
```

### Comparing `coverage-7.5.1/doc/install.rst` & `coverage-7.5.2/doc/install.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png` & `coverage-7.5.2/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png` & `coverage-7.5.2/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/media/sleepy-snake-600.png` & `coverage-7.5.2/doc/media/sleepy-snake-600.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/media/sleepy-snake-circle-150.png` & `coverage-7.5.2/doc/media/sleepy-snake-circle-150.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/migrating.rst` & `coverage-7.5.2/doc/migrating.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/other.rst` & `coverage-7.5.2/doc/other.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/plugins.rst` & `coverage-7.5.2/doc/plugins.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/python-coverage.1.txt` & `coverage-7.5.2/doc/python-coverage.1.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/requirements.pip` & `coverage-7.5.2/doc/requirements.pip`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via sphinx
 anyio==4.3.0
     # via
     #   starlette
     #   watchfiles
 attrs==23.2.0
     # via scriv
-babel==2.14.0
+babel==2.15.0
     # via sphinx
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
@@ -41,36 +41,40 @@
     # via uvicorn
 idna==3.7
     # via
     #   anyio
     #   requests
 imagesize==1.4.1
     # via sphinx
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   scriv
     #   sphinx
 markdown-it-py==3.0.0
     # via scriv
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 packaging==24.0
     # via sphinx
 pbr==6.0.0
     # via stevedore
+polib==1.2.0
+    # via sphinx-lint
 pyenchant==3.2.2
     # via
     #   -r doc/requirements.in
     #   sphinxcontrib-spelling
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   doc8
     #   sphinx
+regex==2024.4.28
+    # via sphinx-lint
 requests==2.31.0
     # via
     #   scriv
     #   sphinx
 restructuredtext-lint==1.4.0
     # via doc8
 scriv==1.5.1
@@ -88,14 +92,16 @@
     #   sphinxcontrib-jquery
     #   sphinxcontrib-restbuilder
     #   sphinxcontrib-spelling
 sphinx-autobuild==2024.4.16
     # via -r doc/requirements.in
 sphinx-code-tabs==0.5.5
     # via -r doc/requirements.in
+sphinx-lint==0.9.1
+    # via -r doc/requirements.in
 sphinx-rtd-theme==2.0.0
     # via -r doc/requirements.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
```

### Comparing `coverage-7.5.1/doc/sample_html/favicon_32_cb_58284776.png` & `coverage-7.5.2/doc/sample_html/favicon_32_cb_58284776.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/sample_html/keybd_closed_cb_ce680311.png` & `coverage-7.5.2/doc/sample_html/keybd_closed_cb_ce680311.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/sleepy.rst` & `coverage-7.5.2/doc/sleepy.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/source.rst` & `coverage-7.5.2/doc/source.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/subprocess.rst` & `coverage-7.5.2/doc/subprocess.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/trouble.rst` & `coverage-7.5.2/doc/trouble.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/doc/whatsnew5x.rst` & `coverage-7.5.2/doc/whatsnew5x.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/howto.txt` & `coverage-7.5.2/howto.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/igor.py` & `coverage-7.5.2/igor.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,15 @@
     # control over message verbosity...
     cov = coverage.Coverage(config_file="metacov.ini", messages=True)
     cov.load()
     show_contexts = bool(
         os.getenv("COVERAGE_DYNCTX") or os.getenv("COVERAGE_CONTEXT"),
     )
     cov.html_report(show_contexts=show_contexts)
+    cov.json_report(show_contexts=show_contexts, pretty_print=True)
 
 
 def do_test_with_core(core, *runner_args):
     """Run tests with a particular core."""
     # If we should skip these tests, skip them.
     skip_msg = should_skip(core)
     if skip_msg:
```

### Comparing `coverage-7.5.1/lab/benchmark/benchmark.py` & `coverage-7.5.2/lab/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/benchmark/empty.py` & `coverage-7.5.2/lab/benchmark/empty.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/benchmark/run.py` & `coverage-7.5.2/lab/benchmark/run.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/branches.py` & `coverage-7.5.2/lab/branches.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/compare_times.sh` & `coverage-7.5.2/lab/compare_times.sh`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/coverage-03.dtd` & `coverage-7.5.2/lab/coverage-03.dtd`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/coverage-04.dtd` & `coverage-7.5.2/lab/coverage-04.dtd`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/extract_code.py` & `coverage-7.5.2/lab/extract_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Licensed under the Apache License: http://www.apache.org/licenses/LICENSE-2.0
 # For details: https://github.com/nedbat/coveragepy/blob/master/NOTICE.txt
 
 """
 Use this to copy some indented code from the coverage.py test suite into a
 standalone file for deeper testing, or writing bug reports.
 
-Give it a file name and a line number, and it will find the indentend
-multiline string containing that line number, and output the dedented
+Give it a file name and a line number, and it will find the indented
+multi-line string containing that line number, and output the dedented
 contents of the string.
 
 If tests/test_arcs.py has this (partial) content::
 
     1630	    def test_partial_generators(self):
     1631	        # https://github.com/nedbat/coveragepy/issues/475
     1632	        # Line 2 is executed completely.
```

### Comparing `coverage-7.5.1/lab/find_class.py` & `coverage-7.5.2/lab/find_class.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/genpy.py` & `coverage-7.5.2/lab/genpy.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/goals.py` & `coverage-7.5.2/lab/goals.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/hack_pyc.py` & `coverage-7.5.2/lab/hack_pyc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/new-data.js` & `coverage-7.5.2/lab/new-data.js`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/notes/bug1303.txt` & `coverage-7.5.2/lab/notes/bug1303.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/notes/pypy-738-decorated-functions.txt` & `coverage-7.5.2/lab/notes/pypy-738-decorated-functions.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/parse_all.py` & `coverage-7.5.2/lab/parse_all.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/parser.py` & `coverage-7.5.2/lab/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,45 +76,51 @@
             pyparser.parse_source()
         except Exception as err:
             print(f"{err}")
             return
 
         if options.dis:
             print("Main code:")
-            disassemble(pyparser)
+            disassemble(pyparser.text)
 
         arcs = pyparser.arcs()
 
         if options.source or options.tokens:
             pyparser.show_tokens = options.tokens
             pyparser.parse_source()
 
             if options.source:
                 arc_chars = self.arc_ascii_art(arcs)
                 if arc_chars:
                     arc_width = max(len(a) for a in arc_chars.values())
 
                 exit_counts = pyparser.exit_counts()
 
-                for lineno, ltext in enumerate(pyparser.lines, start=1):
-                    marks = [' ', ' ', ' ', ' ', ' ']
+                for lineno, ltext in enumerate(pyparser.text.splitlines(), start=1):
+                    marks = [' '] * 6
                     a = ' '
                     if lineno in pyparser.raw_statements:
                         marks[0] = '-'
                     if lineno in pyparser.statements:
                         marks[1] = '='
                     exits = exit_counts.get(lineno, 0)
                     if exits > 1:
                         marks[2] = str(exits)
                     if lineno in pyparser.raw_docstrings:
                         marks[3] = '"'
                     if lineno in pyparser.raw_classdefs:
                         marks[3] = 'C'
                     if lineno in pyparser.raw_excluded:
-                        marks[4] = 'x'
+                        marks[4] = 'X'
+                    elif lineno in pyparser.excluded:
+                        marks[4] = '×'
+                    if lineno in pyparser._multiline.values():
+                        marks[5] = 'o'
+                    elif lineno in pyparser._multiline.keys():
+                        marks[5] = '.'
 
                     if arc_chars:
                         a = arc_chars[lineno].ljust(arc_width)
                     else:
                         a = ""
 
                     print("%4d %s%s %s" % (lineno, "".join(marks), a, ltext))
@@ -169,21 +175,21 @@
         # We're going to return the code object on the stack, but first
         # push its children for later returning.
         code = stack.pop()
         stack.extend(c for c in code.co_consts if isinstance(c, types.CodeType))
         yield code
 
 
-def disassemble(pyparser):
+def disassemble(text):
     """Disassemble code, for ad-hoc experimenting."""
 
-    code = compile(pyparser.text, "", "exec", dont_inherit=True)
+    code = compile(text, "", "exec", dont_inherit=True)
     for code_obj in all_code_objects(code):
-        if pyparser.text:
-            srclines = pyparser.text.splitlines()
+        if text:
+            srclines = text.splitlines()
         else:
             srclines = None
         print("\n%s: " % code_obj)
         upto = None
         for inst in dis.get_instructions(code_obj):
             if inst.starts_line is not None:
                 if srclines:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `coverage-7.5.1/lab/pick.py` & `coverage-7.5.2/lab/pick.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/platform_info.py` & `coverage-7.5.2/lab/platform_info.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/run_sysmon.py` & `coverage-7.5.2/lab/run_sysmon.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/run_trace.py` & `coverage-7.5.2/lab/run_trace.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/select_contexts.py` & `coverage-7.5.2/lab/select_contexts.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/lab/show_pyc.py` & `coverage-7.5.2/lab/show_pyc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/metacov.ini` & `coverage-7.5.2/metacov.ini`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/pyproject.toml` & `coverage-7.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/dev.in` & `coverage-7.5.2/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/dev.pip` & `coverage-7.5.2/requirements/dev.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/kit.pip` & `coverage-7.5.2/requirements/kit.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/light-threads.pip` & `coverage-7.5.2/requirements/light-threads.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/mypy.pip` & `coverage-7.5.2/requirements/mypy.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/pip-tools.pip` & `coverage-7.5.2/requirements/pip-tools.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/pytest.in` & `coverage-7.5.2/requirements/pytest.in`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/pytest.pip` & `coverage-7.5.2/requirements/pytest.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/requirements/tox.pip` & `coverage-7.5.2/requirements/tox.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/setup.py` & `coverage-7.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/balance_xdist_plugin.py` & `coverage-7.5.2/tests/balance_xdist_plugin.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/conftest.py` & `coverage-7.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/coveragetest.py` & `coverage-7.5.2/tests/coveragetest.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         else:
             return ""
 
     def check_coverage(
         self,
         text: str,
         lines: Sequence[TLineNo] | Sequence[list[TLineNo]] | None = None,
-        missing: str | Sequence[str] = "",
+        missing: str = "",
         report: str = "",
         excludes: Iterable[str] | None = None,
         partials: Iterable[str] = (),
         arcz: str | None = None,
         arcz_missing: str | None = None,
         arcz_unpredicted: str | None = None,
         arcs: Iterable[TArc] | None = None,
@@ -222,23 +222,16 @@
                 for line_list in lines:
                     if statements == line_list:
                         break
                 else:
                     assert False, f"None of the lines choices matched {statements!r}"
 
             missing_formatted = analysis.missing_formatted()
-            if isinstance(missing, str):
-                msg = f"missing: {missing_formatted!r} != {missing!r}"
-                assert missing_formatted == missing, msg
-            else:
-                for missing_list in missing:
-                    if missing_formatted == missing_list:
-                        break
-                else:
-                    assert False, f"None of the missing choices matched {missing_formatted!r}"
+            msg = f"missing: {missing_formatted!r} != {missing!r}"
+            assert missing_formatted == missing, msg
 
         if arcs is not None:
             # print("Possible arcs:")
             # print(" expected:", arcs)
             # print(" actual:", analysis.arc_possibilities)
             # print("Executed:")
             # print(" actual:", sorted(set(analysis.arcs_executed)))
```

### Comparing `coverage-7.5.1/tests/gold/README.rst` & `coverage-7.5.2/tests/gold/README.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/annotate/white/white.py,cover` & `coverage-7.5.2/tests/gold/annotate/white/white.py,cover`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/Makefile` & `coverage-7.5.2/tests/gold/html/Makefile`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/a/a_py.html` & `coverage-7.5.2/tests/gold/html/a/a_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/a/class_index.html` & `coverage-7.5.2/tests/gold/html/a/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/a/function_index.html` & `coverage-7.5.2/tests/gold/html/a/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/a/index.html` & `coverage-7.5.2/tests/gold/html/a/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/b_branch/b_py.html` & `coverage-7.5.2/tests/gold/html/b_branch/b_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/b_branch/class_index.html` & `coverage-7.5.2/tests/gold/html/b_branch/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/b_branch/function_index.html` & `coverage-7.5.2/tests/gold/html/b_branch/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/b_branch/index.html` & `coverage-7.5.2/tests/gold/html/b_branch/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/bom/bom_py.html` & `coverage-7.5.2/tests/gold/html/bom/bom_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/bom/class_index.html` & `coverage-7.5.2/tests/gold/html/bom/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/bom/function_index.html` & `coverage-7.5.2/tests/gold/html/bom/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/bom/index.html` & `coverage-7.5.2/tests/gold/html/bom/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/contexts/class_index.html` & `coverage-7.5.2/tests/gold/html/contexts/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/contexts/function_index.html` & `coverage-7.5.2/tests/gold/html/contexts/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/contexts/index.html` & `coverage-7.5.2/tests/gold/html/contexts/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/contexts/two_tests_py.html` & `coverage-7.5.2/tests/gold/html/contexts/two_tests_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/isolatin1/class_index.html` & `coverage-7.5.2/tests/gold/html/isolatin1/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/isolatin1/function_index.html` & `coverage-7.5.2/tests/gold/html/isolatin1/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/isolatin1/index.html` & `coverage-7.5.2/tests/gold/html/isolatin1/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/isolatin1/isolatin1_py.html` & `coverage-7.5.2/tests/gold/html/isolatin1/isolatin1_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_1/class_index.html` & `coverage-7.5.2/tests/gold/html/omit_1/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_1/function_index.html` & `coverage-7.5.2/tests/gold/html/omit_1/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_1/index.html` & `coverage-7.5.2/tests/gold/html/omit_1/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_1/m1_py.html` & `coverage-7.5.2/tests/gold/html/omit_1/m1_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_1/m2_py.html` & `coverage-7.5.2/tests/gold/html/omit_1/m2_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_1/m3_py.html` & `coverage-7.5.2/tests/gold/html/omit_1/m3_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_1/main_py.html` & `coverage-7.5.2/tests/gold/html/omit_1/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_2/class_index.html` & `coverage-7.5.2/tests/gold/html/omit_2/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_2/function_index.html` & `coverage-7.5.2/tests/gold/html/omit_2/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_2/index.html` & `coverage-7.5.2/tests/gold/html/omit_2/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_2/m2_py.html` & `coverage-7.5.2/tests/gold/html/omit_2/m2_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_2/m3_py.html` & `coverage-7.5.2/tests/gold/html/omit_2/m3_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_2/main_py.html` & `coverage-7.5.2/tests/gold/html/omit_2/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_3/class_index.html` & `coverage-7.5.2/tests/gold/html/omit_3/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_3/function_index.html` & `coverage-7.5.2/tests/gold/html/omit_3/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_3/index.html` & `coverage-7.5.2/tests/gold/html/omit_3/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_3/m3_py.html` & `coverage-7.5.2/tests/gold/html/omit_3/m3_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_3/main_py.html` & `coverage-7.5.2/tests/gold/html/omit_3/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_4/class_index.html` & `coverage-7.5.2/tests/gold/html/omit_4/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_4/function_index.html` & `coverage-7.5.2/tests/gold/html/omit_4/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_4/index.html` & `coverage-7.5.2/tests/gold/html/omit_4/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_4/m1_py.html` & `coverage-7.5.2/tests/gold/html/omit_4/m1_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_4/m3_py.html` & `coverage-7.5.2/tests/gold/html/omit_4/m3_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_4/main_py.html` & `coverage-7.5.2/tests/gold/html/omit_4/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_5/class_index.html` & `coverage-7.5.2/tests/gold/html/omit_5/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_5/function_index.html` & `coverage-7.5.2/tests/gold/html/omit_5/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_5/index.html` & `coverage-7.5.2/tests/gold/html/omit_5/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_5/m1_py.html` & `coverage-7.5.2/tests/gold/html/omit_5/m1_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/omit_5/main_py.html` & `coverage-7.5.2/tests/gold/html/omit_5/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/other/blah_blah_other_py.html` & `coverage-7.5.2/tests/gold/html/other/blah_blah_other_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/other/class_index.html` & `coverage-7.5.2/tests/gold/html/other/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/other/function_index.html` & `coverage-7.5.2/tests/gold/html/other/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/other/here_py.html` & `coverage-7.5.2/tests/gold/html/other/here_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/other/index.html` & `coverage-7.5.2/tests/gold/html/other/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/partial/class_index.html` & `coverage-7.5.2/tests/gold/html/partial/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/partial/function_index.html` & `coverage-7.5.2/tests/gold/html/partial/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/partial/index.html` & `coverage-7.5.2/tests/gold/html/partial/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/partial/partial_py.html` & `coverage-7.5.2/tests/gold/html/partial/partial_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/partial_626/class_index.html` & `coverage-7.5.2/tests/gold/html/partial_626/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/partial_626/function_index.html` & `coverage-7.5.2/tests/gold/html/partial_626/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/partial_626/index.html` & `coverage-7.5.2/tests/gold/html/partial_626/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/partial_626/partial_py.html` & `coverage-7.5.2/tests/gold/html/partial_626/partial_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/styled/a_py.html` & `coverage-7.5.2/tests/gold/html/styled/a_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/styled/class_index.html` & `coverage-7.5.2/tests/gold/html/styled/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/styled/function_index.html` & `coverage-7.5.2/tests/gold/html/styled/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/styled/index.html` & `coverage-7.5.2/tests/gold/html/styled/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/styled/style.css` & `coverage-7.5.2/tests/gold/html/styled/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/support/coverage_html.js` & `coverage-7.5.2/tests/gold/html/support/coverage_html.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -123,14 +123,24 @@
             }
         });
     });
 };
 
 // Create the events for the filter box.
 coverage.wire_up_filter = function() {
+    // Populate the filter and hide100 inputs if there are saved values for them.
+    const saved_filter_value = localStorage.getItem(coverage.FILTER_STORAGE);
+    if (saved_filter_value) {
+        document.getElementById("filter").value = saved_filter_value;
+    }
+    const saved_hide100_value = localStorage.getItem(coverage.HIDE100_STORAGE);
+    if (saved_hide100_value) {
+        document.getElementById("hide100").checked = JSON.parse(saved_hide100_value);
+    }
+
     // Cache elements.
     const table = document.querySelector("table.index");
     const table_body_rows = table.querySelectorAll("tbody tr");
     const no_rows = document.getElementById("no_rows");
 
     // Observe filter keyevents.
     const filter_handler = (event => {
@@ -139,16 +149,20 @@
         // Accumulate the percentage as fraction
         totals[totals.length - 1] = {
             "numer": 0,
             "denom": 0
         }; // nosemgrep: eslint.detect-object-injection
 
         var text = document.getElementById("filter").value;
+        // Store filter value
+        localStorage.setItem(coverage.FILTER_STORAGE, text);
         const casefold = (text === text.toLowerCase());
         const hide100 = document.getElementById("hide100").checked;
+        // Store hide value.
+        localStorage.setItem(coverage.HIDE100_STORAGE, JSON.stringify(hide100));
 
         // Hide / show elements.
         table_body_rows.forEach(row => {
             var show = false;
             // Check the text filter.
             for (let column = 0; column < totals.length; column++) {
                 cell = row.cells[column];
@@ -242,14 +256,16 @@
     document.getElementById("hide100").addEventListener("input", debounce(filter_handler));
 
     // Trigger change event on setup, to force filter on page refresh
     // (filter value may still be present).
     document.getElementById("filter").dispatchEvent(new Event("input"));
     document.getElementById("hide100").dispatchEvent(new Event("input"));
 };
+coverage.FILTER_STORAGE = "COVERAGE_FILTER_VALUE";
+coverage.HIDE100_STORAGE = "COVERAGE_HIDE100_VALUE";
 
 // Set up the click-to-sort columns.
 coverage.wire_up_sorting = function() {
     document.querySelectorAll("[data-sortable] th[aria-sort]").forEach(
         th => th.addEventListener("click", e => sortColumn(e.target))
     );
```

### Comparing `coverage-7.5.1/tests/gold/html/support/favicon_32.png` & `coverage-7.5.2/tests/gold/html/support/favicon_32.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/support/keybd_closed.png` & `coverage-7.5.2/tests/gold/html/support/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/support/style.css` & `coverage-7.5.2/tests/gold/html/support/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/unicode/class_index.html` & `coverage-7.5.2/tests/gold/html/unicode/class_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/unicode/function_index.html` & `coverage-7.5.2/tests/gold/html/unicode/function_index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/unicode/index.html` & `coverage-7.5.2/tests/gold/html/unicode/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/html/unicode/unicode_py.html` & `coverage-7.5.2/tests/gold/html/unicode/unicode_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/xml/x_xml/coverage.xml` & `coverage-7.5.2/tests/gold/xml/x_xml/coverage.xml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/gold/xml/y_xml_branch/coverage.xml` & `coverage-7.5.2/tests/gold/xml/y_xml_branch/coverage.xml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/goldtest.py` & `coverage-7.5.2/tests/goldtest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/helpers.py` & `coverage-7.5.2/tests/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from __future__ import annotations
 
 import collections
 import contextlib
 import dis
 import io
+import locale
 import os
 import os.path
 import re
 import shutil
 import subprocess
 import textwrap
 import warnings
@@ -24,15 +25,14 @@
 
 import flaky
 import pytest
 
 from coverage import env
 from coverage.debug import DebugControl
 from coverage.exceptions import CoverageWarning
-from coverage.misc import output_encoding
 from coverage.types import TArc, TLineNo
 
 
 def run_command(cmd: str) -> tuple[int, str]:
     """Run a command in a sub-process.
 
     Returns the exit status code and the combined stdout and stderr.
@@ -40,33 +40,35 @@
     """
     # Subprocesses are expensive, but convenient, and so may be over-used in
     # the test suite.  Use these lines to get a list of the tests using them:
     if 0:  # pragma: debugging
         with open("/tmp/processes.txt", "a") as proctxt:  # type: ignore[unreachable]
             print(os.getenv("PYTEST_CURRENT_TEST", "unknown"), file=proctxt, flush=True)
 
+    encoding = os.device_encoding(1) or locale.getpreferredencoding()
+
     # In some strange cases (PyPy3 in a virtualenv!?) the stdout encoding of
     # the subprocess is set incorrectly to ascii.  Use an environment variable
     # to force the encoding to be the same as ours.
     sub_env = dict(os.environ)
-    sub_env['PYTHONIOENCODING'] = output_encoding()
+    sub_env['PYTHONIOENCODING'] = encoding
 
     proc = subprocess.Popen(
         cmd,
         shell=True,
         env=sub_env,
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
     )
     output, _ = proc.communicate()
     status = proc.returncode
 
     # Get the output, and canonicalize it to strings with newlines.
-    output_str = output.decode(output_encoding()).replace("\r", "")
+    output_str = output.decode(encoding).replace("\r", "")
     return status, output_str
 
 
 # $set_env.py: COVERAGE_DIS - Disassemble test code to /tmp/dis
 SHOW_DIS = bool(int(os.getenv("COVERAGE_DIS", "0")))
 
 def make_file(
@@ -110,16 +112,19 @@
 
     if text and basename.endswith(".py") and SHOW_DIS:      # pragma: debugging
         os.makedirs("/tmp/dis", exist_ok=True)
         with open(f"/tmp/dis/{basename}.dis", "w") as fdis:
             print(f"# {os.path.abspath(filename)}", file=fdis)
             cur_test = os.getenv("PYTEST_CURRENT_TEST", "unknown")
             print(f"# PYTEST_CURRENT_TEST = {cur_test}", file=fdis)
+            kwargs = {}
+            if env.PYVERSION >= (3, 13):
+                kwargs["show_offsets"] = True
             try:
-                dis.dis(text, file=fdis)
+                dis.dis(text, file=fdis, **kwargs)
             except Exception as exc:
                 # Some tests make .py files that aren't Python, so dis will
                 # fail, which is expected.
                 print(f"#! {exc!r}", file=fdis)
 
     # For debugging, enable this to show the contents of files created.
     if 0:  # pragma: debugging
```

### Comparing `coverage-7.5.1/tests/js/index.html` & `coverage-7.5.2/tests/js/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/js/tests.js` & `coverage-7.5.2/tests/js/tests.js`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/mixins.py` & `coverage-7.5.2/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/modules/plugins/another.py` & `coverage-7.5.2/tests/modules/plugins/another.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/modules/process_test/try_execfile.py` & `coverage-7.5.2/tests/modules/process_test/try_execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/osinfo.py` & `coverage-7.5.2/tests/osinfo.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/plugin1.py` & `coverage-7.5.2/tests/plugin1.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/plugin2.py` & `coverage-7.5.2/tests/plugin2.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/plugin_config.py` & `coverage-7.5.2/tests/plugin_config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/qunit/jquery.tmpl.min.js` & `coverage-7.5.2/tests/qunit/jquery.tmpl.min.js`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/select_plugin.py` & `coverage-7.5.2/tests/select_plugin.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/stress_phystoken.tok` & `coverage-7.5.2/tests/stress_phystoken.tok`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/stress_phystoken_dos.tok` & `coverage-7.5.2/tests/stress_phystoken_dos.tok`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_annotate.py` & `coverage-7.5.2/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_api.py` & `coverage-7.5.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_arcs.py` & `coverage-7.5.2/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_cmdline.py` & `coverage-7.5.2/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_collector.py` & `coverage-7.5.2/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_concurrency.py` & `coverage-7.5.2/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_config.py` & `coverage-7.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_context.py` & `coverage-7.5.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_coverage.py` & `coverage-7.5.2/tests/test_coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,23 +37,14 @@
             a = 1
             if a == 2:
                 a = 3
             """,
             [1,2,3],
             missing="3",
         )
-        # You can specify a list of possible missing lines.
-        self.check_coverage("""\
-            a = 1
-            if a == 2:
-                a = 3
-            """,
-            [1,2,3],
-            missing=("47-49", "3", "100,102"),
-        )
 
     def test_failed_coverage(self) -> None:
         # If the lines are wrong, the message shows right and wrong.
         with pytest.raises(AssertionError, match=r"\[1, 2] != \[1]"):
             self.check_coverage("""\
                 a = 1
                 b = 2
@@ -75,25 +66,14 @@
                 a = 1
                 if a == 2:
                     a = 3
                 """,
                 [1,2,3],
                 missing="37",
             )
-        # If the missing lines possibilities are wrong, the msg shows right.
-        msg = r"None of the missing choices matched '3'"
-        with pytest.raises(AssertionError, match=msg):
-            self.check_coverage("""\
-                a = 1
-                if a == 2:
-                    a = 3
-                """,
-                [1,2,3],
-                missing=("37", "4-10"),
-            )
 
     def test_exceptions_really_fail(self) -> None:
         # An assert in the checked code will really raise up to us.
         with pytest.raises(AssertionError, match="This is bad"):
             self.check_coverage("""\
                 a = 1
                 assert a == 99, "This is bad"
@@ -498,14 +478,15 @@
                 a = 4
             assert a == 11
             """,
             lines=lines, missing=missing,
         )
 
     def test_strange_unexecuted_continue(self) -> None:
+        # This used to be true, but no longer is:
         # Peephole optimization of jumps to jumps can mean that some statements
         # never hit the line tracer.  The behavior is different in different
         # versions of Python, so be careful when running this test.
         self.check_coverage("""\
             a = b = c = 0
             for n in range(100):
                 if n % 2:
@@ -525,15 +506,15 @@
                     continue    # <-- This line is always hit.
                 else:
                     b += 1
                 c += 1
             assert a == 33 and b == 50 and c == 50
             """,
             lines=[1,2,3,4,5,6,8,9,10, 12,13,14,15,16,17,19,20,21],
-            missing=["", "6"],
+            missing="",
         )
 
     def test_import(self) -> None:
         self.check_coverage("""\
             import string
             from sys import path
             a = 1
@@ -678,22 +659,21 @@
         self.check_coverage("""\
             '''I am a module docstring.'''
             a = 2
             b = 3
             """,
             [2, 3],
         )
-        lines = [2, 3, 4]
         self.check_coverage("""\
-            # Start with a comment, because it changes the behavior(!?)
+            # Start with a comment, even though it doesn't change the behavior.
             '''I am a module docstring.'''
             a = 3
             b = 4
             """,
-            lines,
+            [3, 4],
         )
 
 
 class CompoundStatementTest(CoverageTest):
     """Testing coverage of multi-line compound statements."""
 
     def test_statement_list(self) -> None:
```

### Comparing `coverage-7.5.1/tests/test_data.py` & `coverage-7.5.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_debug.py` & `coverage-7.5.2/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_execfile.py` & `coverage-7.5.2/tests/test_execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_filereporter.py` & `coverage-7.5.2/tests/test_filereporter.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_files.py` & `coverage-7.5.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_goldtest.py` & `coverage-7.5.2/tests/test_goldtest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_html.py` & `coverage-7.5.2/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_json.py` & `coverage-7.5.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_lcov.py` & `coverage-7.5.2/tests/test_lcov.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_misc.py` & `coverage-7.5.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_mixins.py` & `coverage-7.5.2/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_numbits.py` & `coverage-7.5.2/tests/test_numbits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_oddball.py` & `coverage-7.5.2/tests/test_oddball.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_parser.py` & `coverage-7.5.2/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,38 +120,31 @@
                     a = 3
                 else:   # nocover
                     a = 5
             b = 6
             """)
         assert parser.exit_counts() == { 1:1, 2:1, 3:1, 6:1 }
 
-    def test_indentation_error(self) -> None:
-        msg = (
-            "Couldn't parse '<code>' as Python source: " +
-            "'unindent does not match any outer indentation level.*' at line 3"
-        )
-        with pytest.raises(NotPython, match=msg):
-            _ = self.parse_text("""\
-                0 spaces
-                  2
-                 1
-                """)
-
-    def test_token_error(self) -> None:
-        submsgs = [
-            r"EOF in multi-line string",                                        # before 3.12.0b1
-            r"unterminated triple-quoted string literal .detected at line 1.",  # after 3.12.0b1
-        ]
-        msg = (
-            r"Couldn't parse '<code>' as Python source: '"
-            + r"(" + "|".join(submsgs) + ")"
-            + r"' at line 1"
-        )
+    @pytest.mark.parametrize("text", [
+        pytest.param("0 spaces\n  2\n 1", id="bad_indent"),
+        pytest.param("'''", id="string_eof"),
+        pytest.param("$hello", id="dollar"),
+        # on 3.10 this passes ast.parse but fails on tokenize.generate_tokens
+        pytest.param(
+            "\r'\\\n'''",
+            id="leading_newline_eof",
+            marks=[
+                pytest.mark.skipif(env.PYVERSION >= (3, 12), reason="parses fine in 3.12"),
+            ]
+        )
+    ])
+    def test_not_python(self, text: str) -> None:
+        msg = r"Couldn't parse '<code>' as Python source: '.*' at line \d+"
         with pytest.raises(NotPython, match=msg):
-            _ = self.parse_text("'''")
+            _ = self.parse_text(text)
 
     def test_empty_decorated_function(self) -> None:
         parser = self.parse_text("""\
             def decorator(func):
                 return func
 
             @decorator
@@ -176,14 +169,28 @@
             expected_arcs.update(set(arcz_to_arcs("54 98")))
             expected_exits.update({9: 2, 5: 2})
 
         assert expected_statements == parser.statements
         assert expected_arcs == parser.arcs()
         assert expected_exits == parser.exit_counts()
 
+    def test_module_docstrings(self) -> None:
+        parser = self.parse_text("""\
+            '''The docstring on line 1'''
+            a = 2
+            """)
+        assert {2} == parser.statements
+
+        parser = self.parse_text("""\
+            # Docstring is not line 1
+            '''The docstring on line 2'''
+            a = 3
+            """)
+        assert {3} == parser.statements
+
     def test_fuzzed_double_parse(self) -> None:
         # https://bugs.chromium.org/p/oss-fuzz/issues/detail?id=50381
         # The second parse used to raise `TypeError: 'NoneType' object is not iterable`
         msg = (
             r"(EOF in multi-line statement)"        # before 3.12.0b1
             + r"|(unmatched ']')"                   # after 3.12.0b1
         )
@@ -736,28 +743,48 @@
             def g():
                 x = 9
             """)
         raw_statements = {1, 2, 3, 4, 6, 7, 8, 9}
         assert parser.raw_statements == raw_statements
         assert parser.statements == set()
 
+    @pytest.mark.xfail(
+        env.PYPY and env.PYVERSION[:2] == (3, 8),
+        reason="AST doesn't mark end of classes correctly",
+    )
     def test_class_decorator_pragmas(self) -> None:
         parser = self.parse_text("""\
             class Foo(object):
                 def __init__(self):
                     self.x = 3
 
             @foo                        # nocover
             class Bar(object):
                 def __init__(self):
                     self.x = 8
             """)
         assert parser.raw_statements == {1, 2, 3, 5, 6, 7, 8}
         assert parser.statements == {1, 2, 3}
 
+    def test_over_exclusion_bug1779(self) -> None:
+        # https://github.com/nedbat/coveragepy/issues/1779
+        parser = self.parse_text("""\
+            import abc
+
+            class MyProtocol:               # nocover 3
+                @abc.abstractmethod         # nocover 4
+                def my_method(self) -> int:
+                    ...     # 6
+
+            def function() -> int:
+                return 9
+            """)
+        assert parser.raw_statements == {1, 3, 4, 5, 6, 8, 9}
+        assert parser.statements == {1, 8, 9}
+
 
 class ParserMissingArcDescriptionTest(PythonParserTestBase):
     """Tests for PythonParser.missing_arc_description."""
 
     def test_missing_arc_description(self) -> None:
         # This code is never run, so the actual values don't matter.
         parser = self.parse_text("""\
```

### Comparing `coverage-7.5.1/tests/test_phystokens.py` & `coverage-7.5.2/tests/test_phystokens.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_plugins.py` & `coverage-7.5.2/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_process.py` & `coverage-7.5.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_python.py` & `coverage-7.5.2/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_regions.py` & `coverage-7.5.2/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_report.py` & `coverage-7.5.2/tests/test_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,14 +664,42 @@
         # TOTAL                3      3   0.000000%
 
         assert self.line_count(report) == 6, report
         assert "empty.py             0      0 100.000000%" in report
         assert "not_covered.py       3      3   0.000000%" in report
         assert "TOTAL                3      3   0.000000%" in report
 
+    def test_report_module_docstrings(self) -> None:
+        self.make_file("main.py", """\
+            # Line 1
+            '''Line 2 docstring.'''
+            import other
+            a = 4
+            """)
+        self.make_file("other.py", """\
+            '''Line 1'''
+            a = 2
+            """)
+        cov = coverage.Coverage()
+        self.start_import_stop(cov, "main")
+        report = self.get_report(cov)
+
+        # Name       Stmts   Miss  Cover
+        # ------------------------------
+        # main.py        2      0   100%
+        # other.py       1      0   100%
+        # ------------------------------
+        # TOTAL          3      0   100%
+
+        assert self.line_count(report) == 6, report
+        squeezed = self.squeezed_lines(report)
+        assert squeezed[2] == "main.py 2 0 100%"
+        assert squeezed[3] == "other.py 1 0 100%"
+        assert squeezed[5] == "TOTAL 3 0 100%"
+
     def test_dotpy_not_python(self) -> None:
         # We run a .py file, and when reporting, we can't parse it as Python.
         # We should get an error message in the report.
 
         self.make_data_file(lines={"mycode.py": [1]})
         self.make_file("mycode.py", "This isn't python at all!")
         cov = coverage.Coverage()
```

### Comparing `coverage-7.5.1/tests/test_report_common.py` & `coverage-7.5.2/tests/test_report_common.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_report_core.py` & `coverage-7.5.2/tests/test_report_core.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_results.py` & `coverage-7.5.2/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_setup.py` & `coverage-7.5.2/tests/test_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 from __future__ import annotations
 
 import sys
 
 from typing import List, cast
 
+import pytest
+
 import coverage
+from coverage import env
 
 from tests.coveragetest import CoverageTest
 
 
 class SetupPyTest(CoverageTest):
     """Tests of setup.py"""
 
@@ -31,14 +34,18 @@
         assert status == 0
         out = output.splitlines()
         assert "measurement" in out[0]
         assert coverage.__version__ == out[1]
         assert "github.com/nedbat/coveragepy" in out[2]
         assert "Ned Batchelder" in out[3]
 
+    @pytest.mark.skipif(
+        env.PYVERSION[3:5] == ("alpha", 0),
+        reason="don't expect classifiers until labelled builds",
+    )
     def test_more_metadata(self) -> None:
         # Let's be sure we pick up our own setup.py
         # CoverageTest restores the original sys.path for us.
         sys.path.insert(0, '')
         from setup import setup_args
 
         classifiers = cast(List[str], setup_args['classifiers'])
```

### Comparing `coverage-7.5.1/tests/test_sqlitedb.py` & `coverage-7.5.2/tests/test_sqlitedb.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_templite.py` & `coverage-7.5.2/tests/test_templite.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_testing.py` & `coverage-7.5.2/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_venv.py` & `coverage-7.5.2/tests/test_venv.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_version.py` & `coverage-7.5.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/test_xml.py` & `coverage-7.5.2/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tests/testenv.py` & `coverage-7.5.2/tests/testenv.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.1/tox.ini` & `coverage-7.5.2/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     python igor.py zip_mods
 
     # Build the C extension and test with the CTracer
     python setup.py --quiet build_ext --inplace
     python -m pip install {env:COVERAGE_PIP_ARGS} -q -e .
     python igor.py test_with_core ctrace {posargs}
 
-    py3{12,13},anypy: python igor.py test_with_core sysmon {posargs}
+    py3{12,13,14},anypy: python igor.py test_with_core sysmon {posargs}
 
     # Remove the C extension so that we can test the PyTracer
     python igor.py remove_extension
 
     # Test with the PyTracer
     python igor.py test_with_core pytrace {posargs}
 
@@ -72,14 +72,15 @@
     -r doc/requirements.pip
 allowlist_externals =
     make
 commands =
     # If this command fails, see the comment at the top of doc/cmd.rst
     python -m cogapp -cP --check --verbosity=1 doc/*.rst
     doc8 -q --ignore-path 'doc/_*' doc CHANGES.rst README.rst
+    sphinx-lint doc CHANGES.rst README.rst
     sphinx-build -b html -aEnqW doc doc/_build/html
     rst2html.py --strict README.rst doc/_build/trash
     - sphinx-build -b html -b linkcheck -aEnq doc doc/_build/html
     - sphinx-build -b html -b linkcheck -aEnQW doc doc/_build/html
 
 [testenv:lint]
 # Minimum of PYVERSIONS
@@ -92,15 +93,15 @@
     LINTABLE=coverage tests doc ci igor.py setup.py __main__.py
 
 commands =
     python -m tabnanny {env:LINTABLE}
     # If this command fails, see the comment at the top of doc/cmd.rst
     python -m cogapp -cP --check --verbosity=1 doc/*.rst
     python -m cogapp -cP --check --verbosity=1 .github/workflows/*.yml
-    python -m pylint --notes= --ignore-paths 'doc/_build/.*' {env:LINTABLE}
+    python -m pylint -j 0 --notes= --ignore-paths 'doc/_build/.*' {env:LINTABLE}
     check-manifest --ignore 'doc/sample_html/*,.treerc'
     # If 'build -q' becomes a thing (https://github.com/pypa/build/issues/188),
     # this can be simplified:
     python igor.py quietly "python -m build"
     twine check dist/*
 
 [testenv:mypy]
@@ -124,8 +125,9 @@
 python =
     3.8 = py38
     3.9 = py39
     3.10 = py310
     3.11 = py311
     3.12 = py312
     3.13 = py313
+    3.14 = py314
     pypy-3 = pypy3
```

