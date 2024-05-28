# Comparing `tmp/sentry_cli-2.31.2.tar.gz` & `tmp/sentry_cli-2.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.31.2.tar", last modified: Thu May  2 14:17:09 2024, max compression
+gzip compressed data, was "sentry_cli-2.32.0.tar", last modified: Tue May 28 09:10:52 2024, max compression
```

## Comparing `sentry_cli-2.31.2.tar` & `sentry_cli-2.32.0.tar`

### file list

```diff
@@ -1,143 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/
--rw-r--r--   0 runner    (1001) docker     (127)    92408 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-02 14:17:09.000000 sentry_cli-2.31.2/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-02 14:17:09.000000 sentry_cli-2.31.2/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:17:09.000000 sentry_cli-2.31.2/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:17:09.000000 sentry_cli-2.31.2/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.246627 sentry_cli-2.31.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.246627 sentry_cli-2.31.2/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/connection_manager.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/encoding.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.246627 sentry_cli-2.31.2/src/api/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/errors/api_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/errors/sentry_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)    83793 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/api/pagination.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.246627 sentry_cli-2.31.2/src/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.250627 sentry_cli-2.31.2/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.254627 sentry_cli-2.31.2/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.258627 sentry_cli-2.31.2/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/args.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/src/utils/auth_token/
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/auth_token_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/org_auth_token.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/test.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/auth_token/user_auth_token.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (127)    72264 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:09.262627 sentry_cli-2.31.2/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (127)    36324 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-05-02 14:16:52.000000 sentry_cli-2.31.2/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.336048 sentry_cli-2.32.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    94065 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-28 09:10:52.336048 sentry_cli-2.32.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.336048 sentry_cli-2.32.0/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-28 09:10:52.000000 sentry_cli-2.32.0/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-28 09:10:52.000000 sentry_cli-2.32.0/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:10:52.000000 sentry_cli-2.32.0/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:10:52.000000 sentry_cli-2.32.0/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-28 09:10:52.336048 sentry_cli-2.32.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.316048 sentry_cli-2.32.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.320048 sentry_cli-2.32.0/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/api/connection_manager.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/api/encoding.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/api/envelopes_api.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.320048 sentry_cli-2.32.0/src/api/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/api/errors/api_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/api/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/api/errors/sentry_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    83940 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/api/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/api/pagination.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.320048 sentry_cli-2.32.0/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.324048 sentry_cli-2.32.0/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.324048 sentry_cli-2.32.0/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/deploys/new.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/derive_parser.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.324048 sentry_cli-2.32.0/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.324048 sentry_cli-2.32.0/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.324048 sentry_cli-2.32.0/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/issues/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.324048 sentry_cli-2.32.0/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.324048 sentry_cli-2.32.0/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.324048 sentry_cli-2.32.0/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.328048 sentry_cli-2.32.0/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.328048 sentry_cli-2.32.0/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.328048 sentry_cli-2.32.0/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.328048 sentry_cli-2.32.0/src/commands/send_metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/send_metric/common_args.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/send_metric/distribution.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/send_metric/gauge.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/send_metric/increment.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/send_metric/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/send_metric/set.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.328048 sentry_cli-2.32.0/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    25826 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.336048 sentry_cli-2.32.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/args.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.336048 sentry_cli-2.32.0/src/utils/auth_token/
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/auth_token/auth_token_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/auth_token/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/auth_token/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/auth_token/org_auth_token.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/auth_token/test.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/auth_token/user_auth_token.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    72264 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/metrics.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.336048 sentry_cli-2.32.0/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:52.336048 sentry_cli-2.32.0/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/value_parsers.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    36324 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-05-28 09:10:34.000000 sentry_cli-2.32.0/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.31.2/Cargo.lock` & `sentry_cli-2.32.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -352,29 +352,44 @@
 [[package]]
 name = "clap"
 version = "4.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0b0588d44d4d63a87dbd75c136c166bbfd9a86a31cb89e09906521c7d3f5e3"
 dependencies = [
  "bitflags 1.3.2",
+ "clap_derive",
  "clap_lex",
+ "once_cell",
  "strsim",
  "terminal_size",
 ]
 
 [[package]]
 name = "clap_complete"
 version = "4.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3ae8ba90b9d8b007efe66e55e48fb936272f5ca00349b5b0e89877520d35ea7"
 dependencies = [
  "clap",
 ]
 
 [[package]]
+name = "clap_derive"
+version = "4.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "684a277d672e91966334af371f1a7b5833f9aa00b07c84e92fbce95e00208ce8"
+dependencies = [
+ "heck",
+ "proc-macro-error",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.107",
+]
+
+[[package]]
 name = "clap_lex"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "783fe232adfca04f90f56201b26d79682d4cd2625e0bc7290b95123afe558ade"
 dependencies = [
  "os_str_bytes",
 ]
@@ -458,17 +473,17 @@
 checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
 version = "0.5.6"
@@ -1083,14 +1098,20 @@
 [[package]]
 name = "hashbrown"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
@@ -1117,21 +1138,21 @@
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "hostname"
-version = "0.3.1"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c731c3e10504cc8ed35cfe2f1db4c9274c3d35fa486e3b31df46f068ef3e867"
+checksum = "f9c7c7c8ac16c798734b8a24560c1362120597c40d5e1459f09498f8f6c8f2ba"
 dependencies = [
+ "cfg-if",
  "libc",
- "match_cfg",
- "winapi 0.3.9",
+ "windows",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
@@ -1315,14 +1336,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b71991ff56294aa922b450139ee08b3bfc70982c6b2c7562771375cf73542dd4"
 
 [[package]]
 name = "itoa"
@@ -1481,20 +1511,14 @@
  "regex",
  "serde",
  "serde_json",
  "vlq",
 ]
 
 [[package]]
-name = "match_cfg"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffbee8634e0d45d258acb448e7eaab3fce7a0a467395d4d9f228e3c1f01fb2e4"
-
-[[package]]
 name = "maybe-owned"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4facc753ae494aeb6e3c22f839b158aebd4f9270f55cd3c79906c45476c47ab4"
 
 [[package]]
 name = "memchr"
@@ -1977,15 +2001,15 @@
 name = "predicates"
 version = "2.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "59230a63c37f3e18569bdb90e4a89cbf5bf8b06fea0b84e65ea10cc4df47addd"
 dependencies = [
  "difflib",
  "float-cmp",
- "itertools",
+ "itertools 0.10.5",
  "normalize-line-endings",
  "predicates-core",
  "regex",
 ]
 
 [[package]]
 name = "predicates-core"
@@ -2004,14 +2028,38 @@
  "is-terminal",
  "lazy_static",
  "term",
  "unicode-width",
 ]
 
 [[package]]
+name = "proc-macro-error"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
+dependencies = [
+ "proc-macro-error-attr",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.107",
+ "version_check",
+]
+
+[[package]]
+name = "proc-macro-error-attr"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "version_check",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
@@ -2392,51 +2440,51 @@
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "sentry"
-version = "0.32.2"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "766448f12e44d68e675d5789a261515c46ac6ccd240abdd451a9c46c84a49523"
+checksum = "3b73ab9d5b35ed718611e89db8c886647821cfce79723b9e2e4e7cb3fd9cdd49"
 dependencies = [
  "curl",
  "httpdate",
  "sentry-anyhow",
  "sentry-contexts",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-anyhow"
-version = "0.32.2"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4da4015667c99f88d68ca7ff02b90c762d6154a4ceb7c02922b9a1dbd3959eeb"
+checksum = "3c7825549eb646ef0224b0b7fc6d38faa459d7e5e1f902a4c12bbd8de4ad060f"
 dependencies = [
  "anyhow",
  "sentry-backtrace",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-backtrace"
-version = "0.32.2"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32701cad8b3c78101e1cd33039303154791b0ff22e7802ed8cc23212ef478b45"
+checksum = "8ce52a2633e0332821389f865762b94852e71b359cd8e95cbf91f38c154302cb"
 dependencies = [
  "backtrace",
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.31.2"
+version = "2.32.0"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
@@ -2456,15 +2504,15 @@
  "flate2",
  "git2",
  "glob",
  "if_chain",
  "ignore",
  "indicatif",
  "insta",
- "itertools",
+ "itertools 0.10.5",
  "java-properties",
  "lazy_static",
  "libc",
  "log",
  "mac-process-info",
  "magic_string",
  "might-be-minified",
@@ -2504,44 +2552,47 @@
  "which",
  "winapi 0.3.9",
  "zip",
 ]
 
 [[package]]
 name = "sentry-contexts"
-version = "0.32.2"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17ddd2a91a13805bd8dab4ebf47323426f758c35f7bf24eacc1aded9668f3824"
+checksum = "10565e6eb013737bf7555250f8b4b8248a571e1de4de7230037f5dd5ea51bc63"
 dependencies = [
  "hostname",
  "libc",
  "os_info",
  "rustc_version 0.4.0",
  "sentry-core",
  "uname",
 ]
 
 [[package]]
 name = "sentry-core"
-version = "0.32.2"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1189f68d7e7e102ef7171adf75f83a59607fafd1a5eecc9dc06c026ff3bdec4"
+checksum = "a2c5e7a0430cfa86b7cb6e7bc01a56331937b2ba08ab703c2e7331139a99f121"
 dependencies = [
+ "crc32fast",
+ "itertools 0.13.0",
  "once_cell",
  "rand",
+ "regex",
  "sentry-types",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "sentry-types"
-version = "0.32.2"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7173fd594569091f68a7c37a886e202f4d0c1db1e1fa1d18a051ba695b2e2ec"
+checksum = "10d5ad9e33b9f6f598387a6a23aa23c7f13e4e7740a34cd4d9c8db851bfdae05"
 dependencies = [
  "debugid",
  "hex",
  "rand",
  "serde",
  "serde_json",
  "thiserror",
@@ -3352,14 +3403,33 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
+dependencies = [
+ "windows-core",
+ "windows-targets 0.52.0",
+]
+
+[[package]]
+name = "windows-core"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+dependencies = [
+ "windows-targets 0.52.0",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.1",
  "windows_aarch64_msvc 0.42.1",
```

### Comparing `sentry_cli-2.31.2/Cargo.toml` & `sentry_cli-2.32.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.31.2"
+version = "2.32.0"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
 backtrace = "0.3.67"
 brotli2 = "0.3.2"
 bytecount = "0.6.3"
 chardet = "0.2.4"
 chrono = { version = "0.4.31", features = ["serde"] }
 clap = { version = "4.1.6", default-features = false, features = [
+  "derive",
   "std",
   "suggestions",
   "wrap_help",
   "string",
   "help",
   "usage",
   "error-context",
@@ -54,18 +55,19 @@
 proguard = { version = "5.0.0", features = ["uuid"] }
 r2d2 = "0.8.10"
 rayon = "1.6.1"
 regex = "1.7.3"
 runas = "1.0.0"
 rust-ini = "0.18.0"
 semver = "1.0.16"
-sentry = { version = "0.32.2", default-features = false, features = [
+sentry = { version = "0.33.0", default-features = false, features = [
   "anyhow",
   "curl",
   "contexts",
+  "UNSTABLE_metrics",
 ] }
 serde = { version = "1.0.152", features = ["derive"] }
 serde_json = "1.0.93"
 sha1_smol = { version = "1.0.0", features = ["serde"] }
 sourcemap = { version = "7.0.1", features = ["ram_bundle"] }
 symbolic = { version = "12.4.1", features = ["debuginfo-serde", "il2cpp"] }
 thiserror = "1.0.38"
```

### Comparing `sentry_cli-2.31.2/LICENSE` & `sentry_cli-2.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/PKG-INFO` & `sentry_cli-2.32.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.31.2
+Version: 2.32.0
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.2 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.32.0 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.31.2/README.md` & `sentry_cli-2.32.0/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/build.rs` & `sentry_cli-2.32.0/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.32.0/sentry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.31.2
+Version: 2.32.0
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.2 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.32.0 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.31.2/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.32.0/sentry_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 sentry_cli.egg-info/top_level.txt
 src/bashsupport.sh
 src/config.rs
 src/constants.rs
 src/main.rs
 src/api/connection_manager.rs
 src/api/encoding.rs
+src/api/envelopes_api.rs
 src/api/mod.rs
 src/api/pagination.rs
 src/api/errors/api_error.rs
 src/api/errors/mod.rs
 src/api/errors/sentry_error.rs
 src/commands/bash_hook.rs
+src/commands/derive_parser.rs
 src/commands/info.rs
 src/commands/login.rs
 src/commands/mod.rs
 src/commands/send_envelope.rs
 src/commands/send_event.rs
 src/commands/uninstall.rs
 src/commands/update.rs
@@ -73,14 +75,20 @@
 src/commands/releases/mod.rs
 src/commands/releases/new.rs
 src/commands/releases/propose_version.rs
 src/commands/releases/restore.rs
 src/commands/releases/set_commits.rs
 src/commands/repos/list.rs
 src/commands/repos/mod.rs
+src/commands/send_metric/common_args.rs
+src/commands/send_metric/distribution.rs
+src/commands/send_metric/gauge.rs
+src/commands/send_metric/increment.rs
+src/commands/send_metric/mod.rs
+src/commands/send_metric/set.rs
 src/commands/sourcemaps/explain.rs
 src/commands/sourcemaps/inject.rs
 src/commands/sourcemaps/mod.rs
 src/commands/sourcemaps/resolve.rs
 src/commands/sourcemaps/upload.rs
 src/utils/android.rs
 src/utils/appcenter.rs
@@ -92,22 +100,24 @@
 src/utils/event.rs
 src/utils/file_search.rs
 src/utils/file_upload.rs
 src/utils/formatting.rs
 src/utils/fs.rs
 src/utils/http.rs
 src/utils/logging.rs
+src/utils/metrics.rs
 src/utils/mod.rs
 src/utils/progress.rs
 src/utils/releases.rs
 src/utils/retry.rs
 src/utils/sourcemaps.rs
 src/utils/system.rs
 src/utils/ui.rs
 src/utils/update.rs
+src/utils/value_parsers.rs
 src/utils/vcs.rs
 src/utils/xcode.rs
 src/utils/auth_token/auth_token_impl.rs
 src/utils/auth_token/error.rs
 src/utils/auth_token/mod.rs
 src/utils/auth_token/org_auth_token.rs
 src/utils/auth_token/test.rs
```

### Comparing `sentry_cli-2.31.2/setup.cfg` & `sentry_cli-2.32.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/setup.py` & `sentry_cli-2.32.0/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/api/connection_manager.rs` & `sentry_cli-2.32.0/src/api/connection_manager.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/api/encoding.rs` & `sentry_cli-2.32.0/src/api/encoding.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/api/errors/api_error.rs` & `sentry_cli-2.32.0/src/api/errors/api_error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 }
 
 /// Represents API errors.
 #[derive(Copy, Clone, Eq, PartialEq, Debug, thiserror::Error)]
 pub(in crate::api) enum ApiErrorKind {
     #[error("could not serialize value as JSON")]
     CannotSerializeAsJson,
+    #[error("could not serialize envelope")]
+    CannotSerializeEnvelope,
     #[error("could not parse JSON response")]
     BadJson,
     #[error("not a JSON response")]
     NotJson,
     #[error("request failed because API URL was incorrectly formatted")]
     BadApiUrl,
     #[error("organization not found")]
@@ -34,14 +36,18 @@
     CompressionFailed,
     #[error("region overrides cannot be applied to absolute urls")]
     InvalidRegionRequest,
     #[error(
         "Auth token is required for this request. Please run `sentry-cli login` and try again!"
     )]
     AuthMissing,
+    #[error(
+        "DSN missing. Please set the `SENTRY_DSN` environment variable to your project's DSN."
+    )]
+    DsnMissing,
 }
 
 impl fmt::Display for ApiError {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         fmt::Display::fmt(&self.inner, f)
     }
 }
```

### Comparing `sentry_cli-2.31.2/src/api/errors/sentry_error.rs` & `sentry_cli-2.32.0/src/api/errors/sentry_error.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/api/mod.rs` & `sentry_cli-2.32.0/src/api/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 //! This module implements the API access to the Sentry API as well
 //! as some other APIs we interact with.  In particular it can talk
 //! to the GitHub API to figure out if there are new releases of the
 //! sentry-cli tool.
 
+pub mod envelopes_api;
+
 mod connection_manager;
 mod encoding;
 mod errors;
 mod pagination;
 
 use std::borrow::Cow;
 use std::cell::RefCell;
@@ -1742,14 +1744,19 @@
             .map_err(|err| ApiError::with_source(ApiErrorKind::CannotSerializeAsJson, err))?;
         debug!("json body: {}", String::from_utf8_lossy(&body_bytes));
         self.body = Some(body_bytes);
         self.headers.append("Content-Type: application/json")?;
         Ok(self)
     }
 
+    pub fn with_body(mut self, body: Vec<u8>) -> ApiResult<Self> {
+        self.body = Some(body);
+        Ok(self)
+    }
+
     /// attaches some form data to the request.
     pub fn with_form_data(mut self, form: curl::easy::Form) -> ApiResult<Self> {
         debug!("sending form data");
         self.handle.httppost(form)?;
         self.body = None;
         Ok(self)
     }
```

### Comparing `sentry_cli-2.31.2/src/api/pagination.rs` & `sentry_cli-2.32.0/src/api/pagination.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/bashsupport.sh` & `sentry_cli-2.32.0/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/bash_hook.rs` & `sentry_cli-2.32.0/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.32.0/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.32.0/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/debug_files/check.rs` & `sentry_cli-2.32.0/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/debug_files/find.rs` & `sentry_cli-2.32.0/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/debug_files/mod.rs` & `sentry_cli-2.32.0/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.32.0/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/debug_files/upload.rs` & `sentry_cli-2.32.0/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/deploys/list.rs` & `sentry_cli-2.32.0/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/deploys/mod.rs` & `sentry_cli-2.32.0/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/deploys/new.rs` & `sentry_cli-2.32.0/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/events/list.rs` & `sentry_cli-2.32.0/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/events/mod.rs` & `sentry_cli-2.32.0/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/files/delete.rs` & `sentry_cli-2.32.0/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/files/list.rs` & `sentry_cli-2.32.0/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/files/mod.rs` & `sentry_cli-2.32.0/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/files/upload.rs` & `sentry_cli-2.32.0/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/info.rs` & `sentry_cli-2.32.0/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/issues/list.rs` & `sentry_cli-2.32.0/src/commands/issues/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/issues/mod.rs` & `sentry_cli-2.32.0/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/issues/mute.rs` & `sentry_cli-2.32.0/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/issues/resolve.rs` & `sentry_cli-2.32.0/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/issues/unresolve.rs` & `sentry_cli-2.32.0/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/login.rs` & `sentry_cli-2.32.0/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/mod.rs` & `sentry_cli-2.32.0/src/commands/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 use crate::constants::{ARCH, PLATFORM, VERSION};
 use crate::utils::auth_token::AuthToken;
 use crate::utils::logging::set_quiet_mode;
 use crate::utils::logging::Logger;
 use crate::utils::system::{init_backtrace, load_dotenv, print_error, QuietExit};
 use crate::utils::update::run_sentrycli_update_nagger;
 
+mod derive_parser;
+
 macro_rules! each_subcommand {
     ($mac:ident) => {
         $mac!(bash_hook);
         $mac!(debug_files);
         $mac!(deploys);
         $mac!(events);
         $mac!(files);
@@ -32,14 +34,15 @@
         $mac!(organizations);
         $mac!(projects);
         $mac!(react_native);
         $mac!(releases);
         $mac!(repos);
         $mac!(send_event);
         $mac!(send_envelope);
+        $mac!(send_metric);
         $mac!(sourcemaps);
         #[cfg(not(feature = "managed"))]
         $mac!(uninstall);
         #[cfg(not(feature = "managed"))]
         $mac!(update);
         $mac!(upload_dif);
         $mac!(upload_dsym);
```

### Comparing `sentry_cli-2.31.2/src/commands/monitors/list.rs` & `sentry_cli-2.32.0/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/monitors/mod.rs` & `sentry_cli-2.32.0/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/monitors/run.rs` & `sentry_cli-2.32.0/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/organizations/list.rs` & `sentry_cli-2.32.0/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/organizations/mod.rs` & `sentry_cli-2.32.0/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/projects/list.rs` & `sentry_cli-2.32.0/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/projects/mod.rs` & `sentry_cli-2.32.0/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/react_native/appcenter.rs` & `sentry_cli-2.32.0/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/react_native/gradle.rs` & `sentry_cli-2.32.0/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/react_native/mod.rs` & `sentry_cli-2.32.0/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/react_native/xcode.rs` & `sentry_cli-2.32.0/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/archive.rs` & `sentry_cli-2.32.0/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/delete.rs` & `sentry_cli-2.32.0/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/finalize.rs` & `sentry_cli-2.32.0/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/info.rs` & `sentry_cli-2.32.0/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/list.rs` & `sentry_cli-2.32.0/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/mod.rs` & `sentry_cli-2.32.0/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/new.rs` & `sentry_cli-2.32.0/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/restore.rs` & `sentry_cli-2.32.0/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/releases/set_commits.rs` & `sentry_cli-2.32.0/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/repos/list.rs` & `sentry_cli-2.32.0/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/repos/mod.rs` & `sentry_cli-2.32.0/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/send_envelope.rs` & `sentry_cli-2.32.0/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/send_event.rs` & `sentry_cli-2.32.0/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.32.0/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.32.0/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.32.0/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.32.0/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.32.0/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/uninstall.rs` & `sentry_cli-2.32.0/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/update.rs` & `sentry_cli-2.32.0/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/commands/upload_proguard.rs` & `sentry_cli-2.32.0/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/config.rs` & `sentry_cli-2.32.0/src/config.rs`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 use clap::ArgMatches;
 use ini::Ini;
 use lazy_static::lazy_static;
 use log::{debug, info, set_max_level, warn};
 use parking_lot::Mutex;
 use sentry::types::Dsn;
 
+use crate::constants::CONFIG_INI_FILE_PATH;
 use crate::constants::DEFAULT_MAX_DIF_ITEM_SIZE;
 use crate::constants::DEFAULT_MAX_DIF_UPLOAD_SIZE;
 use crate::constants::{CONFIG_RC_FILE_NAME, DEFAULT_RETRIES, DEFAULT_URL};
 use crate::utils::auth_token::AuthToken;
 use crate::utils::auth_token::AuthTokenPayload;
 use crate::utils::http::is_absolute_url;
 
@@ -522,20 +523,22 @@
             } else {
                 false
             }
     }
 }
 
 fn find_global_config_file() -> Result<PathBuf> {
-    dirs::home_dir()
+    let home_dir_file = dirs::home_dir().map(|p| p.join(CONFIG_RC_FILE_NAME));
+    let config_dir_file = dirs::config_dir().map(|p| p.join(CONFIG_INI_FILE_PATH));
+    home_dir_file
+        .clone()
+        .filter(|p| p.exists())
+        .or(config_dir_file.filter(|p| p.exists()))
+        .or(home_dir_file)
         .ok_or_else(|| format_err!("Could not find home dir"))
-        .map(|mut path| {
-            path.push(CONFIG_RC_FILE_NAME);
-            path
-        })
 }
 
 fn find_project_config_file() -> Option<PathBuf> {
     env::current_dir().ok().and_then(|mut path| loop {
         path.push(CONFIG_RC_FILE_NAME);
         if path.exists() {
             return Some(path);
```

### Comparing `sentry_cli-2.31.2/src/constants.rs` & `sentry_cli-2.32.0/src/constants.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 /// The version of the library
 pub const VERSION: &str = env!("CARGO_PKG_VERSION");
 
 /// The name of the configuration file.
 pub const CONFIG_RC_FILE_NAME: &str = ".sentryclirc";
 
+/// The relative path of the configuration file in dirs::config_dir()
+pub const CONFIG_INI_FILE_PATH: &str = "sentry/sentrycli.ini";
+
 /// The release registry URL where the latest released version of sentry-cli can be found
 pub const RELEASE_REGISTRY_LATEST_URL: &str =
     "https://release-registry.services.sentry.io/apps/sentry-cli/latest";
 
 /// The file extension of the binary (.exe or empty string)
 #[cfg(windows)]
 pub const EXT: &str = ".exe";
```

### Comparing `sentry_cli-2.31.2/src/utils/android.rs` & `sentry_cli-2.32.0/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/appcenter.rs` & `sentry_cli-2.32.0/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/args.rs` & `sentry_cli-2.32.0/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/auth_token/auth_token_impl.rs` & `sentry_cli-2.32.0/src/utils/auth_token/auth_token_impl.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/auth_token/error.rs` & `sentry_cli-2.32.0/src/utils/auth_token/error.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/auth_token/org_auth_token.rs` & `sentry_cli-2.32.0/src/utils/auth_token/org_auth_token.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/auth_token/test.rs` & `sentry_cli-2.32.0/src/utils/auth_token/test.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/auth_token/user_auth_token.rs` & `sentry_cli-2.32.0/src/utils/auth_token/user_auth_token.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/chunks.rs` & `sentry_cli-2.32.0/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/cordova.rs` & `sentry_cli-2.32.0/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/dif.rs` & `sentry_cli-2.32.0/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/dif_upload.rs` & `sentry_cli-2.32.0/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/event.rs` & `sentry_cli-2.32.0/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/file_search.rs` & `sentry_cli-2.32.0/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/file_upload.rs` & `sentry_cli-2.32.0/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/formatting.rs` & `sentry_cli-2.32.0/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/fs.rs` & `sentry_cli-2.32.0/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/http.rs` & `sentry_cli-2.32.0/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/logging.rs` & `sentry_cli-2.32.0/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/progress.rs` & `sentry_cli-2.32.0/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/releases.rs` & `sentry_cli-2.32.0/src/utils/releases.rs`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,22 @@
     }
 
     Ok(None)
 }
 
 /// Detects the release name for the current working directory.
 pub fn detect_release_name() -> Result<String> {
-    // cordova release detection first.
+    // try SENTRY_RELEASE environment variable
+    if let Ok(release) = env::var("SENTRY_RELEASE") {
+        if !release.is_empty() {
+            return Ok(release);
+        }
+    }
+
+    // try cordova release detection
     if let Some(release) = get_cordova_release_name(None)? {
         return Ok(release);
     }
 
     // try Heroku #1 https://devcenter.heroku.com/changelog-items/630
     if let Ok(release) = env::var("SOURCE_VERSION") {
         if !release.is_empty() {
@@ -138,14 +145,21 @@
     // For android we badly parse gradle files.  We do this because most of the
     // time now people set the ids and versions in the gradle files instead of
     // the xml manifests.
     if let Some(release) = infer_gradle_release_name(None)? {
         return Ok(release);
     }
 
+    // try Google App Engine: https://cloud.google.com/appengine/docs/standard/python3/runtime#environment_variables
+    if let Ok(release) = env::var("GAE_DEPLOYMENT_ID") {
+        if !release.is_empty() {
+            return Ok(release);
+        }
+    }
+
     match vcs::find_head() {
         Ok(head) => Ok(head),
         Err(e) => Err(anyhow!(
             "Could not automatically determine release name:\n\t {e} \n\n\
             Please ensure your version control system is configured correctly, \
             or provide a release name manually."
         )),
```

### Comparing `sentry_cli-2.31.2/src/utils/retry.rs` & `sentry_cli-2.32.0/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.32.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.32.0/src/utils/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/sourcemaps.rs` & `sentry_cli-2.32.0/src/utils/sourcemaps.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/system.rs` & `sentry_cli-2.32.0/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/ui.rs` & `sentry_cli-2.32.0/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/update.rs` & `sentry_cli-2.32.0/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/vcs.rs` & `sentry_cli-2.32.0/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.2/src/utils/xcode.rs` & `sentry_cli-2.32.0/src/utils/xcode.rs`

 * *Files identical despite different names*

