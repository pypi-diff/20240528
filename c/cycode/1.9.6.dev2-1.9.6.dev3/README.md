# Comparing `tmp/cycode-1.9.6.dev2.tar.gz` & `tmp/cycode-1.9.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-1.9.6.dev2.tar", max compression
+gzip compressed data, was "cycode-1.9.6.dev3.tar", max compression
```

## Comparing `cycode-1.9.6.dev2.tar` & `cycode-1.9.6.dev3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    42867 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/README.md
--rw-r--r--   0        0        0      114 2024-05-27 09:34:13.427385 cycode-1.9.6.dev2/cycode/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/auth/__init__.py
--rw-r--r--   0        0        0     2897 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/auth/auth_command.py
--rw-r--r--   0        0        0     4726 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/auth/auth_manager.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/configure/__init__.py
--rw-r--r--   0        0        0     5423 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/configure/configure_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/ignore/__init__.py
--rw-r--r--   0        0        0     3873 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/ignore/ignore_command.py
--rw-r--r--   0        0        0     2497 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/main_cli.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/__init__.py
--rw-r--r--   0        0        0      563 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/report_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/__init__.py
--rw-r--r--   0        0        0     3435 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/common.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/path/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/path/path_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/repository_url/__init__.py
--rw-r--r--   0        0        0     2143 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
--rw-r--r--   0        0        0     2358 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/sbom_command.py
--rw-r--r--   0        0        0     1533 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/sbom_report_file.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/__init__.py
--rw-r--r--   0        0        0    38773 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/code_scanner.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/commit_history/__init__.py
--rw-r--r--   0        0        0      975 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/commit_history/commit_history_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/path/__init__.py
--rw-r--r--   0        0        0      590 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/path/path_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_commit/__init__.py
--rw-r--r--   0        0        0     1605 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_receive/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/repository/__init__.py
--rw-r--r--   0        0        0     2710 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/repository/repository_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/__init__.py
--rw-r--r--   0        0        0     1588 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/ci_integrations.py
--rw-r--r--   0        0        0      552 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
--rw-r--r--   0        0        0     5082 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_command.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/version/__init__.py
--rw-r--r--   0        0        0      509 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/version/version_command.py
--rw-r--r--   0        0        0      466 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/config.py
--rw-r--r--   0        0        0      463 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/config.yaml
--rw-r--r--   0        0        0     6194 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     2109 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0     1620 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/exceptions/handle_report_sbom_errors.py
--rw-r--r--   0        0        0     2785 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/exceptions/handle_scan_errors.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/__init__.py
--rw-r--r--   0        0        0     6243 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/excluder.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/iac/__init__.py
--rw-r--r--   0        0        0     2457 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/iac/tf_content_generator.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/models/__init__.py
--rw-r--r--   0        0        0     1247 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/models/in_memory_zip.py
--rw-r--r--   0        0        0     4394 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/path_documents.py
--rw-r--r--   0        0        0     4940 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/repository_documents.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/__init__.py
--rw-r--r--   0        0        0     2412 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0     1136 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     3119 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     6400 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/sca_code_scanner.py
--rw-r--r--   0        0        0     1873 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/zip_documents.py
--rw-r--r--   0        0        0      387 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/main.py
--rw-r--r--   0        0        0     2051 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0     2395 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     2290 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     1613 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/printer_base.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/__init__.py
--rw-r--r--   0        0        0     7660 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/sca_table_printer.py
--rw-r--r--   0        0        0     2281 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/table.py
--rw-r--r--   0        0        0      480 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/table_models.py
--rw-r--r--   0        0        0     5216 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/table_printer.py
--rw-r--r--   0        0        0     2400 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/table_printer_base.py
--rw-r--r--   0        0        0    10484 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      630 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4939 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     7591 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     2987 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0      745 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/jwt_creator.py
--rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      211 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     1584 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/get_api_client.py
--rw-r--r--   0        0        0     1953 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     9940 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2794 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      967 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     2034 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2748 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      934 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0       71 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1777 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     1072 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/client_creator.py
--rw-r--r--   0        0        0     3349 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      120 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      257 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3699 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      670 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     3600 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     1319 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/headers.py
--rw-r--r--   0        0        0    13226 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/models.py
--rw-r--r--   0        0        0     3971 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/report_client.py
--rw-r--r--   0        0        0    12573 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0     1658 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/scan_config_base.py
--rw-r--r--   0        0        0     3467 2024-05-27 09:34:13.423385 cycode-1.9.6.dev2/pyproject.toml
--rw-r--r--   0        0        0    44445 1970-01-01 00:00:00.000000 cycode-1.9.6.dev2/PKG-INFO
+-rw-r--r--   0        0        0    42867 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/README.md
+-rw-r--r--   0        0        0      114 2024-05-28 10:47:48.925091 cycode-1.9.6.dev3/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/auth/__init__.py
+-rw-r--r--   0        0        0     2897 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/auth/auth_command.py
+-rw-r--r--   0        0        0     4726 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/auth/auth_manager.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/configure/__init__.py
+-rw-r--r--   0        0        0     5423 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/configure/configure_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/ignore/__init__.py
+-rw-r--r--   0        0        0     3873 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/ignore/ignore_command.py
+-rw-r--r--   0        0        0     2497 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/main_cli.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/__init__.py
+-rw-r--r--   0        0        0      563 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/report_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/__init__.py
+-rw-r--r--   0        0        0     3435 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/common.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/path/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/repository_url/__init__.py
+-rw-r--r--   0        0        0     2143 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
+-rw-r--r--   0        0        0     2358 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/sbom_command.py
+-rw-r--r--   0        0        0     1533 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/sbom_report_file.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/__init__.py
+-rw-r--r--   0        0        0    39829 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/code_scanner.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/commit_history/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/commit_history/commit_history_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/path/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_commit/__init__.py
+-rw-r--r--   0        0        0     1605 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_receive/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/repository/__init__.py
+-rw-r--r--   0        0        0     2710 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/repository/repository_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/__init__.py
+-rw-r--r--   0        0        0     1588 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/ci_integrations.py
+-rw-r--r--   0        0        0      552 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
+-rw-r--r--   0        0        0     5082 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_command.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/version/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-28 10:47:40.157019 cycode-1.9.6.dev3/cycode/cli/commands/version/version_command.py
+-rw-r--r--   0        0        0      466 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/config.py
+-rw-r--r--   0        0        0      463 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     6194 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/exceptions/handle_report_sbom_errors.py
+-rw-r--r--   0        0        0     2785 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/exceptions/handle_scan_errors.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/__init__.py
+-rw-r--r--   0        0        0     6243 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/excluder.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/iac/__init__.py
+-rw-r--r--   0        0        0     2457 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/iac/tf_content_generator.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/models/__init__.py
+-rw-r--r--   0        0        0     1247 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/models/in_memory_zip.py
+-rw-r--r--   0        0        0     4394 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/path_documents.py
+-rw-r--r--   0        0        0     4940 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/repository_documents.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/__init__.py
+-rw-r--r--   0        0        0     2412 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0     1136 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     3119 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     6400 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/sca/sca_code_scanner.py
+-rw-r--r--   0        0        0     1873 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/files_collector/zip_documents.py
+-rw-r--r--   0        0        0      387 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/main.py
+-rw-r--r--   0        0        0     2051 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0     2496 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     2490 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     1613 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/printer_base.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/__init__.py
+-rw-r--r--   0        0        0     7762 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/sca_table_printer.py
+-rw-r--r--   0        0        0     2281 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/table.py
+-rw-r--r--   0        0        0      480 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/table_models.py
+-rw-r--r--   0        0        0     5264 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/table_printer.py
+-rw-r--r--   0        0        0     2618 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/tables/table_printer_base.py
+-rw-r--r--   0        0        0    10847 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4939 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     7591 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     2987 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0      745 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/user_settings/jwt_creator.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     1584 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/get_api_client.py
+-rw-r--r--   0        0        0     1953 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     9940 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2794 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      967 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     2034 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2748 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      934 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0       71 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1777 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     1072 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/client_creator.py
+-rw-r--r--   0        0        0     3349 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      257 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3699 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      670 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     3600 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     1319 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/headers.py
+-rw-r--r--   0        0        0    13226 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     3971 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/report_client.py
+-rw-r--r--   0        0        0    13213 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0     1658 2024-05-28 10:47:40.161020 cycode-1.9.6.dev3/cycode/cyclient/scan_config_base.py
+-rw-r--r--   0        0        0     3467 2024-05-28 10:47:48.921091 cycode-1.9.6.dev3/pyproject.toml
+-rw-r--r--   0        0        0    44445 1970-01-01 00:00:00.000000 cycode-1.9.6.dev3/PKG-INFO
```

### Comparing `cycode-1.9.6.dev2/README.md` & `cycode-1.9.6.dev3/README.md`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/auth/auth_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/auth/auth_manager.py` & `cycode-1.9.6.dev3/cycode/cli/commands/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/configure/configure_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/configure/configure_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/ignore/ignore_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/ignore/ignore_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/main_cli.py` & `cycode-1.9.6.dev3/cycode/cli/commands/main_cli.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/report/report_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/report/report_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/common.py` & `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/common.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/path/path_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/sbom_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/sbom_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/sbom_report_file.py` & `cycode-1.9.6.dev3/cycode/cli/commands/report/sbom/sbom_report_file.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/code_scanner.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/code_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,22 +144,22 @@
             detection.detection_details['remediation_guidelines'] = detection_rule.remediation_guidelines
             detection.detection_details['description'] = detection_rule.description
             detection.detection_details['policy_display_name'] = detection_rule.display_name
 
 
 def _get_scan_documents_thread_func(
     context: click.Context, is_git_diff: bool, is_commit_range: bool, scan_parameters: dict
-) -> Callable[[List[Document]], Tuple[str, CliError, LocalScanResult]]:
+) -> Tuple[Callable[[List[Document]], Tuple[str, CliError, LocalScanResult]], str]:
     cycode_client = context.obj['client']
     scan_type = context.obj['scan_type']
     severity_threshold = context.obj['severity_threshold']
     sync_option = context.obj['sync']
     command_scan_type = context.info_name
-
-    scan_parameters['aggregation_id'] = str(_generate_unique_id())
+    aggregation_id = str(_generate_unique_id())
+    scan_parameters['aggregation_id'] = aggregation_id
 
     def _scan_batch_thread_func(batch: List[Document]) -> Tuple[str, CliError, LocalScanResult]:
         local_scan_result = error = error_message = None
         detections_count = relevant_detections_count = zip_file_size = 0
 
         scan_id = str(_generate_unique_id())
         scan_completed = False
@@ -220,15 +220,15 @@
             command_scan_type,
             error_message,
             should_use_scan_service,
         )
 
         return scan_id, error, local_scan_result
 
-    return _scan_batch_thread_func
+    return _scan_batch_thread_func, aggregation_id
 
 
 def scan_commit_range(
     context: click.Context, path: str, commit_range: str, max_commits_count: Optional[int] = None
 ) -> None:
     scan_type = context.obj['scan_type']
 
@@ -309,27 +309,51 @@
                 code='no_relevant_files',
                 message='Error: The scan could not be completed - relevant files to scan are not found. '
                 'Enable verbose mode to see more details.',
             )
         )
         return
 
-    scan_batch_thread_func = _get_scan_documents_thread_func(context, is_git_diff, is_commit_range, scan_parameters)
+    scan_batch_thread_func, aggregation_id = _get_scan_documents_thread_func(
+        context, is_git_diff, is_commit_range, scan_parameters
+    )
     errors, local_scan_results = run_parallel_batched_scan(
         scan_batch_thread_func, documents_to_scan, progress_bar=progress_bar
     )
-
+    aggregation_report_url = _try_get_aggregation_report_url_if_needed(
+        scan_parameters, context.obj['client'], context.obj['scan_type']
+    )
+    set_aggregation_report_url(context, aggregation_report_url)
     progress_bar.set_section_length(ScanProgressBarSection.GENERATE_REPORT, 1)
     progress_bar.update(ScanProgressBarSection.GENERATE_REPORT)
     progress_bar.stop()
 
     set_issue_detected_by_scan_results(context, local_scan_results)
     print_results(context, local_scan_results, errors)
 
 
+def set_aggregation_report_url(context: click.Context, aggregation_report_url: Optional[str] = None) -> None:
+    context.obj['aggregation_report_url'] = aggregation_report_url
+
+
+def _try_get_aggregation_report_url_if_needed(
+    scan_parameters: dict, cycode_client: 'ScanClient', scan_type: str
+) -> Optional[str]:
+    aggregation_id = scan_parameters.get('aggregation_id')
+    if not scan_parameters.get('report'):
+        return None
+    if aggregation_id is None:
+        return None
+    try:
+        report_url_response = cycode_client.get_scan_aggregation_report_url(aggregation_id, scan_type)
+        return report_url_response.report_url
+    except Exception as e:
+        logger.debug('Failed to get aggregation report url: %s', str(e))
+
+
 def scan_commit_range_documents(
     context: click.Context,
     from_documents_to_scan: List[Document],
     to_documents_to_scan: List[Document],
     scan_parameters: Optional[dict] = None,
     timeout: Optional[int] = None,
 ) -> None:
```

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/commit_history/commit_history_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/commit_history/commit_history_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/path/path_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_commit/pre_commit_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_commit/pre_commit_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_receive/pre_receive_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/pre_receive/pre_receive_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/repository/repository_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/repository/repository_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/ci_integrations.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/scan_ci_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_ci/scan_ci_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_command.py` & `cycode-1.9.6.dev3/cycode/cli/commands/scan/scan_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/consts.py` & `cycode-1.9.6.dev3/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/exceptions/custom_exceptions.py` & `cycode-1.9.6.dev3/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/exceptions/handle_report_sbom_errors.py` & `cycode-1.9.6.dev3/cycode/cli/exceptions/handle_report_sbom_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/exceptions/handle_scan_errors.py` & `cycode-1.9.6.dev3/cycode/cli/exceptions/handle_scan_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/excluder.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/excluder.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/iac/tf_content_generator.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/iac/tf_content_generator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/models/in_memory_zip.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/models/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/path_documents.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/path_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/repository_documents.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/repository_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/sca/sca_code_scanner.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/sca/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/files_collector/zip_documents.py` & `cycode-1.9.6.dev3/cycode/cli/files_collector/zip_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/models.py` & `cycode-1.9.6.dev3/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/printers/console_printer.py` & `cycode-1.9.6.dev3/cycode/cli/printers/console_printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,21 +24,23 @@
         'text_sca': ScaTablePrinter,
     }
 
     def __init__(self, context: click.Context) -> None:
         self.context = context
         self.scan_type = self.context.obj.get('scan_type')
         self.output_type = self.context.obj.get('output')
-
+        self.aggregation_report_url = self.context.obj.get('aggregation_report_url')
         self._printer_class = self._AVAILABLE_PRINTERS.get(self.output_type)
         if self._printer_class is None:
             raise CycodeError(f'"{self.output_type}" output type is not supported.')
 
     def print_scan_results(
-        self, local_scan_results: List['LocalScanResult'], errors: Optional[Dict[str, 'CliError']] = None
+        self,
+        local_scan_results: List['LocalScanResult'],
+        errors: Optional[Dict[str, 'CliError']] = None,
     ) -> None:
         printer = self._get_scan_printer()
         printer.print_scan_results(local_scan_results, errors)
 
     def _get_scan_printer(self) -> 'PrinterBase':
         printer_class = self._printer_class
```

### Comparing `cycode-1.9.6.dev2/cycode/cli/printers/json_printer.py` & `cycode-1.9.6.dev3/cycode/cli/printers/json_printer.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,21 +24,23 @@
 
     def print_scan_results(
         self, local_scan_results: List['LocalScanResult'], errors: Optional[Dict[str, 'CliError']] = None
     ) -> None:
         scan_ids = []
         report_urls = []
         detections = []
+        aggregation_report_url = self.context.obj.get('aggregation_report_url')
+        if aggregation_report_url:
+            report_urls.append(aggregation_report_url)
 
         for local_scan_result in local_scan_results:
             scan_ids.append(local_scan_result.scan_id)
 
-            if local_scan_result.report_url:
+            if not aggregation_report_url and local_scan_result.report_url:
                 report_urls.append(local_scan_result.report_url)
-
             for document_detections in local_scan_result.document_detections:
                 detections.extend(document_detections.detections)
 
         detections_dict = DetectionSchema(many=True).dump(detections)
 
         inlined_errors = []
         if errors:
```

### Comparing `cycode-1.9.6.dev2/cycode/cli/printers/printer_base.py` & `cycode-1.9.6.dev3/cycode/cli/printers/printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/printers/tables/sca_table_printer.py` & `cycode-1.9.6.dev3/cycode/cli/printers/tables/sca_table_printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from cycode.cli.printers.tables.table_models import ColumnInfoBuilder, ColumnWidths
 from cycode.cli.printers.tables.table_printer_base import TablePrinterBase
 from cycode.cli.utils.string_utils import shortcut_dependency_paths
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult
 
-
 column_builder = ColumnInfoBuilder()
 
 # Building must have strict order. Represents the order of the columns in the table (from left to right)
 SEVERITY_COLUMN = column_builder.build(name='Severity')
 REPOSITORY_COLUMN = column_builder.build(name='Repository')
 CODE_PROJECT_COLUMN = column_builder.build(name='Code Project')  # File path to manifest file
 ECOSYSTEM_COLUMN = column_builder.build(name='Ecosystem')
@@ -25,39 +24,39 @@
 CVE_COLUMNS = column_builder.build(name='CVE')
 DEPENDENCY_PATHS_COLUMN = column_builder.build(name='Dependency Paths')
 UPGRADE_COLUMN = column_builder.build(name='Upgrade')
 LICENSE_COLUMN = column_builder.build(name='License')
 DIRECT_DEPENDENCY_COLUMN = column_builder.build(name='Direct Dependency')
 DEVELOPMENT_DEPENDENCY_COLUMN = column_builder.build(name='Development Dependency')
 
-
 COLUMN_WIDTHS_CONFIG: ColumnWidths = {
     REPOSITORY_COLUMN: 2,
     CODE_PROJECT_COLUMN: 2,
     PACKAGE_COLUMN: 3,
     CVE_COLUMNS: 5,
     UPGRADE_COLUMN: 3,
     LICENSE_COLUMN: 2,
 }
 
 
 class ScaTablePrinter(TablePrinterBase):
     def _print_results(self, local_scan_results: List['LocalScanResult']) -> None:
+        aggregation_report_url = self.context.obj.get('aggregation_report_url')
         detections_per_policy_id = self._extract_detections_per_policy_id(local_scan_results)
         for policy_id, detections in detections_per_policy_id.items():
             table = self._get_table(policy_id)
             table.set_cols_width(COLUMN_WIDTHS_CONFIG)
 
             for detection in self._sort_and_group_detections(detections):
                 self._enrich_table_with_values(table, detection)
 
             self._print_summary_issues(len(detections), self._get_title(policy_id))
             self._print_table(table)
 
-        self._print_report_urls(local_scan_results)
+        self._print_report_urls(local_scan_results, aggregation_report_url)
 
     @staticmethod
     def _get_title(policy_id: str) -> str:
         if policy_id == PACKAGE_VULNERABILITY_POLICY_ID:
             return 'Dependency Vulnerabilities'
         if policy_id == LICENSE_COMPLIANCE_POLICY_ID:
             return 'License Compliance'
```

### Comparing `cycode-1.9.6.dev2/cycode/cli/printers/tables/table.py` & `cycode-1.9.6.dev3/cycode/cli/printers/tables/table.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/printers/tables/table_printer.py` & `cycode-1.9.6.dev3/cycode/cli/printers/tables/table_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         for local_scan_result in local_scan_results:
             for document_detections in local_scan_result.document_detections:
                 for detection in document_detections.detections:
                     table.set(SCAN_ID_COLUMN, local_scan_result.scan_id)
                     self._enrich_table_with_values(table, detection, document_detections.document)
 
         self._print_table(table)
-        self._print_report_urls(local_scan_results)
+        self._print_report_urls(local_scan_results, self.context.obj.get('aggregation_report_url'))
 
     def _get_table(self) -> Table:
         table = Table()
 
         table.add(ISSUE_TYPE_COLUMN)
         table.add(RULE_ID_COLUMN)
         table.add(FILE_PATH_COLUMN)
```

### Comparing `cycode-1.9.6.dev2/cycode/cli/printers/tables/table_printer_base.py` & `cycode-1.9.6.dev3/cycode/cli/printers/tables/table_printer_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,21 @@
 
     @staticmethod
     def _print_table(table: 'Table') -> None:
         if table.get_rows():
             click.echo(table.get_table().draw())
 
     @staticmethod
-    def _print_report_urls(local_scan_results: List['LocalScanResult']) -> None:
+    def _print_report_urls(
+        local_scan_results: List['LocalScanResult'],
+        aggregation_report_url: Optional[str] = None,
+    ) -> None:
         report_urls = [scan_result.report_url for scan_result in local_scan_results if scan_result.report_url]
-        if not report_urls:
+        if not report_urls and not aggregation_report_url:
+            return
+        if aggregation_report_url:
+            click.echo(f'Report URL: {aggregation_report_url}')
             return
 
         click.echo('Report URLs:')
         for report_url in report_urls:
             click.echo(f'- {report_url}')
```

### Comparing `cycode-1.9.6.dev2/cycode/cli/printers/text_printer.py` & `cycode-1.9.6.dev3/cycode/cli/printers/text_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,77 +35,83 @@
     ) -> None:
         if not errors and all(result.issue_detected == 0 for result in local_scan_results):
             click.secho('Good job! No issues were found!!! 👏👏👏', fg=self.GREEN_COLOR_NAME)
             return
 
         for local_scan_result in local_scan_results:
             for document_detections in local_scan_result.document_detections:
-                self._print_document_detections(
-                    document_detections, local_scan_result.scan_id, local_scan_result.report_url
-                )
+                self._print_document_detections(document_detections, local_scan_result.scan_id)
 
+        report_urls = [scan_result.report_url for scan_result in local_scan_results if scan_result.report_url]
+
+        self._print_report_urls(report_urls, self.context.obj.get('aggregation_report_url'))
         if not errors:
             return
 
         click.secho(
             'Unfortunately, Cycode was unable to complete the full scan. '
             'Please note that not all results may be available:',
             fg='red',
         )
         for scan_id, error in errors.items():
             click.echo(f'- {scan_id}: ', nl=False)
             self.print_error(error)
 
-    def _print_document_detections(
-        self, document_detections: DocumentDetections, scan_id: str, report_url: Optional[str]
-    ) -> None:
+    def _print_document_detections(self, document_detections: DocumentDetections, scan_id: str) -> None:
         document = document_detections.document
         lines_to_display = self._get_lines_to_display_count()
         for detection in document_detections.detections:
-            self._print_detection_summary(detection, document.path, scan_id, report_url)
+            self._print_detection_summary(detection, document.path, scan_id)
             self._print_detection_code_segment(detection, document, lines_to_display)
 
-    def _print_detection_summary(
-        self, detection: Detection, document_path: str, scan_id: str, report_url: Optional[str]
-    ) -> None:
+    def _print_detection_summary(self, detection: Detection, document_path: str, scan_id: str) -> None:
         detection_name = detection.type if self.scan_type == SECRET_SCAN_TYPE else detection.message
         detection_name_styled = click.style(detection_name, fg='bright_red', bold=True)
 
         detection_sha = detection.detection_details.get('sha512')
         detection_sha_message = f'\nSecret SHA: {detection_sha}' if detection_sha else ''
 
         scan_id_message = f'\nScan ID: {scan_id}'
-        report_url_message = f'\nReport URL: {report_url}' if report_url else ''
-
         detection_commit_id = detection.detection_details.get('commit_id')
         detection_commit_id_message = f'\nCommit SHA: {detection_commit_id}' if detection_commit_id else ''
 
         company_guidelines = detection.detection_details.get('custom_remediation_guidelines')
         company_guidelines_message = f'\nCompany Guideline: {company_guidelines}' if company_guidelines else ''
 
         click.echo(
             f'⛔  '
             f'Found issue of type: {detection_name_styled} '
             f'(rule ID: {detection.detection_rule_id}) in file: {click.format_filename(document_path)} '
             f'{detection_sha_message}'
             f'{scan_id_message}'
-            f'{report_url_message}'
             f'{detection_commit_id_message}'
             f'{company_guidelines_message}'
             f'  ⛔'
         )
 
     def _print_detection_code_segment(self, detection: Detection, document: Document, code_segment_size: int) -> None:
         if self._is_git_diff_based_scan():
             self._print_detection_from_git_diff(detection, document)
             return
 
         self._print_detection_from_file(detection, document, code_segment_size)
 
     @staticmethod
+    def _print_report_urls(report_urls: List[str], aggregation_report_url: Optional[str] = None) -> None:
+        if not report_urls and not aggregation_report_url:
+            return
+        if aggregation_report_url:
+            click.echo(f'Report URL: {aggregation_report_url}')
+            return
+
+        click.echo('Report URLs:')
+        for report_url in report_urls:
+            click.echo(f'- {report_url}')
+
+    @staticmethod
     def _get_code_segment_start_line(detection_line: int, code_segment_size: int) -> int:
         start_line = detection_line - math.ceil(code_segment_size / 2)
         return 0 if start_line < 0 else start_line
 
     def _print_line_of_code_segment(
         self,
         document: Document,
```

### Comparing `cycode-1.9.6.dev2/cycode/cli/user_settings/base_file_manager.py` & `cycode-1.9.6.dev3/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/user_settings/config_file_manager.py` & `cycode-1.9.6.dev3/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/user_settings/configuration_manager.py` & `cycode-1.9.6.dev3/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/user_settings/credentials_manager.py` & `cycode-1.9.6.dev3/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/user_settings/jwt_creator.py` & `cycode-1.9.6.dev3/cycode/cli/user_settings/jwt_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/utils/get_api_client.py` & `cycode-1.9.6.dev3/cycode/cli/utils/get_api_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/utils/path_utils.py` & `cycode-1.9.6.dev3/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/utils/progress_bar.py` & `cycode-1.9.6.dev3/cycode/cli/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/utils/scan_batch.py` & `cycode-1.9.6.dev3/cycode/cli/utils/scan_batch.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/utils/shell_executor.py` & `cycode-1.9.6.dev3/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/utils/string_utils.py` & `cycode-1.9.6.dev3/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/utils/task_timer.py` & `cycode-1.9.6.dev3/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cli/utils/yaml_utils.py` & `cycode-1.9.6.dev3/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/auth_client.py` & `cycode-1.9.6.dev3/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/client_creator.py` & `cycode-1.9.6.dev3/cycode/cyclient/client_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/config.py` & `cycode-1.9.6.dev3/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/cycode_client_base.py` & `cycode-1.9.6.dev3/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/cycode_dev_based_client.py` & `cycode-1.9.6.dev3/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/cycode_token_based_client.py` & `cycode-1.9.6.dev3/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/headers.py` & `cycode-1.9.6.dev3/cycode/cyclient/headers.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/models.py` & `cycode-1.9.6.dev3/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/report_client.py` & `cycode-1.9.6.dev3/cycode/cyclient/report_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/scan_client.py` & `cycode-1.9.6.dev3/cycode/cyclient/scan_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         return ''
 
     def get_scan_service_url_path(
         self, scan_type: str, should_use_scan_service: bool = False, should_use_sync_flow: bool = False
     ) -> str:
         service_path = self.scan_config.get_service_name(scan_type, should_use_scan_service)
-        controller_path = self.get_scan_controller_path(scan_type)
+        controller_path = self.get_scan_controller_path(scan_type, should_use_scan_service)
         flow_type = self.get_scan_flow_type(should_use_sync_flow)
         return f'{service_path}/{controller_path}{flow_type}'
 
     def content_scan(self, scan_type: str, file_name: str, content: str, is_git_diff: bool = True) -> models.ScanResult:
         path = f'{self.get_scan_service_url_path(scan_type)}/content'
         body = {'name': file_name, 'content': content, 'is_git_diff': is_git_diff}
         response = self.scan_cycode_client.post(
@@ -88,14 +88,20 @@
 
         return self.parse_zipped_file_scan_response(response)
 
     def get_scan_report_url(self, scan_id: str, scan_type: str) -> models.ScanReportUrlResponse:
         response = self.scan_cycode_client.get(url_path=self.get_scan_report_url_path(scan_id, scan_type))
         return models.ScanReportUrlResponseSchema().build_dto(response.json())
 
+    def get_scan_aggregation_report_url(self, aggregation_id: str, scan_type: str) -> models.ScanReportUrlResponse:
+        response = self.scan_cycode_client.get(
+            url_path=self.get_scan_aggregation_report_url_path(aggregation_id, scan_type)
+        )
+        return models.ScanReportUrlResponseSchema().build_dto(response.json())
+
     def get_zipped_file_scan_async_url_path(self, scan_type: str, should_use_sync_flow: bool = False) -> str:
         async_scan_type = self.scan_config.get_async_scan_type(scan_type)
         async_entity_type = self.scan_config.get_async_entity_type(scan_type)
         scan_service_url_path = self.get_scan_service_url_path(
             scan_type, should_use_scan_service=True, should_use_sync_flow=should_use_sync_flow
         )
         return f'{scan_service_url_path}/{async_scan_type}/{async_entity_type}'
@@ -151,14 +157,20 @@
 
     def get_scan_details_path(self, scan_type: str, scan_id: str) -> str:
         return f'{self.get_scan_service_url_path(scan_type, should_use_scan_service=True)}/{scan_id}'
 
     def get_scan_report_url_path(self, scan_id: str, scan_type: str) -> str:
         return f'{self.get_scan_service_url_path(scan_type, should_use_scan_service=True)}/reportUrl/{scan_id}'
 
+    def get_scan_aggregation_report_url_path(self, aggregation_id: str, scan_type: str) -> str:
+        return (
+            f'{self.get_scan_service_url_path(scan_type, should_use_scan_service=True)}'
+            f'/reportUrlByAggregationId/{aggregation_id}'
+        )
+
     def get_scan_details(self, scan_type: str, scan_id: str) -> models.ScanDetailsResponse:
         path = self.get_scan_details_path(scan_type, scan_id)
         response = self.scan_cycode_client.get(url_path=path)
         return models.ScanDetailsResponseSchema().load(response.json())
 
     def get_detection_rules_path(self) -> str:
         return (
```

### Comparing `cycode-1.9.6.dev2/cycode/cyclient/scan_config_base.py` & `cycode-1.9.6.dev3/cycode/cyclient/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev2/pyproject.toml` & `cycode-1.9.6.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "1.9.6.dev2" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "1.9.6.dev3" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning."
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-1.9.6.dev2/PKG-INFO` & `cycode-1.9.6.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 1.9.6.dev2
+Version: 1.9.6.dev3
 Summary: Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning.
 Home-page: https://github.com/cycodehq/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.13
```

