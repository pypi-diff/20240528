# Comparing `tmp/snowflake_cli_labs-2.3.1.tar.gz` & `tmp/snowflake_cli_labs-2.4.0rc0.tar.gz`

## Comparing `snowflake_cli_labs-2.3.1.tar` & `snowflake_cli_labs-2.4.0rc0.tar`

### file list

```diff
@@ -1,582 +1,628 @@
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    17608 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/RELEASE-NOTES.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/SECURITY.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/conftest.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/performance_history_analysis.py
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_5.png
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/scripts/main.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/snyk/dependency-sync.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/snyk/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/cli_global_context.py
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/config.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/constants.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/exceptions.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/feature_flags.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/secure_path.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/secure_utils.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/sql_execution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/alias.py
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/decorators.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/experimental_behaviour.py
--rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/flags.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/project_initialisation.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/snow_typer.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/__init__.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/abc.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/console.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/output/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/output/formats.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/output/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/plugin_config.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/command/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/__init__.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/definition.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/definition_manager.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/errors.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/project_definition.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/updatable_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/__init__.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/application.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/native_app.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/package.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/argument.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/callable.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/cursor.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/error_handling.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/naming_utils.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/path_utils.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/rendering.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/types.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/__main__.py
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/cli_app.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/constants.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/loggers.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/main_typer.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/printing.py
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/snow_connector.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/api_impl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/api_impl/plugin/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/builtin_plugins.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/exception_logging.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/threadsafe.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/typer_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/commands_structure.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/pycharm_remote_debug.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/__init__.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/generator.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/__init__.py
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/commands.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/plugin_spec.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/__init__.py
--rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/commands.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/manager.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/__init__.py
--rw-r--r--   0        0        0    10568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/artifacts.py
--rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/commands.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/common_flags.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/constants.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/exceptions.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/feature_flags.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/init.py
--rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/policy.py
--rw-r--r--   0        0        0    13103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/run_processor.py
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/codegen/__init__.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/__init__.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/commands.py
--rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/__init__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/commands.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/manager.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/plugin_spec.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/__init__.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/commands.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/common.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/plugin_spec.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/stage_deprecated/commands.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/__init__.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/commands.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/common.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/manager.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/models.py
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package_utils.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/plugin_spec.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/zipper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/__init__.py
--rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
--rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/commands.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/manager.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/utils.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/common.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/commands.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/commands.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/commands.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/__init__.py
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/commands.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/__init__.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/commands.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/manager.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/plugin_spec.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/snowsql_templating.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/__init__.py
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/commands.py
--rw-r--r--   0        0        0    10645 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/diff.py
--rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/manager.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/__init__.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/commands.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/plugin_spec.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/environment.yml.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/.gitignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/common.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/functions.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/procedures.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/.gitignore
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/environment.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/snowflake.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/common/hello.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/broken_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/failing_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/override_build_in_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/__init__.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/empty_config.toml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_cli.py
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_command_registration.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_common_decorators.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_common_global_context.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_config.py
--rw-r--r--   0        0        0    25851 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_connection.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_experimental_behaviour.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_help_messages.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_loaded_modules.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_logs.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_main.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_performance.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_project_initialisation.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_snow_connector.py
--rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_sql.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_utils.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_zipper.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/__snapshots__/test_config.ambr
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/__snapshots__/test_connection.ambr
--rw-r--r--   0        0        0   554299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/__snapshots__/test_help_messages.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/__init__.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/test_feature_flags.py
--rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/test_secure_path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/__init__.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/test_flags.py
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/test_snow_typer.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/__snapshots__/test_flags.ambr
--rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/__snapshots__/test_snow_typer.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/console/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/console/test_cli_console_output.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/console/test_console_abc.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/console/test_intermediate_output.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/utils/test_naming_utils.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/utils/test_rendering.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/app/test_telemetry.py
--rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/git/test_git_commands.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/git/__snapshots__/test_git_commands.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/patch_utils.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_annotation_processor_config.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_artifacts.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_commands.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_feature_flags.py
--rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_init.py
--rw-r--r--   0        0        0    26124 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_manager.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_package_scripts.py
--rw-r--r--   0        0        0    43980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_run_processor.py
--rw-r--r--   0        0        0    35934 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_teardown_processor.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_utils.py
--rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_version_create_processor.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_version_drop_processor.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/utils.py
--rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/__snapshots__/test_commands.ambr
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/__snapshots__/test_init.ambr
--rw-r--r--   0        0        0    21526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/codegen/test_sandbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/notebook/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/notebook/test_notebook_commands.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/notebook/test_notebook_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/test_common.py
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/test_object.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/test_stage.py
--rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/__snapshots__/test_object.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/output/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/output/test_format_silent_enforcement.py
--rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/output/test_printing.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/output/test_silent_output.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/plugin/test_broken_plugin.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/plugin/test_failing_plugin.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/plugin/test_override_by_external_plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/fixtures.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/test_config.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/test_definition_manager.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/test_project_schemas.py
--rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/test_util.py
--rw-r--r--   0        0        0    19829 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/__snapshots__/test_config.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/mocks.py
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_anaconda.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_build.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_common.py
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_function.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_models.py
--rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_package.py
--rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_procedure.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_procedure.ambr
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_common.py
--rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_image_repository.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_jobs.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_registry.py
--rw-r--r--   0        0        0    22547 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_services.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/__snapshots__/test_image_repository.ambr
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/__snapshots__/test_registry.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/stage/__init__.py
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/stage/test_diff.py
--rw-r--r--   0        0        0    30692 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/stage/test_stage.py
--rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/stage/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/streamlit/test_commands.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/streamlit/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/anaconda_channel_data.json
--rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/test_data.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/test_streamlit_requirements.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/configs/broken_plugin_config.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/configs/disabled_override_plugin_config.toml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/configs/failing_plugin_config.toml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/configs/override_plugin_config.toml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure/core/file.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
--rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
--rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
--rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/zendesk/file.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/empty_project/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit/environment.yml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit/pages/my_page.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_defaults/main.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_stage/environment.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/snowflake.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/package/002-shared.sql
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/snowflake.local.yml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/snowflake.yml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/package/002-shared.sql
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/minimal/snowflake.yml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/setup.sql
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/app/streamlit/main.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/no_definition_version/snowflake.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/requirements.txt
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/requirements.txt
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/snowflake.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/requirements.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/environment.yml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/utils/utils.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/underspecified/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/unknown_fields/snowflake.yml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/streamlit/another_file_with_list.yml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/streamlit/another_file_with_single_item.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/streamlit/with_list_in_source_file.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/streamlit/with_single_item.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/conversion.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/files_and_dirs.py
--rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/fixtures.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/result_assertions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/conftest.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/test_error_handling.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/test_installation.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/test_snowpark_examples.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/__snapshots__/test_installation.ambr
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/config/config.toml
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/config/malformatted_config.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__init__.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/conftest.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/snowflake_connector.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_config.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_connection.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_external_plugins.py
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_git.py
--rw-r--r--   0        0        0    30602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_nativeapp.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_notebooks.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_object.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_package.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_session_token.py
--rw-r--r--   0        0        0    28873 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_snowpark.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_snowpark_external_access.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_sql.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_stage.py
--rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_streamlit.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_temporary_connection.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_utils.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_git.ambr
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_sql.ambr
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/config/config_with_enabled_all_external_plugins.toml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/config/connection_configs.toml
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/nativeapp/test_version.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/scripts/integration_account_setup.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/__init__.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_image_repository.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_jobs.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_registry.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_services.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/docker/Dockerfile
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/docker/bootstrap_containers_setup.sh
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/docker/echo_service.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/spec/spec.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/spec/spec_upgrade.yml
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/compute_pool_utils.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/spcs_services_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/sql_multi_queries.sql
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/requirements.txt
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_version_check/.gitignore
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_version_check/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/.gitignore
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_execute/script1.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_execute/script2.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_execute/script3.sql
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_execute/script_template.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/environment.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/snowflake.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/pages/my_page.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/utils/utils.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/naming_utils.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/snowpark_utils.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/sql_utils.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/working_directory_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/assertions/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/assertions/test_file_assertions.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/assertions/test_result_assertions.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/LICENSE
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/README.md
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/pyproject.toml
--rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    20371 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/RELEASE-NOTES.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/SECURITY.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/conftest.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/performance_history_analysis.py
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/docs/images/coverage_5.png
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/scripts/main.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/snyk/dependency-sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/snyk/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/__init__.py
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/cli_global_context.py
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/config.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/constants.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/exceptions.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/feature_flags.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/identifiers.py
+-rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/secure_path.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/secure_utils.py
+-rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/sql_execution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/alias.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/decorators.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/experimental_behaviour.py
+-rw-r--r--   0        0        0    19688 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/flags.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/project_initialisation.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/snow_typer.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/console/__init__.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/console/abc.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/console/console.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/console/enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/output/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/output/formats.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/output/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/plugins/__init__.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/plugins/plugin_config.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/plugins/command/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/__init__.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/definition.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/definition_manager.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/errors.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/identifier_model.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/project_definition.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/native_app/__init__.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/snowpark/argument.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/cursor.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/error_handling.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/naming_utils.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/path_utils.py
+-rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/rendering.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/types.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/__main__.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/cli_app.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/constants.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/loggers.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/main_typer.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/printing.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/snow_connector.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/api_impl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/api_impl/plugin/__init__.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/exception_logging.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py
+-rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/commands_structure.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/docs/__init__.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/docs/generator.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/connection/__init__.py
+-rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/connection/commands.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/connection/plugin_spec.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/connection/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/cortex/__init__.py
+-rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/cortex/commands.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/cortex/constants.py
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/cortex/manager.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/cortex/plugin_spec.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/cortex/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/git/__init__.py
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/git/commands.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/git/manager.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/git/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/__init__.py
+-rw-r--r--   0        0        0    21436 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py
+-rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/feature_flags.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/init.py
+-rw-r--r--   0        0        0    21705 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py
+-rw-r--r--   0        0        0    13139 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py
+-rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/__init__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/artifact_processor.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/compiler.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/snowpark/callback_source.py.jinja
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/snowpark/extension_function_utils.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/snowpark/models.py
+-rw-r--r--   0        0        0    18822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/snowpark/python_processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/version/__init__.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py
+-rw-r--r--   0        0        0    13321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/notebook/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/notebook/commands.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/notebook/exceptions.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/notebook/manager.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/notebook/plugin_spec.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/notebook/types.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/command_aliases.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/commands.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/common.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/plugin_spec.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object_stage_deprecated/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object_stage_deprecated/commands.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object_stage_deprecated/plugin_spec.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/__init__.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/commands.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/common.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/manager.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/models.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/plugin_spec.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package/__init__.py
+-rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
+-rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package/utils.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/common.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
+-rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
+-rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/jobs/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/services/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/sql/__init__.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/sql/commands.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/sql/manager.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/sql/plugin_spec.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/sql/snowsql_templating.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/stage/__init__.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/stage/commands.py
+-rw-r--r--   0        0        0    10681 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/stage/diff.py
+-rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/stage/manager.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/stage/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/streamlit/__init__.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/streamlit/commands.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/streamlit/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/streamlit/plugin_spec.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/environment.yml.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/.gitignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/requirements.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/app/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/app/common.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/app/functions.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_streamlit/.gitignore
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_streamlit/environment.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_streamlit/snowflake.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_streamlit/common/hello.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/broken_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/failing_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/multilingual_hello_command_group/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/override_build_in_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/snowpark_hello_single_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/empty_config.toml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_cli.py
+-rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_command_registration.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_common_decorators.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_common_global_context.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_config.py
+-rw-r--r--   0        0        0    25837 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_connection.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_experimental_behaviour.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_help_messages.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_loaded_modules.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_logs.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_main.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_performance.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_project_initialisation.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_snow_connector.py
+-rw-r--r--   0        0        0    13250 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_sql.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_utils.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_zipper.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/__snapshots__/test_config.ambr
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/__snapshots__/test_connection.ambr
+-rw-r--r--   0        0        0   797489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/__snapshots__/test_help_messages.ambr
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/__snapshots__/test_sql.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/__init__.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/test_feature_flags.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/test_fqn.py
+-rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/test_secure_path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/commands/__init__.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/commands/test_flags.py
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/commands/test_snow_typer.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/commands/__snapshots__/test_flags.ambr
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/console/__init__.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/console/test_cli_console_output.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/console/test_console_abc.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/console/test_intermediate_output.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/utils/test_naming_utils.py
+-rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/api/utils/test_rendering.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/app/test_telemetry.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/cortex/test_cortex_commands.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/cortex/__snapshots__/test_cortex_commands.ambr
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/git/test_git_commands.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/git/__snapshots__/test_git_commands.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/patch_utils.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_annotation_processor_config.py
+-rw-r--r--   0        0        0    32867 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_artifacts.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_commands.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_feature_flags.py
+-rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_init.py
+-rw-r--r--   0        0        0    26124 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_manager.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_package_scripts.py
+-rw-r--r--   0        0        0    43980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_run_processor.py
+-rw-r--r--   0        0        0    38854 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_teardown_processor.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_utils.py
+-rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_version_create_processor.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_version_drop_processor.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/utils.py
+-rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/__snapshots__/test_init.ambr
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/codegen/test_compiler.py
+-rw-r--r--   0        0        0    21601 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/codegen/test_sandbox.py
+-rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/codegen/snowpark/test_extension_function_utils.py
+-rw-r--r--   0        0        0    17474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/codegen/snowpark/test_python_processor.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/codegen/snowpark/__snapshots__/test_extension_function_utils.ambr
+-rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/nativeapp/codegen/snowpark/__snapshots__/test_python_processor.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/notebook/__init__.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/notebook/test_notebook_commands.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/notebook/test_notebook_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/object/__init__.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/object/test_common.py
+-rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/object/test_object.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/object/test_stage.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/object/__snapshots__/test_object.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/output/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/output/test_format_silent_enforcement.py
+-rw-r--r--   0        0        0     9869 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/output/test_printing.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/output/test_silent_output.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/plugin/test_broken_plugin.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/plugin/test_failing_plugin.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/plugin/test_override_by_external_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/project/__init__.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/project/fixtures.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/project/test_config.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/project/test_definition_manager.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/project/test_project_schemas.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/project/test_util.py
+-rw-r--r--   0        0        0    20425 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/project/__snapshots__/test_config.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/mocks.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_anaconda.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_build.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_common.py
+-rw-r--r--   0        0        0    12234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_function.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_models.py
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_package.py
+-rw-r--r--   0        0        0    14841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_procedure.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/test_common.py
+-rw-r--r--   0        0        0    17009 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0    10029 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/test_image_repository.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/test_jobs.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/test_registry.py
+-rw-r--r--   0        0        0    23264 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/test_services.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/spcs/__snapshots__/test_registry.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/stage/__init__.py
+-rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/stage/test_diff.py
+-rw-r--r--   0        0        0    31388 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/stage/test_stage.py
+-rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/stage/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0    24012 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/streamlit/test_commands.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/streamlit/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/anaconda_channel_data.json
+-rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/test_data.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/test_streamlit_requirements.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/configs/broken_plugin_config.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/configs/disabled_override_plugin_config.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/configs/failing_plugin_config.toml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/configs/override_plugin_config.toml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/cortex/conversation.json
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/cortex/short_english_text.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure/core/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
+-rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/zendesk/file.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/deploy_root_with_incorrect_setup_script/manifest.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/deploy_root_with_incorrect_setup_script/setup_script.sql
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/deploy_root_with_manifest_artifacts/manifest.yml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/deploy_root_without_manifest_artifacts/manifest.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/empty_project/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit/environment.yml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit_no_defaults/main.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit_no_stage/environment.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration/snowflake.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration/package/002-shared.sql
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration_external/snowflake.local.yml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration_external/snowflake.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration_external/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration_external/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration_external/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration_external/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration_external/package/002-shared.sql
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/minimal/snowflake.yml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_1/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_1/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_1/setup.sql
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_1/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_1/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_1/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/main.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/no_definition_version/snowflake.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_external_access/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_external_access/requirements.txt
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_functions/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_functions/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_functions/requirements.txt
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_functions/snowflake.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures/requirements.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/sql_templating/snowflake.local.yml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/sql_templating/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/streamlit_full_definition/environment.yml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/streamlit_full_definition/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/streamlit_full_definition/utils/utils.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/underspecified/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/unknown_fields/snowflake.yml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/streamlit/another_file_with_list.yml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/streamlit/another_file_with_single_item.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/streamlit/with_list_in_source_file.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/test_data/streamlit/with_single_item.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/testing_utils/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/testing_utils/conversion.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/testing_utils/files_and_dirs.py
+-rw-r--r--   0        0        0    10538 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/testing_utils/fixtures.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests/testing_utils/result_assertions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_e2e/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_e2e/conftest.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_e2e/test_error_handling.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_e2e/test_installation.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_e2e/test_snowpark_examples.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_e2e/__snapshots__/test_installation.ambr
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_e2e/config/config.toml
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_e2e/config/malformatted_config.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/__init__.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/conftest.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/snowflake_connector.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_config.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_connection.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_cortex.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_external_plugins.py
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_git.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_object.py
+-rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_package.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_session_token.py
+-rw-r--r--   0        0        0    29483 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_snowpark.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_snowpark_external_access.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_sql.py
+-rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_stage.py
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_streamlit.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_temporary_connection.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_utils.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/__snapshots__/test_git.ambr
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/__snapshots__/test_sql.ambr
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/config/config_with_enabled_all_external_plugins.toml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/config/connection_configs.toml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/nativeapp/test_bundle.py
+-rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/nativeapp/test_deploy.py
+-rw-r--r--   0        0        0    13808 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/nativeapp/test_init_run.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/nativeapp/test_teardown.py
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/nativeapp/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/notebook/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/notebook/test_notebooks.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/scripts/integration_account_setup.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/__init__.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_image_repository.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_jobs.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_registry.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_services.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/docker/Dockerfile
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/docker/bootstrap_containers_setup.sh
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/docker/echo_service.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/spec/spec.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/spec/spec_upgrade.yml
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/empty.sql
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/sql_multi_queries.sql
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/cortex/conversation.json
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/cortex/english_text.txt
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/notebook/my_notebook.ipynb
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark/requirements.txt
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_coverage/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_external_access/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_version_check/.gitignore
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_version_check/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_import/.gitignore
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/stage_execute/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/stage_execute/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/stage_execute/script3.sql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/stage_execute/script_template.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/streamlit/environment.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/streamlit/snowflake.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/streamlit/utils/utils.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/naming_utils.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/snowpark_utils.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/sql_utils.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/working_directory_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/assertions/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/assertions/test_file_assertions.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/LICENSE
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/README.md
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    16967 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.4.0rc0/PKG-INFO
```

### Comparing `snowflake_cli_labs-2.3.1/.pre-commit-config.yaml` & `snowflake_cli_labs-2.4.0rc0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,16 @@
           (?x)
           ^src/snowflake/cli/api/console/.*$|
           ^src/snowflake/cli/app/printing.py$|
           ^src/snowflake/cli/app/dev/.*$|
           ^src/snowflake/cli/templates/.*$|
           ^src/snowflake/cli/api/utils/rendering.py$|
           ^src/snowflake/cli/plugins/spcs/common.py$|
-          ^src/snowflake/cli/plugins/snowpark/venv.py$
+          ^src/snowflake/cli/plugins/snowpark/venv.py$|
+          ^src/snowflake/cli/app/cli_app.py$
       - id: check-app-imports-in-api
         language: pygrep
         name: "No top level cli.app imports in cli.api"
         entry: "^from snowflake\\.cli\\.app"
         pass_filenames: true
         files: ^src/snowflake/cli/api/.*\.py$
       - id: avoid-snowcli
```

### Comparing `snowflake_cli_labs-2.3.1/CONTRIBUTING.md` & `snowflake_cli_labs-2.4.0rc0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 The user requires a default role with the following grants
 
 ```snowflake
 grant create database on account to role <role_name>;
 grant create role on account to role <role_name>;
 grant usage on warehouse xsmall to role <role_name>;
 grant operate on warehouse xsmall to role <role_name>;
+grant create database on account to role <role_name> with grant option;
 ```
 
 ## Remote debugging with PyCharm or IntelliJ
 
 Snowflake CLI can connect to a remote debug server started in PyCharm or Intellij.
 It allows you to debug any installation of our tool in one of mentioned IDEs.
```

### Comparing `snowflake_cli_labs-2.3.1/RELEASE-NOTES.md` & `snowflake_cli_labs-2.4.0rc0/RELEASE-NOTES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,64 @@
-# v2.3.1
+# Unreleased version
+## Backward incompatibility
+
+## Deprecations
+
+## New additions
+
+## Fixes and improvements
+
+
+# v2.4.0
 ## Backward incompatibility
 
 ## Deprecations
 
 ## New additions
+* Added the `--cascade` option to `snow app teardown` command that drops all application objects owned by the application.
+ * Add external access integration to snow object commands
+ * Add aliases for `snow object list/describe/drop` commands under:
+   * `snow stage` for stages
+   * `snow git` for git repository stages
+   * `snow streamlit` for streamlit apps
+   * `snow snowpark` for procedures and functions
+   * `snow spcs compute-pool` for compute pools
+   * `snow spcs image-repository` for image repositories
+   * `snow spcs service` for services
+ * `snow sql` works now with `snowflake.yml` file. The variables defined in the new `env` section
+       of `snowflake.yml` will be used to expand templates.
+ * `snow sql` support executing multiple files. Users can use `-f/--file` flag more than once to execute queries
+      from many files.
+ * `snow git execute` and `snow stage execute` support passing input variables for SQL execution.
+* Added `snow cortex` commands:
+    * `complete` - Given a prompt, the command generates a response using your choice of language model.
+      In the simplest use case, the prompt is a single string. You may also provide a JSON file with conversation history including multiple prompts and responses for interactive chat-style usage.
+    * `extract-answer` - Extracts an answer to a given question from a text document.
+      The document may be a plain-English document or a string representation of a semi-structured (JSON) data object.
+    * `sentiment` - Returns sentiment as a score between -1 to 1 (with -1 being the most negative and 1 the most positive, with values around 0 neutral) for the given English-language input text.
+    * `summarize` - Summarizes the given English-language input text.
+    * `translate` - Translates text from the indicated or detected source language to a target language.
+    * `search`    - for integration with Cortex Search Service
+* When invoked without command help is displayed by default with list of available commands.
+* Add tab-completion for `snow` command.
 
 ## Fixes and improvements
 * Improved support for quoted identifiers.
+* Fixed creating patches with `snow app version create` when there are 2 or more existing patches on a version
+* Using `--format=json` adds trailing new line to avoid `%` being added by some terminals to signal no new line at the end of output.
+* Fixed `--interactive` flag to be enabled by default in interactive environments and added the `--no-interactive` flag to be able to turn off prompting.
+
+# v2.3.1
+## Backward incompatibility
+
+## Deprecations
+
+## New additions
+
+## Fixes and improvements
 * Fixed bugs in source artifact mapping logic for native applications
 
 # v2.3.0
 
 ## Backward incompatibility
 
 ## Deprecations
@@ -27,14 +75,15 @@
 * More human-friendly errors in case of corrupted `config.toml` file.
 * Fixed a bug in `snow app` that caused files to be re-uploaded unnecessarily.
 * Optimize snowpark dependency search to lower the size of .zip artifacts and
   the number of anaconda dependencies for snowpark projects.
 * Added support for fully qualified stage names in stage and git execute commands.
 * Fixed a bug where `snow app run` was not upgrading the application when the local state and remote stage are identical (for example immediately after `snow app deploy`).
 * Fixed handling of stage path separators on Windows
+* Change to `external_access_integrations` in `snowflake.yml` now also triggers function replace
 * The `--info` callback returns info about configured feature flags.
 
 # v2.2.0
 
 ## Backward incompatibility
 
 ## Deprecations
```

### Comparing `snowflake_cli_labs-2.3.1/conftest.py` & `snowflake_cli_labs-2.4.0rc0/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/performance_history_analysis.py` & `snowflake_cli_labs-2.4.0rc0/performance_history_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 from decimal import Decimal
 from timeit import default_timer as timer
 from typing import List, Optional, Tuple
 
 import typer
 from git import Commit, Repo
```

### Comparing `snowflake_cli_labs-2.3.1/docs/images/coverage_1.png` & `snowflake_cli_labs-2.4.0rc0/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/docs/images/coverage_2.png` & `snowflake_cli_labs-2.4.0rc0/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/docs/images/coverage_3.png` & `snowflake_cli_labs-2.4.0rc0/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/docs/images/coverage_4.png` & `snowflake_cli_labs-2.4.0rc0/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/docs/images/coverage_5.png` & `snowflake_cli_labs-2.4.0rc0/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/scripts/main.py` & `snowflake_cli_labs-2.4.0rc0/scripts/main.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/__init__.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Optional
 
 from snowflake.cli.api.plugins.plugin_config import PluginConfigProvider
 
 
 class Api:
     def __init__(
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/cli_global_context.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/cli_global_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import re
 from pathlib import Path
 from typing import Dict, Optional
 
 from snowflake.cli.api.exceptions import InvalidSchemaError
 from snowflake.cli.api.output.formats import OutputFormat
+from snowflake.cli.api.project.schemas.project_definition import ProjectDefinition
 from snowflake.connector import SnowflakeConnection
 
 schema_pattern = re.compile(r".+\..+")
 
 
 class _ConnectionContext:
     def __init__(self):
@@ -277,14 +280,18 @@
         self._manager = manager
 
     @property
     def connection(self) -> SnowflakeConnection:
         return self._manager.connection
 
     @property
+    def connection_context(self) -> _ConnectionContext:
+        return self._manager.connection_context
+
+    @property
     def enable_tracebacks(self) -> bool:
         return self._manager.enable_tracebacks
 
     @property
     def output_format(self) -> OutputFormat:
         return self._manager.output_format
 
@@ -293,15 +300,15 @@
         return self._manager.verbose
 
     @property
     def experimental(self) -> bool:
         return self._manager.experimental
 
     @property
-    def project_definition(self):
+    def project_definition(self) -> ProjectDefinition | None:
         return self._manager.project_definition
 
     @property
     def project_root(self):
         return self._manager.project_root
 
     @property
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/config.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/constants.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 
 
 class ObjectType(Enum):
     COMPUTE_POOL = ObjectNames("compute-pool", "compute pool", "compute pools")
     DATABASE = ObjectNames("database", "database", "databases")
     FUNCTION = ObjectNames("function", "function", "functions")
     INTEGRATION = ObjectNames("integration", "integration", "integrations")
+    EXTERNAL_ACCESS_INTEGRATION = ObjectNames(
+        "external-access-integration",
+        "external access integration",
+        "external access integrations",
+    )
     # JOB = ObjectNames("job", "job", "jobs")
     NETWORK_RULE = ObjectNames("network-rule", "network rule", "network rules")
     PROCEDURE = ObjectNames("procedure", "procedure", "procedures")
     ROLE = ObjectNames("role", "role", "roles")
     SCHEMA = ObjectNames("schema", "schema", "schemas")
     SERVICE = ObjectNames("service", "service", "services")
     SECRET = ObjectNames("secret", "secret", "secrets")
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/exceptions.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -124,7 +124,19 @@
 
 
 class SchemaNotProvidedError(ClickException):
     def __init__(self):
         super().__init__(
             "Schema not specified. Please update connection to add `schema` parameter, or re-run command using `--schema` option. Use `snow connection list` to list existing connections."
         )
+
+
+class FQNNameError(ClickException):
+    def __init__(self, name: str):
+        super().__init__(f"Specified name '{name}' is not valid name.")
+
+
+class FQNInconsistencyError(ClickException):
+    def __init__(self, part: str, name: str):
+        super().__init__(
+            f"{part.capitalize()} provided but name '{name}' is fully qualified name."
+        )
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/feature_flags.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/secure_path.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/secure_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import errno
 import logging
 import os
 import shutil
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/secure_utils.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/secure_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/sql_execution.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/sql_execution.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.exceptions import (
     DatabaseNotProvidedError,
     SchemaNotProvidedError,
     SnowflakeSQLExecutionError,
 )
+from snowflake.cli.api.identifiers import FQN
 from snowflake.cli.api.project.util import (
     identifier_to_show_like_pattern,
     unquote_identifier,
 )
 from snowflake.cli.api.utils.cursor import find_first_row
-from snowflake.cli.api.utils.naming_utils import from_qualified_name
 from snowflake.connector.cursor import DictCursor, SnowflakeCursor
 from snowflake.connector.errors import ProgrammingError
 
 
 class SqlExecutionMixin:
     def __init__(self):
         pass
@@ -124,64 +124,30 @@
         self.check_database_and_schema_provided(name)
         return self._execute_query(query, **kwargs)
 
     def check_database_and_schema_provided(self, name: Optional[str] = None) -> None:
         """
         Checks if a database and schema are provided, either through the connection context or a qualified name.
         """
-        if name:
-            _, schema, database = from_qualified_name(name)
-        else:
-            schema, database = None, None
-        schema = schema or self._conn.schema
-        database = database or self._conn.database
-        if not database:
+        fqn = FQN.from_string(name).using_connection(self._conn)
+        if not fqn.database:
             raise DatabaseNotProvidedError()
-        if not schema:
+        if not fqn.schema:
             raise SchemaNotProvidedError()
 
-    def to_fully_qualified_name(
-        self, name: str, database: Optional[str] = None, schema: Optional[str] = None
-    ):
-        current_parts = name.split(".")
-        if len(current_parts) == 3:
-            # already fully qualified name
-            return name.upper()
-
-        if not database:
-            if not self._conn.database:
-                raise DatabaseNotProvidedError()
-            database = self._conn.database
-
-        if len(current_parts) == 2:
-            # we assume name is in form of `schema.object`
-            return f"{database}.{name}".upper()
-
-        schema = schema or self._conn.schema or "public"
-        database = database or self._conn.database
-        return f"{database}.{schema}.{name}".upper()
-
     @staticmethod
-    def get_name_from_fully_qualified_name(name):
-        """
-        Returns name of the object from the fully-qualified name.
-        Assumes that [name] is in format [[database.]schema.]name
-        """
-        return from_qualified_name(name)[0]
-
-    @staticmethod
-    def _qualified_name_to_in_clause(name: str) -> Tuple[str, Optional[str]]:
-        unqualified_name, schema, database = from_qualified_name(name)
-        if database:
-            in_clause = f"in schema {database}.{schema}"
-        elif schema:
-            in_clause = f"in schema {schema}"
+    def _qualified_name_to_in_clause(identifier: FQN) -> Tuple[str, Optional[str]]:
+        if identifier.database:
+            schema = identifier.schema or "PUBLIC"
+            in_clause = f"in schema {identifier.database}.{schema}"
+        elif identifier.schema:
+            in_clause = f"in schema {identifier.schema}"
         else:
             in_clause = None
-        return unqualified_name, in_clause
+        return identifier.name, in_clause
 
     class InClauseWithQualifiedNameError(ValueError):
         def __init__(self):
             super().__init__("non-empty 'in_clause' passed with qualified 'name'")
 
     def show_specific_object(
         self,
@@ -198,15 +164,17 @@
 
         Note that this command is analogous to describe and should only return a single row.
         If the target object type is a schema level object, then check_schema should be set to True
         so that the function will verify that a database and schema are provided, either through
         the connection or a qualified name, before executing the query.
         """
 
-        unqualified_name, name_in_clause = self._qualified_name_to_in_clause(name)
+        unqualified_name, name_in_clause = self._qualified_name_to_in_clause(
+            FQN.from_string(name)
+        )
         if in_clause and name_in_clause:
             raise self.InClauseWithQualifiedNameError()
         elif name_in_clause:
             in_clause = name_in_clause
         show_obj_query = f"show {object_type_plural} like {identifier_to_show_like_pattern(unqualified_name)} {in_clause}".strip()
 
         if check_schema:
@@ -226,15 +194,7 @@
             )
 
         show_obj_row = find_first_row(
             show_obj_cursor,
             lambda row: row[name_col] == unquote_identifier(unqualified_name),
         )
         return show_obj_row
-
-    def qualified_name_for_url(
-        self, object_name: str, database: str | None = None, schema: str | None = None
-    ):
-        fqn = self.to_fully_qualified_name(
-            object_name, database=database, schema=schema
-        )
-        return ".".join(unquote_identifier(part) for part in fqn.split("."))
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/decorators.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     SessionTokenOption,
     SilentOption,
     TemporaryConnectionOption,
     UserOption,
     VerboseOption,
     WarehouseOption,
     experimental_option,
-    project_definition_option,
+    project_type_option,
 )
 from snowflake.cli.api.exceptions import CommandReturnTypeError
 from snowflake.cli.api.output.formats import OutputFormat
 from snowflake.cli.api.output.types import CommandResult
 
 
 def global_options(func: Callable):
@@ -63,15 +63,15 @@
         return _options_decorator_factory(
             func,
             additional_options=[
                 inspect.Parameter(
                     "project_definition",
                     inspect.Parameter.KEYWORD_ONLY,
                     annotation=Optional[str],
-                    default=project_definition_option(project_name),
+                    default=project_type_option(project_name),
                 )
             ],
         )
 
     return _decorator
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/flags.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/flags.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Any, Callable, List, Optional, Tuple
 
 import click
 import typer
 from click import ClickException
 from snowflake.cli.api.cli_global_context import cli_context_manager
 from snowflake.cli.api.console import cli_console
+from snowflake.cli.api.exceptions import MissingConfiguration
 from snowflake.cli.api.output.formats import OutputFormat
 
 DEFAULT_CONTEXT_SETTINGS = {"help_option_names": ["--help", "-h"]}
 
 _CONNECTION_SECTION = "Connection configuration"
 _CLI_BEHAVIOUR = "Global configuration"
 
@@ -412,15 +413,14 @@
 )
 
 VariablesOption = typer.Option(
     None,
     "--variable",
     "-D",
     help="Variables for the template. For example: `-D \"<key>=<value>\"`, string values must be in `''`.",
-    hidden=True,
     show_default=False,
 )
 
 
 def like_option(help_example: str):
     return typer.Option(
         "%%",
@@ -465,25 +465,29 @@
         is_flag=True,
         rich_help_panel=_CLI_BEHAVIOUR,
     )
 
 
 def identifier_argument(sf_object: str, example: str) -> typer.Argument:
     return typer.Argument(
-        ..., help=f"Identifier of the {sf_object}. For example: {example}"
+        ...,
+        help=f"Identifier of the {sf_object}. For example: {example}",
+        show_default=False,
     )
 
 
 def execution_identifier_argument(sf_object: str, example: str) -> typer.Argument:
     return typer.Argument(
-        ..., help=f"Execution identifier of the {sf_object}. For example: {example}"
+        ...,
+        help=f"Execution identifier of the {sf_object}. For example: {example}",
+        show_default=False,
     )
 
 
-def project_definition_option(project_name: str):
+def project_type_option(project_name: str):
     from snowflake.cli.api.exceptions import NoProjectDefinitionError
     from snowflake.cli.api.project.definition_manager import DefinitionManager
 
     def _callback(project_path: Optional[str]):
         dm = DefinitionManager(project_path)
         project_definition = getattr(dm.project_definition, project_name, None)
         project_root = dm.project_root
@@ -511,14 +515,55 @@
         help=f"Path where the {project_name_help} project resides. "
         f"Defaults to current working directory.",
         callback=_callback,
         show_default=False,
     )
 
 
+def project_definition_option(optional: bool = False):
+    from snowflake.cli.api.project.definition_manager import DefinitionManager
+
+    def _callback(project_path: Optional[str]):
+        try:
+            dm = DefinitionManager(project_path)
+            project_definition = dm.project_definition
+            project_root = dm.project_root
+        except MissingConfiguration:
+            if optional:
+                project_definition = None
+                project_root = None
+            else:
+                raise
+        cli_context_manager.set_project_definition(project_definition)
+        cli_context_manager.set_project_root(project_root)
+        return project_definition
+
+    return typer.Option(
+        None,
+        "-p",
+        "--project",
+        help=f"Path where Snowflake project resides. Defaults to current working directory.",
+        callback=_callback,
+        show_default=False,
+    )
+
+
+def readable_file_option(param_name: str, help_str: str) -> typer.Option:
+    return typer.Option(
+        None,
+        param_name,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        help=help_str,
+        show_default=False,
+    )
+
+
 def deprecated_flag_callback(msg: str):
     def _warning_callback(ctx: click.Context, param: click.Parameter, value: Any):
         if ctx.get_parameter_source(param.name) != click.core.ParameterSource.DEFAULT:  # type: ignore[attr-defined]
             cli_console.warning(message=msg)
         return value
 
     return _warning_callback
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/project_initialisation.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/project_initialisation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/snow_typer.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/commands/snow_typer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 class SnowTyper(typer.Typer):
     def __init__(self, /, **kwargs):
         super().__init__(
             **kwargs,
             context_settings=DEFAULT_CONTEXT_SETTINGS,
             pretty_exceptions_show_locals=False,
+            no_args_is_help=True,
+            add_completion=True,
         )
 
     @wraps(typer.Typer.command)
     def command(
         self,
         name: Optional[str] = None,
         requires_global_options: bool = True,
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/abc.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/console/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from typing import Callable, Iterator, Optional
 
 from rich import print as rich_print
 from rich.text import Text
 from snowflake.cli.api.cli_global_context import _CliGlobalContextAccess, cli_context
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/console.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/console/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,20 @@
         """A context manager for organising steps into logical group."""
         if self.in_phase:
             raise CliConsoleNestingProhibitedError("Only one phase allowed at a time.")
 
         self._print(self._format_message(enter_message, Output.PHASE))
         self._in_phase = True
 
-        yield self.step
-
-        self._in_phase = False
-        if exit_message:
-            self._print(self._format_message(exit_message, Output.PHASE))
+        try:
+            yield self.step
+        finally:
+            self._in_phase = False
+            if exit_message:
+                self._print(self._format_message(exit_message, Output.PHASE))
 
     def step(self, message: str):
         """Displays a message to output.
 
         If called within a phase, the output will be indented.
         """
         text = self._format_message(message, Output.STEP)
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/output/types.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/output/types.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/command/__init__.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/plugins/command/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from typing import List
 
 import click
 import pluggy
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/definition.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from typing import List
 
 import yaml.loader
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB
 from snowflake.cli.api.project.schemas.project_definition import ProjectDefinition
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/definition_manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/definition_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/errors.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from pydantic import ValidationError
 
 
 class SchemaValidationError(Exception):
     generic_message = "For field {loc} you provided '{loc}'. This caused: {msg}"
     message_templates = {
-        "string_type": "{msg} for field '{loc}', you provided '{input}'",
-        "extra_forbidden": "{msg}. You provided field '{loc}' with value '{input}' that is not present in the schema",
+        "string_type": "{msg} for field '{loc}', you provided '{input}'.",
+        "extra_forbidden": "{msg}. You provided field '{loc}' with value '{input}' that is not supported in given version.",
         "missing": "Your project definition is missing following fields: {loc}",
     }
 
     def __init__(self, error: ValidationError):
         errors = error.errors()
-        message = f"During evaluation of {error.title} schema following errors were encountered:\n"
+        message = f"During evaluation of {error.title} in project definition following errors were encountered:\n"
         message += "\n".join(
             [
                 self.message_templates.get(e["type"], self.generic_message).format(**e)
                 for e in errors
             ]
         )
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/util.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import codecs
 import os
 import re
 from typing import Optional
 
 IDENTIFIER = r'((?:"[^"]*(?:""[^"]*)*")|(?:[A-Za-z_][\w$]{0,254}))'
 IDENTIFIER_NO_LENGTH = r'((?:"[^"]*(?:""[^"]*)*")|(?:[A-Za-z_][\w$]*))'
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/updatable_model.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any, Dict
 
 from pydantic import BaseModel, ConfigDict, Field, ValidationError
 from snowflake.cli.api.project.errors import SchemaValidationError
 from snowflake.cli.api.project.util import IDENTIFIER_NO_LENGTH
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/application.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/native_app.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     artifacts: List[Union[PathMapping, str]] = Field(
         title="List of file source and destination pairs to add to the deploy root",
     )
     deploy_root: Optional[str] = Field(
         title="Folder at the root of your project where the build step copies the artifacts.",
         default="output/deploy/",
     )
+    generated_root: Optional[str] = Field(
+        title="Subdirectory of the deploy root where files generated by the Snowflake CLI will be written.",
+        default="__generated/",
+    )
     source_stage: Optional[str] = Field(
         title="Identifier of the stage that stores the application artifacts.",
         default="app_src.stage",
     )
     package: Optional[Package] = Field(title="PackageSchema", default=None)
     application: Optional[Application] = Field(title="Application info", default=None)
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/package.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/callable.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,20 @@
+from __future__ import annotations
+
 from typing import Dict, List, Optional, Union
 
 from pydantic import Field, field_validator
+from snowflake.cli.api.project.schemas.identifier_model import ObjectIdentifierModel
 from snowflake.cli.api.project.schemas.snowpark.argument import Argument
 from snowflake.cli.api.project.schemas.updatable_model import (
-    IdentifierField,
     UpdatableModel,
 )
 
 
-class Callable(UpdatableModel):
-    name: str = Field(
-        title="Object identifier"
-    )  # TODO: implement validator. If a name is filly qualified, database and schema cannot be specified
-    database: Optional[str] = IdentifierField(
-        title="Name of the database for the function or procedure", default=None
-    )
-
-    schema_name: Optional[str] = IdentifierField(
-        title="Name of the schema for the function or procedure",
-        default=None,
-        alias="schema",
-    )
+class _CallableBase(UpdatableModel):
     handler: str = Field(
         title="Function’s or procedure’s implementation of the object inside source module",
         examples=["functions.hello_function"],
     )
     returns: str = Field(
         title="Type of the result"
     )  # TODO: again, consider Literal/Enum
@@ -51,16 +41,17 @@
     @classmethod
     def convert_runtime(cls, runtime_input: Union[str, float]) -> str:
         if isinstance(runtime_input, float):
             return str(runtime_input)
         return runtime_input
 
 
-class FunctionSchema(Callable):
+class FunctionSchema(_CallableBase, ObjectIdentifierModel(object_name="function")):  # type: ignore
     pass
 
 
-class ProcedureSchema(Callable):
+class ProcedureSchema(_CallableBase, ObjectIdentifierModel(object_name="procedure")):  # type: ignore
     execute_as_caller: Optional[bool] = Field(
-        title="Determine whether the procedure is executed with the privileges of the owner (you) or with the privileges of the caller",
+        title="Determine whether the procedure is executed with the privileges of "
+        "the owner (you) or with the privileges of the caller",
         default=False,
     )
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 from pydantic import Field
+from snowflake.cli.api.project.schemas.identifier_model import ObjectIdentifierModel
 from snowflake.cli.api.project.schemas.updatable_model import UpdatableModel
 
 
-class Streamlit(UpdatableModel):
-    name: str = Field(title="App identifier")
+class Streamlit(UpdatableModel, ObjectIdentifierModel(object_name="Streamlit")):  # type: ignore
     stage: Optional[str] = Field(
         title="Stage in which the app’s artifacts will be stored", default="streamlit"
     )
     query_warehouse: str = Field(
         title="Snowflake warehouse to host the app", default="streamlit"
     )
     main_file: Optional[str] = Field(
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/cursor.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/cursor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Callable, List, Optional
 
 from snowflake.connector.cursor import DictCursor
 
 
 def _rows_generator(cursor: DictCursor, predicate: Callable[[dict], bool]):
     return (row for row in cursor.fetchall() if predicate(row))
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/path_utils.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/types.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/api/utils/types.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/cli_app.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/cli_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,16 +128,17 @@
         print_result(result, output_format=OutputFormat.JSON)
         _exit_with_cleanup()
 
 
 def app_factory() -> SnowCliMainTyper:
     app = SnowCliMainTyper()
 
-    @app.callback()
+    @app.callback(invoke_without_command=True)
     def default(
+        ctx: typer.Context,
         version: bool = typer.Option(
             None,
             "--version",
             help="Shows version of the Snowflake CLI",
             callback=_version_callback,
             is_eager=True,
         ),
@@ -213,14 +214,16 @@
             is_eager=True,
             callback=_commands_registration_callback,
         ),
     ) -> None:
         """
         Snowflake CLI tool for developers.
         """
+        if not ctx.invoked_subcommand:
+            typer.echo(ctx.get_help())
         setup_pycharm_remote_debugger_if_provided(
             pycharm_debug_library_path=pycharm_debug_library_path,
             pycharm_debug_server_host=pycharm_debug_server_host,
             pycharm_debug_server_port=pycharm_debug_server_port,
         )
 
     return app
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/loggers.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/loggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import logging.config
 from dataclasses import asdict, dataclass, field
 from typing import Any, Dict, List
 
 import typer
 from snowflake.cli.api.config import (
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/main_typer.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/main_typer.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     It contains global exception handling.
     """
 
     def __init__(self):
         super().__init__(
             context_settings=DEFAULT_CONTEXT_SETTINGS,
             pretty_exceptions_show_locals=False,
-            add_completion=False,
+            add_completion=True,
         )
 
     def __call__(self, *args, **kwargs):
         # early detection of "--debug" flag
         # necessary in case of errors which happen during argument parsing
         # (for example badly formatted config file)
         # Hack: We have to go around Typer by checking sys.argv as it does not allow
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/printing.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/printing.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,17 @@
 
 
 def print_structured(result: CommandResult):
     """Handles outputs like json, yml and other structured and parsable formats."""
     if isinstance(result, MultipleResults):
         _stream_json(result)
     else:
-        return json.dump(result, sys.stdout, cls=CustomJSONEncoder, indent=4)
+        json.dump(result, sys.stdout, cls=CustomJSONEncoder, indent=4)
+    # Adds empty line at the end
+    print()
 
 
 def _stream_json(result):
     """Simple helper for streaming multiple results as a JSON."""
     indent_size = 2
 
     class _Indented:
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/snow_connector.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/snow_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,16 @@
     return connection_parameters
 
 
 def _update_connection_application_name(connection_parameters: Dict):
     """Update version and name of app handling connection."""
     connection_application_params = {
         "application_name": PARAM_APPLICATION_NAME,
-        "_internal_application_name": PARAM_INTERNAL_APPLICATION_NAME,
-        "_internal_application_version": VERSION,
+        "internal_application_name": PARAM_INTERNAL_APPLICATION_NAME,
+        "internal_application_version": VERSION,
     }
     connection_parameters.update(connection_application_params)
 
 
 def _load_pem_to_der(private_key_path: str) -> bytes:
     """
     Given a private key file path (in PEM format), decode key data into DER
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/telemetry.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List
 
 from snowflake.cli.api import PluginConfigProvider
 from snowflake.cli.api.config import (
     PLUGINS_SECTION_PATH,
     config_section_exists,
     get_config_section,
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/builtin_plugins.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from snowflake.cli.plugins.connection import plugin_spec as connection_plugin_spec
+from snowflake.cli.plugins.cortex import plugin_spec as cortex_plugin_spec
 from snowflake.cli.plugins.git import plugin_spec as git_plugin_spec
 from snowflake.cli.plugins.nativeapp import plugin_spec as nativeapp_plugin_spec
 from snowflake.cli.plugins.notebook import plugin_spec as notebook_plugin_spec
 from snowflake.cli.plugins.object import plugin_spec as object_plugin_spec
+
+# TODO 3.0: remove this import
+from snowflake.cli.plugins.object_stage_deprecated import (
+    plugin_spec as object_stage_deprecated_plugin_spec,
+)
 from snowflake.cli.plugins.snowpark import plugin_spec as snowpark_plugin_spec
 from snowflake.cli.plugins.spcs import plugin_spec as spcs_plugin_spec
 from snowflake.cli.plugins.sql import plugin_spec as sql_plugin_spec
 from snowflake.cli.plugins.stage import plugin_spec as stage_plugin_spec
 from snowflake.cli.plugins.streamlit import plugin_spec as streamlit_plugin_spec
 
 
@@ -19,10 +25,12 @@
         "object": object_plugin_spec,
         "snowpark": snowpark_plugin_spec,
         "stage": stage_plugin_spec,
         "sql": sql_plugin_spec,
         "streamlit": streamlit_plugin_spec,
         "git": git_plugin_spec,
         "notebook": notebook_plugin_spec,
+        "object-stage-deprecated": object_stage_deprecated_plugin_spec,
+        "cortex": cortex_plugin_spec,
     }
 
     return plugin_specs
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/command_plugins_loader.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from typing import Dict, List, Optional
 
 import pluggy
 from snowflake.cli.api.plugins.command import (
     SNOWCLI_COMMAND_PLUGIN_NAMESPACE,
     CommandPath,
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from typing import Callable, List
 
 from snowflake.cli.api.plugins.plugin_config import PluginConfigProvider
 from snowflake.cli.app.commands_registration.command_plugins_loader import (
     load_builtin_and_external_command_plugins,
     load_only_builtin_command_plugins,
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/threadsafe.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/typer_registration.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from typing import List
 
 import click
 from snowflake.cli.api.plugins.command import CommandSpec, CommandType
 from snowflake.cli.app.commands_registration import LoadedCommandPlugin
 from snowflake.cli.app.commands_registration.exception_logging import exception_logging
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/commands_structure.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/commands_structure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/pycharm_remote_debug.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Optional
 
 from click import ClickException
 
 
 def setup_pycharm_remote_debugger_if_provided(
     pycharm_debug_library_path: Optional[str],
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/generator.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/docs/generator.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/connection/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 import typer
 from click import ClickException, Context, Parameter  # type: ignore
 from click.core import ParameterSource  # type: ignore
 from click.types import StringParamType
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.flags import (
     PLAIN_PASSWORD_MSG,
-    ConnectionOption,
-    DiagAllowlistPathOption,
-    DiagLogPathOption,
-    EnableDiagOption,
-    MfaPasscodeOption,
 )
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.config import (
     ConnectionConfig,
     add_connection,
     connection_exists,
     get_all_connections,
@@ -233,21 +228,16 @@
         ),
     )
     return MessageResult(
         f"Wrote new connection {connection_name} to {CONFIG_MANAGER.file_path}"
     )
 
 
-@app.command(requires_connection=False)
+@app.command(requires_connection=True)
 def test(
-    connection: str = ConnectionOption,
-    mfa_passcode: str = MfaPasscodeOption,
-    enable_diag: bool = EnableDiagOption,
-    diag_log_path: str = DiagLogPathOption,
-    diag_allowlist_path: str = DiagAllowlistPathOption,
     **options,
 ) -> CommandResult:
     """
     Tests the connection to Snowflake.
     """
 
     # Test connection
@@ -268,29 +258,30 @@
             om.use(object_type=ObjectType.SCHEMA, name=f'"{schema}"')
         if conn.warehouse:
             om.use(object_type=ObjectType.WAREHOUSE, name=f'"{conn.warehouse}"')
 
     except ProgrammingError as err:
         raise ClickException(str(err))
 
+    conn_ctx = cli_context.connection_context
     result = {
-        "Connection name": connection,
+        "Connection name": conn_ctx.connection_name,
         "Status": "OK",
         "Host": conn.host,
         "Account": conn.account,
         "User": conn.user,
         "Role": f'{conn.role or "not set"}',
         "Database": f'{conn.database or "not set"}',
         "Warehouse": f'{conn.warehouse or "not set"}',
     }
 
-    if enable_diag:
+    if conn_ctx.enable_diag:
         result[
             "Diag Report Location"
-        ] = f"{diag_log_path}/SnowflakeConnectionTestReport.txt"
+        ] = f"{conn_ctx.diag_log_path}/SnowflakeConnectionTestReport.txt"
 
     return ObjectResult(result)
 
 
 @app.command(requires_connection=False)
 def set_default(
     name: str = typer.Argument(
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/util.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/connection/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     assume it's regionless, as this is true for most production deployments.
     """
     try:
         *_, cursor = conn.execute_string(REGIONLESS_QUERY, cursor_class=DictCursor)
         return cursor.fetchone()["REGIONLESS"].lower() == "true"
     except:
         # by default, assume that
-        log.exception("Cannot determine regionless redirect; assuming True.")
+        log.warning("Cannot determine regionless redirect; assuming True.")
         return True
 
 
 def get_context(conn: SnowflakeConnection) -> str:
     """
     Determines the first part of the path in a Snowsight URL.
     This could be a region or it could be an organization, depending
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/git/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from typing import List, Optional
 
 import typer
 from click import ClickException
 from snowflake.cli.api.commands.flags import (
     OnErrorOption,
@@ -12,14 +14,18 @@
 )
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.console.console import cli_console
 from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.output.types import CollectionResult, CommandResult, QueryResult
 from snowflake.cli.api.utils.path_utils import is_stage_path
 from snowflake.cli.plugins.git.manager import GitManager
+from snowflake.cli.plugins.object.command_aliases import (
+    add_object_command_aliases,
+    scope_option,
+)
 from snowflake.cli.plugins.object.manager import ObjectManager
 from snowflake.cli.plugins.stage.commands import get
 from snowflake.cli.plugins.stage.manager import OnErrorType
 
 app = SnowTyper(
     name="git",
     help="Manages git repositories in Snowflake.",
@@ -46,14 +52,23 @@
     help=(
         "Path to git repository stage with scope provided."
         " Path to the repository root must end with '/'."
         " For example: @my_repo/branches/main/"
     ),
     callback=_repo_path_argument_callback,
 )
+add_object_command_aliases(
+    app=app,
+    object_type=ObjectType.GIT_REPOSITORY,
+    name_argument=RepoNameArgument,
+    like_option=like_option(
+        help_example='`list --like "my%"` lists all git repositories with name that begin with “my”',
+    ),
+    scope_option=scope_option(help_example="`list --in database my_db`"),
+)
 
 
 def _assure_repository_does_not_exist(om: ObjectManager, repository_name: str) -> None:
     if om.object_exists(
         object_type=ObjectType.GIT_REPOSITORY.value.cli_name, name=repository_name
     ):
         raise ClickException(f"Repository '{repository_name}' already exists")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/git/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from pathlib import Path
 from typing import List, Optional
 
 import typer
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.decorators import (
@@ -27,15 +29,14 @@
 )
 from snowflake.cli.plugins.nativeapp.run_processor import NativeAppRunProcessor
 from snowflake.cli.plugins.nativeapp.teardown_processor import (
     NativeAppTeardownProcessor,
 )
 from snowflake.cli.plugins.nativeapp.utils import (
     get_first_paragraph_from_markdown_file,
-    is_tty_interactive,
     shallow_git_clone,
 )
 from snowflake.cli.plugins.nativeapp.version.commands import app as versions_app
 
 app = SnowTyper(
     name="app",
     help="Manages a Snowflake Native App",
@@ -148,27 +149,27 @@
     from_release_directive: Optional[bool] = typer.Option(
         False,
         "--from-release-directive",
         help=f"""Creates or upgrades an application object to the version and patch specified by the release directive applicable to your Snowflake account.
         The command fails if no release directive exists for your Snowflake account for a given application package, which is determined from the project definition file. Default: unset.""",
         is_flag=True,
     ),
-    interactive: Optional[bool] = InteractiveOption,
+    interactive: bool = InteractiveOption,
     force: Optional[bool] = ForceOption,
     **options,
 ) -> CommandResult:
     """
     Creates an application package in your Snowflake account, uploads code files to its stage,
     then creates or upgrades an application object from the application package.
     """
 
     is_interactive = False
     if force:
         policy = AllowAlwaysPolicy()
-    elif interactive or is_tty_interactive():
+    elif interactive:
         is_interactive = True
         policy = AskAlwaysPolicy()
     else:
         policy = DenyAlwaysPolicy()
 
     processor = NativeAppRunProcessor(
         project_definition=cli_context.project_definition,
@@ -210,24 +211,30 @@
         )
 
 
 @app.command("teardown", requires_connection=True)
 @with_project_definition("native_app")
 def app_teardown(
     force: Optional[bool] = ForceOption,
+    cascade: Optional[bool] = typer.Option(
+        None,
+        help=f"""Whether to drop all application objects owned by the application within the account. Default: false.""",
+        show_default=False,
+    ),
+    interactive: bool = InteractiveOption,
     **options,
 ) -> CommandResult:
     """
     Attempts to drop both the application object and application package as defined in the project definition file.
     """
     processor = NativeAppTeardownProcessor(
         project_definition=cli_context.project_definition,
         project_root=cli_context.project_root,
     )
-    processor.process(force)
+    processor.process(interactive, force, cascade)
     return MessageResult(f"Teardown is now complete.")
 
 
 @app.command("deploy", requires_connection=True)
 @with_project_definition("native_app")
 def app_deploy(
     prune: Optional[bool] = typer.Option(
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/constants.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/exceptions.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/init.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/init.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import os
 from abc import ABC, abstractmethod
 from functools import cached_property
 from pathlib import Path
 from textwrap import dedent
-from typing import List, Optional
+from typing import List, Optional, TypedDict
 
 import jinja2
+from click import ClickException
 from snowflake.cli.api.console import cli_console as cc
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
 from snowflake.cli.api.project.definition import (
     default_app_package,
     default_application,
     default_role,
 )
@@ -20,21 +21,23 @@
     extract_schema,
     to_identifier,
     unquote_identifier,
 )
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.connection.util import make_snowsight_url
 from snowflake.cli.plugins.nativeapp.artifacts import (
-    ArtifactDeploymentMap,
     ArtifactMapping,
+    BundleMap,
     build_bundle,
     resolve_without_follow,
-    source_path_to_deploy_path,
     translate_artifact,
 )
+from snowflake.cli.plugins.nativeapp.codegen.compiler import (
+    NativeAppCompiler,
+)
 from snowflake.cli.plugins.nativeapp.constants import (
     ALLOWED_SPECIAL_COMMENTS,
     COMMENT_COL,
     ERROR_MESSAGE_606,
     ERROR_MESSAGE_2043,
     INTERNAL_DISTRIBUTION,
     NAME_COL,
@@ -43,26 +46,29 @@
 )
 from snowflake.cli.plugins.nativeapp.exceptions import (
     ApplicationPackageAlreadyExistsError,
     InvalidPackageScriptError,
     MissingPackageScriptError,
     UnexpectedOwnerError,
 )
+from snowflake.cli.plugins.nativeapp.feature_flags import FeatureFlag
 from snowflake.cli.plugins.nativeapp.utils import verify_exists, verify_no_directories
 from snowflake.cli.plugins.stage.diff import (
     DiffResult,
     StagePath,
     compute_stage_diff,
     preserve_from_diff,
     sync_local_diff_with_stage,
     to_stage_path,
 )
 from snowflake.connector import ProgrammingError
 from snowflake.connector.cursor import DictCursor
 
+ApplicationOwnedObject = TypedDict("ApplicationOwnedObject", {"name": str, "type": str})
+
 
 def generic_sql_error_handler(
     err: ProgrammingError, role: Optional[str] = None, warehouse: Optional[str] = None
 ):
     # Potential refactor: If moving away from Python 3.8 and 3.9 to >= 3.10, use match ... case
     if err.errno == 2043 or err.msg.__contains__(ERROR_MESSAGE_2043):
         raise ProgrammingError(
@@ -156,14 +162,18 @@
         return [translate_artifact(item) for item in self.definition.artifacts]
 
     @cached_property
     def deploy_root(self) -> Path:
         return Path(self.project_root, self.definition.deploy_root)
 
     @cached_property
+    def generated_root(self) -> Path:
+        return Path(self.deploy_root, self.definition.generated_root)
+
+    @cached_property
     def package_scripts(self) -> List[str]:
         """
         Relative paths to package scripts from the project root.
         """
         if self.definition.package and self.definition.package.scripts:
             return self.definition.package.scripts
         else:
@@ -301,39 +311,48 @@
                     which does not match the value specified in project definition file: {project_def_distribution}.
                     """
                 )
             )
             return False
         return True
 
-    def build_bundle(self) -> ArtifactDeploymentMap:
+    def build_bundle(self) -> BundleMap:
         """
         Populates the local deploy root from artifact sources.
         """
-        return build_bundle(self.project_root, self.deploy_root, self.artifacts)
+        mapped_files = build_bundle(self.project_root, self.deploy_root, self.artifacts)
+        if FeatureFlag.ENABLE_SETUP_SCRIPT_GENERATION.is_enabled():
+            compiler = NativeAppCompiler(
+                project_definition=self._project_definition,
+                project_root=self.project_root,
+                deploy_root=self.deploy_root,
+                generated_root=self.generated_root,
+            )
+            compiler.compile_artifacts()
+        return mapped_files
 
     def sync_deploy_root_with_stage(
         self,
         role: str,
         prune: bool,
         recursive: bool,
         local_paths_to_sync: List[Path] | None = None,
-        mapped_files: Optional[ArtifactDeploymentMap] = None,
+        bundle_map: Optional[BundleMap] = None,
     ) -> DiffResult:
         """
         Ensures that the files on our remote stage match the artifacts we have in
         the local filesystem.
 
         Args:
             role (str): The name of the role to use for queries and commands.
             prune (bool): Whether to prune artifacts from the stage that don't exist locally.
             recursive (bool): Whether to traverse directories recursively.
             local_paths_to_sync (List[Path], optional): List of local paths to sync. Defaults to None to sync all
              local paths. Note that providing an empty list here is equivalent to None.
-            mapped_files: the file mapping computed during the `bundle` step. Required when local_paths_to_sync is
+            bundle_map: the artifact mapping computed during the `bundle` step. Required when local_paths_to_sync is
              provided.
 
         Returns:
             A `DiffResult` instance describing the changes that were performed.
         """
 
         # Does a stage already exist within the application package, or we need to create one?
@@ -355,29 +374,33 @@
             "Performing a diff between the Snowflake stage and your local deploy_root ('%s') directory."
             % self.deploy_root
         )
         diff: DiffResult = compute_stage_diff(self.deploy_root, self.stage_fqn)
 
         files_not_removed = []
         if local_paths_to_sync:
-            assert mapped_files is not None
+            assert bundle_map is not None
 
             # Deploying specific files/directories
             resolved_paths_to_sync = [
                 resolve_without_follow(p) for p in local_paths_to_sync
             ]
             if not recursive:
                 verify_no_directories(resolved_paths_to_sync)
-            deploy_paths_to_sync = [
-                source_path_to_deploy_path(p, mapped_files)
-                for p in resolved_paths_to_sync
-            ]
-            verify_exists(deploy_paths_to_sync)
+
+            deploy_paths_to_sync = []
+            for resolved_path in resolved_paths_to_sync:
+                verify_exists(resolved_path)
+                deploy_paths = bundle_map.to_deploy_paths(resolved_path)
+                if not deploy_paths:
+                    raise ClickException(f"No artifact found for {resolved_path}")
+                deploy_paths_to_sync.extend(deploy_paths)
+
             stage_paths_to_sync = _get_stage_paths_to_sync(
-                deploy_paths_to_sync, self.deploy_root.resolve()
+                deploy_paths_to_sync, resolve_without_follow(self.deploy_root)
             )
             diff = preserve_from_diff(diff, stage_paths_to_sync)
         else:
             # Full deploy
             if not recursive:
                 deploy_files = [p for p in self.deploy_root.resolve().iterdir()]
                 verify_no_directories(deploy_files)
@@ -425,14 +448,24 @@
         """
 
         with self.use_role(self.package_role):
             return self.show_specific_object(
                 "application packages", self.package_name, name_col=NAME_COL
             )
 
+    def get_objects_owned_by_application(self) -> List[ApplicationOwnedObject]:
+        """
+        Returns all application objects owned by this application.
+        """
+        with self.use_role(self.app_role):
+            results = self._execute_query(
+                f"show objects owned by application {self.app_name}"
+            ).fetchall()
+            return [{"name": row[1], "type": row[2]} for row in results]
+
     def get_snowsight_url(self) -> str:
         """Returns the URL that can be used to visit this app via Snowsight."""
         name = unquote_identifier(self.app_name)
         return make_snowsight_url(self._conn, f"/#/apps/application/{name}")
 
     def create_app_package(self) -> None:
         """
@@ -518,24 +551,24 @@
             )
 
     def deploy(
         self,
         prune: bool,
         recursive: bool,
         local_paths_to_sync: List[Path] | None = None,
-        mapped_files: Optional[ArtifactDeploymentMap] = None,
+        bundle_map: Optional[BundleMap] = None,
     ) -> DiffResult:
         """app deploy process"""
 
         # 1. Create an empty application package, if none exists
         self.create_app_package()
 
         with self.use_role(self.package_role):
             # 2. now that the application package exists, create shared data
             self._apply_package_scripts()
 
             # 3. Upload files from deploy root local folder to the above stage
             diff = self.sync_deploy_root_with_stage(
-                self.package_role, prune, recursive, local_paths_to_sync, mapped_files
+                self.package_role, prune, recursive, local_paths_to_sync, bundle_map
             )
 
         return diff
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/policy.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from typing import Optional
 
 import typer
 
 
 class PolicyBase(ABC):
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/run_processor.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from textwrap import dedent
 from typing import Optional
 
 import typer
 from click import UsageError
 from snowflake.cli.api.console import cli_console as cc
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/teardown_processor.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 from pathlib import Path
 from textwrap import dedent
-from typing import Dict
+from typing import Dict, Optional
 
 import typer
 from snowflake.cli.api.console import cli_console as cc
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
 from snowflake.cli.plugins.nativeapp.constants import (
     ALLOWED_SPECIAL_COMMENTS,
     COMMENT_COL,
@@ -12,41 +14,64 @@
     INTERNAL_DISTRIBUTION,
     OWNER_COL,
 )
 from snowflake.cli.plugins.nativeapp.exceptions import (
     CouldNotDropApplicationPackageWithVersions,
 )
 from snowflake.cli.plugins.nativeapp.manager import (
+    ApplicationOwnedObject,
     NativeAppCommandProcessor,
     NativeAppManager,
     ensure_correct_owner,
 )
-from snowflake.cli.plugins.nativeapp.utils import needs_confirmation
+from snowflake.cli.plugins.nativeapp.utils import (
+    needs_confirmation,
+)
 from snowflake.connector.cursor import DictCursor
 
 
 class NativeAppTeardownProcessor(NativeAppManager, NativeAppCommandProcessor):
     def __init__(self, project_definition: Dict, project_root: Path):
         super().__init__(project_definition, project_root)
 
-    def drop_generic_object(self, object_type: str, object_name: str, role: str):
+    def drop_generic_object(
+        self, object_type: str, object_name: str, role: str, cascade: bool = False
+    ):
         """
         Drop object using the given role.
         """
         with self.use_role(role):
             cc.step(f"Dropping {object_type} {object_name} now.")
             drop_query = f"drop {object_type} {object_name}"
+            if cascade:
+                drop_query += " cascade"
             try:
                 self._execute_query(drop_query)
             except:
                 raise SnowflakeSQLExecutionError(drop_query)
 
             cc.message(f"Dropped {object_type} {object_name} successfully.")
 
-    def drop_application(self, auto_yes: bool):
+    def _application_objects_to_str(
+        self, application_objects: ApplicationOwnedObject
+    ) -> str:
+        """
+        Returns a list in an "(Object Type) Object Name" format. Database-level and schema-level object names are fully qualified:
+        (COMPUTE_POOL) POOL_NAME
+        (DATABASE) DB_NAME
+        (SCHEMA) DB_NAME.PUBLIC
+        ...
+        """
+        return "\n".join(
+            [f"({obj['type']}) {obj['name']}" for obj in application_objects]
+        )
+
+    def drop_application(
+        self, auto_yes: bool, interactive: bool = False, cascade: Optional[bool] = None
+    ):
         """
         Attempts to drop the application object if all validations and user prompts allow so.
         """
 
         needs_confirm = True
 
         # 1. If existing application package is not found, exit gracefully
@@ -85,17 +110,53 @@
                         """
                     )
                 )
                 if not should_drop_object:
                     cc.message(f"Did not drop application object {self.app_name}.")
                     return  # The user desires to keep the app, therefore exit gracefully
 
-        # 4. All validations have passed, drop object
+        # 4. Check for application objects owned by the application
+        application_objects = self.get_objects_owned_by_application()
+        if len(application_objects) > 0:
+            application_objects_str = self._application_objects_to_str(
+                application_objects
+            )
+            if cascade is True:
+                cc.message(
+                    f"The following objects are owned by application {self.app_name} and will be dropped:\n{application_objects_str}"
+                )
+            elif cascade is False:
+                cc.message(
+                    f"The following objects are owned by application {self.app_name}:\n{application_objects_str}"
+                )
+            elif interactive:
+                if interactive:
+                    api_integration = typer.prompt(
+                        f"The following objects are owned by application {self.app_name}:\n{application_objects_str}\n\nWould you like to drop these objects in addition to the application? [y/n/ABORT]"
+                    )
+                    if api_integration in ["y", "yes", "Y", "Yes", "YES"]:
+                        cascade = True
+                    elif api_integration in ["n", "no", "N", "No", "NO"]:
+                        cascade = False
+                    else:
+                        raise typer.Abort()
+            else:
+                cc.message(
+                    f"The following application objects are owned by application {self.app_name}:\n{application_objects_str}\n\nRe-run teardown again with --cascade or --no-cascade to specify whether these objects should be dropped along with the application."
+                )
+                raise typer.Abort()
+        elif cascade is None:
+            cascade = False
+
+        # 5. All validations have passed, drop object
         self.drop_generic_object(
-            object_type="application", object_name=self.app_name, role=self.app_role
+            object_type="application",
+            object_name=self.app_name,
+            role=self.app_role,
+            cascade=cascade,
         )
         return  # The application object was successfully dropped, therefore exit gracefully
 
     def drop_package(self, auto_yes: bool):
         """
         Attempts to drop application package unless user specifies otherwise.
         """
@@ -172,14 +233,23 @@
         self.drop_generic_object(
             object_type="application package",
             object_name=self.package_name,
             role=self.package_role,
         )
         return  # The application package was successfully dropped, therefore exit gracefully
 
-    def process(self, force_drop: bool = False, *args, **kwargs):
+    def process(
+        self,
+        interactive: bool,
+        force_drop: bool = False,
+        cascade: Optional[bool] = None,
+        *args,
+        **kwargs,
+    ):
 
         # Drop the application object
-        self.drop_application(auto_yes=force_drop)
+        self.drop_application(
+            auto_yes=force_drop, interactive=interactive, cascade=cascade
+        )
 
         # Drop the application package
         self.drop_package(auto_yes=force_drop)
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/utils.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from os import PathLike
+from __future__ import annotations
+
+import os
 from pathlib import Path
 from sys import stdin, stdout
 from typing import List, Optional, Union
 
 from click import ClickException
 
 
@@ -39,15 +41,15 @@
             if not stripped_line.startswith("#") and stripped_line:
                 paragraph_text = stripped_line
                 break
 
         return paragraph_text
 
 
-def shallow_git_clone(url: Union[str, PathLike], to_path: Union[str, PathLike]):
+def shallow_git_clone(url: Union[str, os.PathLike], to_path: Union[str, os.PathLike]):
     """
     Performs a shallow clone of the repository at the provided url to the path specified
 
     Parameters:
         url (str | PathLike): Valid git url.
         to_path (str | PathLike): Path to which the repository should be cloned to.
 
@@ -73,11 +75,10 @@
     for path in paths_to_sync:
         if path.is_dir():
             raise ClickException(
                 f"{path} is a directory. Add the -r flag to deploy directories."  #
             )
 
 
-def verify_exists(paths_to_sync: List[Path]):
-    for path in paths_to_sync:
-        if not path.exists():
-            raise ClickException(f"The following path does not exist: {path}")
+def verify_exists(path: Path):
+    if not path.exists():
+        raise ClickException(f"The following path does not exist: {path}")
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import shutil
 import subprocess
 import sys
 from enum import Enum
 from pathlib import Path
 from typing import Optional, Sequence, Union
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from typing import Optional
 
 import typer
 from click import MissingParameter
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.decorators import (
@@ -12,15 +14,14 @@
 from snowflake.cli.plugins.nativeapp.common_flags import ForceOption, InteractiveOption
 from snowflake.cli.plugins.nativeapp.policy import (
     AllowAlwaysPolicy,
     AskAlwaysPolicy,
     DenyAlwaysPolicy,
 )
 from snowflake.cli.plugins.nativeapp.run_processor import NativeAppRunProcessor
-from snowflake.cli.plugins.nativeapp.utils import is_tty_interactive
 from snowflake.cli.plugins.nativeapp.version.version_processor import (
     NativeAppVersionCreateProcessor,
     NativeAppVersionDropProcessor,
 )
 
 app = SnowTyper(
     name="version",
@@ -45,28 +46,28 @@
     ),
     skip_git_check: Optional[bool] = typer.Option(
         False,
         "--skip-git-check",
         help="When enabled, the Snowflake CLI skips checking if your project has any untracked or stages files in git. Default: unset.",
         is_flag=True,
     ),
-    interactive: Optional[bool] = InteractiveOption,
+    interactive: bool = InteractiveOption,
     force: Optional[bool] = ForceOption,
     **options,
 ) -> CommandResult:
     """
     Adds a new patch to the provided version defined in your application package. If the version does not exist, creates a version with patch 0.
     """
     if version is None and patch is not None:
         raise MissingParameter("Cannot provide a patch without version!")
 
     is_interactive = False
     if force:
         policy = AllowAlwaysPolicy()
-    elif interactive or is_tty_interactive():
+    elif interactive:
         is_interactive = True
         policy = AskAlwaysPolicy()
     else:
         policy = DenyAlwaysPolicy()
 
     if skip_git_check:
         git_policy = DenyAlwaysPolicy()
@@ -109,26 +110,26 @@
 @app.command(requires_connection=True)
 @with_project_definition("native_app")
 def drop(
     version: Optional[str] = typer.Argument(
         None,
         help="Version defined in an application package that you want to drop. Defaults to the version specified in the `manifest.yml` file.",
     ),
-    interactive: Optional[bool] = InteractiveOption,
+    interactive: bool = InteractiveOption,
     force: Optional[bool] = ForceOption,
     **options,
 ) -> CommandResult:
     """
     Drops a version defined in your application package. Versions can either be passed in as an argument to the command or read from the `manifest.yml` file.
     Dropping patches is not allowed.
     """
     is_interactive = False
     if force:
         policy = AllowAlwaysPolicy()
-    elif interactive or is_tty_interactive():
+    elif interactive:
         is_interactive = True
         policy = AskAlwaysPolicy()
     else:
         policy = DenyAlwaysPolicy()
 
     processor = NativeAppVersionDropProcessor(
         project_definition=cli_context.project_definition,
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/version_processor.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from textwrap import dedent
 from typing import Dict, List, Optional
 
 import typer
 from click import BadOptionUsage, ClickException
 from snowflake.cli.api.console import cli_console as cc
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/notebook/commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,30 @@
 
 import typer
 from snowflake.cli.api.commands.flags import identifier_argument
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.feature_flags import FeatureFlag
 from snowflake.cli.api.output.types import MessageResult
 from snowflake.cli.plugins.notebook.manager import NotebookManager
+from snowflake.cli.plugins.notebook.types import NotebookName, NotebookStagePath
+from typing_extensions import Annotated
 
 app = SnowTyper(
     name="notebook",
     help="Manages notebooks in Snowflake.",
     hidden=FeatureFlag.ENABLE_NOTEBOOKS.is_disabled(),
 )
 log = logging.getLogger(__name__)
 
 NOTEBOOK_IDENTIFIER = identifier_argument(sf_object="notebook", example="MY_NOTEBOOK")
+NotebookFile: NotebookStagePath = typer.Option(
+    "--notebook-file",
+    "-f",
+    help="Stage path with notebook file. For example `@stage/path/to/notebook.ipynb`",
+)
 
 
 @app.command(requires_connection=True)
 def execute(
     identifier: str = NOTEBOOK_IDENTIFIER,
     **options,
 ):
@@ -45,7 +52,21 @@
     identifier: str = NOTEBOOK_IDENTIFIER,
     **options,
 ):
     """Opens a notebook in default browser"""
     url = NotebookManager().get_url(notebook_name=identifier)
     typer.launch(url)
     return MessageResult(message=url)
+
+
+@app.command(requires_connection=True)
+def create(
+    identifier: Annotated[NotebookName, NOTEBOOK_IDENTIFIER],
+    notebook_file: Annotated[NotebookStagePath, NotebookFile],
+    **options,
+):
+    """Creates notebook from stage."""
+    notebook_url = NotebookManager().create(
+        notebook_name=identifier,
+        notebook_file=notebook_file,
+    )
+    return MessageResult(message=notebook_url)
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 from click import ClickException
 from snowflake.cli.api.commands.flags import like_option
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.constants import SUPPORTED_OBJECTS, VALID_SCOPES
 from snowflake.cli.api.output.types import QueryResult
 from snowflake.cli.api.project.util import is_valid_identifier
 from snowflake.cli.plugins.object.manager import ObjectManager
-from snowflake.cli.plugins.object.stage_deprecated.commands import app as stage_app
 
 app = SnowTyper(
     name="object",
     help="Manages Snowflake objects like warehouses and stages",
 )
-app.add_typer(stage_app)
 
 
 NameArgument = typer.Argument(help="Name of the object")
 ObjectArgument = typer.Argument(
     help="Type of object. For example table, procedure, streamlit.",
     case_sensitive=False,
 )
@@ -36,18 +34,24 @@
         raise ClickException(
             f"scope must be one of the following: {', '.join(VALID_SCOPES)}"
         )
     if scope[0] == "compute-pool" and object_type != "service":
         raise ClickException("compute-pool scope is only supported for listing service")
 
 
-ScopeOption = typer.Option(
-    (None, None),
-    "--in",
-    help="Specifies the scope of this command using '--in <scope> <name>' (e.g. list tables --in database my_db). Some object types have specialized scopes (e.g. list service --in compute-pool my_pool)",
+def scope_option(help_example: str):
+    return typer.Option(
+        (None, None),
+        "--in",
+        help=f"Specifies the scope of this command using '--in <scope> <name>', for example {help_example}.",
+    )
+
+
+ScopeOption = scope_option(
+    help_example="`list table --in database my_db`. Some object types have specialized scopes (e.g. list service --in compute-pool my_pool)"
 )
 
 SUPPORTED_TYPES_MSG = "\n\nSupported types: " + ", ".join(SUPPORTED_OBJECTS)
 
 
 @app.command(
     "list",
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/common.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from typing import Optional
 
 from click import ClickException
 from snowflake.cli.api.commands.flags import OverrideableOption
 from snowflake.cli.api.project.util import (
     VALID_IDENTIFIER_REGEX,
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/stage_deprecated/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/object_stage_deprecated/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
-from typing import Dict, List, Optional, Set
+from typing import Dict, List, Optional, Set, Tuple
 
 import typer
 from click import ClickException
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.decorators import (
     with_project_definition,
 )
 from snowflake.cli.api.commands.flags import (
     ReplaceOption,
     deprecated_flag_callback_enum,
     execution_identifier_argument,
+    identifier_argument,
+    like_option,
 )
 from snowflake.cli.api.commands.project_initialisation import add_init_command
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.constants import (
     DEFAULT_SIZE_LIMIT_MB,
     DEPLOYMENT_STAGE,
     ObjectType,
 )
 from snowflake.cli.api.exceptions import (
     SecretsWithoutExternalAccessIntegrationError,
 )
+from snowflake.cli.api.identifiers import FQN
 from snowflake.cli.api.output.types import (
     CollectionResult,
     CommandResult,
     MessageResult,
     SingleQueryResult,
 )
 from snowflake.cli.api.project.schemas.snowpark.callable import (
-    Callable,
     FunctionSchema,
     ProcedureSchema,
 )
 from snowflake.cli.api.secure_path import SecurePath
+from snowflake.cli.plugins.object.commands import (
+    describe as object_describe,
+)
+from snowflake.cli.plugins.object.commands import (
+    drop as object_drop,
+)
+from snowflake.cli.plugins.object.commands import (
+    list_ as object_list,
+)
+from snowflake.cli.plugins.object.commands import (
+    scope_option,
+)
 from snowflake.cli.plugins.object.manager import ObjectManager
 from snowflake.cli.plugins.snowpark import package_utils
 from snowflake.cli.plugins.snowpark.common import (
     build_udf_sproc_identifier,
     check_if_replace_is_required,
 )
 from snowflake.cli.plugins.snowpark.manager import FunctionManager, ProcedureManager
@@ -69,16 +83,23 @@
     name="snowpark",
     help="Manages procedures and functions.",
 )
 
 ObjectTypeArgument = typer.Argument(
     help="Type of Snowpark object",
     case_sensitive=False,
+    show_default=False,
+)
+IdentifierArgument = identifier_argument(
+    "function/procedure",
+    example="hello(int, string)",
+)
+LikeOption = like_option(
+    help_example='`list function --like "my%"` lists all functions that begin with “my”',
 )
-
 add_init_command(app, project_type="Snowpark", template="default_snowpark")
 
 
 @app.command("deploy", requires_connection=True)
 @with_project_definition("snowpark")
 def deploy(
     replace: bool = ReplaceOption(
@@ -128,15 +149,15 @@
         msg += "\n" if existing_functions and existing_procedures else ""
         msg += "\n".join(f"procedure: {n}" for n in existing_procedures)
         raise ClickException(msg)
 
     # Create stage
     stage_name = snowpark.stage_name
     stage_manager = StageManager()
-    stage_name = stage_manager.to_fully_qualified_name(stage_name)
+    stage_name = FQN.from_string(stage_name).using_context()
     stage_manager.create(
         stage_name=stage_name, comment="deployments managed by Snowflake CLI"
     )
 
     snowflake_dependencies = _read_snowflake_requrements_file(
         paths.snowflake_requirements_file
     )
@@ -177,15 +198,15 @@
         )
         deploy_status.append(operation_result)
 
     return CollectionResult(deploy_status)
 
 
 def _assert_object_definitions_are_correct(
-    object_type, object_definitions: List[Callable]
+    object_type, object_definitions: List[FunctionSchema | ProcedureSchema]
 ):
     for definition in object_definitions:
         database = definition.database
         schema = definition.schema_name
         name = definition.name
         fqn_parts = len(name.split("."))
         if fqn_parts == 3 and database:
@@ -252,15 +273,15 @@
     artifact_stage_directory = f"@{(stage_name or DEPLOYMENT_STAGE)}/{project_name}"
     return artifact_stage_directory
 
 
 def _deploy_single_object(
     manager: FunctionManager | ProcedureManager,
     object_type: ObjectType,
-    object_definition: Callable,
+    object_definition: FunctionSchema | ProcedureSchema,
     existing_objects: Dict[str, Dict],
     snowflake_dependencies: List[str],
     stage_artifact_path: str,
 ):
     identifier = build_udf_sproc_identifier(
         object_definition, manager, include_parameter_names=False
     )
@@ -271,24 +292,26 @@
         include_default_values=True,
     )
     log.info("Deploying %s: %s", object_type, identifier_with_default_values)
 
     handler = object_definition.handler
     returns = object_definition.returns
     imports = object_definition.imports
+    external_access_integrations = object_definition.external_access_integrations
     replace_object = False
 
     object_exists = identifier in existing_objects
     if object_exists:
         replace_object = check_if_replace_is_required(
             object_type=object_type,
             current_state=existing_objects[identifier],
             handler=handler,
             return_type=returns,
             snowflake_dependencies=snowflake_dependencies,
+            external_access_integrations=external_access_integrations,
             imports=imports,
             stage_artifact_file=stage_artifact_path,
         )
 
     if object_exists and not replace_object:
         return {
             "object": identifier_with_default_values,
@@ -459,7 +482,40 @@
     **options,
 ) -> CommandResult:
     """Executes a procedure or function in a specified environment."""
     cursor = _execute_object_method(
         "execute", object_type=object_type, execution_identifier=execution_identifier
     )
     return SingleQueryResult(cursor)
+
+
+@app.command("list", requires_connection=True)
+def list_(
+    object_type: _SnowparkObject = ObjectTypeArgument,
+    like: str = LikeOption,
+    scope: Tuple[str, str] = scope_option(
+        help_example="`list function --in database my_db`"
+    ),
+    **options,
+):
+    """Lists all available procedures or functions."""
+    object_list(object_type=object_type.value, like=like, scope=scope, **options)
+
+
+@app.command("drop", requires_connection=True)
+def drop(
+    object_type: _SnowparkObject = ObjectTypeArgument,
+    identifier: str = IdentifierArgument,
+    **options,
+):
+    """Drop procedure or function."""
+    object_drop(object_type=object_type.value, object_name=identifier, **options)
+
+
+@app.command("describe", requires_connection=True)
+def describe(
+    object_type: _SnowparkObject = ObjectTypeArgument,
+    identifier: str = IdentifierArgument,
+    **options,
+):
+    """Provides description of a procedure or function."""
+    object_describe(object_type=object_type.value, object_name=identifier, **options)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/common.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import re
 from typing import Dict, List, Optional, Set
 
 from snowflake.cli.api.constants import ObjectType
+from snowflake.cli.api.identifiers import FQN
 from snowflake.cli.api.project.schemas.snowpark.argument import Argument
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.snowpark.models import Requirement
 from snowflake.cli.plugins.snowpark.package_utils import (
     generate_deploy_stage_name,
 )
 from snowflake.connector.cursor import SnowflakeCursor
@@ -17,14 +18,15 @@
 
 def check_if_replace_is_required(
     object_type: ObjectType,
     current_state,
     handler: str,
     return_type: str,
     snowflake_dependencies: List[str],
+    external_access_integrations: List[str],
     imports: List[str],
     stage_artifact_file: str,
 ) -> bool:
     import logging
 
     log = logging.getLogger(__name__)
     resource_json = _convert_resource_details_to_dict(current_state)
@@ -38,14 +40,23 @@
 
     if _snowflake_dependencies_differ(old_dependencies, snowflake_dependencies):
         log.info(
             "Found difference of package requirements. Replacing the %s.", object_type
         )
         return True
 
+    if set(external_access_integrations) != set(
+        resource_json.get("external_access_integrations", [])
+    ):
+        log.info(
+            "Found difference of external access integrations. Replacing the %s.",
+            object_type,
+        )
+        return True
+
     if (
         resource_json["handler"].lower() != handler.lower()
         or _sql_to_python_return_type_mapper(resource_json["returns"]).lower()
         != return_type.lower()
     ):
         log.info(
             "Return type or handler types do not match. Replacing the %s.", object_type
@@ -185,20 +196,20 @@
         if include_default_values and arg.default:
             val = f"{arg.default}"
             if _is_signature_type_a_string(arg.arg_type):
                 val = f"'{val}'"
             result += f" default {val}"
         return result
 
-    arguments = ", ".join(format_arg(arg) for arg in udf_sproc.signature)
-    name = slq_exec_mixin.to_fully_qualified_name(
-        udf_sproc.name,
-        database=udf_sproc.database,
-        schema=udf_sproc.schema_name,
-    )
+    if udf_sproc.signature and udf_sproc.signature != "null":
+        arguments = ", ".join(format_arg(arg) for arg in udf_sproc.signature)
+    else:
+        arguments = ""
+
+    name = FQN.from_identifier_model(udf_sproc).using_context().identifier
     return f"{name}({arguments})"
 
 
 def _compare_imports(
     resource_json: dict, imports: List[str], artifact_file: str
 ) -> bool:
     pattern = re.compile(r"(?:\[@?\w+_\w+\.)?(\w+(?:/\w+)+\.\w+)(?:\])?")
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/models.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/models.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package_utils.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/snowpark_shared.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/zipper.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/__init__.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/common.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+from __future__ import annotations
+
 from typing import Optional
 
 import typer
 from click import ClickException
-from snowflake.cli.api.commands.flags import IfNotExistsOption, OverrideableOption
+from snowflake.cli.api.commands.flags import (
+    IfNotExistsOption,
+    OverrideableOption,
+    like_option,
+)
 from snowflake.cli.api.commands.snow_typer import SnowTyper
+from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.output.types import CommandResult, SingleQueryResult
 from snowflake.cli.api.project.util import is_valid_object_name
+from snowflake.cli.plugins.object.command_aliases import (
+    add_object_command_aliases,
+)
 from snowflake.cli.plugins.object.common import CommentOption
 from snowflake.cli.plugins.spcs.common import (
     validate_and_set_instances,
 )
 from snowflake.cli.plugins.spcs.compute_pool.manager import ComputePoolManager
 
 app = SnowTyper(
@@ -65,22 +75,33 @@
     "--auto-suspend-secs",
     help=_AUTO_SUSPEND_SECS_HELP,
     min=1,
 )
 
 _COMMENT_HELP = "Comment for the compute pool."
 
+add_object_command_aliases(
+    app=app,
+    object_type=ObjectType.COMPUTE_POOL,
+    name_argument=ComputePoolNameArgument,
+    like_option=like_option(
+        help_example='`list --like "my%"` lists all compute pools that begin with “my”.'
+    ),
+    scope_option=None,
+)
+
 
 @app.command(requires_connection=True)
 def create(
     name: str = ComputePoolNameArgument,
     instance_family: str = typer.Option(
         ...,
         "--family",
         help="Name of the instance family. For more information about instance families, refer to the SQL CREATE COMPUTE POOL command.",
+        show_default=False,
     ),
     min_nodes: int = MinNodesOption(),
     max_nodes: Optional[int] = MaxNodesOption(),
     auto_resume: bool = AutoResumeOption(),
     initially_suspended: bool = typer.Option(
         False,
         "--init-suspend/--no-init-suspend",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List, Optional
 
 from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.spcs.common import (
     NoPropertiesProvidedError,
     handle_object_already_exists,
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,33 @@
+from __future__ import annotations
+
 import json
 from typing import Optional
 
 import requests
 import typer
 from click import ClickException
-from snowflake.cli.api.commands.flags import IfNotExistsOption, ReplaceOption
+from snowflake.cli.api.commands.flags import (
+    IfNotExistsOption,
+    ReplaceOption,
+    like_option,
+)
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.console import cli_console
+from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.output.types import (
     CollectionResult,
     MessageResult,
     SingleQueryResult,
 )
 from snowflake.cli.api.project.util import is_valid_object_name
+from snowflake.cli.plugins.object.command_aliases import (
+    add_object_command_aliases,
+    scope_option,
+)
 from snowflake.cli.plugins.spcs.image_registry.manager import RegistryManager
 from snowflake.cli.plugins.spcs.image_repository.manager import ImageRepositoryManager
 
 app = SnowTyper(
     name="image-repository",
     help="Manages Snowpark Container Services image repositories.",
     short_help="Manages image repositories.",
@@ -30,14 +41,26 @@
         )
     return name
 
 
 REPO_NAME_ARGUMENT = typer.Argument(
     help="Name of the image repository.",
     callback=_repo_name_callback,
+    show_default=False,
+)
+
+add_object_command_aliases(
+    app=app,
+    object_type=ObjectType.IMAGE_REPOSITORY,
+    name_argument=REPO_NAME_ARGUMENT,
+    like_option=like_option(
+        help_example='`list --like "my%"` lists all image repositories that begin with “my”.'
+    ),
+    scope_option=scope_option(help_example="`list --in database my_db`"),
+    ommit_commands=["describe"],
 )
 
 
 @app.command(requires_connection=True)
 def create(
     name: str = REPO_NAME_ARGUMENT,
     replace: bool = ReplaceOption(),
@@ -102,14 +125,15 @@
     name: str = REPO_NAME_ARGUMENT,
     image_name: str = typer.Option(
         ...,
         "--image-name",
         "--image_name",
         "-i",
         help="Fully qualified name of the image as shown in the output of list-images",
+        show_default=False,
     ),
     **options,
 ) -> CollectionResult:
     """Lists tags for the given image in a repository."""
 
     repository_manager = ImageRepositoryManager()
     url = repository_manager.get_repository_url(name)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from urllib.parse import urlparse
 
 from snowflake.cli.api.constants import ObjectType
+from snowflake.cli.api.identifiers import FQN
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.spcs.common import handle_object_already_exists
 from snowflake.connector.errors import ProgrammingError
 
 
 class ImageRepositoryManager(SqlExecutionMixin):
     def get_database(self):
@@ -18,16 +19,17 @@
 
     def get_repository_url(self, repo_name: str, with_scheme: bool = True):
 
         repo_row = self.show_specific_object(
             "image repositories", repo_name, check_schema=True
         )
         if repo_row is None:
+            fqn = FQN.from_string(repo_name).using_connection(self._conn)
             raise ProgrammingError(
-                f"Image repository '{self.to_fully_qualified_name(repo_name)}' does not exist or not authorized."
+                f"Image repository '{fqn.identifier}' does not exist or not authorized."
             )
         if with_scheme:
             return f"https://{repo_row['repository_url']}"
         else:
             return repo_row["repository_url"]
 
     def get_repository_api_url(self, repo_url):
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,33 @@
+from __future__ import annotations
+
 import sys
 from pathlib import Path
 from typing import List, Optional
 
 import typer
 from click import ClickException
-from snowflake.cli.api.commands.flags import IfNotExistsOption, OverrideableOption
+from snowflake.cli.api.commands.flags import (
+    IfNotExistsOption,
+    OverrideableOption,
+    like_option,
+)
 from snowflake.cli.api.commands.snow_typer import SnowTyper
+from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.output.types import (
     CommandResult,
     QueryJsonValueResult,
     QueryResult,
     SingleQueryResult,
 )
 from snowflake.cli.api.project.util import is_valid_object_name
+from snowflake.cli.plugins.object.command_aliases import (
+    add_object_command_aliases,
+    scope_option,
+)
 from snowflake.cli.plugins.object.common import CommentOption, Tag, TagOption
 from snowflake.cli.plugins.spcs.common import (
     print_log_lines,
     validate_and_set_instances,
 )
 from snowflake.cli.plugins.spcs.services.manager import ServiceManager
 
@@ -32,24 +43,28 @@
         raise ClickException(
             f"'{name}' is not a valid service name. Note service names must be unquoted identifiers. The same constraint also applies to database and schema names where you create a service."
         )
     return name
 
 
 ServiceNameArgument = typer.Argument(
-    ..., help="Name of the service.", callback=_service_name_callback
+    ...,
+    help="Name of the service.",
+    callback=_service_name_callback,
+    show_default=False,
 )
 
 SpecPathOption = typer.Option(
     ...,
     "--spec-path",
     help="Path to service specification file.",
     file_okay=True,
     dir_okay=False,
     exists=True,
+    show_default=False,
 )
 
 _MIN_INSTANCES_HELP = "Minimum number of service instances to run."
 MinInstancesOption = OverrideableOption(
     1, "--min-instances", help=_MIN_INSTANCES_HELP, min=1
 )
 
@@ -70,20 +85,33 @@
     True,
     "--auto-resume/--no-auto-resume",
     help=_AUTO_RESUME_HELP,
 )
 
 _COMMENT_HELP = "Comment for the service."
 
+add_object_command_aliases(
+    app=app,
+    object_type=ObjectType.SERVICE,
+    name_argument=ServiceNameArgument,
+    like_option=like_option(
+        help_example='`list --like "my%"` lists all services that begin with “my”.'
+    ),
+    scope_option=scope_option(help_example="`list --in compute-pool my_pool`"),
+)
+
 
 @app.command(requires_connection=True)
 def create(
     name: str = ServiceNameArgument,
     compute_pool: str = typer.Option(
-        ..., "--compute-pool", help="Compute pool to run the service on."
+        ...,
+        "--compute-pool",
+        help="Compute pool to run the service on.",
+        show_default=False,
     ),
     spec_path: Path = SpecPathOption,
     min_instances: int = MinInstancesOption(),
     max_instances: Optional[int] = MaxInstancesOption(),
     auto_resume: bool = AutoResumeOption(),
     external_access_integrations: Optional[List[str]] = typer.Option(
         None,
@@ -127,18 +155,24 @@
     return QueryJsonValueResult(cursor)
 
 
 @app.command(requires_connection=True)
 def logs(
     name: str = ServiceNameArgument,
     container_name: str = typer.Option(
-        ..., "--container-name", help="Name of the container."
+        ...,
+        "--container-name",
+        help="Name of the container.",
+        show_default=False,
     ),
     instance_id: str = typer.Option(
-        ..., "--instance-id", help="ID of the service instance, starting with 0."
+        ...,
+        "--instance-id",
+        help="ID of the service instance, starting with 0.",
+        show_default=False,
     ),
     num_lines: int = typer.Option(
         500, "--num-lines", help="Number of lines to retrieve."
     ),
     **options,
 ):
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 from pathlib import Path
 from typing import List, Optional
 
 import yaml
 from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB, ObjectType
 from snowflake.cli.api.secure_path import SecurePath
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/sql/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+from __future__ import annotations
+
 from pathlib import Path
 from typing import List, Optional
 
 import typer
-from snowflake.cli.api.commands.flags import parse_key_value_variables
+from snowflake.cli.api.commands.flags import (
+    parse_key_value_variables,
+    project_definition_option,
+)
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.output.types import CommandResult, MultipleResults, QueryResult
 from snowflake.cli.plugins.sql.manager import SqlManager
 
 # simple Typer with defaults because it won't become a command group as it contains only one command
 app = SnowTyper()
 
@@ -15,23 +20,23 @@
     parts = key_value_str.split("=")
     if len(parts) < 2:
         raise ValueError("Passed key-value pair does not comform with key=value format")
 
     return parts[0], "=".join(parts[1:])
 
 
-@app.command(name="sql", requires_connection=True)
+@app.command(name="sql", requires_connection=True, no_args_is_help=True)
 def execute_sql(
     query: Optional[str] = typer.Option(
         None,
         "--query",
         "-q",
         help="Query to execute.",
     ),
-    file: Optional[Path] = typer.Option(
+    files: Optional[List[Path]] = typer.Option(
         None,
         "--filename",
         "-f",
         exists=True,
         file_okay=True,
         dir_okay=False,
         readable=True,
@@ -46,26 +51,29 @@
     data_override: List[str] = typer.Option(
         None,
         "--variable",
         "-D",
         help="String in format of key=value. If provided the SQL content will "
         "be treated as template and rendered using provided data.",
     ),
+    _: Optional[str] = project_definition_option(optional=True),
     **options,
 ) -> CommandResult:
     """
     Executes Snowflake query.
 
+    Use either query, filename or input option.
+
     Query to execute can be specified using query option, filename option (all queries from file will be executed)
     or via stdin by piping output from other command. For example `cat my.sql | snow sql -i`.
 
-    The command supports variable substitution that happens on client-side. Both $VARIABLE or ${ VARIABLE }
+    The command supports variable substitution that happens on client-side. Both &VARIABLE or &{ VARIABLE }
     syntax are supported.
     """
     data = {}
     if data_override:
         data = {v.key: v.value for v in parse_key_value_variables(data_override)}
 
-    single_statement, cursors = SqlManager().execute(query, file, std_in, data=data)
+    single_statement, cursors = SqlManager().execute(query, files, std_in, data=data)
     if single_statement:
         return QueryResult(next(cursors))
     return MultipleResults((QueryResult(c) for c in cursors))
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/sql/manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,75 @@
 from __future__ import annotations
 
 import sys
 from io import StringIO
+from itertools import chain
 from pathlib import Path
-from typing import Dict, Iterable, Optional, Tuple
+from typing import Dict, Iterable, List, Tuple
 
 from click import ClickException, UsageError
 from jinja2 import UndefinedError
 from snowflake.cli.api.secure_path import UNLIMITED, SecurePath
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
-from snowflake.cli.api.utils.rendering import snowflake_cli_jinja_render
+from snowflake.cli.api.utils.rendering import snowflake_sql_jinja_render
 from snowflake.cli.plugins.sql.snowsql_templating import transpile_snowsql_templates
 from snowflake.connector.cursor import SnowflakeCursor
 from snowflake.connector.util_text import split_statements
 
+IsSingleStatement = bool
+
 
 class SqlManager(SqlExecutionMixin):
     def execute(
         self,
-        query: Optional[str],
-        file: Optional[Path],
+        query: str | None,
+        files: List[Path] | None,
         std_in: bool,
         data: Dict | None = None,
-    ) -> Tuple[int, Iterable[SnowflakeCursor]]:
-        inputs = [query, file, std_in]
-        if not any(inputs):
-            raise UsageError("Use either query, filename or input option.")
-
+    ) -> Tuple[IsSingleStatement, Iterable[SnowflakeCursor]]:
+        inputs = [query, files, std_in]
         # Check if any two inputs were provided simultaneously
         if len([i for i in inputs if i]) > 1:
             raise UsageError(
                 "Multiple input sources specified. Please specify only one."
             )
 
         if std_in:
             query = sys.stdin.read()
-        elif file:
-            query = SecurePath(file).read_text(file_size_limit_mb=UNLIMITED)
+        if query:
+            return self._execute_single_query(query=query, data=data)
 
-        if data:
-            # Do rendering if any data was provided
-            try:
-                query = transpile_snowsql_templates(query)
-                query = snowflake_cli_jinja_render(content=query, data=data)
-            except UndefinedError as err:
-                raise ClickException(f"SQL template rendering error: {err}")
+        if files:
+            # Multiple files
+            results = []
+            single_statement = False
+            for file in files:
+                query_from_file = SecurePath(file).read_text(
+                    file_size_limit_mb=UNLIMITED
+                )
+                single_statement, result = self._execute_single_query(
+                    query=query_from_file, data=data
+                )
+                results.append(result)
+
+            # Use single_statement if there's only one, otherwise this is multi statement result
+            single_statement = len(files) == 1 and single_statement
+            return single_statement, chain.from_iterable(results)
+
+        # At that point, no stdin, query or files were provided
+        raise UsageError("Use either query, filename or input option.")
+
+    def _execute_single_query(
+        self, query: str, data: Dict | None = None
+    ) -> Tuple[IsSingleStatement, Iterable[SnowflakeCursor]]:
+        try:
+            query = transpile_snowsql_templates(query)
+            query = snowflake_sql_jinja_render(content=query, data=data)
+        except UndefinedError as err:
+            raise ClickException(f"SQL template rendering error: {err}")
 
         statements = tuple(
             statement
             for statement, _ in split_statements(StringIO(query), remove_comments=True)
         )
         single_statement = len(statements) == 1
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/stage/commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,35 +7,51 @@
 
 import click
 import typer
 from snowflake.cli.api.commands.flags import (
     OnErrorOption,
     PatternOption,
     VariablesOption,
+    like_option,
 )
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.console import cli_console
+from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.output.types import (
     CollectionResult,
     CommandResult,
     ObjectResult,
     QueryResult,
     SingleQueryResult,
 )
 from snowflake.cli.api.utils.path_utils import is_stage_path
+from snowflake.cli.plugins.object.command_aliases import (
+    add_object_command_aliases,
+    scope_option,
+)
 from snowflake.cli.plugins.stage.diff import DiffResult, compute_stage_diff
 from snowflake.cli.plugins.stage.manager import OnErrorType, StageManager
 
 app = SnowTyper(
     name="stage",
     help="Manages stages.",
 )
 
 StageNameArgument = typer.Argument(..., help="Name of the stage.", show_default=False)
 
+add_object_command_aliases(
+    app=app,
+    object_type=ObjectType.STAGE,
+    name_argument=StageNameArgument,
+    like_option=like_option(
+        help_example='`list --like "my%"` lists all stages that begin with “my”',
+    ),
+    scope_option=scope_option(help_example="`list --in database my_db`"),
+)
+
 
 @app.command("list-files", requires_connection=True)
 def stage_list_files(
     stage_name: str = StageNameArgument, pattern=PatternOption, **options
 ) -> CommandResult:
     """
     Lists the stage contents.
@@ -108,29 +124,39 @@
     cursor = StageManager().create(stage_name=stage_name)
     return SingleQueryResult(cursor)
 
 
 @app.command("remove", requires_connection=True)
 def stage_remove(
     stage_name: str = StageNameArgument,
-    file_name: str = typer.Argument(..., help="Name of the file to remove."),
+    file_name: str = typer.Argument(
+        ...,
+        help="Name of the file to remove.",
+        show_default=False,
+    ),
     **options,
 ) -> CommandResult:
     """
     Removes a file from a stage.
     """
 
     cursor = StageManager().remove(stage_name=stage_name, path=file_name)
     return SingleQueryResult(cursor)
 
 
 @app.command("diff", hidden=True, requires_connection=True)
 def stage_diff(
-    stage_name: str = typer.Argument(help="Fully qualified name of a stage"),
-    folder_name: str = typer.Argument(help="Path to local folder"),
+    stage_name: str = typer.Argument(
+        help="Fully qualified name of a stage",
+        show_default=False,
+    ),
+    folder_name: str = typer.Argument(
+        help="Path to local folder",
+        show_default=False,
+    ),
     **options,
 ) -> ObjectResult:
     """
     Diffs a stage with a local folder.
     """
     diff: DiffResult = compute_stage_diff(Path(folder_name), stage_name)
     return ObjectResult(str(diff))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/diff.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/stage/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import hashlib
 import logging
 import re
 from dataclasses import dataclass, field
 from pathlib import Path, PurePosixPath
 from typing import Collection, Dict, List, Optional
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/stage/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/commands.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/streamlit/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,75 @@
+from __future__ import annotations
+
 import logging
 from pathlib import Path
 
 import click
 import typer
 from click import ClickException
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.decorators import (
     with_experimental_behaviour,
     with_project_definition,
 )
-from snowflake.cli.api.commands.flags import ReplaceOption
+from snowflake.cli.api.commands.flags import ReplaceOption, like_option
 from snowflake.cli.api.commands.project_initialisation import add_init_command
 from snowflake.cli.api.commands.snow_typer import SnowTyper
+from snowflake.cli.api.constants import ObjectType
+from snowflake.cli.api.identifiers import FQN
 from snowflake.cli.api.output.types import (
     CommandResult,
     MessageResult,
     SingleQueryResult,
 )
 from snowflake.cli.api.project.schemas.streamlit.streamlit import Streamlit
+from snowflake.cli.plugins.object.command_aliases import (
+    add_object_command_aliases,
+    scope_option,
+)
 from snowflake.cli.plugins.streamlit.manager import StreamlitManager
 
 app = SnowTyper(
     name="streamlit",
     help="Manages a Streamlit app in Snowflake.",
 )
 log = logging.getLogger(__name__)
 
 
-StageNameOption: str = typer.Option(
-    "streamlit",
-    "--stage",
-    help="Name of the stage where you want to upload Streamlit app files.",
+StreamlitNameArgument = typer.Argument(
+    ..., help="Name of the Streamlit app.", show_default=False
 )
-
 OpenOption = typer.Option(
     False,
     "--open",
     help="Whether to open the Streamlit app in a browser.",
     is_flag=True,
 )
 
-
 add_init_command(
     app,
     project_type="Streamlit",
     template="default_streamlit",
     help_message="Name of the Streamlit app project directory you want to create. Defaults to `example_streamlit`.",
 )
 
+add_object_command_aliases(
+    app=app,
+    object_type=ObjectType.STREAMLIT,
+    name_argument=StreamlitNameArgument,
+    like_option=like_option(
+        help_example='`list --like "my%"` lists all streamlit apps that begin with “my”'
+    ),
+    scope_option=scope_option(help_example="`list --in database my_db`"),
+)
+
 
 @app.command("share", requires_connection=True)
 def streamlit_share(
-    name: str = typer.Argument(..., help="Name of the Streamlit app to share."),
+    name: str = StreamlitNameArgument,
     to_role: str = typer.Argument(
         ..., help="Role with which to share the Streamlit app."
     ),
     **options,
 ) -> CommandResult:
     """
     Shares a Streamlit app with another role.
@@ -106,16 +120,18 @@
 
     pages_dir = streamlit.pages_dir
     if pages_dir and not Path(pages_dir).exists():
         raise ClickException(f"Provided file {pages_dir} does not exist")
     elif pages_dir is None:
         pages_dir = "pages"
 
+    streamlit_name = FQN.from_identifier_model(streamlit).using_context()
+
     url = StreamlitManager().deploy(
-        streamlit_name=streamlit.name,
+        streamlit=streamlit_name,
         environment_file=Path(environment_file),
         pages_dir=Path(pages_dir),
         stage_name=streamlit.stage,
         main_file=Path(streamlit.main_file),
         replace=replace,
         query_warehouse=streamlit.query_warehouse,
         additional_source_files=streamlit.additional_source_files,
@@ -126,15 +142,15 @@
         typer.launch(url)
 
     return MessageResult(f"Streamlit successfully deployed and available under {url}")
 
 
 @app.command("get-url", requires_connection=True)
 def get_url(
-    name: str = typer.Argument(..., help="Name of the Streamlit app."),
+    name: str = StreamlitNameArgument,
     open_: bool = OpenOption,
     **options,
 ):
     """Returns a URL to the specified Streamlit app"""
     url = StreamlitManager().get_url(streamlit_name=name)
     if open_:
         typer.launch(url)
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/manager.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/plugins/streamlit/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from typing import List, Optional
 
 from snowflake.cli.api.commands.experimental_behaviour import (
     experimental_behaviour_enabled,
 )
 from snowflake.cli.api.feature_flags import FeatureFlag
+from snowflake.cli.api.identifiers import FQN
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.connection.util import (
     MissingConnectionHostError,
     make_snowsight_url,
 )
 from snowflake.cli.plugins.stage.manager import StageManager
 from snowflake.connector.cursor import SnowflakeCursor
@@ -84,32 +85,29 @@
         if query_warehouse:
             query.append(f"QUERY_WAREHOUSE = {query_warehouse}")
 
         self._execute_query("\n".join(query))
 
     def deploy(
         self,
-        streamlit_name: str,
+        streamlit: FQN,
         main_file: Path,
         environment_file: Optional[Path] = None,
         pages_dir: Optional[Path] = None,
         stage_name: Optional[str] = None,
         query_warehouse: Optional[str] = None,
         replace: Optional[bool] = False,
         additional_source_files: Optional[List[str]] = None,
         **options,
     ):
-        stage_manager = StageManager()
         # for backwards compatibility - quoted stage path might be case-sensitive
         # https://docs.snowflake.com/en/sql-reference/identifiers-syntax#double-quoted-identifiers
-        streamlit_name_for_root_location = self.get_name_from_fully_qualified_name(
-            streamlit_name
-        )
-        fully_qualified_name = stage_manager.to_fully_qualified_name(streamlit_name)
-        streamlit_name = self.get_name_from_fully_qualified_name(fully_qualified_name)
+        streamlit_name_for_root_location = streamlit.name
+        fully_qualified_name = streamlit.identifier
+
         if (
             experimental_behaviour_enabled()
             or FeatureFlag.ENABLE_STREAMLIT_EMBEDDED_STAGE.is_enabled()
         ):
             """
             1. Create streamlit object
             2. Upload files to embedded stage
@@ -128,15 +126,15 @@
             except ProgrammingError as e:
                 # If an error is raised because a CHECKOUT has already occurred,
                 # simply skip it and continue
                 if "Checkout already exists" in str(e):
                     log.info("Checkout already exists, continuing")
                 else:
                     raise
-            stage_path = stage_manager.to_fully_qualified_name(streamlit_name)
+            stage_path = streamlit.identifier
             embedded_stage_name = f"snow://streamlit/{stage_path}"
             root_location = f"{embedded_stage_name}/default_checkout"
 
             self._put_streamlit_files(
                 root_location,
                 main_file,
                 environment_file,
@@ -148,15 +146,15 @@
             1. Create stage
             2. Upload files to created stage
             3. Create streamlit from stage
             """
             stage_manager = StageManager()
 
             stage_name = stage_name or "streamlit"
-            stage_name = stage_manager.to_fully_qualified_name(stage_name)
+            stage_name = FQN.from_string(stage_name).using_connection(self._conn)
 
             stage_manager.create(stage_name=stage_name)
 
             root_location = stage_manager.get_standard_stage_prefix(
                 f"{stage_name}/{streamlit_name_for_root_location}"
             )
 
@@ -177,13 +175,14 @@
                 experimental=False,
             )
 
         return self.get_url(fully_qualified_name)
 
     def get_url(self, streamlit_name: str, database=None, schema=None) -> str:
         try:
+            fqn = FQN.from_string(streamlit_name).using_connection(self._conn)
             return make_snowsight_url(
                 self._conn,
-                f"/#/streamlit-apps/{self.qualified_name_for_url(streamlit_name, database=database, schema=schema)}",
+                f"/#/streamlit-apps/{fqn.url_identifier}",
             )
         except MissingConnectionHostError as e:
             return "https://app.snowflake.com"
```

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/snowflake.yml` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/procedures.py` & `snowflake_cli_labs-2.4.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py` & `snowflake_cli_labs-2.4.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py` & `snowflake_cli_labs-2.4.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py` & `snowflake_cli_labs-2.4.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py` & `snowflake_cli_labs-2.4.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/conftest.py` & `snowflake_cli_labs-2.4.0rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_cli.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_command_registration.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_command_registration.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_common_decorators.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_common_decorators.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_common_global_context.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_common_global_context.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_config.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_connection.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,16 +364,16 @@
         account="test_account",
         user="snowcli_test",
         password="top_secret",
         database="test_dv",
         schema="PUBLIC",
         warehouse="xsmall",
         application_name="snowcli",
-        _internal_application_name="snowcli",
-        _internal_application_version="0.0.0-test_patched",
+        internal_application_name="snowcli",
+        internal_application_version="0.0.0-test_patched",
     )
 
 
 @mock.patch.dict(
     os.environ,
     {
         "PRIVATE_KEY_PASSPHRASE": "password",
@@ -446,16 +446,16 @@
         account="test_account",
         user="snowcli_test",
         authenticator="SNOWFLAKE_JWT",
         database="test_dv",
         schema="PUBLIC",
         warehouse="xsmall",
         application_name="snowcli",
-        _internal_application_name="snowcli",
-        _internal_application_version="0.0.0-test_patched",
+        internal_application_name="snowcli",
+        internal_application_version="0.0.0-test_patched",
     )
 
 
 @mock.patch("snowflake.connector.connect")
 def test_session_and_master_tokens(mock_connector, mock_ctx, runner):
     ctx = mock_ctx()
     mock_connector.return_value = ctx
@@ -496,16 +496,16 @@
         user="snowcli_test",
         authenticator="SNOWFLAKE_JWT",
         database="test_dv",
         schema="PUBLIC",
         warehouse="xsmall",
         server_session_keep_alive=True,
         application_name="snowcli",
-        _internal_application_name="snowcli",
-        _internal_application_version="0.0.0-test_patched",
+        internal_application_name="snowcli",
+        internal_application_version="0.0.0-test_patched",
     )
 
 
 @mock.patch.dict(
     os.environ,
     {
         "PRIVATE_KEY_PASSPHRASE": "password",
@@ -545,16 +545,16 @@
     mock_connector.assert_called_once_with(
         application="SNOWCLI.OBJECT.LIST",
         account="my_account",
         user="jdoe",
         authenticator="SNOWFLAKE_JWT",
         private_key="secret value",
         application_name="snowcli",
-        _internal_application_name="snowcli",
-        _internal_application_version="0.0.0-test_patched",
+        internal_application_name="snowcli",
+        internal_application_version="0.0.0-test_patched",
     )
 
 
 @pytest.mark.parametrize(
     "command",
     [
         ["sql", "-q", "select 1"],
@@ -672,16 +672,16 @@
             "application": "SNOWCLI.SQL",
             "database": "test_database",
             "warehouse": "large",
             "schema": "my_schema",
             "role": "role",
             "password": "dummy",
             "application_name": "snowcli",
-            "_internal_application_name": "snowcli",
-            "_internal_application_version": "0.0.0-test_patched",
+            "internal_application_name": "snowcli",
+            "internal_application_version": "0.0.0-test_patched",
         }
 
 
 @pytest.mark.parametrize(
     "env",
     [
         {
@@ -733,16 +733,16 @@
             "application": "SNOWCLI.SQL",
             "database": "database_from_flag",
             "warehouse": "large",
             "schema": "schema_from_flag",
             "password": "password_from_flag",
             "role": "role_from_flag",
             "application_name": "snowcli",
-            "_internal_application_name": "snowcli",
-            "_internal_application_version": "0.0.0-test_patched",
+            "internal_application_name": "snowcli",
+            "internal_application_version": "0.0.0-test_patched",
         }
 
 
 @mock.patch.dict(
     os.environ,
     {
         "SNOWFLAKE_CONNECTIONS_TEST_CONNECTIONS_ACCOUNT": "account_from_connection_env",
@@ -772,16 +772,16 @@
     assert kwargs == {
         "user": "python",  # from config
         "account": "account_from_flag",
         "application": "SNOWCLI.SQL",
         "database": "database_from_connection_env",
         "role": "role_from_global_env",
         "application_name": "snowcli",
-        "_internal_application_name": "snowcli",
-        "_internal_application_version": "0.0.0-test_patched",
+        "internal_application_name": "snowcli",
+        "internal_application_version": "0.0.0-test_patched",
     }
 
 
 def test_set_default_connection_fails_if_no_connection(runner):
     with NamedTemporaryFile("w+", suffix=".toml") as tmp_file:
         result = runner.invoke_with_config_file(
             tmp_file.name, ["connection", "set-default", "foo"]
```

### Comparing `snowflake_cli_labs-2.3.1/tests/test_experimental_behaviour.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_experimental_behaviour.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_help_messages.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_help_messages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,65 @@
+from __future__ import annotations
+
+from typing import List
+
 import pytest
 from snowflake.cli.app.commands_registration.command_plugins_loader import (
     load_only_builtin_command_plugins,
 )
+from typer.core import TyperGroup
 
 
-def iter_through_all_commands_paths():
+def iter_through_all_commands(command_groups_only: bool = False):
     """
     Generator iterating through all commands.
     Paths are yielded as List[str]
     """
-    ignore_plugins = ["render"]
+    ignore_plugins = ["render", "cortex"]
+
+    no_command: List[str] = []
+    yield no_command
 
     def _iter_through_commands(command, path):
-        yield list(path)
+        if not command_groups_only or isinstance(command, TyperGroup):
+            yield list(path)
+
         for subpath, subcommand in getattr(command, "commands", {}).items():
             path.append(subpath)
             yield from _iter_through_commands(subcommand, path)
             path.pop()
 
-    yield []  # "snow" with no commands
     builtin_plugins = load_only_builtin_command_plugins()
     for plugin in builtin_plugins:
         spec = plugin.command_spec
         if not plugin.plugin_name in ignore_plugins:
             yield from _iter_through_commands(
                 spec.command, spec.full_command_path.path_segments
             )
 
 
 @pytest.mark.parametrize(
     "command",
-    iter_through_all_commands_paths(),
-    ids=(".".join(cmd) for cmd in iter_through_all_commands_paths()),
+    iter_through_all_commands(),
+    ids=(".".join(cmd) for cmd in iter_through_all_commands()),
 )
 def test_help_messages(runner, snapshot, command):
     """
     Check help messages against the snapshot
     """
     result = runner.invoke(command + ["--help"])
     assert result.exit_code == 0
     assert result.output == snapshot
+
+
+@pytest.mark.parametrize(
+    "command",
+    iter_through_all_commands(command_groups_only=True),
+    ids=(".".join(cmd) for cmd in iter_through_all_commands(command_groups_only=True)),
+)
+def test_help_messages_no_help_flag(runner, snapshot, command):
+    """
+    Check help messages against the snapshot
+    """
+    result = runner.invoke(command)
+    assert result.exit_code == 0
+    assert result.output == snapshot
```

### Comparing `snowflake_cli_labs-2.3.1/tests/test_logs.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import shutil
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Optional
 
 import pytest
```

### Comparing `snowflake_cli_labs-2.3.1/tests/test_main.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         application="SNOWCLI.OBJECT.LIST",
         database="db_for_test",
         schema="test_public",
         role="test_role",
         warehouse="xs",
         password="dummy_password",
         application_name="snowcli",
-        _internal_application_name="snowcli",
-        _internal_application_version="0.0.0-test_patched",
+        internal_application_name="snowcli",
+        internal_application_version="0.0.0-test_patched",
     )
 
 
 def test_info_callback(runner):
     result = runner.invoke(["--info"])
     assert result.exit_code == 0, result.output
     payload = json.loads(result.output)
```

### Comparing `snowflake_cli_labs-2.3.1/tests/test_project_initialisation.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_project_initialisation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_snow_connector.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_snow_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         application=expected,
         database="db_for_test",
         schema="test_public",
         role="test_role",
         warehouse="xs",
         password="dummy_password",
         application_name="snowcli",
-        _internal_application_name="snowcli",
-        _internal_application_version="0.0.0-test_patched",
+        internal_application_name="snowcli",
+        internal_application_version="0.0.0-test_patched",
     )
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
 def test_returns_nice_error_in_case_of_connectivity_error(runner):
     result = runner.invoke(["sql", "-q", "select 1"])
     assert result.exit_code == 1
```

### Comparing `snowflake_cli_labs-2.3.1/tests/test_sql.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_sql.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
-from tempfile import NamedTemporaryFile
+from tempfile import NamedTemporaryFile, TemporaryDirectory
 from unittest import mock
 
 import pytest
 from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
+from snowflake.cli.api.identifiers import FQN
 from snowflake.cli.api.project.util import identifier_to_show_like_pattern
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.sql.snowsql_templating import transpile_snowsql_templates
 from snowflake.connector.cursor import DictCursor
 from snowflake.connector.errors import ProgrammingError
 
 from tests.testing_utils.result_assertions import assert_that_result_is_usage_error
@@ -34,30 +35,45 @@
         result = runner.invoke(["sql", "-f", tmp_file.name])
 
     assert result.exit_code == 0
     mock_execute.assert_called_once_with(query)
 
 
 @mock.patch("snowflake.cli.plugins.sql.manager.SqlExecutionMixin._execute_string")
+def test_sql_execute_multiple_file(mock_execute, runner, mock_cursor):
+    mock_execute.return_value = (mock_cursor(["row"], []) for _ in range(1))
+    query = "query from file"
+
+    with TemporaryDirectory() as tmp_dir:
+        f1 = Path(tmp_dir).joinpath("f1.sql")
+        f2 = Path(tmp_dir).joinpath("f2.sql")
+
+        f1.write_text(query)
+        f2.write_text(query)
+        result = runner.invoke(["sql", "-f", f1, "-f", f2])
+
+    assert result.exit_code == 0
+    mock_execute.assert_has_calls([mock.call(query), mock.call(query)])
+
+
+@mock.patch("snowflake.cli.plugins.sql.manager.SqlExecutionMixin._execute_string")
 def test_sql_execute_from_stdin(mock_execute, runner, mock_cursor):
     mock_execute.return_value = (mock_cursor(["row"], []) for _ in range(1))
     query = "query from input"
 
     result = runner.invoke(["sql", "-i"], input=query)
 
     assert result.exit_code == 0
     mock_execute.assert_called_once_with(query)
 
 
-def test_sql_fails_if_no_query_file_or_stdin(runner):
+def test_sql_help_if_no_query_file_or_stdin(runner, snapshot):
     result = runner.invoke(["sql"])
-
-    assert_that_result_is_usage_error(
-        result, "Use either query, filename or input option."
-    )
+    assert result.exit_code == 0, result.output
+    assert result.output == snapshot
 
 
 @pytest.mark.parametrize("inputs", [("-i", "-q", "foo"), ("-i",), ("-q", "foo")])
 def test_sql_fails_if_other_inputs_and_file_provided(runner, inputs):
     with NamedTemporaryFile("r") as tmp_file:
         result = runner.invoke(["sql", *inputs, "-f", tmp_file.name])
         assert_that_result_is_usage_error(
@@ -179,37 +195,30 @@
         SqlExecutionMixin().show_specific_object("objects", "example_id", name_col="id")
     mock_execute.assert_called_once_with(
         r"show objects like 'EXAMPLE\\_ID'", cursor_class=DictCursor
     )
 
 
 @pytest.mark.parametrize(
-    "name, name_split, expected_name, expected_in_clause",
+    "fqn, expected_in_clause",
     [
         (
-            "func(number, number)",
-            ("func(number, number)", None, None),
-            "func(number, number)",
+            FQN(None, None, "func(number, number)"),
             None,
         ),
-        ("name", ("name", None, None), "name", None),
-        ("schema.name", ("name", "schema", None), "name", "in schema schema"),
-        ("db.schema.name", ("name", "schema", "db"), "name", "in schema db.schema"),
+        (FQN(None, None, "name"), None),
+        (FQN(None, "schema", "name"), "in schema schema"),
+        (FQN("db", "schema", "name"), "in schema db.schema"),
     ],
 )
-@mock.patch("snowflake.cli.api.sql_execution.from_qualified_name")
-def test_qualified_name_to_in_clause(
-    mock_from_qualified_name, name, name_split, expected_name, expected_in_clause
-):
-    mock_from_qualified_name.return_value = name_split
-    assert SqlExecutionMixin._qualified_name_to_in_clause(name) == (  # noqa: SLF001
-        expected_name,
+def test_qualified_name_to_in_clause(fqn, expected_in_clause):
+    assert SqlExecutionMixin._qualified_name_to_in_clause(fqn) == (  # noqa: SLF001
+        fqn.name,
         expected_in_clause,
     )
-    mock_from_qualified_name.assert_called_once_with(name)
 
 
 @mock.patch("snowflake.cli.plugins.sql.manager.SqlExecutionMixin._execute_query")
 @mock.patch(
     "snowflake.cli.api.sql_execution.SqlExecutionMixin._qualified_name_to_in_clause"
 )
 def test_show_specific_object_qualified_name(
@@ -239,15 +248,17 @@
 ):
     object_name = "db.schema.name"
     mock_qualified_name_to_in_clause.return_value = ("name", "in schema db.schema")
     with pytest.raises(SqlExecutionMixin.InClauseWithQualifiedNameError):
         SqlExecutionMixin().show_specific_object(
             "objects", object_name, in_clause="in database db"
         )
-    mock_qualified_name_to_in_clause.assert_called_once_with(object_name)
+    mock_qualified_name_to_in_clause.assert_called_once_with(
+        FQN.from_string(object_name)
+    )
 
 
 @mock.patch("snowflake.cli.api.sql_execution.SqlExecutionMixin._execute_query")
 def test_show_specific_object_multiple_rows(mock_execute_query):
     cursor = mock.Mock(spec=DictCursor)
     cursor.rowcount = 2
     mock_execute_query.return_value = cursor
@@ -284,29 +295,14 @@
 @mock.patch("snowflake.cli.plugins.sql.commands.SqlManager._execute_string")
 def test_rendering_of_sql(mock_execute_query, query, runner):
     result = runner.invoke(["sql", "-q", query, "-D", "aaa=foo", "-D", "bbb=bar"])
     assert result.exit_code == 0, result.output
     mock_execute_query.assert_called_once_with("select foo.bar")
 
 
-@pytest.mark.parametrize(
-    "query",
-    [
-        "select &{ aaa }.&{ bbb }",
-        "select &aaa.&bbb",
-        "select &aaa.&{ bbb }",
-    ],
-)
-@mock.patch("snowflake.cli.plugins.sql.commands.SqlManager._execute_string")
-def test_no_rendering_of_sql_if_no_data(mock_execute_query, query, runner):
-    result = runner.invoke(["sql", "-q", query])
-    assert result.exit_code == 0, result.output
-    mock_execute_query.assert_called_once_with(query)
-
-
 @pytest.mark.parametrize("query", ["select &{ foo }", "select &foo"])
 def test_execution_fails_if_unknown_variable(runner, query):
     result = runner.invoke(["sql", "-q", query, "-D", "bbb=1"])
     assert "SQL template rendering error: 'foo' is undefined" in result.output
 
 
 @pytest.mark.parametrize(
@@ -321,7 +317,48 @@
         # Test templating is ignored
         ("&{ foo }", "&{ foo }"),
         ("select *  from &{ foo } join bar", "select *  from &{ foo } join bar"),
     ],
 )
 def test_snowsql_compatibility(text, expected):
     assert transpile_snowsql_templates(text) == expected
+
+
+@mock.patch("snowflake.cli.plugins.sql.commands.SqlManager._execute_string")
+def test_uses_variables_from_snowflake_yml(
+    mock_execute_query, project_directory, runner
+):
+    with project_directory("sql_templating"):
+        result = runner.invoke(["sql", "-q", "select &{ ctx.env.sf_var }"])
+
+    assert result.exit_code == 0
+    mock_execute_query.assert_called_once_with("select foo_value")
+
+
+@mock.patch("snowflake.cli.plugins.sql.commands.SqlManager._execute_string")
+def test_uses_variables_from_snowflake_local_yml(
+    mock_execute_query, project_directory, runner
+):
+    with project_directory("sql_templating"):
+        result = runner.invoke(["sql", "-q", "select &{ ctx.env.sf_var_override }"])
+
+    assert result.exit_code == 0
+    mock_execute_query.assert_called_once_with("select foo_value_override")
+
+
+@mock.patch("snowflake.cli.plugins.sql.commands.SqlManager._execute_string")
+def test_uses_variables_from_cli_are_added_outside_context(
+    mock_execute_query, project_directory, runner
+):
+    with project_directory("sql_templating"):
+        result = runner.invoke(
+            [
+                "sql",
+                "-q",
+                "select &{ ctx.env.sf_var } &{ other }",
+                "-D",
+                "other=other_value",
+            ]
+        )
+
+    assert result.exit_code == 0, result.output
+    mock_execute_query.assert_called_once_with("select foo_value other_value")
```

### Comparing `snowflake_cli_labs-2.3.1/tests/test_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_zipper.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/__snapshots__/test_config.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/__snapshots__/test_config.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/__snapshots__/test_connection.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/__snapshots__/test_connection.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/__snapshots__/test_help_messages.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/__snapshots__/test_help_messages.ambr`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,31 @@
   '''
                                                                                   
    Usage: default [OPTIONS] COMMAND [ARGS]...                                     
                                                                                   
    Snowflake CLI tool for developers.                                             
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --version                    Shows version of the Snowflake CLI              │
-  │ --info                       Shows information about the Snowflake CLI       │
-  │ --config-file          FILE  Specifies Snowflake CLI configuration file that │
-  │                              should be used                                  │
-  │                              [default: None]                                 │
-  │ --help         -h            Show this message and exit.                     │
+  │ --version                           Shows version of the Snowflake CLI       │
+  │ --info                              Shows information about the Snowflake    │
+  │                                     CLI                                      │
+  │ --config-file                 FILE  Specifies Snowflake CLI configuration    │
+  │                                     file that should be used                 │
+  │                                     [default: None]                          │
+  │ --install-completion                Install completion for the current       │
+  │                                     shell.                                   │
+  │ --show-completion                   Show completion for the current shell,   │
+  │                                     to copy it or customize the              │
+  │                                     installation.                            │
+  │ --help                -h            Show this message and exit.              │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
   │ app          Manages a Snowflake Native App                                  │
   │ connection   Manages connections to Snowflake.                               │
+  │ cortex       Provides access to Snowflake Cortex.                            │
   │ git          Manages git repositories in Snowflake.                          │
   │ object       Manages Snowflake objects like warehouses and stages            │
   │ snowpark     Manages procedures and functions.                               │
   │ spcs         Manages Snowpark Container Services compute pools, services,    │
   │              image registries, and image repositories.                       │
   │ sql          Executes Snowflake query.                                       │
   │ stage        Manages stages.                                                 │
@@ -305,56 +312,84 @@
    Usage: default app run [OPTIONS]                                               
                                                                                   
    Creates an application package in your Snowflake account, uploads code files   
    to its stage, then creates or upgrades an application object from the          
    application package.                                                           
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --version                         TEXT  The version defined in an existing   │
-  │                                         application package from which you   │
-  │                                         want to create an application        │
-  │                                         object. The application object and   │
-  │                                         application package names are        │
-  │                                         determined from the project          │
-  │                                         definition file.                     │
-  │                                         [default: None]                      │
-  │ --patch                           TEXT  The patch number under the given     │
-  │                                         `--version` defined in an existing   │
-  │                                         application package that should be   │
-  │                                         used to create an application        │
-  │                                         object. The application object and   │
-  │                                         application package names are        │
-  │                                         determined from the project          │
-  │                                         definition file.                     │
-  │                                         [default: None]                      │
-  │ --from-release-directive                Creates or upgrades an application   │
-  │                                         object to the version and patch      │
-  │                                         specified by the release directive   │
-  │                                         applicable to your Snowflake         │
-  │                                         account. The command fails if no     │
-  │                                         release directive exists for your    │
-  │                                         Snowflake account for a given        │
-  │                                         application package, which is        │
-  │                                         determined from the project          │
-  │                                         definition file. Default: unset.     │
-  │ --interactive             -i            When enabled, this option displays   │
-  │                                         prompts even if the standard input   │
-  │                                         and output are not terminal devices. │
-  │                                         Defaults to unset.                   │
-  │ --force                                 When enabled, this option causes the │
-  │                                         command to implicitly approve any    │
-  │                                         prompts that arise. You should       │
-  │                                         enable this option if interactive    │
-  │                                         mode is not specified and if you     │
-  │                                         want perform potentially destructive │
-  │                                         actions. Defaults to unset.          │
-  │ --project                 -p      TEXT  Path where the Snowflake Native App  │
-  │                                         project resides. Defaults to current │
-  │                                         working directory.                   │
-  │ --help                    -h            Show this message and exit.          │
+  │ --version                                       TEXT  The version defined in │
+  │                                                       an existing            │
+  │                                                       application package    │
+  │                                                       from which you want to │
+  │                                                       create an application  │
+  │                                                       object. The            │
+  │                                                       application object and │
+  │                                                       application package    │
+  │                                                       names are determined   │
+  │                                                       from the project       │
+  │                                                       definition file.       │
+  │                                                       [default: None]        │
+  │ --patch                                         TEXT  The patch number under │
+  │                                                       the given `--version`  │
+  │                                                       defined in an existing │
+  │                                                       application package    │
+  │                                                       that should be used to │
+  │                                                       create an application  │
+  │                                                       object. The            │
+  │                                                       application object and │
+  │                                                       application package    │
+  │                                                       names are determined   │
+  │                                                       from the project       │
+  │                                                       definition file.       │
+  │                                                       [default: None]        │
+  │ --from-release-direct…                                Creates or upgrades an │
+  │                                                       application object to  │
+  │                                                       the version and patch  │
+  │                                                       specified by the       │
+  │                                                       release directive      │
+  │                                                       applicable to your     │
+  │                                                       Snowflake account. The │
+  │                                                       command fails if no    │
+  │                                                       release directive      │
+  │                                                       exists for your        │
+  │                                                       Snowflake account for  │
+  │                                                       a given application    │
+  │                                                       package, which is      │
+  │                                                       determined from the    │
+  │                                                       project definition     │
+  │                                                       file. Default: unset.  │
+  │ --interactive               --no-interactive          When enabled, this     │
+  │                                                       option displays        │
+  │                                                       prompts even if the    │
+  │                                                       standard input and     │
+  │                                                       output are not         │
+  │                                                       terminal devices.      │
+  │                                                       Defaults to True in an │
+  │                                                       interactive shell      │
+  │                                                       environment, and False │
+  │                                                       otherwise.             │
+  │ --force                                               When enabled, this     │
+  │                                                       option causes the      │
+  │                                                       command to implicitly  │
+  │                                                       approve any prompts    │
+  │                                                       that arise. You should │
+  │                                                       enable this option if  │
+  │                                                       interactive mode is    │
+  │                                                       not specified and if   │
+  │                                                       you want perform       │
+  │                                                       potentially            │
+  │                                                       destructive actions.   │
+  │                                                       Defaults to unset.     │
+  │ --project               -p                      TEXT  Path where the         │
+  │                                                       Snowflake Native App   │
+  │                                                       project resides.       │
+  │                                                       Defaults to current    │
+  │                                                       working directory.     │
+  │ --help                  -h                            Show this message and  │
+  │                                                       exit.                  │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -412,22 +447,38 @@
                                                                                   
    Usage: default app teardown [OPTIONS]                                          
                                                                                   
    Attempts to drop both the application object and application package as        
    defined in the project definition file.                                        
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --force                  When enabled, this option causes the command to     │
-  │                          implicitly approve any prompts that arise. You      │
-  │                          should enable this option if interactive mode is    │
-  │                          not specified and if you want perform potentially   │
-  │                          destructive actions. Defaults to unset.             │
-  │ --project  -p      TEXT  Path where the Snowflake Native App project         │
-  │                          resides. Defaults to current working directory.     │
-  │ --help     -h            Show this message and exit.                         │
+  │ --force                                      When enabled, this option       │
+  │                                              causes the command to           │
+  │                                              implicitly approve any prompts  │
+  │                                              that arise. You should enable   │
+  │                                              this option if interactive mode │
+  │                                              is not specified and if you     │
+  │                                              want perform potentially        │
+  │                                              destructive actions. Defaults   │
+  │                                              to unset.                       │
+  │ --cascade          --no-cascade              Whether to drop all application │
+  │                                              objects owned by the            │
+  │                                              application within the account. │
+  │                                              Default: false.                 │
+  │ --interactive      --no-interactive          When enabled, this option       │
+  │                                              displays prompts even if the    │
+  │                                              standard input and output are   │
+  │                                              not terminal devices. Defaults  │
+  │                                              to True in an interactive shell │
+  │                                              environment, and False          │
+  │                                              otherwise.                      │
+  │ --project      -p                      TEXT  Path where the Snowflake Native │
+  │                                              App project resides. Defaults   │
+  │                                              to current working directory.   │
+  │ --help         -h                            Show this message and exit.     │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -492,37 +543,53 @@
   │   version      [VERSION]  Version to define in your application package. If  │
   │                           the version already exists, an auto-incremented    │
   │                           patch is added to the version instead. Defaults to │
   │                           the version specified in the `manifest.yml` file.  │
   │                           [default: None]                                    │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --patch                   TEXT  The patch number you want to create for an   │
-  │                                 existing version. Defaults to undefined if   │
-  │                                 it is not set, which means the Snowflake CLI │
-  │                                 either uses the patch specified in the       │
-  │                                 `manifest.yml` file or automatically         │
-  │                                 generates a new patch number.                │
-  │                                 [default: None]                              │
-  │ --skip-git-check                When enabled, the Snowflake CLI skips        │
-  │                                 checking if your project has any untracked   │
-  │                                 or stages files in git. Default: unset.      │
-  │ --interactive     -i            When enabled, this option displays prompts   │
-  │                                 even if the standard input and output are    │
-  │                                 not terminal devices. Defaults to unset.     │
-  │ --force                         When enabled, this option causes the command │
-  │                                 to implicitly approve any prompts that       │
-  │                                 arise. You should enable this option if      │
-  │                                 interactive mode is not specified and if you │
-  │                                 want perform potentially destructive         │
-  │                                 actions. Defaults to unset.                  │
-  │ --project         -p      TEXT  Path where the Snowflake Native App project  │
-  │                                 resides. Defaults to current working         │
-  │                                 directory.                                   │
-  │ --help            -h            Show this message and exit.                  │
+  │ --patch                                   TEXT  The patch number you want to │
+  │                                                 create for an existing       │
+  │                                                 version. Defaults to         │
+  │                                                 undefined if it is not set,  │
+  │                                                 which means the Snowflake    │
+  │                                                 CLI either uses the patch    │
+  │                                                 specified in the             │
+  │                                                 `manifest.yml` file or       │
+  │                                                 automatically generates a    │
+  │                                                 new patch number.            │
+  │                                                 [default: None]              │
+  │ --skip-git-check                                When enabled, the Snowflake  │
+  │                                                 CLI skips checking if your   │
+  │                                                 project has any untracked or │
+  │                                                 stages files in git.         │
+  │                                                 Default: unset.              │
+  │ --interactive         --no-interactive          When enabled, this option    │
+  │                                                 displays prompts even if the │
+  │                                                 standard input and output    │
+  │                                                 are not terminal devices.    │
+  │                                                 Defaults to True in an       │
+  │                                                 interactive shell            │
+  │                                                 environment, and False       │
+  │                                                 otherwise.                   │
+  │ --force                                         When enabled, this option    │
+  │                                                 causes the command to        │
+  │                                                 implicitly approve any       │
+  │                                                 prompts that arise. You      │
+  │                                                 should enable this option if │
+  │                                                 interactive mode is not      │
+  │                                                 specified and if you want    │
+  │                                                 perform potentially          │
+  │                                                 destructive actions.         │
+  │                                                 Defaults to unset.           │
+  │ --project         -p                      TEXT  Path where the Snowflake     │
+  │                                                 Native App project resides.  │
+  │                                                 Defaults to current working  │
+  │                                                 directory.                   │
+  │ --help            -h                            Show this message and exit.  │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -587,26 +654,34 @@
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │   version      [VERSION]  Version defined in an application package that you │
   │                           want to drop. Defaults to the version specified in │
   │                           the `manifest.yml` file.                           │
   │                           [default: None]                                    │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --interactive  -i            When enabled, this option displays prompts even │
-  │                              if the standard input and output are not        │
-  │                              terminal devices. Defaults to unset.            │
-  │ --force                      When enabled, this option causes the command to │
-  │                              implicitly approve any prompts that arise. You  │
-  │                              should enable this option if interactive mode   │
-  │                              is not specified and if you want perform        │
-  │                              potentially destructive actions. Defaults to    │
-  │                              unset.                                          │
-  │ --project      -p      TEXT  Path where the Snowflake Native App project     │
-  │                              resides. Defaults to current working directory. │
-  │ --help         -h            Show this message and exit.                     │
+  │ --interactive      --no-interactive          When enabled, this option       │
+  │                                              displays prompts even if the    │
+  │                                              standard input and output are   │
+  │                                              not terminal devices. Defaults  │
+  │                                              to True in an interactive shell │
+  │                                              environment, and False          │
+  │                                              otherwise.                      │
+  │ --force                                      When enabled, this option       │
+  │                                              causes the command to           │
+  │                                              implicitly approve any prompts  │
+  │                                              that arise. You should enable   │
+  │                                              this option if interactive mode │
+  │                                              is not specified and if you     │
+  │                                              want perform potentially        │
+  │                                              destructive actions. Defaults   │
+  │                                              to unset.                       │
+  │ --project      -p                      TEXT  Path where the Snowflake Native │
+  │                                              App project resides. Defaults   │
+  │                                              to current working directory.   │
+  │ --help         -h                            Show this message and exit.     │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -894,14 +969,43 @@
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
   │ --enable-diag                             Run python connector diagnostic    │
   │                                           test                               │
   │ --diag-log-path                     TEXT  Diagnostic report path             │
   │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
   │                                           allowlist                          │
@@ -936,14 +1040,514 @@
   │ set-default   Changes default connection to provided value.                  │
   │ test          Tests the connection to Snowflake.                             │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[cortex.complete]
+  '''
+                                                                                  
+   Usage: default cortex complete [OPTIONS] [TEXT]                                
+                                                                                  
+   Given a prompt, the command generates a response using your choice of language 
+   model. In the simplest use case, the prompt is a single string. You may also   
+   provide a JSON file with conversation history including multiple prompts and   
+   responses for interactive chat-style usage.                                    
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │   text      [TEXT]  Prompt to be used to generate a completion. Cannot be    │
+  │                     combined with --file option.                             │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --model          TEXT  String specifying the model to be used.               │
+  │                        [default: snowflake-arctic]                           │
+  │ --file           FILE  JSON file containing conversation history to be used  │
+  │                        to generate a completion. Cannot be combined with     │
+  │                        TEXT argument.                                        │
+  │ --help   -h            Show this message and exit.                           │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[cortex.extract-answer]
+  '''
+                                                                                  
+   Usage: default cortex extract-answer [OPTIONS] [QUESTION]                      
+   [SOURCE_DOCUMENT_TEXT]                                                         
+                                                                                  
+   Extracts an answer to a given question from a text document. The document may  
+   be a plain-English document or a string representation of a semi-structured    
+   (JSON) data object.                                                            
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │   question                  [QUESTION]              String containing the    │
+  │                                                     question to be answered. │
+  │   source_document_text      [SOURCE_DOCUMENT_TEXT]  String containing the    │
+  │                                                     plain-text or JSON       │
+  │                                                     document that contains   │
+  │                                                     the answer to the        │
+  │                                                     question. Cannot be      │
+  │                                                     combined with --file     │
+  │                                                     option.                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --file          FILE  File containing the plain-text or JSON document that   │
+  │                       contains the answer to the question. Cannot be         │
+  │                       combined with SOURCE_DOCUMENT_TEXT argument.           │
+  │ --help  -h            Show this message and exit.                            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[cortex.search]
+  '''
+                                                                                  
+   Usage: default cortex search [OPTIONS] QUERY                                   
+                                                                                  
+   Performs query search using Cortex Search Services.                            
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    query      TEXT  The search query string [default: None] [required]     │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ *  --service          TEXT     Cortex search service to be used. Example:    │
+  │                                --service my_cortex_service                   │
+  │                                [default: None]                               │
+  │                                [required]                                    │
+  │    --columns          TEXT     Columns that will be returned with the        │
+  │                                results. If none is provided, only search     │
+  │                                column will be included in results. Example   │
+  │                                --columns "foo" --columns "bar"               │
+  │                                [default: None]                               │
+  │    --limit            INTEGER  Maximum number of results retrieved           │
+  │                                [default: 1]                                  │
+  │    --help     -h               Show this message and exit.                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[cortex.sentiment]
+  '''
+                                                                                  
+   Usage: default cortex sentiment [OPTIONS] [TEXT]                               
+                                                                                  
+   Returns sentiment as a score between -1 to 1 (with -1 being the most negative  
+   and 1 the most positive, with values around 0 neutral) for the given           
+   English-language input text.                                                   
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │   text      [TEXT]  String containing the text for which a sentiment score   │
+  │                     should be calculated. Cannot be combined with --file     │
+  │                     option.                                                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --file          FILE  File containing the text for which a sentiment score   │
+  │                       should be calculated. Cannot be combined with TEXT     │
+  │                       argument.                                              │
+  │ --help  -h            Show this message and exit.                            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[cortex.summarize]
+  '''
+                                                                                  
+   Usage: default cortex summarize [OPTIONS] [TEXT]                               
+                                                                                  
+   Summarizes the given English-language input text.                              
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │   text      [TEXT]  String containing the English text from which a summary  │
+  │                     should be generated. Cannot be combined with --file      │
+  │                     option.                                                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --file          FILE  File containing the English text from which a summary  │
+  │                       should be generated. Cannot be combined with TEXT      │
+  │                       argument.                                              │
+  │ --help  -h            Show this message and exit.                            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[cortex.translate]
+  '''
+                                                                                  
+   Usage: default cortex translate [OPTIONS] [TEXT]                               
+                                                                                  
+   Translates text from the indicated or detected source language to a target     
+   language.                                                                      
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │   text      [TEXT]  String containing the text to be translated. Cannot be   │
+  │                     combined with --file option.                             │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │    --from          TEXT  String specifying the language code for the         │
+  │                          language the text is currently in. See Snowflake    │
+  │                          Cortex documentation for a list of supported        │
+  │                          language codes.                                     │
+  │ *  --to            TEXT  String specifying the language code into which the  │
+  │                          text should be translated. See Snowflake Cortex     │
+  │                          documentation for a list of supported language      │
+  │                          codes.                                              │
+  │                          [required]                                          │
+  │    --file          FILE  File containing the text to be translated. Cannot   │
+  │                          be combined with TEXT argument.                     │
+  │    --help  -h            Show this message and exit.                         │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[cortex]
+  '''
+                                                                                  
+   Usage: default cortex [OPTIONS] COMMAND [ARGS]...                              
+                                                                                  
+   Provides access to Snowflake Cortex.                                           
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ complete         Given a prompt, the command generates a response using your │
+  │                  choice of language model. In the simplest use case, the     │
+  │                  prompt is a single string. You may also provide a JSON file │
+  │                  with conversation history including multiple prompts and    │
+  │                  responses for interactive chat-style usage.                 │
+  │ extract-answer   Extracts an answer to a given question from a text          │
+  │                  document. The document may be a plain-English document or a │
+  │                  string representation of a semi-structured (JSON) data      │
+  │                  object.                                                     │
+  │ search           Performs query search using Cortex Search Services.         │
+  │ sentiment        Returns sentiment as a score between -1 to 1 (with -1 being │
+  │                  the most negative and 1 the most positive, with values      │
+  │                  around 0 neutral) for the given English-language input      │
+  │                  text.                                                       │
+  │ summarize        Summarizes the given English-language input text.           │
+  │ translate        Translates text from the indicated or detected source       │
+  │                  language to a target language.                              │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[git.copy]
   '''
                                                                                   
    Usage: default git copy [OPTIONS] REPOSITORY_PATH DESTINATION_PATH             
                                                                                   
    Copies all files from given state of repository to local directory or stage.   
    If the source path ends with '/', the command copies contents of specified     
@@ -1020,14 +1624,152 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[git.describe]
+  '''
+                                                                                  
+   Usage: default git describe [OPTIONS] NAME                                     
+                                                                                  
+   Provides description of git repository.                                        
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Identifier of the git repository. For example: my_repo  │
+  │                      [required]                                              │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git.drop]
+  '''
+                                                                                  
+   Usage: default git drop [OPTIONS] NAME                                         
+                                                                                  
+   Drops git repository with given name.                                          
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Identifier of the git repository. For example: my_repo  │
+  │                      [required]                                              │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[git.execute]
   '''
                                                                                   
    Usage: default git execute [OPTIONS] REPOSITORY_PATH                           
                                                                                   
    Execute immediate all files from the repository path. Files can be filtered    
    with glob like pattern, e.g. `@my_repo/branches/main/*.sql`,                   
@@ -1042,14 +1784,17 @@
   │                                 [default: None]                              │
   │                                 [required]                                   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --on-error          [break|continue]  What to do when an error occurs.       │
   │                                       Defaults to break.                     │
   │                                       [default: break]                       │
+  │ --variable  -D      TEXT              Variables for the template. For        │
+  │                                       example: `-D "<key>=<value>"`, string  │
+  │                                       values must be in `''`.                │
   │ --help      -h                        Show this message and exit.            │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
@@ -1109,15 +1854,14 @@
    Usage: default git fetch [OPTIONS] REPOSITORY_NAME                             
                                                                                   
    Fetch changes from origin to Snowflake repository.                             
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    repository_name      TEXT  Identifier of the git repository. For        │
   │                                 example: my_repo                             │
-  │                                 [default: None]                              │
   │                                 [required]                                   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
@@ -1180,15 +1924,14 @@
    Usage: default git list-branches [OPTIONS] REPOSITORY_NAME                     
                                                                                   
    List all branches in the repository.                                           
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    repository_name      TEXT  Identifier of the git repository. For        │
   │                                 example: my_repo                             │
-  │                                 [default: None]                              │
   │                                 [required]                                   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --like  -l      TEXT  SQL LIKE pattern for filtering objects by name. For    │
   │                       example, `list-branches --like "%_test"` lists all     │
   │                       branches that end with "_test".                        │
   │                       [default: %%]                                          │
@@ -1331,15 +2074,14 @@
    Usage: default git list-tags [OPTIONS] REPOSITORY_NAME                         
                                                                                   
    List all tags in the repository.                                               
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    repository_name      TEXT  Identifier of the git repository. For        │
   │                                 example: my_repo                             │
-  │                                 [default: None]                              │
   │                                 [required]                                   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --like  -l      TEXT  SQL LIKE pattern for filtering objects by name. For    │
   │                       example, `list-tags --like "v2.0%"` lists all tags     │
   │                       that start with "v2.0".                                │
   │                       [default: %%]                                          │
@@ -1396,14 +2138,88 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[git.list]
+  '''
+                                                                                  
+   Usage: default git list [OPTIONS]                                              
+                                                                                  
+   Lists all available git repositories.                                          
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT            SQL LIKE pattern for filtering objects by    │
+  │                                 name. For example, `list --like "my%"` lists │
+  │                                 all git repositories with name that begin    │
+  │                                 with “my”.                                   │
+  │                                 [default: %%]                                │
+  │ --in            <TEXT TEXT>...  Specifies the scope of this command using    │
+  │                                 '--in <scope> <name>', for example `list     │
+  │                                 --in database my_db`.                        │
+  │                                 [default: None, None]                        │
+  │ --help  -h                      Show this message and exit.                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[git.setup]
   '''
                                                                                   
    Usage: default git setup [OPTIONS] REPOSITORY_NAME                             
                                                                                   
    Sets up a git repository object.                                               
    You will be prompted for:                                                      
@@ -1412,15 +2228,14 @@
    if origin repository does not require authentication for RO operations (clone, 
    fetch)                                                                         
    * API integration - object allowing Snowflake to interact with git repository. 
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    repository_name      TEXT  Identifier of the git repository. For        │
   │                                 example: my_repo                             │
-  │                                 [default: None]                              │
   │                                 [required]                                   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
@@ -1486,40 +2301,116 @@
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
   │ copy            Copies all files from given state of repository to local     │
   │                 directory or stage.                                          │
+  │ describe        Provides description of git repository.                      │
+  │ drop            Drops git repository with given name.                        │
   │ execute         Execute immediate all files from the repository path. Files  │
   │                 can be filtered with glob like pattern, e.g.                 │
   │                 `@my_repo/branches/main/*.sql`,                              │
   │                 `@my_repo/branches/main/dev/*`. Only files with `.sql`       │
   │                 extension will be executed.                                  │
   │ fetch           Fetch changes from origin to Snowflake repository.           │
+  │ list            Lists all available git repositories.                        │
   │ list-branches   List all branches in the repository.                         │
   │ list-files      List files from given state of git repository.               │
   │ list-tags       List all tags in the repository.                             │
   │ setup           Sets up a git repository object.                             │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[notebook.create]
+  '''
+                                                                                  
+   Usage: default notebook create [OPTIONS] IDENTIFIER                            
+                                                                                  
+   Creates notebook from stage.                                                   
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    identifier      TEXT  Identifier of the notebook. For example:          │
+  │                            MY_NOTEBOOK                                       │
+  │                            [required]                                        │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ *  --notebook-file  -f      TEXT  Stage path with notebook file. For example │
+  │                                   `@stage/path/to/notebook.ipynb`            │
+  │                                   [default: None]                            │
+  │                                   [required]                                 │
+  │    --help           -h            Show this message and exit.                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[notebook.execute]
   '''
                                                                                   
    Usage: default notebook execute [OPTIONS] IDENTIFIER                           
                                                                                   
    Executes a notebook in a headless mode.                                        
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    identifier      TEXT  Identifier of the notebook. For example:          │
   │                            MY_NOTEBOOK                                       │
-  │                            [default: None]                                   │
   │                            [required]                                        │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
@@ -1582,15 +2473,14 @@
    Usage: default notebook get-url [OPTIONS] IDENTIFIER                           
                                                                                   
    Return a url to a notebook.                                                    
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    identifier      TEXT  Identifier of the notebook. For example:          │
   │                            MY_NOTEBOOK                                       │
-  │                            [default: None]                                   │
   │                            [required]                                        │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
@@ -1653,15 +2543,14 @@
    Usage: default notebook open [OPTIONS] IDENTIFIER                              
                                                                                   
    Opens a notebook in default browser                                            
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    identifier      TEXT  Identifier of the notebook. For example:          │
   │                            MY_NOTEBOOK                                       │
-  │                            [default: None]                                   │
   │                            [required]                                        │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
@@ -1725,31 +2614,32 @@
                                                                                   
    Manages notebooks in Snowflake.                                                
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ create    Creates notebook from stage.                                       │
   │ execute   Executes a notebook in a headless mode.                            │
   │ get-url   Return a url to a notebook.                                        │
   │ open      Opens a notebook in default browser                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[object.describe]
   '''
                                                                                   
    Usage: default object describe [OPTIONS] OBJECT_TYPE OBJECT_NAME               
                                                                                   
    Provides description of an object of given type.                               
-   Supported types: compute-pool, database, function, git-repository,             
-   integration, network-rule, procedure, role, schema, secret, service, stage,    
-   stream, streamlit, table, task, user, view, warehouse                          
+   Supported types: compute-pool, database, external-access-integration,          
+   function, git-repository, integration, network-rule, procedure, role, schema,  
+   secret, service, stage, stream, streamlit, table, task, user, view, warehouse  
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    object_type      TEXT  Type of object. For example table, procedure,    │
   │                             streamlit.                                       │
   │                             [default: None]                                  │
   │                             [required]                                       │
   │ *    object_name      TEXT  Name of the object [default: None] [required]    │
@@ -1814,17 +2704,18 @@
 # ---
 # name: test_help_messages[object.drop]
   '''
                                                                                   
    Usage: default object drop [OPTIONS] OBJECT_TYPE OBJECT_NAME                   
                                                                                   
    Drops Snowflake object of given name and type.                                 
-   Supported types: compute-pool, database, function, git-repository,             
-   image-repository, integration, network-rule, procedure, role, schema, secret,  
-   service, stage, stream, streamlit, table, task, user, view, warehouse          
+   Supported types: compute-pool, database, external-access-integration,          
+   function, git-repository, image-repository, integration, network-rule,         
+   procedure, role, schema, secret, service, stage, stream, streamlit, table,     
+   task, user, view, warehouse                                                    
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    object_type      TEXT  Type of object. For example table, procedure,    │
   │                             streamlit.                                       │
   │                             [default: None]                                  │
   │                             [required]                                       │
   │ *    object_name      TEXT  Name of the object [default: None] [required]    │
@@ -1889,35 +2780,36 @@
 # ---
 # name: test_help_messages[object.list]
   '''
                                                                                   
    Usage: default object list [OPTIONS] OBJECT_TYPE                               
                                                                                   
    Lists all available Snowflake objects of given type.                           
-   Supported types: compute-pool, database, function, git-repository,             
-   image-repository, integration, network-rule, procedure, role, schema, secret,  
-   service, stage, stream, streamlit, table, task, user, view, warehouse          
+   Supported types: compute-pool, database, external-access-integration,          
+   function, git-repository, image-repository, integration, network-rule,         
+   procedure, role, schema, secret, service, stage, stream, streamlit, table,     
+   task, user, view, warehouse                                                    
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    object_type      TEXT  Type of object. For example table, procedure,    │
   │                             streamlit.                                       │
   │                             [default: None]                                  │
   │                             [required]                                       │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --like  -l      TEXT            SQL LIKE pattern for filtering objects by    │
   │                                 name. For example, `list function --like     │
   │                                 "my%"` lists all functions that begin with   │
   │                                 “my”.                                        │
   │                                 [default: %%]                                │
   │ --in            <TEXT TEXT>...  Specifies the scope of this command using    │
-  │                                 '--in <scope> <name>' (e.g. list tables --in │
-  │                                 database my_db). Some object types have      │
-  │                                 specialized scopes (e.g. list service --in   │
-  │                                 compute-pool my_pool)                        │
+  │                                 '--in <scope> <name>', for example `list     │
+  │                                 table --in database my_db`. Some object      │
+  │                                 types have specialized scopes (e.g. list     │
+  │                                 service --in compute-pool my_pool).          │
   │                                 [default: None, None]                        │
   │ --help  -h                      Show this message and exit.                  │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
@@ -2548,33 +3440,181 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[snowpark.describe]
+  '''
+                                                                                  
+   Usage: default snowpark describe [OPTIONS] OBJECT_TYPE:{procedure|function}    
+                                    IDENTIFIER                                    
+                                                                                  
+   Provides description of a procedure or function.                               
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    object_type      OBJECT_TYPE:{procedure|fun  Type of Snowpark object    │
+  │                       ction}                      [required]                 │
+  │ *    identifier       TEXT                        Identifier of the          │
+  │                                                   function/procedure. For    │
+  │                                                   example: hello(int,        │
+  │                                                   string)                    │
+  │                                                   [required]                 │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[snowpark.drop]
+  '''
+                                                                                  
+   Usage: default snowpark drop [OPTIONS] OBJECT_TYPE:{procedure|function}        
+                                IDENTIFIER                                        
+                                                                                  
+   Drop procedure or function.                                                    
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    object_type      OBJECT_TYPE:{procedure|fun  Type of Snowpark object    │
+  │                       ction}                      [required]                 │
+  │ *    identifier       TEXT                        Identifier of the          │
+  │                                                   function/procedure. For    │
+  │                                                   example: hello(int,        │
+  │                                                   string)                    │
+  │                                                   [required]                 │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[snowpark.execute]
   '''
                                                                                   
    Usage: default snowpark execute [OPTIONS] OBJECT_TYPE:{procedure|function}     
                                    EXECUTION_IDENTIFIER                           
                                                                                   
    Executes a procedure or function in a specified environment.                   
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    object_type               OBJECT_TYPE:{procedur  Type of Snowpark       │
   │                                e|function}            object                 │
-  │                                                       [default: None]        │
   │                                                       [required]             │
   │ *    execution_identifier      TEXT                   Execution identifier   │
   │                                                       of the                 │
   │                                                       procedure/function.    │
   │                                                       For example: hello(1,  │
   │                                                       'world')               │
-  │                                                       [default: None]        │
   │                                                       [required]             │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
@@ -2657,14 +3697,92 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[snowpark.list]
+  '''
+                                                                                  
+   Usage: default snowpark list [OPTIONS] OBJECT_TYPE:{procedure|function}        
+                                                                                  
+   Lists all available procedures or functions.                                   
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    object_type      OBJECT_TYPE:{procedure|fun  Type of Snowpark object    │
+  │                       ction}                      [required]                 │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT            SQL LIKE pattern for filtering objects by    │
+  │                                 name. For example, `list function --like     │
+  │                                 "my%"` lists all functions that begin with   │
+  │                                 “my”.                                        │
+  │                                 [default: %%]                                │
+  │ --in            <TEXT TEXT>...  Specifies the scope of this command using    │
+  │                                 '--in <scope> <name>', for example `list     │
+  │                                 function --in database my_db`.               │
+  │                                 [default: None, None]                        │
+  │ --help  -h                      Show this message and exit.                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[snowpark.package.create]
   '''
                                                                                   
    Usage: default snowpark package create [OPTIONS] NAME                          
                                                                                   
    Creates a Python package as a zip file that can be uploaded to a stage and     
    imported for a Snowpark Python app.                                            
@@ -2914,26 +4032,29 @@
                                                                                   
    Manages procedures and functions.                                              
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ build     Builds the Snowpark project as a `.zip` archive that can be used   │
-  │           by `deploy` command. The archive is built using only the `src`     │
-  │           directory specified in the project file.                           │
-  │ deploy    Deploys procedures and functions defined in project. Deploying the │
-  │           project alters all objects defined in it. By default, if any of    │
-  │           the objects exist already the commands will fail unless            │
-  │           `--replace` flag is provided. All deployed objects use the same    │
-  │           artifact which is deployed only once.                              │
-  │ execute   Executes a procedure or function in a specified environment.       │
-  │ init      Initializes this directory with a sample set of files for creating │
-  │           a Snowpark project.                                                │
-  │ package   Manages custom Python packages for Snowpark                        │
+  │ build      Builds the Snowpark project as a `.zip` archive that can be used  │
+  │            by `deploy` command. The archive is built using only the `src`    │
+  │            directory specified in the project file.                          │
+  │ deploy     Deploys procedures and functions defined in project. Deploying    │
+  │            the project alters all objects defined in it. By default, if any  │
+  │            of the objects exist already the commands will fail unless        │
+  │            `--replace` flag is provided. All deployed objects use the same   │
+  │            artifact which is deployed only once.                             │
+  │ describe   Provides description of a procedure or function.                  │
+  │ drop       Drop procedure or function.                                       │
+  │ execute    Executes a procedure or function in a specified environment.      │
+  │ init       Initializes this directory with a sample set of files for         │
+  │            creating a Snowpark project.                                      │
+  │ list       Lists all available procedures or functions.                      │
+  │ package    Manages custom Python packages for Snowpark                       │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[spcs.compute-pool.create]
   '''
@@ -2951,15 +4072,14 @@
   │                                                             For more         │
   │                                                             information      │
   │                                                             about instance   │
   │                                                             families, refer  │
   │                                                             to the SQL       │
   │                                                             CREATE COMPUTE   │
   │                                                             POOL command.    │
-  │                                                             [default: None]  │
   │                                                             [required]       │
   │    --min-nodes                             INTEGER RANGE    Minimum number   │
   │                                            [x>=1]           of nodes for the │
   │                                                             compute pool.    │
   │                                                             [default: 1]     │
   │    --max-nodes                             INTEGER RANGE    Maximum number   │
   │                                            [x>=1]           of nodes for the │
@@ -3052,14 +4172,219 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[spcs.compute-pool.describe]
+  '''
+                                                                                  
+   Usage: default spcs compute-pool describe [OPTIONS] NAME                       
+                                                                                  
+   Provides description of compute pool.                                          
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the compute pool. [required]                    │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[spcs.compute-pool.drop]
+  '''
+                                                                                  
+   Usage: default spcs compute-pool drop [OPTIONS] NAME                           
+                                                                                  
+   Drops compute pool with given name.                                            
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the compute pool. [required]                    │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[spcs.compute-pool.list]
+  '''
+                                                                                  
+   Usage: default spcs compute-pool list [OPTIONS]                                
+                                                                                  
+   Lists all available compute pools.                                             
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT  SQL LIKE pattern for filtering objects by name. For    │
+  │                       example, `list --like "my%"` lists all compute pools   │
+  │                       that begin with “my”..                                 │
+  │                       [default: %%]                                          │
+  │ --help  -h            Show this message and exit.                            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[spcs.compute-pool.resume]
   '''
                                                                                   
    Usage: default spcs compute-pool resume [OPTIONS] NAME                         
                                                                                   
    Resumes the compute pool from a SUSPENDED state.                               
                                                                                   
@@ -3508,14 +4833,17 @@
    Manages Snowpark Container Services compute pools.                             
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
   │ create     Creates a new compute pool.                                       │
+  │ describe   Provides description of compute pool.                             │
+  │ drop       Drops compute pool with given name.                               │
+  │ list       Lists all available compute pools.                                │
   │ resume     Resumes the compute pool from a SUSPENDED state.                  │
   │ set        Sets one or more properties for the compute pool.                 │
   │ status     Retrieves the status of a compute pool along with a relevant      │
   │            message, if one exists.                                           │
   │ stop-all   Deletes all services running on the compute pool.                 │
   │ suspend    Suspends the compute pool by suspending all currently running     │
   │            services and then releasing compute pool nodes.                   │
@@ -3760,16 +5088,15 @@
   '''
                                                                                   
    Usage: default spcs image-repository create [OPTIONS] NAME                     
                                                                                   
    Creates a new image repository in the current schema.                          
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the image repository. [default: None]           │
-  │                      [required]                                              │
+  │ *    name      TEXT  Name of the image repository. [required]                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --replace                  Replace this object if it already exists.         │
   │ --if-not-exists            Only apply this operation if the specified object │
   │                            does not already exist.                           │
   │ --help           -h        Show this message and exit.                       │
   ╰──────────────────────────────────────────────────────────────────────────────╯
@@ -3824,24 +5151,91 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[spcs.image-repository.drop]
+  '''
+                                                                                  
+   Usage: default spcs image-repository drop [OPTIONS] NAME                       
+                                                                                  
+   Drops image repository with given name.                                        
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the image repository. [required]                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[spcs.image-repository.list-images]
   '''
                                                                                   
    Usage: default spcs image-repository list-images [OPTIONS] NAME                
                                                                                   
    Lists images in the given repository.                                          
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the image repository. [default: None]           │
-  │                      [required]                                              │
+  │ *    name      TEXT  Name of the image repository. [required]                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -3901,22 +5295,20 @@
   '''
                                                                                   
    Usage: default spcs image-repository list-tags [OPTIONS] NAME                  
                                                                                   
    Lists tags for the given image in a repository.                                
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the image repository. [default: None]           │
-  │                      [required]                                              │
+  │ *    name      TEXT  Name of the image repository. [required]                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ *  --image-name,--image_name  -i      TEXT  Fully qualified name of the      │
   │                                             image as shown in the output of  │
   │                                             list-images                      │
-  │                                             [default: None]                  │
   │                                             [required]                       │
   │    --help                     -h            Show this message and exit.      │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
@@ -3967,24 +5359,97 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[spcs.image-repository.list]
+  '''
+                                                                                  
+   Usage: default spcs image-repository list [OPTIONS]                            
+                                                                                  
+   Lists all available image repositories.                                        
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT            SQL LIKE pattern for filtering objects by    │
+  │                                 name. For example, `list --like "my%"` lists │
+  │                                 all image repositories that begin with       │
+  │                                 “my”..                                       │
+  │                                 [default: %%]                                │
+  │ --in            <TEXT TEXT>...  Specifies the scope of this command using    │
+  │                                 '--in <scope> <name>', for example `list     │
+  │                                 --in database my_db`.                        │
+  │                                 [default: None, None]                        │
+  │ --help  -h                      Show this message and exit.                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[spcs.image-repository.url]
   '''
                                                                                   
    Usage: default spcs image-repository url [OPTIONS] NAME                        
                                                                                   
    Returns the URL for the given repository.                                      
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the image repository. [default: None]           │
-  │                      [required]                                              │
+  │ *    name      TEXT  Name of the image repository. [required]                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -4048,14 +5513,16 @@
    Manages Snowpark Container Services image repositories.                        
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
   │ create        Creates a new image repository in the current schema.          │
+  │ drop          Drops image repository with given name.                        │
+  │ list          Lists all available image repositories.                        │
   │ list-images   Lists images in the given repository.                          │
   │ list-tags     Lists tags for the given image in a repository.                │
   │ url           Returns the URL for the given repository.                      │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
@@ -4293,26 +5760,24 @@
   '''
                                                                                   
    Usage: default spcs service create [OPTIONS] NAME                              
                                                                                   
    Creates a new service in the current schema.                                   
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ *  --compute-pool                          TEXT             Compute pool to  │
   │                                                             run the service  │
   │                                                             on.              │
-  │                                                             [default: None]  │
   │                                                             [required]       │
   │ *  --spec-path                             FILE             Path to service  │
   │                                                             specification    │
   │                                                             file.            │
-  │                                                             [default: None]  │
   │                                                             [required]       │
   │    --min-instances                         INTEGER RANGE    Minimum number   │
   │                                            [x>=1]           of service       │
   │                                                             instances to     │
   │                                                             run.             │
   │                                                             [default: 1]     │
   │    --max-instances                         INTEGER RANGE    Maximum number   │
@@ -4417,23 +5882,159 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[spcs.service.describe]
+  '''
+                                                                                  
+   Usage: default spcs service describe [OPTIONS] NAME                            
+                                                                                  
+   Provides description of service.                                               
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the service. [required]                         │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[spcs.service.drop]
+  '''
+                                                                                  
+   Usage: default spcs service drop [OPTIONS] NAME                                
+                                                                                  
+   Drops service with given name.                                                 
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the service. [required]                         │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[spcs.service.list-endpoints]
   '''
                                                                                   
    Usage: default spcs service list-endpoints [OPTIONS] NAME                      
                                                                                   
    Lists the endpoints in a service.                                              
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -4485,30 +6086,101 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[spcs.service.list]
+  '''
+                                                                                  
+   Usage: default spcs service list [OPTIONS]                                     
+                                                                                  
+   Lists all available services.                                                  
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT            SQL LIKE pattern for filtering objects by    │
+  │                                 name. For example, `list --like "my%"` lists │
+  │                                 all services that begin with “my”..          │
+  │                                 [default: %%]                                │
+  │ --in            <TEXT TEXT>...  Specifies the scope of this command using    │
+  │                                 '--in <scope> <name>', for example `list     │
+  │                                 --in compute-pool my_pool`.                  │
+  │                                 [default: None, None]                        │
+  │ --help  -h                      Show this message and exit.                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[spcs.service.logs]
   '''
                                                                                   
    Usage: default spcs service logs [OPTIONS] NAME                                
                                                                                   
    Retrieves local logs from a service container.                                 
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ *  --container-name          TEXT     Name of the container. [default: None] │
-  │                                       [required]                             │
+  │ *  --container-name          TEXT     Name of the container. [required]      │
   │ *  --instance-id             TEXT     ID of the service instance, starting   │
   │                                       with 0.                                │
-  │                                       [default: None]                        │
   │                                       [required]                             │
   │    --num-lines               INTEGER  Number of lines to retrieve.           │
   │                                       [default: 500]                         │
   │    --help            -h               Show this message and exit.            │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
@@ -4569,15 +6241,15 @@
   '''
                                                                                   
    Usage: default spcs service resume [OPTIONS] NAME                              
                                                                                   
    Resumes the service from a SUSPENDED state.                                    
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -4637,15 +6309,15 @@
   '''
                                                                                   
    Usage: default spcs service set [OPTIONS] NAME                                 
                                                                                   
    Sets one or more properties for the service.                                   
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --min-instances                           INTEGER RANGE     Minimum number   │
   │                                           [x>=1]            of service       │
   │                                                             instances to     │
   │                                                             run.             │
   │ --max-instances                           INTEGER RANGE     Maximum number   │
@@ -4734,15 +6406,15 @@
   '''
                                                                                   
    Usage: default spcs service status [OPTIONS] NAME                              
                                                                                   
    Retrieves the status of a service.                                             
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -4802,15 +6474,15 @@
   '''
                                                                                   
    Usage: default spcs service suspend [OPTIONS] NAME                             
                                                                                   
    Suspends the service, shutting down and deleting all its containers.           
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -4870,15 +6542,15 @@
   '''
                                                                                   
    Usage: default spcs service unset [OPTIONS] NAME                               
                                                                                   
    Resets one or more properties for the service to their default value(s).       
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --min-instances              Reset the MIN_INSTANCES property - Minimum      │
   │                              number of service instances to run.             │
   │ --max-instances              Reset the MAX_INSTANCES property - Maximum      │
   │                              number of service instances to run.             │
   │ --query-warehouse            Reset the QUERY_WAREHOUSE property - Warehouse  │
@@ -4951,20 +6623,18 @@
   '''
                                                                                   
    Usage: default spcs service upgrade [OPTIONS] NAME                             
                                                                                   
    Updates an existing service with a new specification file.                     
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the service. [default: None] [required]         │
+  │ *    name      TEXT  Name of the service. [required]                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ *  --spec-path          FILE  Path to service specification file.            │
-  │                               [default: None]                                │
-  │                               [required]                                     │
+  │ *  --spec-path          FILE  Path to service specification file. [required] │
   │    --help       -h            Show this message and exit.                    │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
@@ -5026,14 +6696,17 @@
    Manages Snowpark Container Services services.                                  
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
   │ create           Creates a new service in the current schema.                │
+  │ describe         Provides description of service.                            │
+  │ drop             Drops service with given name.                              │
+  │ list             Lists all available services.                               │
   │ list-endpoints   Lists the endpoints in a service.                           │
   │ logs             Retrieves local logs from a service container.              │
   │ resume           Resumes the service from a SUSPENDED state.                 │
   │ set              Sets one or more properties for the service.                │
   │ status           Retrieves the status of a service.                          │
   │ suspend          Suspends the service, shutting down and deleting all its    │
   │                  containers.                                                 │
@@ -5068,29 +6741,32 @@
 # ---
 # name: test_help_messages[sql]
   '''
                                                                                   
    Usage: default sql [OPTIONS]                                                   
                                                                                   
    Executes Snowflake query.                                                      
+   Use either query, filename or input option.                                    
    Query to execute can be specified using query option, filename option (all     
    queries from file will be executed) or via stdin by piping output from other   
    command. For example `cat my.sql | snow sql -i`.                               
    The command supports variable substitution that happens on client-side. Both   
-   $VARIABLE or ${ VARIABLE } syntax are supported.                               
+   &VARIABLE or &{ VARIABLE } syntax are supported.                               
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --query     -q      TEXT  Query to execute. [default: None]                  │
   │ --filename  -f      FILE  File to execute. [default: None]                   │
   │ --stdin     -i            Read the query from standard input. Use it when    │
   │                           piping input to this command.                      │
   │ --variable  -D      TEXT  String in format of key=value. If provided the SQL │
   │                           content will be treated as template and rendered   │
   │                           using provided data.                               │
   │                           [default: None]                                    │
+  │ --project   -p      TEXT  Path where Snowflake project resides. Defaults to  │
+  │                           current working directory.                         │
   │ --help      -h            Show this message and exit.                        │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
@@ -5292,25 +6968,160 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[stage.describe]
+  '''
+                                                                                  
+   Usage: default stage describe [OPTIONS] NAME                                   
+                                                                                  
+   Provides description of stage.                                                 
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the stage. [required]                           │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[stage.diff]
   '''
                                                                                   
    Usage: default stage diff [OPTIONS] STAGE_NAME FOLDER_NAME                     
                                                                                   
    Diffs a stage with a local folder.                                             
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    stage_name       TEXT  Fully qualified name of a stage [default: None]  │
-  │                             [required]                                       │
-  │ *    folder_name      TEXT  Path to local folder [default: None] [required]  │
+  │ *    stage_name       TEXT  Fully qualified name of a stage [required]       │
+  │ *    folder_name      TEXT  Path to local folder [required]                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[stage.drop]
+  '''
+                                                                                  
+   Usage: default stage drop [OPTIONS] NAME                                       
+                                                                                  
+   Drops stage with given name.                                                   
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the stage. [required]                           │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -5380,14 +7191,17 @@
   │                            `@stage/dev/*`.                                   │
   │                            [required]                                        │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --on-error          [break|continue]  What to do when an error occurs.       │
   │                                       Defaults to break.                     │
   │                                       [default: break]                       │
+  │ --variable  -D      TEXT              Variables for the template. For        │
+  │                                       example: `-D "<key>=<value>"`, string  │
+  │                                       values must be in `''`.                │
   │ --help      -h                        Show this message and exit.            │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
@@ -5508,25 +7322,97 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[stage.list]
+  '''
+                                                                                  
+   Usage: default stage list [OPTIONS]                                            
+                                                                                  
+   Lists all available stages.                                                    
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT            SQL LIKE pattern for filtering objects by    │
+  │                                 name. For example, `list --like "my%"` lists │
+  │                                 all stages that begin with “my”.             │
+  │                                 [default: %%]                                │
+  │ --in            <TEXT TEXT>...  Specifies the scope of this command using    │
+  │                                 '--in <scope> <name>', for example `list     │
+  │                                 --in database my_db`.                        │
+  │                                 [default: None, None]                        │
+  │ --help  -h                      Show this message and exit.                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[stage.remove]
   '''
                                                                                   
    Usage: default stage remove [OPTIONS] STAGE_NAME FILE_NAME                     
                                                                                   
    Removes a file from a stage.                                                   
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    stage_name      TEXT  Name of the stage. [required]                     │
-  │ *    file_name       TEXT  Name of the file to remove. [default: None]       │
-  │                            [required]                                        │
+  │ *    file_name       TEXT  Name of the file to remove. [required]            │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -5593,18 +7479,21 @@
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
   │ copy         Copies all files from target path to target directory. This     │
   │              works for both uploading to and downloading files from the      │
   │              stage.                                                          │
   │ create       Creates a named stage if it does not already exist.             │
+  │ describe     Provides description of stage.                                  │
+  │ drop         Drops stage with given name.                                    │
   │ execute      Execute immediate all files from the stage path. Files can be   │
   │              filtered with glob like pattern, e.g. `@stage/*.sql`,           │
   │              `@stage/dev/*`. Only files with `.sql` extension will be        │
   │              executed.                                                       │
+  │ list         Lists all available stages.                                     │
   │ list-files   Lists the stage contents.                                       │
   │ remove       Removes a file from a stage.                                    │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
@@ -5677,23 +7566,159 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[streamlit.describe]
+  '''
+                                                                                  
+   Usage: default streamlit describe [OPTIONS] NAME                               
+                                                                                  
+   Provides description of streamlit.                                             
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the Streamlit app. [required]                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[streamlit.drop]
+  '''
+                                                                                  
+   Usage: default streamlit drop [OPTIONS] NAME                                   
+                                                                                  
+   Drops streamlit with given name.                                               
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    name      TEXT  Name of the Streamlit app. [required]                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[streamlit.get-url]
   '''
                                                                                   
    Usage: default streamlit get-url [OPTIONS] NAME                                
                                                                                   
    Returns a URL to the specified Streamlit app                                   
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the Streamlit app. [default: None] [required]   │
+  │ *    name      TEXT  Name of the Streamlit app. [required]                   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --open            Whether to open the Streamlit app in a browser.            │
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
@@ -5777,24 +7802,96 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[streamlit.list]
+  '''
+                                                                                  
+   Usage: default streamlit list [OPTIONS]                                        
+                                                                                  
+   Lists all available streamlits.                                                
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT            SQL LIKE pattern for filtering objects by    │
+  │                                 name. For example, `list --like "my%"` lists │
+  │                                 all streamlit apps that begin with “my”.     │
+  │                                 [default: %%]                                │
+  │ --in            <TEXT TEXT>...  Specifies the scope of this command using    │
+  │                                 '--in <scope> <name>', for example `list     │
+  │                                 --in database my_db`.                        │
+  │                                 [default: None, None]                        │
+  │ --help  -h                      Show this message and exit.                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[streamlit.share]
   '''
                                                                                   
    Usage: default streamlit share [OPTIONS] NAME TO_ROLE                          
                                                                                   
    Shares a Streamlit app with another role.                                      
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name         TEXT  Name of the Streamlit app to share. [default: None]  │
-  │                         [required]                                           │
+  │ *    name         TEXT  Name of the Streamlit app. [required]                │
   │ *    to_role      TEXT  Role with which to share the Streamlit app.          │
   │                         [default: None]                                      │
   │                         [required]                                           │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
@@ -5860,21 +7957,514 @@
                                                                                   
    Manages a Streamlit app in Snowflake.                                          
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ deploy    Deploys a Streamlit app defined in the project definition file     │
-  │           (snowflake.yml). By default, the command uploads environment.yml   │
-  │           and any other pages or folders, if present. If you don’t specify a │
-  │           stage name, the `streamlit` stage is used. If the specified stage  │
-  │           does not exist, the command creates it.                            │
-  │ get-url   Returns a URL to the specified Streamlit app                       │
-  │ init      Initializes this directory with a sample set of files for creating │
-  │           a Streamlit app project.                                           │
-  │ share     Shares a Streamlit app with another role.                          │
+  │ deploy     Deploys a Streamlit app defined in the project definition file    │
+  │            (snowflake.yml). By default, the command uploads environment.yml  │
+  │            and any other pages or folders, if present. If you don’t specify  │
+  │            a stage name, the `streamlit` stage is used. If the specified     │
+  │            stage does not exist, the command creates it.                     │
+  │ describe   Provides description of streamlit.                                │
+  │ drop       Drops streamlit with given name.                                  │
+  │ get-url    Returns a URL to the specified Streamlit app                      │
+  │ init       Initializes this directory with a sample set of files for         │
+  │            creating a Streamlit app project.                                 │
+  │ list       Lists all available streamlits.                                   │
+  │ share      Shares a Streamlit app with another role.                         │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[]
+  '''
+                                                                                  
+   Usage: default [OPTIONS] COMMAND [ARGS]...                                     
+                                                                                  
+   Snowflake CLI tool for developers.                                             
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --version                           Shows version of the Snowflake CLI       │
+  │ --info                              Shows information about the Snowflake    │
+  │                                     CLI                                      │
+  │ --config-file                 FILE  Specifies Snowflake CLI configuration    │
+  │                                     file that should be used                 │
+  │                                     [default: None]                          │
+  │ --install-completion                Install completion for the current       │
+  │                                     shell.                                   │
+  │ --show-completion                   Show completion for the current shell,   │
+  │                                     to copy it or customize the              │
+  │                                     installation.                            │
+  │ --help                -h            Show this message and exit.              │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ app          Manages a Snowflake Native App                                  │
+  │ connection   Manages connections to Snowflake.                               │
+  │ cortex       Provides access to Snowflake Cortex.                            │
+  │ git          Manages git repositories in Snowflake.                          │
+  │ object       Manages Snowflake objects like warehouses and stages            │
+  │ snowpark     Manages procedures and functions.                               │
+  │ spcs         Manages Snowpark Container Services compute pools, services,    │
+  │              image registries, and image repositories.                       │
+  │ sql          Executes Snowflake query.                                       │
+  │ stage        Manages stages.                                                 │
+  │ streamlit    Manages a Streamlit app in Snowflake.                           │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[app.version]
+  '''
+                                                                                  
+   Usage: default app version [OPTIONS] COMMAND [ARGS]...                         
+                                                                                  
+   Manages versions defined in an application package                             
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ create   Adds a new patch to the provided version defined in your            │
+  │          application package. If the version does not exist, creates a       │
+  │          version with patch 0.                                               │
+  │ drop     Drops a version defined in your application package. Versions can   │
+  │          either be passed in as an argument to the command or read from the  │
+  │          `manifest.yml` file. Dropping patches is not allowed.               │
+  │ list     Lists all versions defined in an application package.               │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[app]
+  '''
+                                                                                  
+   Usage: default app [OPTIONS] COMMAND [ARGS]...                                 
+                                                                                  
+   Manages a Snowflake Native App                                                 
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ deploy     Creates an application package in your Snowflake account and      │
+  │            syncs the local changes to the stage without creating or updating │
+  │            the application. Running this command with no arguments at all,   │
+  │            as in `snow app deploy`, is a shorthand for `snow app deploy      │
+  │            --prune --recursive`.                                             │
+  │ init       Initializes a Snowflake Native App project.                       │
+  │ open       Opens the Snowflake Native App inside of your browser, once it    │
+  │            has been installed in your account.                               │
+  │ run        Creates an application package in your Snowflake account, uploads │
+  │            code files to its stage, then creates or upgrades an application  │
+  │            object from the application package.                              │
+  │ teardown   Attempts to drop both the application object and application      │
+  │            package as defined in the project definition file.                │
+  │ version    Manages versions defined in an application package                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[connection]
+  '''
+                                                                                  
+   Usage: default connection [OPTIONS] COMMAND [ARGS]...                          
+                                                                                  
+   Manages connections to Snowflake.                                              
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ add           Adds a connection to configuration file.                       │
+  │ list          Lists configured connections.                                  │
+  │ set-default   Changes default connection to provided value.                  │
+  │ test          Tests the connection to Snowflake.                             │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[cortex]
+  '''
+                                                                                  
+   Usage: default cortex [OPTIONS] COMMAND [ARGS]...                              
+                                                                                  
+   Provides access to Snowflake Cortex.                                           
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ complete         Given a prompt, the command generates a response using your │
+  │                  choice of language model. In the simplest use case, the     │
+  │                  prompt is a single string. You may also provide a JSON file │
+  │                  with conversation history including multiple prompts and    │
+  │                  responses for interactive chat-style usage.                 │
+  │ extract-answer   Extracts an answer to a given question from a text          │
+  │                  document. The document may be a plain-English document or a │
+  │                  string representation of a semi-structured (JSON) data      │
+  │                  object.                                                     │
+  │ search           Performs query search using Cortex Search Services.         │
+  │ sentiment        Returns sentiment as a score between -1 to 1 (with -1 being │
+  │                  the most negative and 1 the most positive, with values      │
+  │                  around 0 neutral) for the given English-language input      │
+  │                  text.                                                       │
+  │ summarize        Summarizes the given English-language input text.           │
+  │ translate        Translates text from the indicated or detected source       │
+  │                  language to a target language.                              │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[git]
+  '''
+                                                                                  
+   Usage: default git [OPTIONS] COMMAND [ARGS]...                                 
+                                                                                  
+   Manages git repositories in Snowflake.                                         
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ copy            Copies all files from given state of repository to local     │
+  │                 directory or stage.                                          │
+  │ describe        Provides description of git repository.                      │
+  │ drop            Drops git repository with given name.                        │
+  │ execute         Execute immediate all files from the repository path. Files  │
+  │                 can be filtered with glob like pattern, e.g.                 │
+  │                 `@my_repo/branches/main/*.sql`,                              │
+  │                 `@my_repo/branches/main/dev/*`. Only files with `.sql`       │
+  │                 extension will be executed.                                  │
+  │ fetch           Fetch changes from origin to Snowflake repository.           │
+  │ list            Lists all available git repositories.                        │
+  │ list-branches   List all branches in the repository.                         │
+  │ list-files      List files from given state of git repository.               │
+  │ list-tags       List all tags in the repository.                             │
+  │ setup           Sets up a git repository object.                             │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[notebook]
+  '''
+                                                                                  
+   Usage: default notebook [OPTIONS] COMMAND [ARGS]...                            
+                                                                                  
+   Manages notebooks in Snowflake.                                                
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ create    Creates notebook from stage.                                       │
+  │ execute   Executes a notebook in a headless mode.                            │
+  │ get-url   Return a url to a notebook.                                        │
+  │ open      Opens a notebook in default browser                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[object.stage]
+  '''
+                                                                                  
+   Usage: default object stage [OPTIONS] COMMAND [ARGS]...                        
+                                                                                  
+   (deprecated)                                                                   
+   Manages stages.                                                                
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ copy     Copies all files from target path to target           (deprecated)  │
+  │          directory. This works for both uploading to and                     │
+  │          downloading files from the stage.                                   │
+  │ create   Creates a named stage if it does not already exist.   (deprecated)  │
+  │ list     Lists the stage contents.                             (deprecated)  │
+  │ remove   Removes a file from a stage.                          (deprecated)  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[object]
+  '''
+                                                                                  
+   Usage: default object [OPTIONS] COMMAND [ARGS]...                              
+                                                                                  
+   Manages Snowflake objects like warehouses and stages                           
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ describe   Provides description of an object of given type.                  │
+  │ drop       Drops Snowflake object of given name and type.                    │
+  │ list       Lists all available Snowflake objects of given                    │
+  │            type.                                                             │
+  │ stage      Manages stages.                                     (deprecated)  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[snowpark.package]
+  '''
+                                                                                  
+   Usage: default snowpark package [OPTIONS] COMMAND [ARGS]...                    
+                                                                                  
+   Manages custom Python packages for Snowpark                                    
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ create   Creates a Python package as a zip file that can be uploaded to a    │
+  │          stage and imported for a Snowpark Python app.                       │
+  │ lookup   Checks if a package is available on the Snowflake Anaconda channel. │
+  │ upload   Uploads a Python package zip file to a Snowflake stage so it can be │
+  │          referenced in the imports of a procedure or function.               │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[snowpark]
+  '''
+                                                                                  
+   Usage: default snowpark [OPTIONS] COMMAND [ARGS]...                            
+                                                                                  
+   Manages procedures and functions.                                              
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ build      Builds the Snowpark project as a `.zip` archive that can be used  │
+  │            by `deploy` command. The archive is built using only the `src`    │
+  │            directory specified in the project file.                          │
+  │ deploy     Deploys procedures and functions defined in project. Deploying    │
+  │            the project alters all objects defined in it. By default, if any  │
+  │            of the objects exist already the commands will fail unless        │
+  │            `--replace` flag is provided. All deployed objects use the same   │
+  │            artifact which is deployed only once.                             │
+  │ describe   Provides description of a procedure or function.                  │
+  │ drop       Drop procedure or function.                                       │
+  │ execute    Executes a procedure or function in a specified environment.      │
+  │ init       Initializes this directory with a sample set of files for         │
+  │            creating a Snowpark project.                                      │
+  │ list       Lists all available procedures or functions.                      │
+  │ package    Manages custom Python packages for Snowpark                       │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[spcs.compute-pool]
+  '''
+                                                                                  
+   Usage: default spcs compute-pool [OPTIONS] COMMAND [ARGS]...                   
+                                                                                  
+   Manages Snowpark Container Services compute pools.                             
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ create     Creates a new compute pool.                                       │
+  │ describe   Provides description of compute pool.                             │
+  │ drop       Drops compute pool with given name.                               │
+  │ list       Lists all available compute pools.                                │
+  │ resume     Resumes the compute pool from a SUSPENDED state.                  │
+  │ set        Sets one or more properties for the compute pool.                 │
+  │ status     Retrieves the status of a compute pool along with a relevant      │
+  │            message, if one exists.                                           │
+  │ stop-all   Deletes all services running on the compute pool.                 │
+  │ suspend    Suspends the compute pool by suspending all currently running     │
+  │            services and then releasing compute pool nodes.                   │
+  │ unset      Resets one or more properties for the compute pool to their       │
+  │            default value(s).                                                 │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[spcs.image-registry]
+  '''
+                                                                                  
+   Usage: default spcs image-registry [OPTIONS] COMMAND [ARGS]...                 
+                                                                                  
+   Manages Snowpark Container Services image registries.                          
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ login   Logs in to the account image registry with the current user's        │
+  │         credentials through Docker.                                          │
+  │ token   Retrieves a registry authentication token based on your current      │
+  │         connection.                                                          │
+  │ url     Gets the image registry URL for the current account.                 │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[spcs.image-repository]
+  '''
+                                                                                  
+   Usage: default spcs image-repository [OPTIONS] COMMAND [ARGS]...               
+                                                                                  
+   Manages Snowpark Container Services image repositories.                        
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ create        Creates a new image repository in the current schema.          │
+  │ drop          Drops image repository with given name.                        │
+  │ list          Lists all available image repositories.                        │
+  │ list-images   Lists images in the given repository.                          │
+  │ list-tags     Lists tags for the given image in a repository.                │
+  │ url           Returns the URL for the given repository.                      │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[spcs.job]
+  '''
+                                                                                  
+   Usage: default spcs job [OPTIONS] COMMAND [ARGS]...                            
+                                                                                  
+   Manages Snowpark jobs.                                                         
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ create   Creates a job to run in a compute pool.                             │
+  │ logs     Retrieves local logs from a job container.                          │
+  │ status   Returns the status of a named Snowpark Container Services job.      │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[spcs.service]
+  '''
+                                                                                  
+   Usage: default spcs service [OPTIONS] COMMAND [ARGS]...                        
+                                                                                  
+   Manages Snowpark Container Services services.                                  
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ create           Creates a new service in the current schema.                │
+  │ describe         Provides description of service.                            │
+  │ drop             Drops service with given name.                              │
+  │ list             Lists all available services.                               │
+  │ list-endpoints   Lists the endpoints in a service.                           │
+  │ logs             Retrieves local logs from a service container.              │
+  │ resume           Resumes the service from a SUSPENDED state.                 │
+  │ set              Sets one or more properties for the service.                │
+  │ status           Retrieves the status of a service.                          │
+  │ suspend          Suspends the service, shutting down and deleting all its    │
+  │                  containers.                                                 │
+  │ unset            Resets one or more properties for the service to their      │
+  │                  default value(s).                                           │
+  │ upgrade          Updates an existing service with a new specification file.  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[spcs]
+  '''
+                                                                                  
+   Usage: default spcs [OPTIONS] COMMAND [ARGS]...                                
+                                                                                  
+   Manages Snowpark Container Services compute pools, services, image registries, 
+   and image repositories.                                                        
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ compute-pool       Manages compute pools.                                    │
+  │ image-registry     Manages image registries.                                 │
+  │ image-repository   Manages image repositories.                               │
+  │ service            Manages services.                                         │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[stage]
+  '''
+                                                                                  
+   Usage: default stage [OPTIONS] COMMAND [ARGS]...                               
+                                                                                  
+   Manages stages.                                                                
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ copy         Copies all files from target path to target directory. This     │
+  │              works for both uploading to and downloading files from the      │
+  │              stage.                                                          │
+  │ create       Creates a named stage if it does not already exist.             │
+  │ describe     Provides description of stage.                                  │
+  │ drop         Drops stage with given name.                                    │
+  │ execute      Execute immediate all files from the stage path. Files can be   │
+  │              filtered with glob like pattern, e.g. `@stage/*.sql`,           │
+  │              `@stage/dev/*`. Only files with `.sql` extension will be        │
+  │              executed.                                                       │
+  │ list         Lists all available stages.                                     │
+  │ list-files   Lists the stage contents.                                       │
+  │ remove       Removes a file from a stage.                                    │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages_no_help_flag[streamlit]
+  '''
+                                                                                  
+   Usage: default streamlit [OPTIONS] COMMAND [ARGS]...                           
+                                                                                  
+   Manages a Streamlit app in Snowflake.                                          
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ deploy     Deploys a Streamlit app defined in the project definition file    │
+  │            (snowflake.yml). By default, the command uploads environment.yml  │
+  │            and any other pages or folders, if present. If you don’t specify  │
+  │            a stage name, the `streamlit` stage is used. If the specified     │
+  │            stage does not exist, the command creates it.                     │
+  │ describe   Provides description of streamlit.                                │
+  │ drop       Drops streamlit with given name.                                  │
+  │ get-url    Returns a URL to the specified Streamlit app                      │
+  │ init       Initializes this directory with a sample set of files for         │
+  │            creating a Streamlit app project.                                 │
+  │ list       Lists all available streamlits.                                   │
+  │ share      Shares a Streamlit app with another role.                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
```

### Comparing `snowflake_cli_labs-2.3.1/tests/api/test_feature_flags.py` & `snowflake_cli_labs-2.4.0rc0/tests/api/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/api/test_secure_path.py` & `snowflake_cli_labs-2.4.0rc0/tests/api/test_secure_path.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/api/commands/test_flags.py` & `snowflake_cli_labs-2.4.0rc0/tests/api/commands/test_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/api/commands/test_snow_typer.py` & `snowflake_cli_labs-2.4.0rc0/tests/api/commands/test_snow_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/api/commands/__snapshots__/test_flags.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/api/commands/__snapshots__/test_flags.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/api/commands/__snapshots__/test_snow_typer.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/api/console/test_cli_console_output.py` & `snowflake_cli_labs-2.4.0rc0/tests/api/console/test_cli_console_output.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,7 +60,17 @@
 
 
 def test_phase_nesting_not_allowed(cli_console):
     with cli_console.phase("Enter 1"):
         with pytest.raises(CliConsoleNestingProhibitedError):
             with cli_console.phase("Enter 2"):
                 pass
+
+
+def test_phase_is_cleaned_up_on_exception(cli_console):
+    with pytest.raises(RuntimeError):
+        with cli_console.phase("Enter 1"):
+            raise RuntimeError("Phase failed")
+
+    # If the phase is cleaned up correctly, this will no raise any exception
+    with cli_console.phase("Enter 2") as step:
+        pass
```

### Comparing `snowflake_cli_labs-2.3.1/tests/api/console/test_console_abc.py` & `snowflake_cli_labs-2.4.0rc0/tests/api/console/test_console_abc.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/api/console/test_intermediate_output.py` & `snowflake_cli_labs-2.4.0rc0/tests/api/console/test_intermediate_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/app/test_telemetry.py` & `snowflake_cli_labs-2.4.0rc0/tests/app/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/git/test_git_commands.py` & `snowflake_cli_labs-2.4.0rc0/tests/git/test_git_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -484,14 +484,37 @@
         mock.call("ls @repo/branches/main/", cursor_class=DictCursor),
         mock.call(
             f"execute immediate from @repo/branches/main/s1.sql using (key1=>'string value', key2=>1, key3=>TRUE, key4=>NULL, key5=>'var=value')"
         ),
     ]
 
 
+@mock.patch("snowflake.connector.connect")
+@pytest.mark.parametrize(
+    "command, parameters",
+    [
+        ("list", []),
+        ("list", ["--like", "PATTERN"]),
+        ("describe", ["NAME"]),
+        ("drop", ["NAME"]),
+    ],
+)
+def test_command_aliases(mock_connector, runner, mock_ctx, command, parameters):
+    ctx = mock_ctx()
+    mock_connector.return_value = ctx
+
+    result = runner.invoke(["object", command, "git-repository", *parameters])
+    assert result.exit_code == 0, result.output
+    result = runner.invoke(["git", command, *parameters], catch_exceptions=False)
+    assert result.exit_code == 0, result.output
+
+    queries = ctx.get_queries()
+    assert queries[0] == queries[1]
+
+
 def _assert_invalid_repo_path_error_message(output):
     assert "Error" in output
     assert (
         "REPOSITORY_PATH should be a path to git repository stage with scope" in output
     )
     assert (
         "provided. Path to the repository root must end with '/'. For example:"
```

### Comparing `snowflake_cli_labs-2.3.1/tests/git/__snapshots__/test_git_commands.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/git/__snapshots__/test_git_commands.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/patch_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/patch_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_annotation_processor_config.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_annotation_processor_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import pytest
 from snowflake.cli.api.project.definition import (
     load_project_definition,
 )
+from snowflake.cli.api.project.schemas.native_app.path_mapping import ProcessorMapping
 
 
 @pytest.mark.parametrize(
     "project_definition_files", ["napp_with_annotation_processor"], indirect=True
 )
 def test_napp_project_with_annotation_processor(project_definition_files):
     project = load_project_definition(project_definition_files)
     assert len(project.native_app.artifacts) == 3
 
     result = project.native_app.artifacts[2]
     assert len(result.processors) == 3
-    assert result.processors[0] == "simple_processor_str"
+
+    assert isinstance(result.processors[0], ProcessorMapping)
+    assert result.processors[0].name == "simple_processor_str"
+
+    assert isinstance(result.processors[1], ProcessorMapping)
     assert result.processors[1].name == "processor_without_properties"
     assert result.processors[1].properties is None
-    assert result.processors[2].name == "processor_with_properties"
 
+    assert isinstance(result.processors[2], ProcessorMapping)
+    assert result.processors[2].name == "processor_with_properties"
     properties = result.processors[2].properties
     assert len(properties.keys()) == 2
     assert properties["key_1"] == "value_1"
     assert properties["key_2"]["key_3"] == "value_3"
     assert len(properties["key_2"]["key_4"]) == 3
     assert properties["key_2"]["key_4"][0] == "value_a"
     assert properties["key_2"]["key_4"][1] == "value_b"
```

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_commands.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_feature_flags.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_init.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_init.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_manager.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_package_scripts.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_package_scripts.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_run_processor.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_run_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_teardown_processor.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_teardown_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from unittest import mock
 
 import pytest
+from click import Abort
 from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.cli.plugins.nativeapp.constants import (
     SPECIAL_COMMENT,
     SPECIAL_COMMENT_OLD,
 )
 from snowflake.cli.plugins.nativeapp.exceptions import (
     CouldNotDropApplicationPackageWithVersions,
@@ -17,21 +18,23 @@
 )
 from snowflake.connector import ProgrammingError
 from snowflake.connector.cursor import DictCursor
 
 from tests.nativeapp.patch_utils import mock_get_app_pkg_distribution_in_sf
 from tests.nativeapp.utils import (
     NATIVEAPP_MANAGER_EXECUTE,
+    NATIVEAPP_MANAGER_GET_OBJECTS_OWNED_BY_APPLICATION,
     NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME,
     TEARDOWN_MODULE,
     TEARDOWN_PROCESSOR_DROP_GENERIC_OBJECT,
     TEARDOWN_PROCESSOR_GET_EXISTING_APP_INFO,
     TEARDOWN_PROCESSOR_GET_EXISTING_APP_PKG_INFO,
     TEARDOWN_PROCESSOR_IS_CORRECT_OWNER,
     TYPER_CONFIRM,
+    TYPER_PROMPT,
     mock_execute_helper,
     mock_snowflake_yml_file,
     quoted_override_yml_file,
 )
 from tests.testing_utils.files_and_dirs import create_named_file
 
 
@@ -165,24 +168,26 @@
     mock_get_existing_app_info.assert_called_once()
 
 
 # Test drop_application() successfully when it has special comment
 @mock.patch(TEARDOWN_PROCESSOR_GET_EXISTING_APP_INFO)
 @mock.patch(TEARDOWN_PROCESSOR_IS_CORRECT_OWNER, return_value=True)
 @mock.patch(TEARDOWN_PROCESSOR_DROP_GENERIC_OBJECT, return_value=None)
+@mock.patch(NATIVEAPP_MANAGER_GET_OBJECTS_OWNED_BY_APPLICATION, return_value=[])
 @pytest.mark.parametrize(
     "auto_yes_param, special_comment",  # auto_yes should have no effect on the test
     [
         (True, SPECIAL_COMMENT),
         (True, SPECIAL_COMMENT_OLD),
         (False, SPECIAL_COMMENT),
         (False, SPECIAL_COMMENT_OLD),
     ],
 )
 def test_drop_application_has_special_comment(
+    mock_get_objects_owned_by_application,
     mock_drop_generic_object,
     mock_is_correct_owner,
     mock_get_existing_app_info,
     auto_yes_param,
     special_comment,
     temp_dir,
 ):
@@ -204,24 +209,26 @@
     mock_get_existing_app_info.assert_called_once()
     mock_is_correct_owner.assert_called_once()
     mock_drop_generic_object.assert_called_once()
 
 
 # Test drop_application() successfully when it has special comment but is a quoted string
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
+@mock.patch(NATIVEAPP_MANAGER_GET_OBJECTS_OWNED_BY_APPLICATION, return_value=[])
 @pytest.mark.parametrize(
     "auto_yes_param, special_comment",  # auto_yes should have no effect on the test
     [
         (True, SPECIAL_COMMENT),
         (True, SPECIAL_COMMENT_OLD),
         (False, SPECIAL_COMMENT),
         (False, SPECIAL_COMMENT_OLD),
     ],
 )
 def test_drop_application_has_special_comment_and_quoted_name(
+    mock_get_objects_owned_by_application,
     mock_execute,
     auto_yes_param,
     special_comment,
     temp_dir,
     mock_cursor,
 ):
     side_effects, expected = mock_execute_helper(
@@ -320,19 +327,21 @@
 # Test drop_application() without special comment AND auto_yes is False AND should_drop is True
 # Test drop_application() without special comment AND auto_yes is True
 @mock.patch(TEARDOWN_PROCESSOR_GET_EXISTING_APP_INFO)
 @mock.patch(TEARDOWN_PROCESSOR_IS_CORRECT_OWNER, return_value=True)
 @mock.patch(TEARDOWN_PROCESSOR_DROP_GENERIC_OBJECT, return_value=None)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock.patch(f"{TEARDOWN_MODULE}.{TYPER_CONFIRM}", return_value=True)
+@mock.patch(NATIVEAPP_MANAGER_GET_OBJECTS_OWNED_BY_APPLICATION, return_value=[])
 @pytest.mark.parametrize(
     "auto_yes_param",
     [False, True],
 )
 def test_drop_application_user_allows_drop(
+    mock_get_objects_owned_by_application,
     mock_confirm,
     mock_execute,
     mock_drop_generic_object,
     mock_is_correct_owner,
     mock_get_existing_app_info,
     auto_yes_param,
     temp_dir,
@@ -374,19 +383,21 @@
     mock_execute.mock_calls == expected
 
 
 # Test idempotent drop_application()
 @mock.patch(TEARDOWN_PROCESSOR_GET_EXISTING_APP_INFO)
 @mock.patch(TEARDOWN_PROCESSOR_IS_CORRECT_OWNER, return_value=True)
 @mock.patch(TEARDOWN_PROCESSOR_DROP_GENERIC_OBJECT, return_value=None)
+@mock.patch(NATIVEAPP_MANAGER_GET_OBJECTS_OWNED_BY_APPLICATION, return_value=[])
 @pytest.mark.parametrize(
     "auto_yes_param",
     [False, True],  # This should have no effect on the test
 )
 def test_drop_application_idempotent(
+    mock_get_objects_owned_by_application,
     mock_drop_generic_object,
     mock_is_correct_owner,
     mock_get_existing_app_info,
     auto_yes_param,
     temp_dir,
 ):
     side_effects_for_get_existing_app_info = [
@@ -1000,7 +1011,71 @@
     teardown_processor.drop_package(auto_yes_param)
     teardown_processor.drop_package(auto_yes_param)
 
     mock_get_existing_app_pkg_info.call_count == 3
     mock_is_correct_owner.assert_called_once()
     mock_drop_generic_object.assert_called_once()
     mock_execute.mock_calls == expected
+
+
+@mock.patch(f"{TEARDOWN_MODULE}.{TYPER_PROMPT}")
+@mock.patch(TEARDOWN_PROCESSOR_GET_EXISTING_APP_INFO)
+@mock.patch(TEARDOWN_PROCESSOR_IS_CORRECT_OWNER, return_value=True)
+@mock.patch(TEARDOWN_PROCESSOR_DROP_GENERIC_OBJECT, return_value=None)
+@mock.patch(NATIVEAPP_MANAGER_GET_OBJECTS_OWNED_BY_APPLICATION)
+@pytest.mark.parametrize(
+    "cascade,application_objects,interactive_response,expected_cascade",
+    [
+        # Cascade true
+        [True, [], None, True],
+        [True, [{"type": "DATABASE", "name": "db"}], None, True],
+        # Cascade false
+        [False, [], None, False],
+        [False, [{"type": "DATABASE", "name": "db"}], None, False],
+        # Cascade unset
+        [None, [], None, False],
+        [None, [{"type": "DATABASE", "name": "db"}], None, None],
+        # Interactive
+        [None, [{"type": "DATABASE", "name": "db"}], "yes", True],
+        [None, [{"type": "DATABASE", "name": "db"}], "no", False],
+        [None, [{"type": "DATABASE", "name": "db"}], "abort", None],
+    ],
+)
+def test_drop_application_cascade(
+    mock_get_objects_owned_by_application,
+    mock_drop_generic_object,
+    mock_is_correct_owner,
+    mock_get_existing_app_info,
+    mock_typer_prompt,
+    cascade,
+    application_objects,
+    interactive_response,
+    expected_cascade,
+    temp_dir,
+):
+    mock_get_objects_owned_by_application.return_value = application_objects
+    mock_get_existing_app_info.return_value = {
+        "name": "myapp",
+        "owner": "app_role",
+        "comment": SPECIAL_COMMENT,
+    }
+    current_working_directory = os.getcwd()
+    create_named_file(
+        file_name="snowflake.yml",
+        dir_name=current_working_directory,
+        contents=[mock_snowflake_yml_file],
+    )
+    interactive = interactive_response is not None
+    mock_typer_prompt.return_value = interactive_response
+
+    teardown_processor = _get_na_teardown_processor()
+    if expected_cascade is None:
+        with pytest.raises(Abort):
+            teardown_processor.drop_application(False, interactive, cascade)
+    else:
+        teardown_processor.drop_application(False, interactive, cascade)
+        mock_drop_generic_object.assert_called_once_with(
+            object_type="application",
+            object_name="myapp",
+            role="app_role",
+            cascade=expected_cascade,
+        )
```

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_version_create_processor.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_version_create_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/test_version_drop_processor.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/test_version_drop_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/utils.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from textwrap import dedent
 
 NATIVEAPP_MODULE = "snowflake.cli.plugins.nativeapp.manager"
 TEARDOWN_MODULE = "snowflake.cli.plugins.nativeapp.teardown_processor"
 TYPER_CONFIRM = "typer.confirm"
+TYPER_PROMPT = "typer.prompt"
 RUN_MODULE = "snowflake.cli.plugins.nativeapp.run_processor"
 VERSION_MODULE = "snowflake.cli.plugins.nativeapp.version.version_processor"
 
 TEARDOWN_PROCESSOR = f"{TEARDOWN_MODULE}.NativeAppTeardownProcessor"
 NATIVEAPP_MANAGER = f"{NATIVEAPP_MODULE}.NativeAppManager"
 RUN_PROCESSOR = f"{RUN_MODULE}.NativeAppRunProcessor"
 
@@ -18,14 +19,17 @@
 )
 NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME = (
     f"{NATIVEAPP_MANAGER}.verify_project_distribution"
 )
 NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO = (
     f"{NATIVEAPP_MANAGER}.get_existing_app_pkg_info"
 )
+NATIVEAPP_MANAGER_GET_OBJECTS_OWNED_BY_APPLICATION = (
+    f"{NATIVEAPP_MANAGER}.get_objects_owned_by_application"
+)
 
 TEARDOWN_PROCESSOR_GET_EXISTING_APP_INFO = f"{TEARDOWN_PROCESSOR}.get_existing_app_info"
 TEARDOWN_PROCESSOR_GET_EXISTING_APP_PKG_INFO = (
     f"{TEARDOWN_PROCESSOR}.get_existing_app_pkg_info"
 )
 TEARDOWN_PROCESSOR_IS_CORRECT_OWNER = f"{TEARDOWN_MODULE}.ensure_correct_owner"
 TEARDOWN_PROCESSOR_DROP_GENERIC_OBJECT = f"{TEARDOWN_PROCESSOR}.drop_generic_object"
```

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/__snapshots__/test_commands.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/__snapshots__/test_init.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/__snapshots__/test_init.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/nativeapp/codegen/test_sandbox.py` & `snowflake_cli_labs-2.4.0rc0/tests/nativeapp/codegen/test_sandbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     mock_which.return_value = None
 
     with pytest.raises(sandbox.SandboxExecutionError):
         sandbox.execute_script_in_sandbox(
             PYTHON_SCRIPT, sandbox.ExecutionEnvironmentType.CONDA, name="foo"
         )
 
-    assert mock_which.called_once_with("conda")
+    mock_which.assert_has_calls((mock.call("conda"),))
     assert not mock_run.called
 
 
 @mock.patch("subprocess.run")
 @mock.patch("shutil.which")
 def test_execute_in_conda_env_fails_when_conda_env_cannot_be_determined(
     mock_which, mock_run, mock_environ
@@ -441,16 +441,16 @@
     )
 
     assert actual.args == SCRIPT_ARGS
     assert actual.returncode == 0
     assert actual.stdout == SCRIPT_OUT
     assert actual.stderr == SCRIPT_ERR
 
-    assert mock_which.called_once_with("python3")
-    assert mock_which.called_once_with("python")
+    assert mock_which.call_count == 2, mock_which.call_count
+    mock_which.assert_has_calls((mock.call("python3"), mock.call("python")))
 
 
 @mock.patch("subprocess.run")
 @mock.patch("shutil.which")
 @mock.patch("sys.executable", "/path/to/python")
 def test_execute_system_python_falls_back_to_current_interpreter(
     mock_which, mock_run, mock_environ
@@ -477,16 +477,16 @@
     )
 
     assert actual.args == SCRIPT_ARGS
     assert actual.returncode == 0
     assert actual.stdout == SCRIPT_OUT
     assert actual.stderr == SCRIPT_ERR
 
-    assert mock_which.called_once_with("python3")
-    assert mock_which.called_once_with("python")
+    assert mock_which.call_count == 2, mock_which.call_count
+    mock_which.assert_has_calls((mock.call("python3"), mock.call("python")))
 
 
 @mock.patch("subprocess.run")
 @mock.patch("shutil.which")
 @mock.patch("sys.executable", None)
 def test_execute_system_python_fails_when_no_interpreter_available(
     mock_which, mock_run, mock_environ
@@ -495,16 +495,16 @@
 
     with pytest.raises(sandbox.SandboxExecutionError):
         sandbox.execute_script_in_sandbox(
             PYTHON_SCRIPT, sandbox.ExecutionEnvironmentType.SYSTEM_PATH
         )
 
     assert not mock_run.called
-    assert mock_which.called_once_with("python3")
-    assert mock_which.called_once_with("python")
+    assert mock_which.call_count == 2, mock_which.call_count
+    mock_which.assert_has_calls((mock.call("python3"), mock.call("python")))
 
 
 @pytest.mark.parametrize(
     "expected_timeout, expected_cwd",
     [
         (None, None),
         (TIMEOUT, None),
@@ -649,16 +649,14 @@
     )
 
     assert actual.args == SCRIPT_ARGS
     assert actual.returncode == 0
     assert actual.stdout == SCRIPT_OUT
     assert actual.stderr == SCRIPT_ERR
 
-    assert mock_run.called_once_with("python3")
-
 
 @mock.patch("subprocess.run")
 @mock.patch("shutil.which")
 def test_execute_auto_detect_chooses_venv_over_conda(
     mock_which, mock_run, mock_environ, fake_venv_root
 ):
     mock_environ.side_effect = {
```

### Comparing `snowflake_cli_labs-2.3.1/tests/notebook/test_notebook_commands.py` & `snowflake_cli_labs-2.4.0rc0/tests/notebook/test_notebook_commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,7 +29,23 @@
     mock_url.return_value = "http://my.url"
     result = runner.invoke(["notebook", "open", "my_notebook"])
 
     assert result.exit_code == 0, result.output
     assert result.output == "http://my.url\n"
     mock_url.assert_called_once_with(notebook_name="my_notebook")
     mock_launch.assert_called_once_with("http://my.url")
+
+
+@mock.patch.object(NotebookManager, "create")
+def test_create(mock_create, runner):
+    notebook_name = "my_notebook"
+    notebook_file = "@stage/notebook.ipynb"
+
+    result = runner.invoke(
+        ("notebook", "create", notebook_name, "--notebook-file", notebook_file)
+    )
+    assert result.exit_code == 0, result.output
+
+    mock_create.assert_called_once_with(
+        notebook_name=notebook_name,
+        notebook_file=notebook_file,
+    )
```

### Comparing `snowflake_cli_labs-2.3.1/tests/object/test_common.py` & `snowflake_cli_labs-2.4.0rc0/tests/object/test_common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Tuple
 
 import pytest
 from snowflake.cli.plugins.object.common import (
     Tag,
     TagError,
     _parse_tag,
```

### Comparing `snowflake_cli_labs-2.3.1/tests/object/test_object.py` & `snowflake_cli_labs-2.4.0rc0/tests/object/test_object.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/object/test_stage.py` & `snowflake_cli_labs-2.4.0rc0/tests/object/test_stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/object/__snapshots__/test_object.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/object/__snapshots__/test_object.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/output/test_format_silent_enforcement.py` & `snowflake_cli_labs-2.4.0rc0/tests/output/test_format_silent_enforcement.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/output/test_printing.py` & `snowflake_cli_labs-2.4.0rc0/tests/output/test_printing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from datetime import datetime
 from textwrap import dedent
 from typing import NamedTuple
 
 import pytest
 from snowflake.cli.api.output.formats import OutputFormat
 from snowflake.cli.api.output.types import (
@@ -284,26 +285,32 @@
 def test_print_with_no_data_table(capsys):
     print_result(None)
     assert get_output(capsys) == "Done\n"
 
 
 def test_print_with_no_data_in_query_json(capsys, _empty_cursor):
     print_result(QueryResult(_empty_cursor()), output_format=OutputFormat.JSON)
-    assert get_output(capsys) == "[]"
+    json_str = get_output(capsys)
+    json.loads(json_str)
+    assert json_str == "[]\n"
 
 
 def test_print_with_no_data_in_single_value_query_json(capsys, _empty_cursor):
     print_result(SingleQueryResult(_empty_cursor()), output_format=OutputFormat.JSON)
-    assert get_output(capsys) == "null"
+    json_str = get_output(capsys)
+    json.loads(json_str)
+    assert json_str == "null\n"
 
 
 def test_print_with_no_response_json(capsys):
     print_result(None, output_format=OutputFormat.JSON)
 
-    assert get_output(capsys) == "null"
+    json_str = get_output(capsys)
+    json.loads(json_str)
+    assert json_str == "null\n"
 
 
 @pytest.fixture
 def _empty_cursor(mock_cursor):
     return lambda: mock_cursor(
         columns=["string", "number", "array", "object", "date"],
         rows=[],
```

### Comparing `snowflake_cli_labs-2.3.1/tests/output/test_silent_output.py` & `snowflake_cli_labs-2.4.0rc0/tests/output/test_silent_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/plugin/test_broken_plugin.py` & `snowflake_cli_labs-2.4.0rc0/tests/plugin/test_broken_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/plugin/test_failing_plugin.py` & `snowflake_cli_labs-2.4.0rc0/tests/plugin/test_failing_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/plugin/test_override_by_external_plugins.py` & `snowflake_cli_labs-2.4.0rc0/tests/plugin/test_override_by_external_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/project/fixtures.py` & `snowflake_cli_labs-2.4.0rc0/tests/project/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import shutil
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Generator, List
 
 import pytest
```

### Comparing `snowflake_cli_labs-2.3.1/tests/project/test_config.py` & `snowflake_cli_labs-2.4.0rc0/tests/project/test_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from __future__ import annotations
+
 from pathlib import Path
 from typing import List, Optional
 from unittest import mock
 from unittest.mock import PropertyMock
 
 import pytest
 from snowflake.cli.api.project.definition import (
     generate_local_override_yml,
     load_project_definition,
 )
 from snowflake.cli.api.project.errors import SchemaValidationError
+from snowflake.cli.api.project.schemas.project_definition import ProjectDefinition
 
 
 @pytest.mark.parametrize("project_definition_files", ["napp_project_1"], indirect=True)
 def test_napp_project_1(project_definition_files):
     project = load_project_definition(project_definition_files)
     assert project.native_app.name == "myapp"
     assert project.native_app.deploy_root == "output/deploy/"
@@ -55,15 +58,15 @@
 
 
 @pytest.mark.parametrize("project_definition_files", ["underspecified"], indirect=True)
 def test_underspecified_project(project_definition_files):
     with pytest.raises(SchemaValidationError) as exc_info:
         load_project_definition(project_definition_files)
 
-    assert "NativeApp schema" in str(exc_info)
+    assert "NativeApp" in str(exc_info)
     assert "Your project definition is missing following fields: ('artifacts',)" in str(
         exc_info.value
     )
 
 
 @pytest.mark.parametrize(
     "project_definition_files", ["no_definition_version"], indirect=True
@@ -78,19 +81,19 @@
         in str(exc_info.value)
     )
 
 
 @pytest.mark.parametrize("project_definition_files", ["unknown_fields"], indirect=True)
 def test_does_not_accept_unknown_fields(project_definition_files):
     with pytest.raises(SchemaValidationError) as exc_info:
-        project = load_project_definition(project_definition_files)
+        load_project_definition(project_definition_files)
 
-    assert "NativeApp schema" in str(exc_info)
+    assert "NativeApp" in str(exc_info)
     assert (
-        "You provided field '('unknown_fields_accepted',)' with value 'true' that is not present in the schema"
+        "You provided field '('unknown_fields_accepted',)' with value 'true' that is not supported in given version."
         in str(exc_info)
     )
 
 
 @pytest.mark.parametrize(
     "project_definition_files",
     [
@@ -111,7 +114,21 @@
         "streamlit_full_definition",
     ],
     indirect=True,
 )
 def test_fields_are_parsed_correctly(project_definition_files, snapshot):
     result = load_project_definition(project_definition_files).model_dump()
     assert result == snapshot
+
+
+@pytest.mark.parametrize(
+    "data",
+    [
+        {"definition_version": "1", "env": {"foo": "bar"}},
+        {"definition_version": "1.1", "unknown": {}},
+    ],
+)
+def test_schema_is_validated_for_version(data):
+    with pytest.raises(SchemaValidationError) as err:
+        ProjectDefinition(**data)
+
+    assert "is not supported in given version" in str(err.value)
```

### Comparing `snowflake_cli_labs-2.3.1/tests/project/test_definition_manager.py` & `snowflake_cli_labs-2.4.0rc0/tests/project/test_definition_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/project/test_project_schemas.py` & `snowflake_cli_labs-2.4.0rc0/tests/project/test_project_schemas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 from pydantic import ValidationError
+from snowflake.cli.api.project.errors import SchemaValidationError
 from snowflake.cli.api.project.schemas.project_definition import ProjectDefinition
 from snowflake.cli.api.project.schemas.snowpark.argument import Argument
 from snowflake.cli.api.project.schemas.snowpark.callable import FunctionSchema
 
 
 def test_if_fields_are_updated_correctly_by_assignment(argument_instance: Argument):
     argument_instance.name = "Baz"
@@ -59,7 +60,21 @@
     assert native_app_project_instance.native_app.name == "napp_test"
     assert native_app_project_instance.native_app.package.distribution == "internal"
     update_dict = {"native_app": {"package": {"distribution": "external"}}}
 
     native_app_project_instance.update_from_dict(update_dict)
     assert native_app_project_instance.native_app.name == "napp_test"
     assert native_app_project_instance.native_app.package.distribution == "external"
+
+
+def test_project_definition_work_for_int_version():
+    p = ProjectDefinition(definition_version=1)
+    assert p.definition_version == "1"
+
+
+def test_project_definition_fails_for_unknown_version():
+    with pytest.raises(SchemaValidationError) as err:
+        ProjectDefinition(definition_version="6.2.3")
+
+    assert "Version 6.2.3 is not supported. Supported versions: 1, 1.1" in str(
+        err.value
+    )
```

### Comparing `snowflake_cli_labs-2.3.1/tests/project/test_util.py` & `snowflake_cli_labs-2.4.0rc0/tests/project/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/project/__snapshots__/test_config.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/project/__snapshots__/test_config.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # serializer version: 1
 # name: test_fields_are_parsed_correctly[integration]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': dict({
       'application': None,
       'artifacts': list([
         dict({
           'dest': './',
-          'processors': None,
+          'processors': list([
+          ]),
           'src': 'app/*',
         }),
       ]),
       'deploy_root': 'output/deploy/',
+      'generated_root': '__generated/',
       'name': 'integration',
       'package': dict({
         'distribution': 'internal',
         'name': None,
         'role': None,
         'scripts': list([
           'package/001-shared.sql',
@@ -27,25 +30,28 @@
     }),
     'snowpark': None,
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[integration_external]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': dict({
       'application': None,
       'artifacts': list([
         dict({
           'dest': './',
-          'processors': None,
+          'processors': list([
+          ]),
           'src': 'app/*',
         }),
       ]),
       'deploy_root': 'output/deploy/',
+      'generated_root': '__generated/',
       'name': 'integration_external',
       'package': dict({
         'distribution': 'external',
         'name': None,
         'role': None,
         'scripts': list([
           'package/001-shared.sql',
@@ -57,50 +63,55 @@
     }),
     'snowpark': None,
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[minimal]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': dict({
       'application': None,
       'artifacts': list([
         'setup.sql',
         'README.md',
       ]),
       'deploy_root': 'output/deploy/',
+      'generated_root': '__generated/',
       'name': 'minimal',
       'package': None,
       'source_stage': 'app_src.stage',
     }),
     'snowpark': None,
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[napp_project_1]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': dict({
       'application': dict({
         'debug': True,
         'name': 'myapp_polly',
         'role': 'myapp_consumer',
         'warehouse': None,
       }),
       'artifacts': list([
         'setup.sql',
         'app/README.md',
         dict({
           'dest': 'ui/',
-          'processors': None,
+          'processors': list([
+          ]),
           'src': 'app/streamlit/*.py',
         }),
       ]),
       'deploy_root': 'output/deploy/',
+      'generated_root': '__generated/',
       'name': 'myapp',
       'package': dict({
         'distribution': 'internal',
         'name': 'myapp_pkg_polly',
         'role': 'accountadmin',
         'scripts': list([
           '001-shared.sql',
@@ -112,32 +123,35 @@
     }),
     'snowpark': None,
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[napp_project_with_pkg_warehouse]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': dict({
       'application': dict({
         'debug': True,
         'name': 'myapp_polly',
         'role': 'myapp_consumer',
         'warehouse': None,
       }),
       'artifacts': list([
         'setup.sql',
         'app/README.md',
         dict({
           'dest': 'ui/',
-          'processors': None,
+          'processors': list([
+          ]),
           'src': 'app/streamlit/*.py',
         }),
       ]),
       'deploy_root': 'output/deploy/',
+      'generated_root': '__generated/',
       'name': 'myapp',
       'package': dict({
         'distribution': 'internal',
         'name': 'myapp_pkg_polly',
         'role': 'accountadmin',
         'scripts': list([
           '001-shared.sql',
@@ -149,15 +163,16 @@
     }),
     'snowpark': None,
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_function_external_access]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
         dict({
           'database': None,
           'external_access_integrations': list([
             'external_1',
@@ -195,15 +210,16 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_function_fully_qualified_name]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
         dict({
           'database': None,
           'external_access_integrations': list([
           ]),
@@ -337,15 +353,16 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_function_secrets_without_external_access]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
         dict({
           'database': None,
           'external_access_integrations': list([
           ]),
@@ -381,15 +398,16 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_functions]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
         dict({
           'database': None,
           'external_access_integrations': list([
           ]),
@@ -423,15 +441,16 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_procedure_external_access]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
       ]),
       'procedures': list([
         dict({
           'database': None,
@@ -465,15 +484,16 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_procedure_fully_qualified_name]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
       ]),
       'procedures': list([
         dict({
           'database': None,
@@ -613,15 +633,16 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_procedure_secrets_without_external_access]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
       ]),
       'procedures': list([
         dict({
           'database': None,
@@ -653,15 +674,16 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_procedures]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
       ]),
       'procedures': list([
         dict({
           'database': None,
@@ -707,15 +729,16 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[snowpark_procedures_coverage]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': dict({
       'functions': list([
       ]),
       'procedures': list([
         dict({
           'database': None,
@@ -745,24 +768,27 @@
       'stage_name': 'dev_deployment',
     }),
     'streamlit': None,
   })
 # ---
 # name: test_fields_are_parsed_correctly[streamlit_full_definition]
   dict({
-    'definition_version': 1,
+    'definition_version': '1',
+    'env': None,
     'native_app': None,
     'snowpark': None,
     'streamlit': dict({
       'additional_source_files': list([
         'utils/utils.py',
         'extra_file.py',
       ]),
+      'database': None,
       'env_file': 'environment.yml',
       'main_file': 'streamlit_app.py',
       'name': 'test_streamlit',
       'pages_dir': 'pages',
       'query_warehouse': 'test_warehouse',
+      'schema_name': None,
       'stage': 'streamlit',
     }),
   })
 # ---
```

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/mocks.py` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/mocks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/test_anaconda.py` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_anaconda.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/test_build.py` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_build.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/test_common.py` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Tuple
 
 import pytest
 from snowflake.cli.plugins.snowpark.common import (
     _convert_resource_details_to_dict,
     _snowflake_dependencies_differ,
     _sql_to_python_return_type_mapper,
```

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/test_function.py` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_function.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 
+import pytest
 from snowflake.connector import ProgrammingError
 
 
 @mock.patch("snowflake.connector.connect")
 @mock.patch("snowflake.cli.plugins.snowpark.commands.ObjectManager")
 def test_deploy_function(
     mock_object_manager,
@@ -27,24 +28,24 @@
                 "deploy",
             ],
             catch_exceptions=False,
         )
 
     assert result.exit_code == 0, result.output
     assert ctx.get_queries() == [
-        "create stage if not exists MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT comment='deployments managed by Snowflake CLI'",
-        f"put file://{Path(project_dir).resolve()}/app.zip @MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project"
+        "create stage if not exists MockDatabase.MockSchema.dev_deployment comment='deployments managed by Snowflake CLI'",
+        f"put file://{Path(project_dir).resolve()}/app.zip @MockDatabase.MockSchema.dev_deployment/my_snowpark_project"
         f" auto_compress=false parallel=4 overwrite=True",
         dedent(
             """\
-            create or replace function MOCKDATABASE.MOCKSCHEMA.FUNC1(a string default 'default value', b variant)
+            create or replace function MockDatabase.MockSchema.func1(a string default 'default value', b variant)
             returns string
             language python
             runtime_version=3.10
-            imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
+            imports=('@MockDatabase.MockSchema.dev_deployment/my_snowpark_project/app.zip')
             handler='app.func1_handler'
             packages=()
             """
         ).strip(),
     ]
 
 
@@ -74,24 +75,24 @@
                 "deploy",
             ],
             catch_exceptions=False,
         )
 
     assert result.exit_code == 0, result.output
     assert ctx.get_queries() == [
-        "create stage if not exists MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT comment='deployments managed by Snowflake CLI'",
-        f"put file://{Path(project_dir).resolve()}/app.zip @MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project"
+        "create stage if not exists MockDatabase.MockSchema.dev_deployment comment='deployments managed by Snowflake CLI'",
+        f"put file://{Path(project_dir).resolve()}/app.zip @MockDatabase.MockSchema.dev_deployment/my_snowpark_project"
         f" auto_compress=false parallel=4 overwrite=True",
         dedent(
             """\
-            create or replace function MOCKDATABASE.MOCKSCHEMA.FUNC1(a string, b variant)
+            create or replace function MockDatabase.MockSchema.func1(a string, b variant)
             returns string
             language python
             runtime_version=3.8
-            imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
+            imports=('@MockDatabase.MockSchema.dev_deployment/my_snowpark_project/app.zip')
             handler='app.func1_handler'
             packages=()
             external_access_integrations=(external_1,external_2)
             secrets=('cred'=cred_name,'other'=other_name)
             """
         ).strip(),
     ]
@@ -134,15 +135,15 @@
     mock_cursor,
     project_directory,
 ):
     rows = [
         ("packages", '["foo==1.2.3", "bar>=3.0.0"]'),
         ("handler", "app.func1_handler"),
         ("returns", "string"),
-        ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
+        ("imports", "dev_deployment/my_snowpark_project/app.zip"),
     ]
 
     queries, result, project_dir = _deploy_function(
         rows,
         mock_connector,
         runner,
         mock_ctx,
@@ -150,22 +151,22 @@
         project_directory,
         "--replace",
     )
 
     assert result.exit_code == 0, result.output
     assert json.loads(result.output) == [
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.FUNC1(a string default 'default value', b variant)",
+            "object": "MockDatabase.MockSchema.func1(a string default 'default value', b variant)",
             "status": "packages updated",
             "type": "function",
         }
     ]
     assert queries == [
-        "create stage if not exists MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT comment='deployments managed by Snowflake CLI'",
-        f"put file://{Path(project_dir).resolve()}/app.zip @MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project auto_compress=false parallel=4 overwrite=True",
+        "create stage if not exists MockDatabase.MockSchema.dev_deployment comment='deployments managed by Snowflake CLI'",
+        f"put file://{Path(project_dir).resolve()}/app.zip @MockDatabase.MockSchema.dev_deployment/my_snowpark_project auto_compress=false parallel=4 overwrite=True",
     ]
 
 
 @mock.patch("snowflake.connector.connect")
 def test_deploy_function_needs_update_because_packages_changes(
     mock_connector,
     runner,
@@ -188,29 +189,29 @@
         project_directory,
         "--replace",
     )
 
     assert result.exit_code == 0, result.output
     assert json.loads(result.output) == [
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.FUNC1(a string default 'default value', b variant)",
+            "object": "MockDatabase.MockSchema.func1(a string default 'default value', b variant)",
             "status": "definition updated",
             "type": "function",
         }
     ]
     assert queries == [
-        "create stage if not exists MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT comment='deployments managed by Snowflake CLI'",
-        f"put file://{Path(project_dir).resolve()}/app.zip @MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project auto_compress=false parallel=4 overwrite=True",
+        "create stage if not exists MockDatabase.MockSchema.dev_deployment comment='deployments managed by Snowflake CLI'",
+        f"put file://{Path(project_dir).resolve()}/app.zip @MockDatabase.MockSchema.dev_deployment/my_snowpark_project auto_compress=false parallel=4 overwrite=True",
         dedent(
             """\
-            create or replace function MOCKDATABASE.MOCKSCHEMA.FUNC1(a string default 'default value', b variant)
+            create or replace function MockDatabase.MockSchema.func1(a string default 'default value', b variant)
             returns string
             language python
             runtime_version=3.10
-            imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
+            imports=('@MockDatabase.MockSchema.dev_deployment/my_snowpark_project/app.zip')
             handler='app.func1_handler'
             packages=('foo==1.2.3','bar>=3.0.0')
             """
         ).strip(),
     ]
 
 
@@ -237,30 +238,30 @@
         project_directory,
         "--replace",
     )
 
     assert result.exit_code == 0, result.output
     assert json.loads(result.output) == [
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.FUNC1(a string default 'default value', b variant)",
+            "object": "MockDatabase.MockSchema.func1(a string default 'default value', b variant)",
             "status": "definition updated",
             "type": "function",
         }
     ]
     assert queries == [
-        "create stage if not exists MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT comment='deployments managed by Snowflake CLI'",
-        f"put file://{Path(project_dir).resolve()}/app.zip @MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project"
+        "create stage if not exists MockDatabase.MockSchema.dev_deployment comment='deployments managed by Snowflake CLI'",
+        f"put file://{Path(project_dir).resolve()}/app.zip @MockDatabase.MockSchema.dev_deployment/my_snowpark_project"
         f" auto_compress=false parallel=4 overwrite=True",
         dedent(
             """\
-            create or replace function MOCKDATABASE.MOCKSCHEMA.FUNC1(a string default 'default value', b variant)
+            create or replace function MockDatabase.MockSchema.func1(a string default 'default value', b variant)
             returns string
             language python
             runtime_version=3.10
-            imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
+            imports=('@MockDatabase.MockSchema.dev_deployment/my_snowpark_project/app.zip')
             handler='app.func1_handler'
             packages=('foo==1.2.3','bar>=3.0.0')
             """
         ).strip(),
     ]
 
 
@@ -352,7 +353,32 @@
                     "--format",
                     "json",
                     *args,
                 ]
             )
     queries = ctx.get_queries()
     return queries, result, temp_dir
+
+
+@mock.patch("snowflake.connector.connect")
+@pytest.mark.parametrize(
+    "command, parameters",
+    [
+        ("list", []),
+        ("list", ["--like", "PATTERN"]),
+        ("describe", ["NAME"]),
+        ("drop", ["NAME"]),
+    ],
+)
+def test_command_aliases(mock_connector, runner, mock_ctx, command, parameters):
+    ctx = mock_ctx()
+    mock_connector.return_value = ctx
+
+    result = runner.invoke(["object", command, "function", *parameters])
+    assert result.exit_code == 0, result.output
+    result = runner.invoke(
+        ["snowpark", command, "function", *parameters], catch_exceptions=False
+    )
+    assert result.exit_code == 0, result.output
+
+    queries = ctx.get_queries()
+    assert queries[0] == queries[1]
```

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/test_models.py` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_models.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/test_package.py` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_package.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         self,
         mock_pip_wheel,
         mock_download,
         caplog,
         temp_dir,
         runner,
         extra_flags,
+        mock_available_packages_sql_result,
     ) -> None:
         mock_pip_wheel.return_value = 9
 
         mock_download.return_value = DownloadUnavailablePackagesResult(
             succeeded=True,
             anaconda_packages=[Requirement.parse("in-anaconda-package>=2")],
         )
@@ -136,25 +137,29 @@
             ["--yes"],
             ["--pypi-download", "-y"],
         ],
     )
     @patch(
         "snowflake.cli.plugins.snowpark.package.commands.AnacondaPackagesManager.find_packages_available_in_snowflake_anaconda"
     )
-    def test_lookup_install_flag_are_deprecated(self, _, flags, runner):
+    def test_lookup_install_flag_are_deprecated(
+        self, _, flags, runner, mock_available_packages_sql_result
+    ):
         result = runner.invoke(["snowpark", "package", "lookup", "foo", *flags])
         assert (
             "is deprecated. Lookup command no longer checks for package in PyPi"
             in result.output
         )
 
     @patch(
         "snowflake.cli.plugins.snowpark.package.commands.AnacondaPackagesManager.find_packages_available_in_snowflake_anaconda"
     )
-    def test_lookup_install_without_flags_does_not_warn(self, _, runner):
+    def test_lookup_install_without_flags_does_not_warn(
+        self, _, runner, mock_available_packages_sql_result
+    ):
         result = runner.invoke(["snowpark", "package", "lookup", "foo"])
         assert (
             "is deprecated. Lookup command no longer checks for package in PyPi"
             not in result.output
         )
 
     @pytest.mark.parametrize(
@@ -170,15 +175,21 @@
         "snowflake.cli.plugins.snowpark.package.commands.download_unavailable_packages"
     )
     @mock.patch("snowflake.cli.plugins.snowpark.package.commands.zip_dir")
     @mock.patch(
         "snowflake.cli.plugins.snowpark.package.commands.get_package_name_from_pip_wheel"
     )
     def test_create_install_flag_are_deprecated(
-        self, _mock_pip_wheel, _mock_zip, _mock_download, flags, runner
+        self,
+        _mock_pip_wheel,
+        _mock_zip,
+        _mock_download,
+        flags,
+        runner,
+        mock_available_packages_sql_result,
     ):
         result = runner.invoke(["snowpark", "package", "create", "foo", *flags])
         assert (
             "is deprecated. Create command always checks for package in PyPi."
             in result.output
         )
 
@@ -194,28 +205,39 @@
         "snowflake.cli.plugins.snowpark.package.commands.download_unavailable_packages"
     )
     @mock.patch("snowflake.cli.plugins.snowpark.package.commands.zip_dir")
     @mock.patch(
         "snowflake.cli.plugins.snowpark.package.commands.get_package_name_from_pip_wheel"
     )
     def test_create_deprecated_flags_throw_warning(
-        self, _mock_pip_wheel, _mock_zip, _mock_download, flags, runner
+        self,
+        _mock_pip_wheel,
+        _mock_zip,
+        _mock_download,
+        flags,
+        runner,
+        mock_available_packages_sql_result,
     ):
         result = runner.invoke(["snowpark", "package", "create", "foo", *flags])
         assert "is deprecated." in result.output
 
     @mock.patch(
         "snowflake.cli.plugins.snowpark.package.commands.download_unavailable_packages"
     )
     @mock.patch("snowflake.cli.plugins.snowpark.package.commands.zip_dir")
     @mock.patch(
         "snowflake.cli.plugins.snowpark.package.commands.get_package_name_from_pip_wheel"
     )
     def test_create_without_flags_does_not_warn(
-        self, _mock_pip_wheel, _mock_zip, _mock_download, runner
+        self,
+        _mock_pip_wheel,
+        _mock_zip,
+        _mock_download,
+        runner,
+        mock_available_packages_sql_result,
     ):
         result = runner.invoke(["snowpark", "package", "create", "foo"])
         assert "is deprecated" not in result.output
 
     @staticmethod
     def mocked_anaconda_response(response: dict):
         mock_response = MagicMock()
```

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/test_procedure.py` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/test_procedure.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 from unittest.mock import call
 
+import pytest
 from snowflake.cli.api.constants import ObjectType
 from snowflake.connector import ProgrammingError
 
 
 def test_deploy_function_no_procedure(runner, project_directory):
     with project_directory("empty_project"):
         result = runner.invoke(
@@ -48,34 +49,34 @@
     mock_om_describe.return_value(
         [
             call(object_type=str(ObjectType.PROCEDURE), name="procedureName(string)"),
             call(object_type=str(ObjectType.PROCEDURE), name="test()"),
         ]
     )
     assert ctx.get_queries() == [
-        "create stage if not exists MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT comment='deployments managed by Snowflake CLI'",
-        f"put file://{Path(tmp).resolve()}/app.zip @MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project auto_compress=false parallel=4 overwrite=True",
+        "create stage if not exists MockDatabase.MockSchema.dev_deployment comment='deployments managed by Snowflake CLI'",
+        f"put file://{Path(tmp).resolve()}/app.zip @MockDatabase.MockSchema.dev_deployment/my_snowpark_project auto_compress=false parallel=4 overwrite=True",
         dedent(
             """\
-            create or replace procedure MOCKDATABASE.MOCKSCHEMA.PROCEDURENAME(name string)
+            create or replace procedure MockDatabase.MockSchema.procedureName(name string)
             returns string
             language python
             runtime_version=3.8
-            imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
+            imports=('@MockDatabase.MockSchema.dev_deployment/my_snowpark_project/app.zip')
             handler='hello'
             packages=()
             """
         ).strip(),
         dedent(
             """\
-            create or replace procedure MOCKDATABASE.MOCKSCHEMA.TEST()
+            create or replace procedure MockDatabase.MockSchema.test()
             returns string
             language python
             runtime_version=3.10
-            imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
+            imports=('@MockDatabase.MockSchema.dev_deployment/my_snowpark_project/app.zip')
             handler='test'
             packages=()
             """
         ).strip(),
     ]
 
 
@@ -108,29 +109,29 @@
         )
 
     assert result.exit_code == 0, result.output
     mock_om_describe.assert_has_calls(
         [
             call(
                 object_type=str(ObjectType.PROCEDURE),
-                name="MOCKDATABASE.MOCKSCHEMA.PROCEDURENAME(string)",
+                name="MockDatabase.MockSchema.procedureName(string)",
             ),
         ]
     )
     assert ctx.get_queries() == [
-        "create stage if not exists MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT comment='deployments managed by Snowflake CLI'",
-        f"put file://{Path(project_dir).resolve()}/app.zip @MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project"
+        "create stage if not exists MockDatabase.MockSchema.dev_deployment comment='deployments managed by Snowflake CLI'",
+        f"put file://{Path(project_dir).resolve()}/app.zip @MockDatabase.MockSchema.dev_deployment/my_snowpark_project"
         f" auto_compress=false parallel=4 overwrite=True",
         dedent(
             """\
-            create or replace procedure MOCKDATABASE.MOCKSCHEMA.PROCEDURENAME(name string)
+            create or replace procedure MockDatabase.MockSchema.procedureName(name string)
             returns string
             language python
             runtime_version=3.8
-            imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
+            imports=('@MockDatabase.MockSchema.dev_deployment/my_snowpark_project/app.zip')
             handler='app.hello'
             packages=()
             external_access_integrations=(external_1,external_2)
             secrets=('cred'=cred_name,'other'=other_name)
             """
         ).strip(),
     ]
@@ -250,43 +251,43 @@
 ):
     mock_om_describe.side_effect = [
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "hello"),
                 ("returns", "string"),
-                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
+                ("imports", "dev_deployment/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "test"),
                 ("returns", "string"),
-                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
+                ("imports", "dev_deployment/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
     ]
     ctx = mock_ctx()
     mock_conn.return_value = ctx
 
     with project_directory("snowpark_procedures"):
         result = runner.invoke(["snowpark", "deploy", "--replace", "--format", "json"])
 
     assert result.exit_code == 0, result.output
     assert json.loads(result.output) == [
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.PROCEDURENAME(name string)",
+            "object": "MockDatabase.MockSchema.procedureName(name string)",
             "status": "packages updated",
             "type": "procedure",
         },
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.TEST()",
+            "object": "MockDatabase.MockSchema.test()",
             "status": "packages updated",
             "type": "procedure",
         },
     ]
 
 
 @mock.patch("snowflake.connector.connect")
@@ -303,43 +304,43 @@
 ):
     mock_om_describe.side_effect = [
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "hello"),
                 ("returns", "string"),
-                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
+                ("imports", "dev_deployment/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "foo"),
                 ("returns", "string"),
-                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
+                ("imports", "dev_deployment/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
     ]
     ctx = mock_ctx()
     mock_conn.return_value = ctx
 
     with project_directory("snowpark_procedures"):
         result = runner.invoke(["snowpark", "deploy", "--replace", "--format", "json"])
 
     assert result.exit_code == 0
     assert json.loads(result.output) == [
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.PROCEDURENAME(name string)",
+            "object": "MockDatabase.MockSchema.procedureName(name string)",
             "status": "packages updated",
             "type": "procedure",
         },
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.TEST()",
+            "object": "MockDatabase.MockSchema.test()",
             "status": "definition updated",
             "type": "procedure",
         },
     ]
 
 
 @mock.patch("snowflake.connector.connect")
@@ -356,35 +357,35 @@
 ):
     mock_om_describe.side_effect = [
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "hello"),
                 ("returns", "string"),
-                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
+                ("imports", "dev_deployment/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
         ProgrammingError("does not exist or not authorized"),
     ]
     ctx = mock_ctx()
     mock_conn.return_value = ctx
 
     with project_directory("snowpark_procedures"):
         result = runner.invoke(["snowpark", "deploy", "--replace", "--format", "json"])
 
     assert result.exit_code == 0
     assert json.loads(result.output) == [
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.PROCEDURENAME(name string)",
+            "object": "MockDatabase.MockSchema.procedureName(name string)",
             "status": "packages updated",
             "type": "procedure",
         },
         {
-            "object": "MOCKDATABASE.MOCKSCHEMA.TEST()",
+            "object": "MockDatabase.MockSchema.test()",
             "status": "created",
             "type": "procedure",
         },
     ]
 
 
 @mock.patch("snowflake.connector.connect")
@@ -450,7 +451,32 @@
     "snowflake.cli.api.commands.project_initialisation._create_project_template"
 )
 def test_init_procedure(mock_create_project_template, runner, temp_dir):
     runner.invoke(["snowpark", "init", "my_project2"])
     mock_create_project_template.assert_called_once_with(
         "default_snowpark", project_directory="my_project2"
     )
+
+
+@mock.patch("snowflake.connector.connect")
+@pytest.mark.parametrize(
+    "command, parameters",
+    [
+        ("list", []),
+        ("list", ["--like", "PATTERN"]),
+        ("describe", ["NAME"]),
+        ("drop", ["NAME"]),
+    ],
+)
+def test_command_aliases(mock_connector, runner, mock_ctx, command, parameters):
+    ctx = mock_ctx()
+    mock_connector.return_value = ctx
+
+    result = runner.invoke(["object", command, "procedure", *parameters])
+    assert result.exit_code == 0, result.output
+    result = runner.invoke(
+        ["snowpark", command, "procedure", *parameters], catch_exceptions=False
+    )
+    assert result.exit_code == 0, result.output
+
+    queries = ctx.get_queries()
+    assert queries[0] == queries[1]
```

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/__snapshots__/test_function.ambr`

 * *Files 25% similar despite different names*

```diff
@@ -17,21 +17,21 @@
   '''
 # ---
 # name: test_deploy_procedure_fully_qualified_name[ok]
   '''
   +------------------------------------------------------------------------------+
   | object                                                  | type     | status  |
   |---------------------------------------------------------+----------+---------|
-  | CUSTOM_DB.CUSTOM_SCHEMA.FQN_FUNCTION(name string)       | function | created |
-  | MOCKDATABASE.CUSTOM_SCHEMA.FQN_FUNCTION_ONLY_SCHEMA(nam | function | created |
+  | custom_db.custom_schema.fqn_function(name string)       | function | created |
+  | MockDatabase.custom_schema.fqn_function_only_schema(nam | function | created |
   | e string)                                               |          |         |
-  | MOCKDATABASE.CUSTOM_SCHEMA.SCHEMA_FUNCTION(name string) | function | created |
-  | CUSTOM_DB.MOCKSCHEMA.DATABASE_FUNCTION(name string)     | function | created |
-  | CUSTOM_DB.CUSTOM_SCHEMA.DATABASE_FUNCTION(name string)  | function | created |
-  | CUSTOM_DATABASE.CUSTOM_SCHEMA.FQN_FUNCTION3(name        | function | created |
+  | MockDatabase.custom_schema.schema_function(name string) | function | created |
+  | custom_db.MockSchema.database_function(name string)     | function | created |
+  | custom_db.custom_schema.database_function(name string)  | function | created |
+  | custom_database.custom_schema.fqn_function3(name        | function | created |
   | string)                                                 |          |         |
   +------------------------------------------------------------------------------+
   
   '''
 # ---
 # name: test_deploy_procedure_fully_qualified_name[schema error]
   '''
```

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_package.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/__snapshots__/test_package.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_procedure.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr`

 * *Files 21% similar despite different names*

```diff
@@ -8,16 +8,16 @@
   
   '''
 # ---
 # name: test_deploy_procedure_fails_if_object_exists_and_no_replace
   '''
   ╭─ Error ──────────────────────────────────────────────────────────────────────╮
   │ Following objects already exists. Consider using --replace.                  │
-  │ procedure: MOCKDATABASE.MOCKSCHEMA.PROCEDURENAME(string)                     │
-  │ procedure: MOCKDATABASE.MOCKSCHEMA.TEST()                                    │
+  │ procedure: MockDatabase.MockSchema.procedureName(string)                     │
+  │ procedure: MockDatabase.MockSchema.test()                                    │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   '''
 # ---
 # name: test_deploy_procedure_fully_qualified_name[database error]
   '''
   ╭─ Error ──────────────────────────────────────────────────────────────────────╮
@@ -28,23 +28,23 @@
   '''
 # ---
 # name: test_deploy_procedure_fully_qualified_name[ok]
   '''
   +------------------------------------------------------------------------------+
   | object                                                 | type      | status  |
   |--------------------------------------------------------+-----------+---------|
-  | CUSTOM_DB.CUSTOM_SCHEMA.FQN_PROCEDURE(name string)     | procedure | created |
-  | MOCKDATABASE.CUSTOM_SCHEMA.FQN_PROCEDURE_ONLY_SCHEMA(n | procedure | created |
+  | custom_db.custom_schema.fqn_procedure(name string)     | procedure | created |
+  | MockDatabase.custom_schema.fqn_procedure_only_schema(n | procedure | created |
   | ame string)                                            |           |         |
-  | MOCKDATABASE.CUSTOM_SCHEMA.SCHEMA_PROCEDURE(name       | procedure | created |
+  | MockDatabase.custom_schema.schema_procedure(name       | procedure | created |
   | string)                                                |           |         |
-  | CUSTOM_DB.MOCKSCHEMA.DATABASE_PROCEDURE(name string)   | procedure | created |
-  | CUSTOM_DB.CUSTOM_SCHEMA.DATABASE_PROCEDURE(name        | procedure | created |
+  | custom_db.MockSchema.database_procedure(name string)   | procedure | created |
+  | custom_db.custom_schema.database_procedure(name        | procedure | created |
   | string)                                                |           |         |
-  | CUSTOM_DATABASE.CUSTOM_SCHEMA.FQN_PROCEDURE3(name      | procedure | created |
+  | custom_database.custom_schema.fqn_procedure3(name      | procedure | created |
   | string)                                                |           |         |
   +------------------------------------------------------------------------------+
   
   '''
 # ---
 # name: test_deploy_procedure_fully_qualified_name[schema error]
   '''
```

### Comparing `snowflake_cli_labs-2.3.1/tests/spcs/test_common.py` & `snowflake_cli_labs-2.4.0rc0/tests/spcs/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.4.0rc0/tests/spcs/test_compute_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -474,7 +474,32 @@
 @patch("snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.status")
 def test_status_cli(mock_status, mock_statement_success, runner):
     pool_name = "test_pool"
     mock_status.return_value = mock_statement_success()
     result = runner.invoke(["spcs", "compute-pool", "status", pool_name])
     mock_status.assert_called_once_with(pool_name=pool_name)
     assert_that_result_is_successful_and_executed_successfully(result)
+
+
+@patch("snowflake.connector.connect")
+@pytest.mark.parametrize(
+    "command, parameters",
+    [
+        ("list", []),
+        ("list", ["--like", "PATTERN"]),
+        ("describe", ["NAME"]),
+        ("drop", ["NAME"]),
+    ],
+)
+def test_command_aliases(mock_connector, runner, mock_ctx, command, parameters):
+    ctx = mock_ctx()
+    mock_connector.return_value = ctx
+
+    result = runner.invoke(["object", command, "compute-pool", *parameters])
+    assert result.exit_code == 0, result.output
+    result = runner.invoke(
+        ["spcs", "compute-pool", command, *parameters], catch_exceptions=False
+    )
+    assert result.exit_code == 0, result.output
+
+    queries = ctx.get_queries()
+    assert queries[0] == queries[1]
```

### Comparing `snowflake_cli_labs-2.3.1/tests/spcs/test_image_repository.py` & `snowflake_cli_labs-2.4.0rc0/tests/spcs/test_image_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -291,7 +291,31 @@
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager._conn"
 )
 def test_get_repository_url_no_schema_provided(mock_conn):
     mock_conn.database = "DB"
     mock_conn.schema = None
     with pytest.raises(SchemaNotProvidedError):
         ImageRepositoryManager().get_repository_url("IMAGES")
+
+
+@mock.patch("snowflake.connector.connect")
+@pytest.mark.parametrize(
+    "command, parameters",
+    [
+        ("list", []),
+        ("list", ["--like", "PATTERN"]),
+        ("drop", ["NAME"]),
+    ],
+)
+def test_command_aliases(mock_connector, runner, mock_ctx, command, parameters):
+    ctx = mock_ctx()
+    mock_connector.return_value = ctx
+
+    result = runner.invoke(["object", command, "image-repository", *parameters])
+    assert result.exit_code == 0, result.output
+    result = runner.invoke(
+        ["spcs", "image-repository", command, *parameters], catch_exceptions=False
+    )
+    assert result.exit_code == 0, result.output
+
+    queries = ctx.get_queries()
+    assert queries[0] == queries[1]
```

### Comparing `snowflake_cli_labs-2.3.1/tests/spcs/test_jobs.py` & `snowflake_cli_labs-2.4.0rc0/tests/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/spcs/test_registry.py` & `snowflake_cli_labs-2.4.0rc0/tests/spcs/test_registry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/spcs/test_services.py` & `snowflake_cli_labs-2.4.0rc0/tests/spcs/test_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -619,7 +619,32 @@
 @patch("snowflake.cli.plugins.spcs.services.commands.is_valid_object_name")
 def test_service_name_parser_invalid_object_name(mock_is_valid_object_name):
     invalid_service_name = "account.db.schema.test_service"
     mock_is_valid_object_name.return_value = False
     with pytest.raises(ClickException) as e:
         _service_name_callback(invalid_service_name)
     assert f"'{invalid_service_name}' is not a valid service name." in e.value.message
+
+
+@patch("snowflake.connector.connect")
+@pytest.mark.parametrize(
+    "command, parameters",
+    [
+        ("list", []),
+        ("list", ["--like", "PATTERN"]),
+        ("describe", ["NAME"]),
+        ("drop", ["NAME"]),
+    ],
+)
+def test_command_aliases(mock_connector, runner, mock_ctx, command, parameters):
+    ctx = mock_ctx()
+    mock_connector.return_value = ctx
+
+    result = runner.invoke(["object", command, "service", *parameters])
+    assert result.exit_code == 0, result.output
+    result = runner.invoke(
+        ["spcs", "service", command, *parameters], catch_exceptions=False
+    )
+    assert result.exit_code == 0, result.output
+
+    queries = ctx.get_queries()
+    assert queries[0] == queries[1]
```

### Comparing `snowflake_cli_labs-2.3.1/tests/spcs/__snapshots__/test_image_repository.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/spcs/__snapshots__/test_registry.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/spcs/__snapshots__/test_registry.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/stage/test_diff.py` & `snowflake_cli_labs-2.4.0rc0/tests/stage/test_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import hashlib
 import typing
 from pathlib import Path
 from typing import Dict, List, Union
 from unittest import mock
 
 import pytest
```

### Comparing `snowflake_cli_labs-2.3.1/tests/stage/test_stage.py` & `snowflake_cli_labs-2.4.0rc0/tests/stage/test_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -898,7 +898,30 @@
     assert result.output == snapshot
     assert mock_execute.mock_calls == [
         mock.call("ls @exe", cursor_class=DictCursor),
         mock.call(f"execute immediate from @exe/s1.sql"),
         mock.call(f"execute immediate from @exe/s2.sql"),
         mock.call(f"execute immediate from @exe/s3.sql"),
     ]
+
+
+@mock.patch("snowflake.connector.connect")
+@pytest.mark.parametrize(
+    "command, parameters",
+    [
+        ("list", []),
+        ("list", ["--like", "PATTERN"]),
+        ("describe", ["NAME"]),
+        ("drop", ["NAME"]),
+    ],
+)
+def test_command_aliases(mock_connector, runner, mock_ctx, command, parameters):
+    ctx = mock_ctx()
+    mock_connector.return_value = ctx
+
+    result = runner.invoke(["object", command, "stage", *parameters])
+    assert result.exit_code == 0, result.output
+    result = runner.invoke(["stage", command, *parameters], catch_exceptions=False)
+    assert result.exit_code == 0, result.output
+
+    queries = ctx.get_queries()
+    assert queries[0] == queries[1]
```

### Comparing `snowflake_cli_labs-2.3.1/tests/stage/__snapshots__/test_stage.ambr` & `snowflake_cli_labs-2.4.0rc0/tests/stage/__snapshots__/test_stage.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/streamlit/test_config.py` & `snowflake_cli_labs-2.4.0rc0/tests/streamlit/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/anaconda_channel_data.json` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/anaconda_channel_data.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/packages_available_in_snowflake_sql_result_rows.json` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/test_data.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/app/manifest.yml` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/app/manifest.yml` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/integration_external/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/app.zip` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/app.zip` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_functions/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/app.zip` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/app.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/app.zip` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/app.py` & `snowflake_cli_labs-2.4.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests/testing_utils/files_and_dirs.py` & `snowflake_cli_labs-2.4.0rc0/tests/testing_utils/files_and_dirs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import os
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Dict, Generator, List, Union
+from typing import Dict, Generator, List, Optional, Union
 
 from snowflake.cli.api.secure_utils import file_permissions_are_strict
 
 
 def create_temp_file(suffix: str, dir_name: str, contents: List[str]) -> str:
     with tempfile.NamedTemporaryFile(suffix=suffix, dir=dir_name, delete=False) as tmp:
         _write_to_file(tmp.name, contents)
@@ -26,28 +28,43 @@
 
 
 def assert_file_permissions_are_strict(file_path: Path) -> None:
     assert file_permissions_are_strict(file_path)
 
 
 @contextmanager
-def temp_local_dir(files: Dict[str, Union[str, bytes]]) -> Generator[Path, None, None]:
+def temp_local_dir(
+    dir_structure: Dict[str, Optional[Union[str, bytes]]]
+) -> Generator[Path, None, None]:
     """
     Creates a temporary local directory structure from a dictionary
     of local paths and their file contents (either strings to be encoded
     as UTF-8, or binary bytes).
+
+    Parameters:
+     dir_structure (Dict[str, Optional[Union[str, bytes]]]): A dictionary of file or directory names along with their contents.
+        For creating a file, 'contents' must be a string, empty or otherwise.
+        For creating a directory, 'contents' must be set to None.
     """
     with tempfile.TemporaryDirectory() as tmpdir:
-        for relpath, contents in files.items():
+        for relpath, contents in dir_structure.items():
             path = Path(tmpdir, relpath)
-            path.parent.mkdir(parents=True, exist_ok=True)
-            mode = "wb" if isinstance(contents, bytes) else "w"
-            encoding = None if isinstance(contents, bytes) else "UTF-8"
-            with open(path, mode=mode, encoding=encoding) as fh:
-                fh.write(contents)
+            is_directory = contents is None
+            if is_directory:
+                path.mkdir(parents=True, exist_ok=True)
+            else:
+                path.parent.mkdir(parents=True, exist_ok=True)
+                if contents is None:
+                    f = open(path, "x")
+                    f.close()
+                else:
+                    mode = "wb" if isinstance(contents, bytes) else "w"
+                    encoding = None if isinstance(contents, bytes) else "UTF-8"
+                    with open(path, mode=mode, encoding=encoding) as fh:
+                        fh.write(contents)
 
         yield Path(tmpdir)
 
 
 def merge_left(target: Dict, source: Dict) -> None:
     """
     Recursively merges key/value pairs from source into target.
```

### Comparing `snowflake_cli_labs-2.3.1/tests/testing_utils/fixtures.py` & `snowflake_cli_labs-2.4.0rc0/tests/testing_utils/fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+from __future__ import annotations
+
 import functools
 import importlib
 import os
 import shutil
 import sys
 import tempfile
 from contextlib import contextmanager
 from io import StringIO
 from pathlib import Path
-from typing import Generator, List, NamedTuple, Optional, Union
+from typing import Any, Dict, Generator, List, NamedTuple, Optional, Union
 from unittest import mock
 
 import pytest
 import yaml
 from snowflake.cli.api.project.schemas.project_definition import ProjectDefinition
 from snowflake.cli.api.project.schemas.snowpark.argument import Argument
 from snowflake.cli.api.project.schemas.snowpark.callable import FunctionSchema
 from snowflake.cli.app.cli_app import app_factory
+from snowflake.cli.plugins.nativeapp.codegen.snowpark.models import (
+    NativeAppExtensionFunction,
+)
 from snowflake.connector.cursor import SnowflakeCursor
 from snowflake.connector.errors import ProgrammingError
 from typer import Typer
 from typer.testing import CliRunner
 
 from tests.test_data import test_data
 from tests.testing_utils.files_and_dirs import (
@@ -334,7 +339,34 @@
                     "scripts": [
                         "package/001.sql",
                     ]
                 },
             },
         }
     )
+
+
+@pytest.fixture
+def native_app_extension_function_raw_data() -> Dict[str, Any]:
+    return {
+        "type": "procedure",
+        "lineno": 42,
+        "name": "my_function",
+        "signature": [{"name": "first", "type": "int", "default": "42"}],
+        "returns": "int",
+        "runtime": "3.11",
+        "handler": "my_function_handler",
+        "external_access_integrations": ["integration_one", "integration_two"],
+        "secrets": {"key1": "secret_one", "key2": "integration_two"},
+        "packages": ["package_one==1.0.2", "package_two"],
+        "imports": ["/path/to/import1.py", "/path/to/import2.zip"],
+        "execute_as_caller": False,
+        "schema": "DATA",
+        "application_roles": ["APP_ADMIN", "APP_VIEWER"],
+    }
+
+
+@pytest.fixture
+def native_app_extension_function(
+    native_app_extension_function_raw_data,
+) -> NativeAppExtensionFunction:
+    return NativeAppExtensionFunction(**native_app_extension_function_raw_data)
```

### Comparing `snowflake_cli_labs-2.3.1/tests_e2e/conftest.py` & `snowflake_cli_labs-2.4.0rc0/tests_e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_e2e/test_error_handling.py` & `snowflake_cli_labs-2.4.0rc0/tests_e2e/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_e2e/test_installation.py` & `snowflake_cli_labs-2.4.0rc0/tests_e2e/test_installation.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     output = subprocess.check_output(
         [
             snowcli,
             "--config-file",
             test_root_path / "config" / "config.toml",
             "sql",
             "-q",
-            "select ln(10)",
+            "select round(ln(10), 2)",
             "-c",
             "integration",
         ],
         encoding="utf-8",
     )
     snapshot.assert_match(output)
```

### Comparing `snowflake_cli_labs-2.3.1/tests_e2e/test_snowpark_examples.py` & `snowflake_cli_labs-2.4.0rc0/tests_e2e/test_snowpark_examples.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_e2e/__snapshots__/test_installation.ambr` & `snowflake_cli_labs-2.4.0rc0/tests_e2e/__snapshots__/test_installation.ambr`

 * *Files 20% similar despite different names*

```diff
@@ -13,24 +13,31 @@
   '''
                                                                                   
    Usage: snow [OPTIONS] COMMAND [ARGS]...                                        
                                                                                   
    Snowflake CLI tool for developers.                                             
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --version                    Shows version of the Snowflake CLI              │
-  │ --info                       Shows information about the Snowflake CLI       │
-  │ --config-file          FILE  Specifies Snowflake CLI configuration file that │
-  │                              should be used                                  │
-  │                              [default: None]                                 │
-  │ --help         -h            Show this message and exit.                     │
+  │ --version                           Shows version of the Snowflake CLI       │
+  │ --info                              Shows information about the Snowflake    │
+  │                                     CLI                                      │
+  │ --config-file                 FILE  Specifies Snowflake CLI configuration    │
+  │                                     file that should be used                 │
+  │                                     [default: None]                          │
+  │ --install-completion                Install completion for the current       │
+  │                                     shell.                                   │
+  │ --show-completion                   Show completion for the current shell,   │
+  │                                     to copy it or customize the              │
+  │                                     installation.                            │
+  │ --help                -h            Show this message and exit.              │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
   │ app          Manages a Snowflake Native App                                  │
   │ connection   Manages connections to Snowflake.                               │
+  │ cortex       Provides access to Snowflake Cortex.                            │
   │ git          Manages git repositories in Snowflake.                          │
   │ object       Manages Snowflake objects like warehouses and stages            │
   │ snowpark     Manages procedures and functions.                               │
   │ spcs         Manages Snowpark Container Services compute pools, services,    │
   │              image registries, and image repositories.                       │
   │ sql          Executes Snowflake query.                                       │
   │ stage        Manages stages.                                                 │
@@ -38,20 +45,20 @@
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_snow_sql
   '''
-  select ln(10)
-  +-------------------+
-  | LN(10)            |
-  |-------------------|
-  | 2.302585092994046 |
-  +-------------------+
+  select round(ln(10), 2)
+  +------------------+
+  | ROUND(LN(10), 2) |
+  |------------------|
+  | 2.3              |
+  +------------------+
   
   '''
 # ---
 # name: test_snow_streamlit_init
   '''
   Initialized the new project in streamlit_test/
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/conftest.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,17 @@
             ],
             **kwargs,
         )
 
         if result.output == "" or result.output.strip() == "Done":
             return CommandResult(result.exit_code, json=[])
         try:
-            return CommandResult(result.exit_code, json.loads(result.output))
+            return CommandResult(
+                result.exit_code, json.loads(result.output), output=result.output
+            )
         except JSONDecodeError:
             return CommandResult(result.exit_code, output=result.output)
 
     def invoke_json(self, args, **kwargs) -> CommandResult:
         return self.invoke_with_config([*args, "--format", "JSON"], **kwargs)
 
     def invoke_with_connection_json(
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/snowflake_connector.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/snowflake_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import os
 import uuid
+from contextlib import contextmanager
+from unittest import mock
 
 import pytest
 from snowflake import connector
 from snowflake.cli.api.exceptions import EnvironmentVariableNotFoundError
-from contextlib import contextmanager
-from unittest import mock
 
 _ENV_PARAMETER_PREFIX = "SNOWFLAKE_CONNECTIONS_INTEGRATION"
 SCHEMA_ENV_PARAMETER = f"{_ENV_PARAMETER_PREFIX}_SCHEMA"
 DATABASE_ENV_PARAMETER = f"{_ENV_PARAMETER_PREFIX}_DATABASE"
 
 
 def add_uuid_to_name(name: str) -> str:
@@ -75,14 +75,16 @@
 def snowflake_session():
     config = {
         "application": "INTEGRATION_TEST",
         "account": _get_from_env("ACCOUNT"),
         "user": _get_from_env("USER"),
         "password": _get_from_env("PASSWORD"),
         "host": _get_from_env("HOST", allow_none=True),
+        "warehouse": _get_from_env("WAREHOUSE", allow_none=True),
+        "role": _get_from_env("ROLE", allow_none=True),
     }
     config = {k: v for k, v in config.items() if v is not None}
     connection = connector.connect(**config)
     yield connection
     connection.close()
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_config.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_connection.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_external_plugins.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_external_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_git.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_git.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_object.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import pytest
 
 from tests_integration.test_utils import row_from_cursor
 from tests_integration.testing_utils.naming_utils import ObjectNameProvider
 
 
 @pytest.mark.integration
-@pytest.mark.parametrize("object_type", ["warehouse", "schema"])
-def test_show(object_type, runner, test_database, snowflake_session):
+@pytest.mark.parametrize(
+    "object_type,plural_object_type",
+    [
+        ("warehouse", "warehouses"),
+        ("schema", "schemas"),
+        ("external-access-integration", "external access integrations"),
+    ],
+)
+def test_show(
+    object_type, plural_object_type, runner, test_database, snowflake_session
+):
     result = runner.invoke_with_connection_json(
         ["object", "list", object_type, "--format", "json"]
     )
 
-    curr = snowflake_session.execute_string(f"show {object_type}s")
+    curr = snowflake_session.execute_string(f"show {plural_object_type}")
     expected = row_from_cursor(curr[-1])
 
     actual = result.json
     assert len(actual) == len(expected)
     assert actual[0].keys() == expected[0].keys()
     assert actual[0]["name"] == expected[0]["name"]
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_package.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_package.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import tempfile
 from pathlib import Path
 from typing import List
 from zipfile import ZipFile
 
 import pytest
+from pkg_resources.extern.packaging.requirements import InvalidRequirement
+
 
 from tests_integration.test_utils import contains_row_with, row_from_snowflake_session
 
 
 class TestPackage:
     STAGE_NAME = "PACKAGE_TEST"
 
@@ -48,15 +50,15 @@
             [],
             ["--ignore-anaconda"],
             ["--index-url", "https://pypi.org/simple"],
             ["--skip-version-check"],
         ],
     )
     def test_package_create_with_non_anaconda_package(
-        self, directory_for_test, runner, extra_flags
+        self, directory_for_test, runner, extra_flags, caplog
     ):
         result = runner.invoke_with_connection_json(
             [
                 "snowpark",
                 "package",
                 "create",
                 "dummy-pkg-for-tests-with-deps",
@@ -70,14 +72,20 @@
             "dummy_pkg_for_tests_with_deps.zip"
         )
         assert (
             "dummy_pkg_for_tests_with_deps/shrubbery.py"
             in self._get_filenames_from_zip("dummy_pkg_for_tests_with_deps.zip")
         )
 
+        def _assert_message_in_logs(expected_message):
+            return any(expected_message in record.message for record in caplog.records)
+
+        _assert_message_in_logs("Running pip wheel with command: %s")
+        _assert_message_in_logs("Pip wheel command executed successfully")
+
     @pytest.mark.integration
     @pytest.mark.parametrize("ignore_anaconda", (True, False))
     def test_create_package_with_deps(
         self, directory_for_test, runner, ignore_anaconda
     ):
         command = [
             "snowpark",
@@ -184,14 +192,25 @@
     def test_package_with_native_libraries(self, directory_for_test, runner):
         result = runner.invoke(
             ["snowpark", "package", "create", "numpy", "--ignore-anaconda"]
         )
         assert result.exit_code == 1
         assert "at https://support.anaconda.com/" in result.output
 
+    @pytest.mark.integration
+    def test_incorrect_input(self, runner):
+        with pytest.raises(InvalidRequirement) as err:
+            runner.invoke_with_connection(
+                ["snowpark", "package", "create", "this is incorrect"]
+            )
+        assert (
+            "Expected end or semicolon (after name and no valid version specifier)"
+            in str(err)
+        )
+
     @pytest.fixture(scope="function")
     def directory_for_test(self):
         init_dir = os.getcwd()
 
         with tempfile.TemporaryDirectory() as tmp:
             os.chdir(tmp)
             yield tmp
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_session_token.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_session_token.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_snowpark.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_snowpark.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     SnowparkTestSteps,
 )
 from tests_integration.testing_utils.snowpark_utils import (
     SnowparkTestSetup,
 )
 from typing import List
 from zipfile import ZipFile
+from pkg_resources.extern.packaging.requirements import InvalidRequirement
 
 
 STAGE_NAME = "dev_deployment"
 
 
 @pytest.mark.integration
 def test_snowpark_flow(
@@ -25,36 +26,36 @@
     database = test_database.upper()
     with project_directory("snowpark") as tmp_dir:
         _test_steps.snowpark_build_should_zip_files()
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             [
                 {
-                    "object": f"{database}.PUBLIC.HELLO_PROCEDURE(name string)",
+                    "object": f"{database}.PUBLIC.hello_procedure(name string)",
                     "status": "created",
                     "type": "procedure",
                 },
                 {
-                    "object": f"{database}.PUBLIC.TEST()",
+                    "object": f"{database}.PUBLIC.test()",
                     "status": "created",
                     "type": "procedure",
                 },
                 {
-                    "object": f"{database}.PUBLIC.HELLO_FUNCTION(name string)",
+                    "object": f"{database}.PUBLIC.hello_function(name string)",
                     "status": "created",
                     "type": "function",
                 },
             ]
         )
 
         _test_steps.assert_those_procedures_are_in_snowflake(
-            "HELLO_PROCEDURE(VARCHAR) RETURN VARCHAR"
+            "hello_procedure(VARCHAR) RETURN VARCHAR"
         )
         _test_steps.assert_those_functions_are_in_snowflake(
-            "HELLO_FUNCTION(VARCHAR) RETURN VARCHAR"
+            "hello_function(VARCHAR) RETURN VARCHAR"
         )
 
         expected_files = [
             f"{STAGE_NAME}/my_snowpark_project/app.zip",
         ]
         _test_steps.assert_that_only_these_files_are_staged_in_test_db(
             *expected_files, stage_name=STAGE_NAME
@@ -69,22 +70,22 @@
             object_type="function",
             identifier=("hello_function", "(VARCHAR) RETURN VARCHAR"),
         )
 
         # Created objects can be described
         _test_steps.object_describe_should_return_entity_description(
             object_type="procedure",
-            identifier="HELLO_PROCEDURE(VARCHAR)",
+            identifier="hello_procedure(VARCHAR)",
             signature="(NAME VARCHAR)",
             returns="VARCHAR(16777216)",
         )
 
         _test_steps.object_describe_should_return_entity_description(
             object_type="function",
-            identifier="HELLO_FUNCTION(VARCHAR)",
+            identifier="hello_function(VARCHAR)",
             signature="(NAME VARCHAR)",
             returns="VARCHAR(16777216)",
         )
 
         # Created objects can be executed
         _test_steps.snowpark_execute_should_return_expected_value(
             object_type="procedure",
@@ -116,37 +117,37 @@
         )
 
         # Now we deploy with replace flag, it should update existing objects
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             additional_arguments=["--replace"],
             expected_result=[
                 {
-                    "object": f"{database}.PUBLIC.HELLO_PROCEDURE(name string)",
+                    "object": f"{database}.PUBLIC.hello_procedure(name string)",
                     "status": "definition updated",
                     "type": "procedure",
                 },
                 {
-                    "object": f"{database}.PUBLIC.TEST()",
+                    "object": f"{database}.PUBLIC.test()",
                     "status": "packages updated",
                     "type": "procedure",
                 },
                 {
-                    "object": f"{database}.PUBLIC.HELLO_FUNCTION(name string)",
+                    "object": f"{database}.PUBLIC.hello_function(name string)",
                     "status": "definition updated",
                     "type": "function",
                 },
             ],
         )
 
         # Check if objects were updated
         _test_steps.assert_those_procedures_are_in_snowflake(
-            "HELLO_PROCEDURE(VARCHAR) RETURN VARIANT"
+            "hello_procedure(VARCHAR) RETURN VARIANT"
         )
         _test_steps.assert_those_functions_are_in_snowflake(
-            "HELLO_FUNCTION(VARCHAR) RETURN VARIANT"
+            "hello_function(VARCHAR) RETURN VARIANT"
         )
 
         _test_steps.assert_that_only_these_files_are_staged_in_test_db(
             *expected_files, stage_name=STAGE_NAME
         )
 
         # Listing procedures or functions shows updated objects
@@ -186,25 +187,25 @@
             value=["@dev_deployment/dummy_pkg_for_tests.zip"],
         )
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             additional_arguments=["--replace"],
             expected_result=[
                 {
-                    "object": f"{database}.PUBLIC.HELLO_PROCEDURE(name string)",
+                    "object": f"{database}.PUBLIC.hello_procedure(name string)",
                     "status": "packages updated",
                     "type": "procedure",
                 },
                 {
-                    "object": f"{database}.PUBLIC.TEST()",
+                    "object": f"{database}.PUBLIC.test()",
                     "status": "packages updated",
                     "type": "procedure",
                 },
                 {
-                    "object": f"{database}.PUBLIC.HELLO_FUNCTION(name string)",
+                    "object": f"{database}.PUBLIC.hello_function(name string)",
                     "status": "definition updated",
                     "type": "function",
                 },
             ],
         )
 
         # Same file should be present, with addition of uploaded package
@@ -252,15 +253,15 @@
     with project_directory("snowpark_with_import") as p_dir:
 
         _test_steps.snowpark_build_should_zip_files(additional_files=[Path("app.zip")])
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             [
                 {
-                    "object": f"{test_database.upper()}.PUBLIC.TEST_FUNC(name string)",
+                    "object": f"{test_database.upper()}.PUBLIC.test_func(name string)",
                     "status": "created",
                     "type": "function",
                 },
             ]
         )
         _test_steps.snowpark_execute_should_return_expected_value(
             object_type="function",
@@ -284,15 +285,15 @@
         assert result.exit_code == 0
 
         assert "dummy_pkg_for_tests/shrubbery.py" in ZipFile("app.zip").namelist()
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             [
                 {
-                    "object": f"{test_database.upper()}.PUBLIC.TEST_FUNC(name string)",
+                    "object": f"{test_database.upper()}.PUBLIC.test_func(name string)",
                     "type": "function",
                     "status": "created",
                 }
             ]
         )
 
         _test_steps.snowpark_execute_should_return_expected_value(
@@ -319,15 +320,15 @@
         files = ZipFile("app.zip").namelist()
         assert "dummy_pkg_for_tests_with_deps/shrubbery.py" in files
         assert "dummy_pkg_for_tests/shrubbery.py" in files  # as transient dep
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             [
                 {
-                    "object": f"{test_database.upper()}.PUBLIC.TEST_FUNC(name string)",
+                    "object": f"{test_database.upper()}.PUBLIC.test_func(name string)",
                     "type": "function",
                     "status": "created",
                 }
             ]
         )
 
         _test_steps.snowpark_execute_should_return_expected_value(
@@ -361,15 +362,15 @@
         assert "dummy_pkg_for_tests_with_deps/shrubbery.py" in files
         assert "dummy_pkg_for_tests/shrubbery.py" in files  # as transient dep
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             additional_arguments=["--project", project_subpath],
             expected_result=[
                 {
-                    "object": f"{test_database.upper()}.PUBLIC.TEST_FUNC(name string)",
+                    "object": f"{test_database.upper()}.PUBLIC.test_func(name string)",
                     "type": "function",
                     "status": "created",
                 }
             ],
         )
 
         _test_steps.snowpark_execute_should_return_expected_value(
@@ -386,27 +387,27 @@
     database = test_database.upper()
     with project_directory("snowpark_with_default_values") as tmp_dir:
         _test_steps.snowpark_build_should_zip_files()
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             [
                 {
-                    "object": f"{database}.PUBLIC.WHOLE_NEW_WORD_PROCEDURE(base varchar default 'word', "
+                    "object": f"{database}.PUBLIC.whole_new_word_procedure(base varchar default 'word', "
                     "mult number default 2, suffix varchar default ', but a procedure')",
                     "type": "procedure",
                     "status": "created",
                 },
                 {
-                    "object": f"{database}.PUBLIC.WHOLE_NEW_WORD(base string default 'word', "
+                    "object": f"{database}.PUBLIC.whole_new_word(base string default 'word', "
                     "mult int default 2, suffix string default '!')",
                     "type": "function",
                     "status": "created",
                 },
                 {
-                    "object": f"{database}.PUBLIC.CHECK_ALL_TYPES("
+                    "object": f"{database}.PUBLIC.check_all_types("
                     "s string default '<str>', "
                     "i int default 7, "
                     "b1 boolean default true, "
                     "b2 boolean default True, "
                     "f float default 1.5, "
                     "l array default [1, 2, 3])",
                     "status": "created",
@@ -529,68 +530,68 @@
             parameter_path="snowpark.functions.4.database",
             value=database,
         )
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             [
                 {
-                    "object": f"{database}.{default_schema}.FQN_FUNCTION(name string)",
+                    "object": f"{database}.{default_schema}.fqn_function(name string)",
                     "status": "created",
                     "type": "function",
                 },
                 {
-                    "object": f"{database}.{different_schema}.FQN_FUNCTION2(name string)",
+                    "object": f"{database}.{different_schema}.fqn_function2(name string)",
                     "status": "created",
                     "type": "function",
                 },
                 {
-                    "object": f"{database}.{different_schema}.SCHEMA_FUNCTION(name "
+                    "object": f"{database}.{different_schema}.schema_function(name "
                     "string)",
                     "status": "created",
                     "type": "function",
                 },
                 {
-                    "object": f"{database}.{default_schema}.DATABASE_FUNCTION(name string)",
+                    "object": f"{database}.{default_schema}.database_function(name string)",
                     "status": "created",
                     "type": "function",
                 },
                 {
-                    "object": f"{database}.{different_schema}.DATABASE_SCHEMA_FUNCTION(name "
+                    "object": f"{database}.{different_schema}.database_schema_function(name "
                     "string)",
                     "status": "created",
                     "type": "function",
                 },
             ]
         )
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             [
                 {
-                    "object": f"{database}.{default_schema}.FQN_FUNCTION(name string)",
+                    "object": f"{database}.{default_schema}.fqn_function(name string)",
                     "status": "packages updated",
                     "type": "function",
                 },
                 {
-                    "object": f"{database}.{different_schema}.FQN_FUNCTION2(name string)",
+                    "object": f"{database}.{different_schema}.fqn_function2(name string)",
                     "status": "packages updated",
                     "type": "function",
                 },
                 {
-                    "object": f"{database}.{different_schema}.SCHEMA_FUNCTION(name "
+                    "object": f"{database}.{different_schema}.schema_function(name "
                     "string)",
                     "status": "packages updated",
                     "type": "function",
                 },
                 {
-                    "object": f"{database}.{default_schema}.DATABASE_FUNCTION(name string)",
+                    "object": f"{database}.{default_schema}.database_function(name string)",
                     "status": "packages updated",
                     "type": "function",
                 },
                 {
-                    "object": f"{database}.{different_schema}.DATABASE_SCHEMA_FUNCTION(name "
+                    "object": f"{database}.{different_schema}.database_schema_function(name "
                     "string)",
                     "status": "packages updated",
                     "type": "function",
                 },
             ],
             additional_arguments=["--replace"],
         )
@@ -607,15 +608,15 @@
     database = test_database.upper()
     with project_directory("snowpark_vectorized") as tmp_dir:
         _test_steps.snowpark_build_should_zip_files()
 
         _test_steps.snowpark_deploy_should_finish_successfully_and_return(
             [
                 {
-                    "object": f"{database}.PUBLIC.VECTOR_FUNC(x number(10, 5), y number(10, 5))",
+                    "object": f"{database}.PUBLIC.vector_func(x number(10, 5), y number(10, 5))",
                     "status": "created",
                     "type": "function",
                 },
             ]
         )
 
         result = snowflake_session.execute_string(
@@ -770,14 +771,28 @@
             ["snowpark", "execute", "function", "check_mypy_version()"]
         )
         assert result.exit_code == 0, result.output
         # earliest mypy 1.* version is 1.5
         assert result.json == {"CHECK_MYPY_VERSION()": "1.3.0"}
 
 
+@pytest.mark.integration
+def test_incorrect_requirements(project_directory, runner, alter_requirements_txt):
+    with project_directory("snowpark") as tmp_dir:
+        alter_requirements_txt(
+            tmp_dir / "requirements.txt", ["this is incorrect requirement"]
+        )
+        with pytest.raises(InvalidRequirement) as err:
+            runner.invoke_with_connection(["snowpark", "build"])
+        assert (
+            "Expected end or semicolon (after name and no valid version specifier)"
+            in str(err)
+        )
+
+
 @pytest.fixture
 def _test_setup(
     runner,
     sql_test_helper,
     test_database,
     temporary_working_directory,
     snapshot,
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_sql.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_sql.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,21 +20,40 @@
             "-f",
             f"{test_root_path}/test_data/sql_multi_queries.sql",
         ]
     )
 
     assert result.exit_code == 0
     assert _round_values_for_multi_queries(result.json) == [
-        [{"LN(1)": 0.00}],
-        [{"LN(10)": 2.30}],
-        [{"LN(100)": 4.61}],
+        [{"ROUND(LN(1), 4)": 0.0}],
+        [{"ROUND(LN(10), 4)": 2.3}],
+        [{"ROUND(LN(100), 4)": 4.61}],
     ]
 
 
 @pytest.mark.integration
+def test_multiple_files(runner, snowflake_session, test_root_path, snapshot):
+    query_file = f"{test_root_path}/test_data/sql_multi_queries.sql"
+    result = runner.invoke_with_connection(
+        [
+            "sql",
+            "-f",
+            query_file,
+            "-f",
+            f"{test_root_path}/test_data/empty.sql",
+            "-f",
+            query_file,
+        ]
+    )
+
+    assert result.exit_code == 0
+    assert result.output == snapshot
+
+
+@pytest.mark.integration
 def test_multi_queries_where_one_of_them_is_failing(
     runner, snowflake_session, test_root_path, snapshot
 ):
     result = runner.invoke_with_connection_json(
         ["sql", "-q", f"select 1; select 2; select foo; select 4", "--format", "json"],
         catch_exceptions=True,
     )
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_stage.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,22 @@
 
     result = runner.invoke_with_connection_json(["stage", "create", stage_name])
     assert contains_row_with(
         result.json,
         {"status": f"Stage area {stage_name.upper()} successfully created."},
     )
 
-    result = runner.invoke_with_connection_json(["object", "list", "stage"])
+    result = runner.invoke_with_connection_json(["stage", "list"])
     expect = snowflake_session.execute_string(f"show stages like '{stage_name}'")
     assert contains_row_with(result.json, row_from_snowflake_session(expect)[0])
 
+    result = runner.invoke_with_connection_json(["stage", "describe", stage_name])
+    expect = snowflake_session.execute_string(f"describe stage {stage_name}")
+    assert contains_row_with(result.json, row_from_snowflake_session(expect)[0])
+
     filename = "test.txt"
     another_filename = "another.md"
     with tempfile.TemporaryDirectory() as td:
         file_path = Path(td) / filename
         another_file_path = Path(td) / another_filename
 
         for path in [file_path, another_file_path]:
@@ -69,15 +73,15 @@
         {"name": f"{stage_name}/{filename}", "result": "removed"},
     )
     expect = snowflake_session.execute_string(f"list @{stage_name}")
     assert not_contains_row_with(
         row_from_snowflake_session(expect), {"name": f"{stage_name}/{filename}"}
     )
 
-    result = runner.invoke_with_connection_json(["object", "drop", "stage", stage_name])
+    result = runner.invoke_with_connection_json(["stage", "drop", stage_name])
     assert contains_row_with(
         result.json,
         {"status": f"{stage_name.upper()} successfully dropped."},
     )
     expect = snowflake_session.execute_string(f"show stages like '%{stage_name}%'")
     assert row_from_snowflake_session(expect) == []
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_streamlit.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_streamlit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import uuid
+from pathlib import Path
 
 import pytest
 
 from tests_integration.test_utils import (
     contains_row_with,
     row_from_snowflake_session,
     rows_from_snowflake_session,
@@ -20,24 +21,24 @@
 ):
     streamlit_name = "test_streamlit_deploy_snowcli"
 
     with project_directory("streamlit"):
         result = runner.invoke_with_connection_json(["streamlit", "deploy"])
         assert result.exit_code == 0
 
-        result = runner.invoke_with_connection_json(["object", "list", "streamlit"])
+        result = runner.invoke_with_connection_json(["streamlit", "list"])
         assert_that_result_is_successful(result)
 
         expect = snowflake_session.execute_string(
             f"show streamlits like '{streamlit_name}'"
         )
         assert contains_row_with(result.json, row_from_snowflake_session(expect)[0])
 
         result = runner.invoke_with_connection_json(
-            ["object", "describe", "streamlit", streamlit_name]
+            ["streamlit", "describe", streamlit_name]
         )
         expect = snowflake_session.execute_string(
             f"describe streamlit {streamlit_name}"
         )
         assert contains_row_with(result.json, row_from_snowflake_session(expect)[0])
 
         result = runner.invoke_with_connection_json(
@@ -58,17 +59,15 @@
         expect = snowflake_session.execute_string(
             f"use role {_new_streamlit_role}; show streamlits like '{streamlit_name}'; use role integration_tests;"
         )
         assert contains_row_with(
             rows_from_snowflake_session(expect)[1], {"name": streamlit_name.upper()}
         )
 
-    result = runner.invoke_with_connection_json(
-        ["object", "drop", "streamlit", streamlit_name]
-    )
+    result = runner.invoke_with_connection_json(["streamlit", "drop", streamlit_name])
     assert contains_row_with(
         result.json,
         {"status": f"{streamlit_name.upper()} successfully dropped."},
     )
     expect = snowflake_session.execute_string(
         f"show streamlits like '{streamlit_name}'"
     )
@@ -96,24 +95,24 @@
 
         # Test that second deploy does not fail
         result = runner.invoke_with_connection_json(
             ["streamlit", "deploy", "--experimental"]
         )
         assert result.exit_code == 0
 
-        result = runner.invoke_with_connection_json(["object", "list", "streamlit"])
+        result = runner.invoke_with_connection_json(["streamlit", "list"])
         assert_that_result_is_successful(result)
 
         expect = snowflake_session.execute_string(
             f"show streamlits like '{streamlit_name}'"
         )
         assert result.json == row_from_snowflake_session(expect)[0]
 
         result = runner.invoke_with_connection_json(
-            ["object", "describe", "streamlit", streamlit_name]
+            ["streamlit", "describe", streamlit_name]
         )
         expect = snowflake_session.execute_string(
             f"describe streamlit {streamlit_name}"
         )
         assert result.json == row_from_snowflake_session(expect)[0]
 
         result = runner.invoke_with_connection_json(
@@ -189,24 +188,41 @@
         result = runner.invoke_with_connection_json(["streamlit", "deploy"])
         assert result.exit_code == 0
         assert result.json == {
             "message": "Streamlit successfully deployed and available under "
             f"https://app.snowflake.com/SFENGINEERING/snowcli_it/#/streamlit-apps/{database}.{different_schema}.{streamlit_name.upper()}",
         }
 
-        # FQN with just schema provided - should update
+        # FQN with just schema provided - should require update
         alter_snowflake_yml(
             snowflake_yml,
             parameter_path="streamlit.name",
             value=f"{different_schema}.{streamlit_name}",
         )
         result = runner.invoke_with_connection(
             ["streamlit", "deploy"], catch_exceptions=True
         )
         assert result.exit_code == 1
+        # Same if name is not fqn but schema is specified
+        alter_snowflake_yml(
+            snowflake_yml,
+            parameter_path="streamlit.name",
+            value=streamlit_name,
+        )
+        alter_snowflake_yml(
+            snowflake_yml,
+            parameter_path="streamlit.schema",
+            value=different_schema,
+        )
+        result = runner.invoke_with_connection(
+            ["streamlit", "deploy"], catch_exceptions=True
+        )
+        assert result.exit_code == 1
+
+        # Should succeed with --replace flag
         result = runner.invoke_with_connection_json(
             ["streamlit", "deploy", "--replace"]
         )
         assert result.exit_code == 0
         assert result.json == {
             "message": "Streamlit successfully deployed and available under "
             f"https://app.snowflake.com/SFENGINEERING/snowcli_it/#/streamlit-apps/{database}.{different_schema}.{streamlit_name.upper()}",
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_temporary_connection.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_temporary_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_utils.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,26 @@
-import datetime
 import os
+import datetime
+from typing import Any, Dict, List
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Dict, List
 
 from snowflake.connector.cursor import SnowflakeCursor
 
 
+@contextmanager
+def pushd(directory: Path):
+    cwd = os.getcwd()
+    os.chdir(directory)
+    try:
+        yield directory
+    finally:
+        os.chdir(cwd)
+
+
 def row_from_mock(mock_print) -> List[Dict[str, Any]]:
     return row_from_cursor(mock_print.call_args.args[0])
 
 
 def rows_from_mock(mock_print) -> List[List[Dict[str, Any]]]:
     return [row_from_cursor(args.args[0]) for args in mock_print.call_args_list]
 
@@ -50,17 +60,7 @@
 
 def not_contains_row_with(rows: List[Dict[str, Any]], values: Dict[str, Any]) -> bool:
     values_items = values.items()
     for row in rows:
         if row.items() >= values_items:
             return False
     return True
-
-
-@contextmanager
-def pushd(directory: Path):
-    cwd = os.getcwd()
-    os.chdir(directory)
-    try:
-        yield directory
-    finally:
-        os.chdir(cwd)
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.4.0rc0/tests_integration/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_stage.ambr` & `snowflake_cli_labs-2.4.0rc0/tests_integration/__snapshots__/test_stage.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/nativeapp/test_version.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/nativeapp/test_version.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import uuid
 
 from snowflake.cli.api.project.util import generate_user_env
 
 from tests.project.fixtures import *
 from tests_integration.test_utils import (
+    pushd,
     contains_row_with,
     not_contains_row_with,
     row_from_snowflake_session,
-    pushd,
 )
 
 USER_NAME = f"user_{uuid.uuid4().hex}"
 TEST_ENV = generate_user_env(USER_NAME)
 
 
 # Tests a simple flow of an existing project, executing snow app version create, drop and teardown, all with distribution=internal
```

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_compute_pool.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_image_repository.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_image_repository.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_jobs.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_registry.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_registry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_services.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/test_services.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/docker/echo_service.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/docker/echo_service.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/compute_pool_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/spcs_jobs_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/spcs_services_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/snowflake.yml` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/app/app.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/app/app.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml` & `snowflake_cli_labs-2.4.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/naming_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/snowpark_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/snowpark_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/sql_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/working_directory_utils.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/working_directory_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/assertions/test_result_assertions.py` & `snowflake_cli_labs-2.4.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,19 @@
     assert result.exit_code == 0, result.output
 
 
 def assert_that_result_is_error(result: CommandResult, expected_exit_code: int) -> None:
     assert result.exit_code == expected_exit_code, result.output
 
 
+def assert_successful_result_message(result: CommandResult, expected_msg: str) -> None:
+    assert result.exit_code == 0, result.output
+    assert result.output == expected_msg + "\n"
+
+
 def assert_that_result_is_successful_and_output_json_contains(
     result: CommandResult,
     expected_output: Dict,
 ) -> None:
     assert_that_result_is_successful(result)
     assert_that_result_contains_row_with(result, expected_output)
```

### Comparing `snowflake_cli_labs-2.3.1/LICENSE` & `snowflake_cli_labs-2.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/README.md` & `snowflake_cli_labs-2.4.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.1/pyproject.toml` & `snowflake_cli_labs-2.4.0rc0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 requires-python = ">=3.8"
 description = "Snowflake CLI"
 readme = "README.md"
 dependencies = [
   "jinja2==3.1.4",
   "pluggy==1.5.0",
   "PyYAML==6.0.1",
+  "packaging",
   "rich==13.7.1",
   "requests==2.31.0",
   "requirements-parser==0.9.0",
   "setuptools==69.5.1",
+  'snowflake.core==0.8.0; python_version < "3.12"',
   "snowflake-connector-python[secure-local-storage]==3.10.0",
-  "tomlkit==0.12.3",
+  "tomlkit==0.12.5",
   "typer==0.12.3",
   "urllib3>=1.21.1,<2.3",
   "GitPython==3.1.43",
   "pip",
   "pydantic==2.7.1",
 ]
 classifiers = [
@@ -92,19 +94,20 @@
 test = ["pytest -m performance"]
 
 [tool.hatch.envs.integration]
 template = "integration"
 pre-install-commands = [
   "pip install test_external_plugins/snowpark_hello_single_command",
   "pip install test_external_plugins/multilingual_hello_command_group",
+  "pip install pytest-xdist",
 ]
 features = ["development"]
 
 [tool.hatch.envs.integration.scripts]
-test = ["pytest -m integration --snapshot-warn-unused"]
+test = ["pytest -m integration -n4 --dist=loadfile --snapshot-warn-unused"]
 test-experimental = [
   "pytest -m integration_experimental --snapshot-warn-unused",
 ]
 
 [[tool.hatch.envs.local.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
@@ -121,14 +124,15 @@
   "G",      # flake8-logging-format
   "N",      # pep8 naming
   "A",      # flake 8 builtins
   "TID252", # relative imports
   "SLF",    # Accessing private methods
   "F401",   # unused imports
   "F403",   # star imports
+  "FA100",  # Missing from __future__ import annotations
 ]
 
 [tool.pytest.ini_options]
 addopts = "-m 'not integration and not performance and not e2e and not spcs and not loaded_modules and not integration_experimental'"
 markers = [
   "integration: mark test as integration test",
   "performance: mark test as performance test",
```

### Comparing `snowflake_cli_labs-2.3.1/PKG-INFO` & `snowflake_cli_labs-2.4.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snowflake-cli-labs
-Version: 2.3.1
+Version: 2.4.0rc0
 Summary: Snowflake CLI
 Project-URL: Source code, https://github.com/snowflakedb/snowflake-cli
 Project-URL: Bug Tracker, https://github.com/snowflakedb/snowflake-cli/issues
 Author: Snowflake Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -215,24 +215,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Requires-Python: >=3.8
 Requires-Dist: gitpython==3.1.43
 Requires-Dist: jinja2==3.1.4
+Requires-Dist: packaging
 Requires-Dist: pip
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: requirements-parser==0.9.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: snowflake-connector-python[secure-local-storage]==3.10.0
-Requires-Dist: tomlkit==0.12.3
+Requires-Dist: snowflake-core==0.8.0; python_version < '3.12'
+Requires-Dist: tomlkit==0.12.5
 Requires-Dist: typer==0.12.3
 Requires-Dist: urllib3<2.3,>=1.21.1
 Provides-Extra: development
 Requires-Dist: coverage==7.5.0; extra == 'development'
 Requires-Dist: pre-commit>=3.5.0; extra == 'development'
 Requires-Dist: pytest-randomly==3.15.0; extra == 'development'
 Requires-Dist: pytest==8.2.0; extra == 'development'
```

