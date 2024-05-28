# Comparing `tmp/adeploy-1.0.0.tar.gz` & `tmp/adeploy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adeploy-1.0.0.tar", last modified: Tue Feb 27 00:11:26 2024, max compression
+gzip compressed data, was "adeploy-1.1.0.tar", last modified: Tue May 28 08:10:29 2024, max compression
```

## Comparing `adeploy-1.0.0.tar` & `adeploy-1.1.0.tar`

### file list

```diff
@@ -1,396 +1,396 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1274 2024-02-26 14:18:48.000000 adeploy-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3162 2024-02-27 00:05:28.000000 adeploy-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2321 2024-02-26 16:37:25.000000 adeploy-1.0.0/DEVELOP.md
--rw-rw-rw-   0 root         (0) root         (0)     1543 2023-12-08 14:22:49.000000 adeploy-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3776 2024-02-27 00:11:26.779227 adeploy-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2589 2024-02-26 16:37:25.000000 adeploy-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.751226 adeploy-1.0.0/adeploy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-27 00:11:20.000000 adeploy-1.0.0/adeploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.755226 adeploy-1.0.0/adeploy/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-27 00:11:20.000000 adeploy-1.0.0/adeploy/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5604 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/args.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     3671 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3756 2024-02-08 16:32:20.000000 adeploy-1.0.0/adeploy/common/gopass.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2024-02-26 15:21:25.000000 adeploy-1.0.0/adeploy/common/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.755226 adeploy-1.0.0/adeploy/common/jinja/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-27 00:11:20.000000 adeploy-1.0.0/adeploy/common/jinja/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/jinja/dict.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2024-02-26 14:18:48.000000 adeploy-1.0.0/adeploy/common/jinja/env.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2024-02-26 23:57:43.000000 adeploy-1.0.0/adeploy/common/jinja/filters.py
--rw-rw-rw-   0 root         (0) root         (0)    22662 2024-02-26 14:18:48.000000 adeploy-1.0.0/adeploy/common/jinja/globals.py
--rw-rw-rw-   0 root         (0) root         (0)     7699 2023-12-08 14:42:13.000000 adeploy-1.0.0/adeploy/common/kubectl.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7959 2024-02-26 14:18:48.000000 adeploy-1.0.0/adeploy/common/provider.py
--rw-rw-rw-   0 root         (0) root         (0)    15231 2024-02-26 14:18:48.000000 adeploy-1.0.0/adeploy/common/secret.py
--rw-rw-rw-   0 root         (0) root         (0)      988 2024-02-26 14:18:48.000000 adeploy-1.0.0/adeploy/common/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.755226 adeploy-1.0.0/adeploy/common/yaml/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/yaml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/yaml/find.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/yaml/labels.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/yaml/probes.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/yaml/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/common/yaml/update.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2024-02-26 14:18:48.000000 adeploy-1.0.0/adeploy/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.755226 adeploy-1.0.0/adeploy/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-27 00:11:20.000000 adeploy-1.0.0/adeploy/providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.755226 adeploy-1.0.0/adeploy/providers/helm/
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/helm/README.md
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/helm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.755226 adeploy-1.0.0/adeploy/providers/helm/common/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/helm/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3065 2024-02-26 14:58:18.000000 adeploy-1.0.0/adeploy/providers/helm/common/helm.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/helm/common/helm_output.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/helm/common/helm_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/helm/deployer.py
--rw-rw-rw-   0 root         (0) root         (0)     7448 2024-02-26 14:58:18.000000 adeploy-1.0.0/adeploy/providers/helm/renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     7093 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/helm/tester.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/helm/watcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.759226 adeploy-1.0.0/adeploy/providers/jinja/
--rw-rw-rw-   0 root         (0) root         (0)    10768 2024-02-08 16:32:20.000000 adeploy-1.0.0/adeploy/providers/jinja/README.md
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/jinja/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/jinja/deployer.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2024-01-03 16:14:38.000000 adeploy-1.0.0/adeploy/providers/jinja/renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     2216 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/jinja/tester.py
--rw-rw-rw-   0 root         (0) root         (0)     8370 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/providers/jinja/watcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.759226 adeploy-1.0.0/adeploy/steps/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/steps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2168 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/steps/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/steps/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)     2768 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/steps/render.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/steps/test.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-12-08 14:22:49.000000 adeploy-1.0.0/adeploy/steps/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/adeploy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3776 2024-02-27 00:11:26.000000 adeploy-1.0.0/adeploy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11992 2024-02-27 00:11:26.000000 adeploy-1.0.0/adeploy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 00:11:26.000000 adeploy-1.0.0/adeploy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-02-27 00:11:26.000000 adeploy-1.0.0/adeploy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-02-27 00:11:26.000000 adeploy-1.0.0/adeploy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-02-27 00:11:26.000000 adeploy-1.0.0/adeploy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.759226 adeploy-1.0.0/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.759226 adeploy-1.0.0/docs/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.759226 adeploy-1.0.0/docs/assets/css/
--rw-rw-rw-   0 root         (0) root         (0)    39561 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/assets/css/asciinema-player.css
--rw-rw-rw-   0 root         (0) root         (0)      333 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/assets/css/badges.css
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/assets/css/docstrings.css
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-02-26 22:31:48.000000 adeploy-1.0.0/docs/assets/css/footer.css
--rwxrwxrwx   0 root         (0) root         (0)      331 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/assets/download.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.759226 adeploy-1.0.0/docs/assets/img/
--rw-rw-rw-   0 root         (0) root         (0)    12255 2024-02-26 16:37:25.000000 adeploy-1.0.0/docs/assets/img/awesome-logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.759226 adeploy-1.0.0/docs/assets/js/
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/assets/js/asciinema-init.js
--rw-rw-rw-   0 root         (0) root         (0)   158918 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/assets/js/asciinema-player.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/docs/common/
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/_more.md
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/filters.md
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/functions.md
--rw-rw-rw-   0 root         (0) root         (0)     4585 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/includes.md
--rw-rw-rw-   0 root         (0) root         (0)     1028 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/index.md
--rw-rw-rw-   0 root         (0) root         (0)     2573 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/labels.md
--rw-rw-rw-   0 root         (0) root         (0)     1272 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/macros.md
--rw-rw-rw-   0 root         (0) root         (0)     2049 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/probes.md
--rw-rw-rw-   0 root         (0) root         (0)     2017 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/resource-limits.md
--rw-rw-rw-   0 root         (0) root         (0)     8627 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/common/secrets.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/docs/helm/
--rw-rw-rw-   0 root         (0) root         (0)     3559 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/helm/helm-deploy.cast
--rw-rw-rw-   0 root         (0) root         (0)     1759 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/helm/helm-render.cast
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/helm/helm-test.cast
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/helm/hooks.md
--rw-rw-rw-   0 root         (0) root         (0)     4727 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/helm/index.md
--rw-rw-rw-   0 root         (0) root         (0)    11676 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/helm.cast
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/docs/hooks/
--rw-rw-rw-   0 root         (0) root         (0)     1450 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/hooks/asciinema.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/hooks/badges.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-02-26 16:37:25.000000 adeploy-1.0.0/docs/index.md
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 16:37:25.000000 adeploy-1.0.0/docs/install.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/docs/jinja/
--rw-rw-rw-   0 root         (0) root         (0)     3994 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/jinja/index.md
--rw-rw-rw-   0 root         (0) root         (0)     2603 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/jinja/jinja-deploy.cast
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/jinja/jinja-render.cast
--rw-rw-rw-   0 root         (0) root         (0)     2393 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/jinja/jinja-test.cast
--rw-rw-rw-   0 root         (0) root         (0)    34470 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/jinja.cast
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/docs/overrides/partials/
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-02-26 23:51:51.000000 adeploy-1.0.0/docs/overrides/partials/copyright.html
--rw-rw-rw-   0 root         (0) root         (0)     8821 2024-02-26 14:18:48.000000 adeploy-1.0.0/docs/usage.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/examples/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-02-26 15:24:59.000000 adeploy-1.0.0/examples/.exclude-from-test
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/examples/helm/001-quickstart/
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/helm/001-quickstart/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/001-quickstart/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/.helmignore
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/Chart.yaml
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/NOTES.txt
--rw-rw-rw-   0 root         (0) root         (0)     1822 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/_helpers.tpl
--rw-rw-rw-   0 root         (0) root         (0)      988 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/deployment.yaml
--rw-rw-rw-   0 root         (0) root         (0)      373 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/service.yaml
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/serviceaccount.yaml
--rw-rw-rw-   0 root         (0) root         (0)      640 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/values.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/playground/hello-world/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/playground/hello-world/test/
--rw-rw-rw-   0 root         (0) root         (0)     1885 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/playground/hello-world/test/manifest.yml
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/001-quickstart/build/helm/playground/hello-world/test/values.yml
--rw-rw-rw-   0 root         (0) root         (0)      761 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/helm/001-quickstart/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/001-quickstart/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/examples/helm/001-quickstart/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)      653 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/helm/001-quickstart/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.763226 adeploy-1.0.0/examples/helm/002-hooks/
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/helm/002-hooks/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/002-hooks/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/002-hooks/build/helm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/.helmignore
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/Chart.yaml
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/NOTES.txt
--rw-rw-rw-   0 root         (0) root         (0)     1822 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/_helpers.tpl
--rw-rw-rw-   0 root         (0) root         (0)     1060 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/deployment.yaml
--rw-rw-rw-   0 root         (0) root         (0)      373 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/service.yaml
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/serviceaccount.yaml
--rw-rw-rw-   0 root         (0) root         (0)      640 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/values.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/002-hooks/build/helm/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/002-hooks/build/helm/playground/hello-world/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/helm/002-hooks/build/helm/playground/hello-world/test/
--rw-rw-rw-   0 root         (0) root         (0)     1957 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/playground/hello-world/test/manifest.yml
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/helm/002-hooks/build/helm/playground/hello-world/test/values.yml
--rw-rw-rw-   0 root         (0) root         (0)      761 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/helm/002-hooks/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/helm/002-hooks/hooks/
--rwxrwxrwx   0 root         (0) root         (0)       98 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/helm/002-hooks/hooks/patch.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/helm/002-hooks/hooks/patches.d/
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/helm/002-hooks/hooks/patches.d/001-add-env.patch
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.739226 adeploy-1.0.0/examples/helm/002-hooks/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/helm/002-hooks/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)      653 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/helm/002-hooks/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/jinja/001-general-structure/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/001-general-structure/.exclude-from-test
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/001-general-structure/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/001-general-structure/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/
--rw-rw-rw-   0 root         (0) root         (0)     1363 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/job.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/
--rw-rw-rw-   0 root         (0) root         (0)     1316 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/job.yml
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/001-general-structure/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/001-general-structure/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/jinja/001-general-structure/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/001-general-structure/namespaces/playground/prod.yml
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/001-general-structure/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/jinja/001-general-structure/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1403 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/001-general-structure/templates/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/001-general-structure/templates/job.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/jinja/002-secrets/
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/secret-7e33ba97416ba4d45b6ce4c6c68b6aace36eacc5
--rw-rw-rw-   0 root         (0) root         (0)      689 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/secret-e5e0c551a537d65bcea7c18eb47badaf9c09c349
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/secret-7929a442fae0ceee9eef9558a9a2ef02cc9d4421
--rw-rw-rw-   0 root         (0) root         (0)      689 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/secret-f310a9ad786b3fb5f7160436346e69795693b951
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/prod/
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/prod/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/test/
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/test/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)      466 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/002-secrets/namespaces/playground/prod.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets/namespaces/playground/secrets/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets/namespaces/playground/secrets/my_secret_prod
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets/namespaces/playground/secrets/my_secret_test
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1666 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/002-secrets/templates/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.767227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/
--rw-rw-rw-   0 root         (0) root         (0)     1110 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-6e1adb2c4c075e35335e851dd6ebc5f0f7397a80
--rw-rw-rw-   0 root         (0) root         (0)     1111 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-7e33ba97416ba4d45b6ce4c6c68b6aace36eacc5
--rw-rw-rw-   0 root         (0) root         (0)     1044 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-e5e0c551a537d65bcea7c18eb47badaf9c09c349
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/
--rw-rw-rw-   0 root         (0) root         (0)     1116 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-7929a442fae0ceee9eef9558a9a2ef02cc9d4421
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-dcf2a6e7bd78ee395f73f6434b19a9044790c00a
--rw-rw-rw-   0 root         (0) root         (0)     1049 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-f310a9ad786b3fb5f7160436346e69795693b951
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/
--rw-rw-rw-   0 root         (0) root         (0)     1574 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/ingress.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/
--rw-rw-rw-   0 root         (0) root         (0)     1574 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/ingress.yml
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/prod.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/mydomain.com.crt
--rw-rw-rw-   0 root         (0) root         (0)     1679 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/mydomain.com.key
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/mydomain.com.crt
--rw-rw-rw-   0 root         (0) root         (0)     1679 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/mydomain.com.key
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/my_secret_prod
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/my_secret_test
--rw-rw-rw-   0 root         (0) root         (0)      997 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/002-secrets-ingress/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/templates/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/002-secrets-ingress/templates/ingress.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/003-include/
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-01-03 16:14:38.000000 adeploy-1.0.0/examples/jinja/003-include/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/003-include/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/003-include/build/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/common/
--rw-rw-rw-   0 root         (0) root         (0)     1233 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/common/configmap.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     2085 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.771227 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/redis/
--rw-rw-rw-   0 root         (0) root         (0)     2164 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/redis/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.743226 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/common/
--rw-rw-rw-   0 root         (0) root         (0)     1233 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/common/configmap.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     2085 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/redis/
--rw-rw-rw-   0 root         (0) root         (0)     2164 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/redis/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-01-03 16:14:38.000000 adeploy-1.0.0/examples/jinja/003-include/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/003-include/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-01-03 16:14:38.000000 adeploy-1.0.0/examples/jinja/003-include/namespaces/playground/prod.yml
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-01-03 16:14:38.000000 adeploy-1.0.0/examples/jinja/003-include/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/003-include/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/templates/common/
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/003-include/templates/common/__affinity.yml
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-01-03 16:14:38.000000 adeploy-1.0.0/examples/jinja/003-include/templates/common/__env.yml
--rw-rw-rw-   0 root         (0) root         (0)      439 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/003-include/templates/common/configmap.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/templates/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/templates/files/conf.d/
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-01-03 16:14:38.000000 adeploy-1.0.0/examples/jinja/003-include/templates/files/conf.d/alpha.json
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-01-03 16:14:38.000000 adeploy-1.0.0/examples/jinja/003-include/templates/files/conf.d/beta.json
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-01-03 16:14:38.000000 adeploy-1.0.0/examples/jinja/003-include/templates/files/nginx.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/templates/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     1523 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/003-include/templates/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/003-include/templates/redis/
--rw-rw-rw-   0 root         (0) root         (0)     1619 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/003-include/templates/redis/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/004-probes/
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/004-probes/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/004-probes/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     1729 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/redis/
--rw-rw-rw-   0 root         (0) root         (0)     1506 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/redis/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     1729 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/redis/
--rw-rw-rw-   0 root         (0) root         (0)     1506 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/redis/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/004-probes/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/004-probes/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/004-probes/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/004-probes/namespaces/playground/prod.yml
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/004-probes/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/004-probes/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/004-probes/templates/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/004-probes/templates/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/004-probes/templates/redis/
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/004-probes/templates/redis/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/005-labels/
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/005-labels/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/005-labels/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/005-labels/build/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/005-labels/build/jinja/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/005-labels/build/jinja/playground/005-labels/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/005-labels/build/jinja/playground/005-labels/prod/
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/005-labels/build/jinja/playground/005-labels/prod/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/005-labels/build/jinja/playground/005-labels/test/
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/005-labels/build/jinja/playground/005-labels/test/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/005-labels/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/005-labels/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/005-labels/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/005-labels/namespaces/playground/prod.yml
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-12-08 14:22:49.000000 adeploy-1.0.0/examples/jinja/005-labels/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/005-labels/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/005-labels/templates/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.775227 adeploy-1.0.0/examples/jinja/006-nested-labels/
--rw-rw-rw-   0 root         (0) root         (0)      794 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/006-nested-labels/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/006-nested-labels/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/prod/
--rw-rw-rw-   0 root         (0) root         (0)     1650 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/prod/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/test/
--rw-rw-rw-   0 root         (0) root         (0)     1650 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/test/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/006-nested-labels/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/006-nested-labels/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/006-nested-labels/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/006-nested-labels/namespaces/playground/prod.yml
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/006-nested-labels/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/006-nested-labels/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1205 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/006-nested-labels/templates/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/007-resources/
--rw-rw-rw-   0 root         (0) root         (0)      947 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/007-resources/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/007-resources/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/redis/
--rw-rw-rw-   0 root         (0) root         (0)     1251 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/redis/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/redis/
--rw-rw-rw-   0 root         (0) root         (0)     1251 2024-02-27 00:10:58.000000 adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/redis/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/007-resources/defaults.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.747226 adeploy-1.0.0/examples/jinja/007-resources/namespaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/007-resources/namespaces/playground/
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/007-resources/namespaces/playground/prod.yml
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/007-resources/namespaces/playground/test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.751226 adeploy-1.0.0/examples/jinja/007-resources/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/007-resources/templates/nginx/
--rw-rw-rw-   0 root         (0) root         (0)     1214 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/007-resources/templates/nginx/deployment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 00:11:26.779227 adeploy-1.0.0/examples/jinja/007-resources/templates/redis/
--rw-rw-rw-   0 root         (0) root         (0)     1210 2024-02-26 14:18:48.000000 adeploy-1.0.0/examples/jinja/007-resources/templates/redis/deployment.yml
--rw-rw-rw-   0 root         (0) root         (0)     2009 2024-02-26 16:37:25.000000 adeploy-1.0.0/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     1572 2024-02-27 00:10:04.000000 adeploy-1.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-02-09 15:02:42.000000 adeploy-1.0.0/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      192 2023-12-08 14:22:49.000000 adeploy-1.0.0/runner.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 00:11:26.779227 adeploy-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-02-26 14:18:48.000000 adeploy-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.664312 adeploy-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-02-26 14:18:48.000000 adeploy-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2024-02-27 00:05:28.000000 adeploy-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2024-02-26 16:37:25.000000 adeploy-1.1.0/DEVELOP.md
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2023-12-08 14:22:49.000000 adeploy-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3776 2024-05-28 08:10:29.664312 adeploy-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2024-02-26 16:37:25.000000 adeploy-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/adeploy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 08:10:26.000000 adeploy-1.1.0/adeploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.644312 adeploy-1.1.0/adeploy/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 08:10:26.000000 adeploy-1.1.0/adeploy/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5604 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/args.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3756 2024-02-08 16:32:20.000000 adeploy-1.1.0/adeploy/common/gopass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2024-02-26 15:21:25.000000 adeploy-1.1.0/adeploy/common/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.644312 adeploy-1.1.0/adeploy/common/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 08:10:26.000000 adeploy-1.1.0/adeploy/common/jinja/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/jinja/dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2024-02-26 14:18:48.000000 adeploy-1.1.0/adeploy/common/jinja/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     3677 2024-02-26 23:57:43.000000 adeploy-1.1.0/adeploy/common/jinja/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    22670 2024-04-26 11:57:19.000000 adeploy-1.1.0/adeploy/common/jinja/globals.py
+-rw-rw-rw-   0 root         (0) root         (0)     7699 2023-12-08 14:42:13.000000 adeploy-1.1.0/adeploy/common/kubectl.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7959 2024-02-26 14:18:48.000000 adeploy-1.1.0/adeploy/common/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    15231 2024-02-26 14:18:48.000000 adeploy-1.1.0/adeploy/common/secret.py
+-rw-rw-rw-   0 root         (0) root         (0)      988 2024-02-26 14:18:48.000000 adeploy-1.1.0/adeploy/common/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.644312 adeploy-1.1.0/adeploy/common/yaml/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/yaml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/yaml/find.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/yaml/labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/yaml/probes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/common/yaml/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-04-26 10:39:35.000000 adeploy-1.1.0/adeploy/common/yaml/update.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2024-02-26 14:18:48.000000 adeploy-1.1.0/adeploy/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.644312 adeploy-1.1.0/adeploy/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 08:10:26.000000 adeploy-1.1.0/adeploy/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.644312 adeploy-1.1.0/adeploy/providers/helm/
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/helm/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/helm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.644312 adeploy-1.1.0/adeploy/providers/helm/common/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/helm/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3065 2024-02-26 14:58:18.000000 adeploy-1.1.0/adeploy/providers/helm/common/helm.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/helm/common/helm_output.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/helm/common/helm_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/helm/deployer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7448 2024-02-26 14:58:18.000000 adeploy-1.1.0/adeploy/providers/helm/renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7093 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/helm/tester.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/helm/watcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.644312 adeploy-1.1.0/adeploy/providers/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)    10768 2024-02-08 16:32:20.000000 adeploy-1.1.0/adeploy/providers/jinja/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/jinja/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2496 2024-04-26 08:39:29.000000 adeploy-1.1.0/adeploy/providers/jinja/deployer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6221 2024-05-28 07:27:36.000000 adeploy-1.1.0/adeploy/providers/jinja/renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2216 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/jinja/tester.py
+-rw-rw-rw-   0 root         (0) root         (0)     8370 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/providers/jinja/watcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/adeploy/steps/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/steps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2168 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/steps/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/steps/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2768 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/steps/render.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/steps/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-12-08 14:22:49.000000 adeploy-1.1.0/adeploy/steps/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.664312 adeploy-1.1.0/adeploy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3776 2024-05-28 08:10:29.000000 adeploy-1.1.0/adeploy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11992 2024-05-28 08:10:29.000000 adeploy-1.1.0/adeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 08:10:29.000000 adeploy-1.1.0/adeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 08:10:29.000000 adeploy-1.1.0/adeploy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-28 08:10:29.000000 adeploy-1.1.0/adeploy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 08:10:29.000000 adeploy-1.1.0/adeploy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/assets/css/
+-rw-rw-rw-   0 root         (0) root         (0)    39561 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/assets/css/asciinema-player.css
+-rw-rw-rw-   0 root         (0) root         (0)      333 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/assets/css/badges.css
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/assets/css/docstrings.css
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-02-26 22:31:48.000000 adeploy-1.1.0/docs/assets/css/footer.css
+-rwxrwxrwx   0 root         (0) root         (0)      331 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/assets/download.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/assets/img/
+-rw-rw-rw-   0 root         (0) root         (0)    12255 2024-02-26 16:37:25.000000 adeploy-1.1.0/docs/assets/img/awesome-logo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/assets/js/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/assets/js/asciinema-init.js
+-rw-rw-rw-   0 root         (0) root         (0)   158918 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/assets/js/asciinema-player.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/common/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/_more.md
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/filters.md
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/functions.md
+-rw-rw-rw-   0 root         (0) root         (0)     4585 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/includes.md
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/index.md
+-rw-rw-rw-   0 root         (0) root         (0)     2573 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/labels.md
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/macros.md
+-rw-rw-rw-   0 root         (0) root         (0)     2049 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/probes.md
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/resource-limits.md
+-rw-rw-rw-   0 root         (0) root         (0)     8627 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/common/secrets.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/helm/
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/helm/helm-deploy.cast
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/helm/helm-render.cast
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/helm/helm-test.cast
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/helm/hooks.md
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/helm/index.md
+-rw-rw-rw-   0 root         (0) root         (0)    11676 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/helm.cast
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/hooks/asciinema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/hooks/badges.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-02-26 16:37:25.000000 adeploy-1.1.0/docs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 16:37:25.000000 adeploy-1.1.0/docs/install.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)     3994 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/jinja/index.md
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/jinja/jinja-deploy.cast
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/jinja/jinja-render.cast
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/jinja/jinja-test.cast
+-rw-rw-rw-   0 root         (0) root         (0)    34470 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/jinja.cast
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/docs/overrides/partials/
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-02-26 23:51:51.000000 adeploy-1.1.0/docs/overrides/partials/copyright.html
+-rw-rw-rw-   0 root         (0) root         (0)     8821 2024-02-26 14:18:48.000000 adeploy-1.1.0/docs/usage.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.648312 adeploy-1.1.0/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-02-26 15:24:59.000000 adeploy-1.1.0/examples/.exclude-from-test
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/001-quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/helm/001-quickstart/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/001-quickstart/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/.helmignore
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/Chart.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/NOTES.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/_helpers.tpl
+-rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/deployment.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      373 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/service.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/serviceaccount.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      640 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/values.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/playground/hello-world/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/playground/hello-world/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/playground/hello-world/test/manifest.yml
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/001-quickstart/build/helm/playground/hello-world/test/values.yml
+-rw-rw-rw-   0 root         (0) root         (0)      761 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/helm/001-quickstart/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/001-quickstart/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/001-quickstart/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/helm/001-quickstart/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/002-hooks/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/helm/002-hooks/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/002-hooks/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/002-hooks/build/helm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/.helmignore
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/Chart.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/NOTES.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/_helpers.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/deployment.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      373 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/service.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/serviceaccount.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      640 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/values.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/002-hooks/build/helm/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/002-hooks/build/helm/playground/hello-world/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/002-hooks/build/helm/playground/hello-world/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/playground/hello-world/test/manifest.yml
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/helm/002-hooks/build/helm/playground/hello-world/test/values.yml
+-rw-rw-rw-   0 root         (0) root         (0)      761 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/helm/002-hooks/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/002-hooks/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)       98 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/helm/002-hooks/hooks/patch.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/002-hooks/hooks/patches.d/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/helm/002-hooks/hooks/patches.d/001-add-env.patch
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/helm/002-hooks/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/helm/002-hooks/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/helm/002-hooks/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/jinja/001-general-structure/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/001-general-structure/.exclude-from-test
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/001-general-structure/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/jinja/001-general-structure/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/job.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/job.yml
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/001-general-structure/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.632311 adeploy-1.1.0/examples/jinja/001-general-structure/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/jinja/001-general-structure/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/001-general-structure/namespaces/playground/prod.yml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/001-general-structure/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/jinja/001-general-structure/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/001-general-structure/templates/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/001-general-structure/templates/job.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.652312 adeploy-1.1.0/examples/jinja/002-secrets/
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/secret-7e33ba97416ba4d45b6ce4c6c68b6aace36eacc5
+-rw-rw-rw-   0 root         (0) root         (0)      689 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/secret-e5e0c551a537d65bcea7c18eb47badaf9c09c349
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/secret-7929a442fae0ceee9eef9558a9a2ef02cc9d4421
+-rw-rw-rw-   0 root         (0) root         (0)      689 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/secret-f310a9ad786b3fb5f7160436346e69795693b951
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/prod/
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/prod/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/test/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)      466 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/002-secrets/namespaces/playground/prod.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets/namespaces/playground/secrets/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets/namespaces/playground/secrets/my_secret_prod
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets/namespaces/playground/secrets/my_secret_test
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/002-secrets/templates/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-6e1adb2c4c075e35335e851dd6ebc5f0f7397a80
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-7e33ba97416ba4d45b6ce4c6c68b6aace36eacc5
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-e5e0c551a537d65bcea7c18eb47badaf9c09c349
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-7929a442fae0ceee9eef9558a9a2ef02cc9d4421
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-dcf2a6e7bd78ee395f73f6434b19a9044790c00a
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-f310a9ad786b3fb5f7160436346e69795693b951
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/ingress.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/ingress.yml
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/prod.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/mydomain.com.crt
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/mydomain.com.key
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/mydomain.com.crt
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/mydomain.com.key
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/my_secret_prod
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/my_secret_test
+-rw-rw-rw-   0 root         (0) root         (0)      997 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/002-secrets-ingress/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/templates/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/002-secrets-ingress/templates/ingress.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/003-include/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-01-03 16:14:38.000000 adeploy-1.1.0/examples/jinja/003-include/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/003-include/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/common/
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/common/configmap.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     2164 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/redis/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/common/
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/common/configmap.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.656312 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     2164 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/redis/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-01-03 16:14:38.000000 adeploy-1.1.0/examples/jinja/003-include/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/003-include/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/003-include/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-01-03 16:14:38.000000 adeploy-1.1.0/examples/jinja/003-include/namespaces/playground/prod.yml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-01-03 16:14:38.000000 adeploy-1.1.0/examples/jinja/003-include/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/003-include/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/003-include/templates/common/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/003-include/templates/common/__affinity.yml
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-01-03 16:14:38.000000 adeploy-1.1.0/examples/jinja/003-include/templates/common/__env.yml
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/003-include/templates/common/configmap.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/003-include/templates/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/003-include/templates/files/conf.d/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-01-03 16:14:38.000000 adeploy-1.1.0/examples/jinja/003-include/templates/files/conf.d/alpha.json
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-01-03 16:14:38.000000 adeploy-1.1.0/examples/jinja/003-include/templates/files/conf.d/beta.json
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-01-03 16:14:38.000000 adeploy-1.1.0/examples/jinja/003-include/templates/files/nginx.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/003-include/templates/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/003-include/templates/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/003-include/templates/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/003-include/templates/redis/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/004-probes/
+-rw-rw-rw-   0 root         (0) root         (0)      971 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/004-probes/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/004-probes/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/redis/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/redis/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/004-probes/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/004-probes/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/004-probes/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/004-probes/namespaces/playground/prod.yml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/004-probes/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/004-probes/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/004-probes/templates/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/004-probes/templates/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/004-probes/templates/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/004-probes/templates/redis/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/005-labels/
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/005-labels/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.636312 adeploy-1.1.0/examples/jinja/005-labels/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/005-labels/build/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/005-labels/build/jinja/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/005-labels/build/jinja/playground/005-labels/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/005-labels/build/jinja/playground/005-labels/prod/
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/005-labels/build/jinja/playground/005-labels/prod/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/005-labels/build/jinja/playground/005-labels/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/005-labels/build/jinja/playground/005-labels/test/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/005-labels/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/005-labels/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/005-labels/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/005-labels/namespaces/playground/prod.yml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-12-08 14:22:49.000000 adeploy-1.1.0/examples/jinja/005-labels/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/005-labels/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/005-labels/templates/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/006-nested-labels/
+-rw-rw-rw-   0 root         (0) root         (0)      794 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/006-nested-labels/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/006-nested-labels/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/prod/
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/prod/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/test/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/006-nested-labels/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/006-nested-labels/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/006-nested-labels/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/006-nested-labels/namespaces/playground/prod.yml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/006-nested-labels/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/006-nested-labels/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/006-nested-labels/templates/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/007-resources/
+-rw-rw-rw-   0 root         (0) root         (0)      947 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/007-resources/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/007-resources/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/redis/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2024-05-28 07:57:42.000000 adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/redis/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/007-resources/defaults.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/007-resources/namespaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.660312 adeploy-1.1.0/examples/jinja/007-resources/namespaces/playground/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/007-resources/namespaces/playground/prod.yml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/007-resources/namespaces/playground/test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.640312 adeploy-1.1.0/examples/jinja/007-resources/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.664312 adeploy-1.1.0/examples/jinja/007-resources/templates/nginx/
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/007-resources/templates/nginx/deployment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:10:29.664312 adeploy-1.1.0/examples/jinja/007-resources/templates/redis/
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2024-02-26 14:18:48.000000 adeploy-1.1.0/examples/jinja/007-resources/templates/redis/deployment.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2009 2024-02-26 16:37:25.000000 adeploy-1.1.0/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2024-02-27 00:10:04.000000 adeploy-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-02-09 15:02:42.000000 adeploy-1.1.0/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      192 2023-12-08 14:22:49.000000 adeploy-1.1.0/runner.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 08:10:29.664312 adeploy-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-02-26 14:18:48.000000 adeploy-1.1.0/setup.py
```

### Comparing `adeploy-1.0.0/.gitignore` & `adeploy-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/.gitlab-ci.yml` & `adeploy-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/DEVELOP.md` & `adeploy-1.1.0/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/LICENSE` & `adeploy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/PKG-INFO` & `adeploy-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adeploy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Universal deployment tool for Kubernetes that supports rendering and deployment of lightweight Jinja templated k8s manifests as well as complex Helm charts.
 Author: awesome IT
 Author-email: Daniel Morlock <daniel.morlock@awesome-it.de>, Daniel Bross <daniel.bross@awesome-it.de>, Robin Lutz <robin.lutz@awesome-it.de>, Adrian Vielsack <adrian.vielsack@awesome-it.de>, Philip Flohr <philip.flohr@awesome-it.de>
 Project-URL: Homepage, https://awesome-it.de
 Project-URL: Source, https://github.com/awesome-it/adeploy
 Project-URL: Issues, https://github.com/awesome-it/adeploy/issues
 Project-URL: Documentation, https://awesome-it.de/docs/adeploy/latest
```

### Comparing `adeploy-1.0.0/README.md` & `adeploy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/args.py` & `adeploy-1.1.0/adeploy/common/args.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/colors.py` & `adeploy-1.1.0/adeploy/common/colors.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/deployment.py` & `adeploy-1.1.0/adeploy/common/deployment.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/errors.py` & `adeploy-1.1.0/adeploy/common/errors.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/gopass.py` & `adeploy-1.1.0/adeploy/common/gopass.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/helpers.py` & `adeploy-1.1.0/adeploy/common/helpers.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/jinja/dict.py` & `adeploy-1.1.0/adeploy/common/jinja/dict.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/jinja/env.py` & `adeploy-1.1.0/adeploy/common/jinja/env.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/jinja/filters.py` & `adeploy-1.1.0/adeploy/common/jinja/filters.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/jinja/globals.py` & `adeploy-1.1.0/adeploy/common/jinja/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         Returns:
             dict: A dict with filename as key and the formatted content as value.
 
         !!!example "Example: Include all files form `files/conf.d` into a config map"
             --8<-- "docs/common/includes.md:example"
         """
         contents = {}
-        for item in pathlib.Path(pathlib.Path(self.templates_dir) / dir).iterdir():
+        for item in sorted(pathlib.Path(pathlib.Path(self.templates_dir) / dir).iterdir()):
             if item.is_file():
                 self.env.loader.searchpath.append(str(item.parent))
                 contents[item.name] = self.include_file(
                     str(item.relative_to(self.templates_dir)), direct, render, indent, skip, escape)
 
         return contents
```

### Comparing `adeploy-1.0.0/adeploy/common/kubectl.py` & `adeploy-1.1.0/adeploy/common/kubectl.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/logging.py` & `adeploy-1.1.0/adeploy/common/logging.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/provider.py` & `adeploy-1.1.0/adeploy/common/provider.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/secret.py` & `adeploy-1.1.0/adeploy/common/secret.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/version.py` & `adeploy-1.1.0/adeploy/common/version.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/yaml/labels.py` & `adeploy-1.1.0/adeploy/common/yaml/labels.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/yaml/probes.py` & `adeploy-1.1.0/adeploy/common/yaml/probes.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/common/yaml/resources.py` & `adeploy-1.1.0/adeploy/common/yaml/resources.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/main.py` & `adeploy-1.1.0/adeploy/main.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/helm/README.md` & `adeploy-1.1.0/adeploy/providers/helm/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/helm/common/helm.py` & `adeploy-1.1.0/adeploy/providers/helm/common/helm.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/helm/common/helm_output.py` & `adeploy-1.1.0/adeploy/providers/helm/common/helm_output.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/helm/deployer.py` & `adeploy-1.1.0/adeploy/providers/helm/deployer.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/helm/renderer.py` & `adeploy-1.1.0/adeploy/providers/helm/renderer.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/helm/tester.py` & `adeploy-1.1.0/adeploy/providers/helm/tester.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/jinja/README.md` & `adeploy-1.1.0/adeploy/providers/jinja/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/jinja/renderer.py` & `adeploy-1.1.0/adeploy/providers/jinja/renderer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import glob
 import json
 import os
 from logging import Logger
 from pathlib import Path
 
 import jinja2
+from ruamel.yaml import YAML
+from ruamel.yaml.error import MarkedYAMLError
 
 from adeploy.common import colors
+from adeploy.common.deployment import Deployment
 from adeploy.common.errors import RenderError
 from adeploy.common.jinja import env as jinja_env
 from adeploy.common.provider import Provider
 from adeploy.common.yaml import update
 
 
 class Renderer(Provider):
@@ -35,18 +38,25 @@
                  namespaces_dir: str or Path, args: argparse.Namespace, log: Logger, **kwargs):
         super().__init__(name, src_dir, build_dir, namespaces_dir, args, log, **kwargs)
         if not os.path.isabs(templates_dir):
             self.templates_dir = f'{self.src_dir}/{templates_dir}'
 
         if self.templates_dir[-1] == '/':
             self.templates_dir = self.templates_dir[:-1]
-        self.jinja_pathes = ['.', '..', self.templates_dir, str(Path(self.templates_dir).parent), str(Path(self.templates_dir).parent.parent)]
+        self.jinja_pathes = ['.', '..', self.templates_dir, str(Path(self.templates_dir).parent),
+                             str(Path(self.templates_dir).parent.parent)]
         self.log.debug(f'Using Jinja file system loader with pathes: {", ".join(self.jinja_pathes)}')
         self.env = jinja_env.create(self.jinja_pathes, log=self.log, templates_dir=self.templates_dir)
 
+        yaml = YAML(typ='rt')
+        yaml.default_flow_style = False
+        yaml.preserve_quotes = True
+        yaml.sort_keys = False
+        self.yaml = yaml
+
     def parse_args(self, args):
         self.templates_dir = args.get('templates_dir')
         self.macros_dirs = args.get('macros_dirs')
 
     def load_templates(self, extensions=None):
 
         if extensions is None:
@@ -72,40 +82,56 @@
     def get_template_output_path(self, deployment, template):
         return Path(self.build_dir) \
             .joinpath(deployment.namespace) \
             .joinpath(self.name) \
             .joinpath(deployment.release) \
             .joinpath(template)
 
-    def render_template(self, deployment, template, prefix='...'):
+    def render_template(self, deployment: Deployment, template_path: str, prefix: str = '...'):
         jinja_env.register_globals(self.env, deployment, self.log, self.templates_dir)
         values = deployment.get_template_values()
-        output_path = self.get_template_output_path(deployment, template)
-        self.log.info(f'{prefix} render "{colors.bold(template)}" in "{colors.bold(output_path)}" ...')
-
         try:
-            data = self.env.get_template(template).render(**values)
-            if len(data.replace('---', '').replace('\n', '').strip()) > 0:
-                data = update(self.log, data, deployment)
-                output_path.parent.mkdir(parents=True, exist_ok=True)
-                with open(output_path, 'w') as fd:
-                    fd.write(data)
-
+            rendered_template = self.env.get_template(template_path).render(**values)
         except jinja2.exceptions.TemplateNotFound as e:
             self.log.debug(f'Used Jinja variables: {json.dumps(values)}')
-            raise RenderError(f'Jinja template error: Template "{e}" not found in "{template}"')
+            raise RenderError(f'Jinja template error: Template "{e}" not found in "{template_path}"')
 
         except jinja2.exceptions.TemplateSyntaxError as e:
             self.log.debug(f'Used Jinja variables: {json.dumps(values)}')
             raise RenderError(
                 f'Jinja template syntax error in "{colors.bold(e.filename)}", line {colors.bold(e.lineno)}: {e}')
 
         except jinja2.exceptions.TemplateError as e:
             self.log.debug(f'Used Jinja variables: {json.dumps(values)}')
-            raise RenderError(f'Jinja template error in "{colors.bold(template)}": {e}')
+            raise RenderError(f'Jinja template error in "{colors.bold(template_path)}": {e}')
+
+        try:
+            output_path = self.get_template_output_path(deployment, template_path)
+            output_path.parent.mkdir(parents=True, exist_ok=True)
+            documents = self.yaml.load_all(rendered_template)
+
+            documents = [d for d in documents if d is not None]
+            if len(documents) == 0:
+                self.log.warning(f'{prefix} {colors.bold(template_path)} is empty ...')
+
+            for index, doc in enumerate(documents):
+                doc = update(self.log, doc, deployment)
+
+                object_kind = doc.get('kind', None)
+                object_name = doc.get('metadata', {}).get('name', None)
+                object_output_path = output_path.with_suffix(f'.{index}.yml') if len(documents) > 1 else output_path
+
+                with open(object_output_path, 'w') as fd:
+                    self.log.info(f'{prefix} render {colors.bold(object_kind)} "{colors.bold(object_name)}" '
+                                  f'from "{colors.bold(template_path)}" '
+                                  f'in "{colors.bold(object_output_path)}" ...')
+                    self.yaml.dump(doc, fd)
+
+        except MarkedYAMLError as e:
+            raise RenderError(f'YAML error in "{colors.bold(template_path)}": {e}')
 
     def run(self):
         self.log.debug(f'Working on deployment "{self.name}" ...')
         self.clean_build_dir()
         template_dir, templates = self.load_templates()
         for deployment in self.load_deployments():
             self.log.info(f'Rendering deployment "{colors.blue(deployment)}" ...')
```

### Comparing `adeploy-1.0.0/adeploy/providers/jinja/tester.py` & `adeploy-1.1.0/adeploy/providers/jinja/tester.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/providers/jinja/watcher.py` & `adeploy-1.1.0/adeploy/providers/jinja/watcher.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/steps/config.py` & `adeploy-1.1.0/adeploy/steps/config.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/steps/deploy.py` & `adeploy-1.1.0/adeploy/steps/deploy.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/steps/render.py` & `adeploy-1.1.0/adeploy/steps/render.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/steps/test.py` & `adeploy-1.1.0/adeploy/steps/test.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy/steps/watch.py` & `adeploy-1.1.0/adeploy/steps/watch.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/adeploy.egg-info/PKG-INFO` & `adeploy-1.1.0/adeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adeploy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Universal deployment tool for Kubernetes that supports rendering and deployment of lightweight Jinja templated k8s manifests as well as complex Helm charts.
 Author: awesome IT
 Author-email: Daniel Morlock <daniel.morlock@awesome-it.de>, Daniel Bross <daniel.bross@awesome-it.de>, Robin Lutz <robin.lutz@awesome-it.de>, Adrian Vielsack <adrian.vielsack@awesome-it.de>, Philip Flohr <philip.flohr@awesome-it.de>
 Project-URL: Homepage, https://awesome-it.de
 Project-URL: Source, https://github.com/awesome-it/adeploy
 Project-URL: Issues, https://github.com/awesome-it/adeploy/issues
 Project-URL: Documentation, https://awesome-it.de/docs/adeploy/latest
```

### Comparing `adeploy-1.0.0/adeploy.egg-info/SOURCES.txt` & `adeploy-1.1.0/adeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/assets/css/asciinema-player.css` & `adeploy-1.1.0/docs/assets/css/asciinema-player.css`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/assets/img/awesome-logo.png` & `adeploy-1.1.0/docs/assets/img/awesome-logo.png`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/assets/js/asciinema-player.min.js` & `adeploy-1.1.0/docs/assets/js/asciinema-player.min.js`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/common/includes.md` & `adeploy-1.1.0/docs/common/includes.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/common/index.md` & `adeploy-1.1.0/docs/common/index.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/common/labels.md` & `adeploy-1.1.0/docs/common/labels.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/common/macros.md` & `adeploy-1.1.0/docs/common/macros.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/common/probes.md` & `adeploy-1.1.0/docs/common/probes.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/common/resource-limits.md` & `adeploy-1.1.0/docs/common/resource-limits.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/common/secrets.md` & `adeploy-1.1.0/docs/common/secrets.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/helm/helm-deploy.cast` & `adeploy-1.1.0/docs/helm/helm-deploy.cast`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/helm/helm-render.cast` & `adeploy-1.1.0/docs/helm/helm-render.cast`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/helm/helm-test.cast` & `adeploy-1.1.0/docs/helm/helm-test.cast`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/helm/hooks.md` & `adeploy-1.1.0/docs/helm/hooks.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/helm/index.md` & `adeploy-1.1.0/docs/helm/index.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/helm.cast` & `adeploy-1.1.0/docs/helm.cast`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/hooks/asciinema.py` & `adeploy-1.1.0/docs/hooks/asciinema.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/hooks/badges.py` & `adeploy-1.1.0/docs/hooks/badges.py`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/jinja/index.md` & `adeploy-1.1.0/docs/jinja/index.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/jinja/jinja-deploy.cast` & `adeploy-1.1.0/docs/jinja/jinja-deploy.cast`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/jinja/jinja-render.cast` & `adeploy-1.1.0/docs/jinja/jinja-render.cast`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/jinja/jinja-test.cast` & `adeploy-1.1.0/docs/jinja/jinja-test.cast`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/jinja.cast` & `adeploy-1.1.0/docs/jinja.cast`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/overrides/partials/copyright.html` & `adeploy-1.1.0/docs/overrides/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/docs/usage.md` & `adeploy-1.1.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/001-quickstart/README.md` & `adeploy-1.1.0/examples/helm/001-quickstart/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/NOTES.txt` & `adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/_helpers.tpl` & `adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/deployment.yaml` & `adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/001-quickstart/build/helm/charts/hello-world/values.yaml` & `adeploy-1.1.0/examples/helm/001-quickstart/build/helm/charts/hello-world/values.yaml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/001-quickstart/build/helm/playground/hello-world/test/manifest.yml` & `adeploy-1.1.0/examples/helm/001-quickstart/build/helm/playground/hello-world/test/manifest.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/001-quickstart/defaults.yml` & `adeploy-1.1.0/examples/helm/001-quickstart/defaults.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/001-quickstart/namespaces/playground/test.yml` & `adeploy-1.1.0/examples/helm/001-quickstart/namespaces/playground/test.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/002-hooks/README.md` & `adeploy-1.1.0/examples/helm/002-hooks/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/NOTES.txt` & `adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/_helpers.tpl` & `adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/deployment.yaml` & `adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/002-hooks/build/helm/charts/hello-world/values.yaml` & `adeploy-1.1.0/examples/helm/002-hooks/build/helm/charts/hello-world/values.yaml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/002-hooks/build/helm/playground/hello-world/test/manifest.yml` & `adeploy-1.1.0/examples/helm/002-hooks/build/helm/playground/hello-world/test/manifest.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/002-hooks/defaults.yml` & `adeploy-1.1.0/examples/helm/002-hooks/defaults.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/helm/002-hooks/namespaces/playground/test.yml` & `adeploy-1.1.0/examples/helm/002-hooks/namespaces/playground/test.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/001-general-structure/README.md` & `adeploy-1.1.0/examples/jinja/001-general-structure/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/deployment.yml` & `adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/job.yml` & `adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/prod/job.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/deployment.yml` & `adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/job.yml` & `adeploy-1.1.0/examples/jinja/001-general-structure/build/jinja/playground/001-general-structure/test/job.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/001-general-structure/templates/deployment.yml` & `adeploy-1.1.0/examples/jinja/001-general-structure/templates/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/001-general-structure/templates/job.yml` & `adeploy-1.1.0/examples/jinja/001-general-structure/templates/job.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets/README.md` & `adeploy-1.1.0/examples/jinja/002-secrets/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/secret-7e33ba97416ba4d45b6ce4c6c68b6aace36eacc5` & `adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/secret-7e33ba97416ba4d45b6ce4c6c68b6aace36eacc5`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/secret-e5e0c551a537d65bcea7c18eb47badaf9c09c349` & `adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/prod/secret-e5e0c551a537d65bcea7c18eb47badaf9c09c349`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/secret-7929a442fae0ceee9eef9558a9a2ef02cc9d4421` & `adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/secret-7929a442fae0ceee9eef9558a9a2ef02cc9d4421`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/secret-f310a9ad786b3fb5f7160436346e69795693b951` & `adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/002-secrets/secrets/playground/test/secret-f310a9ad786b3fb5f7160436346e69795693b951`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/prod/deployment.yml` & `adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/prod/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/test/deployment.yml` & `adeploy-1.1.0/examples/jinja/002-secrets/build/jinja/playground/002-secrets/test/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets/templates/deployment.yml` & `adeploy-1.1.0/examples/jinja/002-secrets/templates/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/README.md` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-6e1adb2c4c075e35335e851dd6ebc5f0f7397a80` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-6e1adb2c4c075e35335e851dd6ebc5f0f7397a80`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-7e33ba97416ba4d45b6ce4c6c68b6aace36eacc5` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-7e33ba97416ba4d45b6ce4c6c68b6aace36eacc5`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-e5e0c551a537d65bcea7c18eb47badaf9c09c349` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/prod/secret-e5e0c551a537d65bcea7c18eb47badaf9c09c349`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-7929a442fae0ceee9eef9558a9a2ef02cc9d4421` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-7929a442fae0ceee9eef9558a9a2ef02cc9d4421`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-dcf2a6e7bd78ee395f73f6434b19a9044790c00a` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-dcf2a6e7bd78ee395f73f6434b19a9044790c00a`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-f310a9ad786b3fb5f7160436346e69795693b951` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/002-secrets-ingress/secrets/playground/test/secret-f310a9ad786b3fb5f7160436346e69795693b951`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/deployment.yml` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/ingress.yml` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/prod/ingress.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
----
 kind: Ingress
 apiVersion: networking.k8s.io/v1
 metadata:
   name: 002-secrets-ingress-prod-ingress
   namespace: playground
   annotations:
     nginx.ingress.kubernetes.io/proxy-send-timeout: "300"
```

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/deployment.yml` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/ingress.yml` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/build/jinja/playground/002-secrets-ingress/test/ingress.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
----
 kind: Ingress
 apiVersion: networking.k8s.io/v1
 metadata:
   name: 002-secrets-ingress-test-ingress
   namespace: playground
   annotations:
     nginx.ingress.kubernetes.io/proxy-send-timeout: "300"
```

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/prod.yml` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/prod.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/mydomain.com.crt` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/mydomain.com.crt`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/mydomain.com.key` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_prod/mydomain.com.key`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/mydomain.com.crt` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/mydomain.com.crt`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/mydomain.com.key` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/secrets/domain_test/mydomain.com.key`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/namespaces/playground/test.yml` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/namespaces/playground/test.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/templates/deployment.yml` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/templates/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/002-secrets-ingress/templates/ingress.yml` & `adeploy-1.1.0/examples/jinja/002-secrets-ingress/templates/ingress.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/003-include/README.md` & `adeploy-1.1.0/examples/jinja/003-include/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/common/configmap.yml` & `adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/common/configmap.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 apiVersion: v1
 kind: ConfigMap
 metadata:
-  name: 003-include-prod-config
+  name: 003-include-test-config
   namespace: playground
   labels:
     app.kubernetes.io/part-of: 003-include
-    app.kubernetes.io/instance: prod
+    app.kubernetes.io/instance: test
     app.kubernetes.io/component: config
 data:
   nginx.conf: |
     user  nginx;
     worker_processes  auto;
 
     error_log  /var/log/nginx/error.log notice;
@@ -43,12 +43,12 @@
 
   alpha.json: |
     {
         "name": "Alpha",
         "content": "This is a config file to include in configmap.yml"
     }
 
-  beta.json: |-
+  beta.json: |
     {
         "name": "Beta",
         "content": "This is a another config file to include in configmap.yml"
     }
```

### Comparing `adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/common/configmap.yml` & `adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/prod/common/configmap.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 apiVersion: v1
 kind: ConfigMap
 metadata:
-  name: 003-include-test-config
+  name: 003-include-prod-config
   namespace: playground
   labels:
     app.kubernetes.io/part-of: 003-include
-    app.kubernetes.io/instance: test
+    app.kubernetes.io/instance: prod
     app.kubernetes.io/component: config
 data:
   nginx.conf: |
     user  nginx;
     worker_processes  auto;
 
     error_log  /var/log/nginx/error.log notice;
@@ -43,12 +43,12 @@
 
   alpha.json: |
     {
         "name": "Alpha",
         "content": "This is a config file to include in configmap.yml"
     }
 
-  beta.json: |-
+  beta.json: |
     {
         "name": "Beta",
         "content": "This is a another config file to include in configmap.yml"
     }
```

### Comparing `adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/003-include/build/jinja/playground/003-include/test/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/003-include/build/jinja/playground/003-include/test/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/003-include/templates/files/nginx.conf` & `adeploy-1.1.0/examples/jinja/003-include/templates/files/nginx.conf`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/003-include/templates/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/003-include/templates/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/003-include/templates/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/003-include/templates/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/004-probes/README.md` & `adeploy-1.1.0/examples/jinja/004-probes/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/prod/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/004-probes/build/jinja/playground/004-probes/test/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/004-probes/defaults.yml` & `adeploy-1.1.0/examples/jinja/004-probes/defaults.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/004-probes/templates/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/004-probes/templates/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/004-probes/templates/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/004-probes/templates/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/005-labels/README.md` & `adeploy-1.1.0/examples/jinja/005-labels/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/005-labels/build/jinja/playground/005-labels/prod/deployment.yml` & `adeploy-1.1.0/examples/jinja/005-labels/build/jinja/playground/005-labels/prod/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/005-labels/build/jinja/playground/005-labels/test/deployment.yml` & `adeploy-1.1.0/examples/jinja/005-labels/build/jinja/playground/005-labels/test/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/005-labels/defaults.yml` & `adeploy-1.1.0/examples/jinja/005-labels/defaults.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/005-labels/templates/deployment.yml` & `adeploy-1.1.0/examples/jinja/005-labels/templates/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/006-nested-labels/README.md` & `adeploy-1.1.0/examples/jinja/006-nested-labels/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/prod/deployment.yml` & `adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/prod/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/test/deployment.yml` & `adeploy-1.1.0/examples/jinja/006-nested-labels/build/jinja/playground/006-nested-labels/test/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/006-nested-labels/templates/deployment.yml` & `adeploy-1.1.0/examples/jinja/006-nested-labels/templates/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/007-resources/README.md` & `adeploy-1.1.0/examples/jinja/007-resources/README.md`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/prod/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/007-resources/build/jinja/playground/007-resources/test/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/007-resources/defaults.yml` & `adeploy-1.1.0/examples/jinja/007-resources/defaults.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/007-resources/templates/nginx/deployment.yml` & `adeploy-1.1.0/examples/jinja/007-resources/templates/nginx/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/examples/jinja/007-resources/templates/redis/deployment.yml` & `adeploy-1.1.0/examples/jinja/007-resources/templates/redis/deployment.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/mkdocs.yml` & `adeploy-1.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/pyproject.toml` & `adeploy-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adeploy-1.0.0/setup.py` & `adeploy-1.1.0/setup.py`

 * *Files identical despite different names*

