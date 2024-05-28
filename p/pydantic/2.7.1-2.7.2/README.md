# Comparing `tmp/pydantic-2.7.1.tar.gz` & `tmp/pydantic-2.7.2.tar.gz`

## Comparing `pydantic-2.7.1.tar` & `pydantic-2.7.2.tar`

### file list

```diff
@@ -1,314 +1,314 @@
--rw-r--r--   0        0        0   199669 2020-02-02 00:00:00.000000 pydantic-2.7.1/HISTORY.md
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pydantic-2.7.1/Makefile
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 pydantic-2.7.1/README.md
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/__init__.py
--rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_migration.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/alias_generators.py
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/aliases.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/annotated_handlers.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/class_validators.py
--rw-r--r--   0        0        0    21493 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/color.py
--rw-r--r--   0        0        0    32206 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/config.py
--rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/dataclasses.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/datetime_parse.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/decorator.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/env_settings.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/errors.py
--rw-r--r--   0        0        0    49922 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/fields.py
--rw-r--r--   0        0        0    14635 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/functional_serializers.py
--rw-r--r--   0        0        0    24322 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/functional_validators.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/generics.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/json.py
--rw-r--r--   0        0        0   105243 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/json_schema.py
--rw-r--r--   0        0        0    69938 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/main.py
--rw-r--r--   0        0        0    55574 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/mypy.py
--rw-r--r--   0        0        0    22461 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/networks.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/py.typed
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/root_model.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/schema.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/tools.py
--rw-r--r--   0        0        0    18834 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/type_adapter.py
--rw-r--r--   0        0        0    94034 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/typing.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/utils.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/validate_call_decorator.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/validators.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/version.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0    12208 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    24268 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    30623 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    26435 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_docs_extraction.py
--rw-r--r--   0        0        0    14184 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0   101871 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    22218 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_git.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0    17271 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_mock_val_ser.py
--rw-r--r--   0        0        0    31789 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_signature.py
--rw-r--r--   0        0        0    28696 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/deprecated/class_validators.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/plugin/__init__.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/plugin/_loader.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/plugin/_schema_validator.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/__init__.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/_hypothesis_plugin.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/annotated_types.py
--rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/class_validators.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/color.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/config.py
--rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/dataclasses.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/datetime_parse.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/decorator.py
--rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/env_settings.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/error_wrappers.py
--rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/errors.py
--rw-r--r--   0        0        0    50485 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/fields.py
--rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/generics.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/json.py
--rw-r--r--   0        0        0    44376 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/main.py
--rw-r--r--   0        0        0    38737 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/mypy.py
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/networks.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/py.typed
--rw-r--r--   0        0        0    47614 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/schema.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/tools.py
--rw-r--r--   0        0        0    35379 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/types.py
--rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/typing.py
--rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/utils.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/v1.py
--rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/validators.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydantic-2.7.1/pydantic/v1/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/__init__.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/check_usage_docs.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/conftest.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_abc.py
--rw-r--r--   0        0        0    23964 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_aliases.py
--rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_annotated.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_assert_in_validators.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_callable.py
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_color.py
--rw-r--r--   0        0        0    22717 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_computed_fields.py
--rw-r--r--   0        0        0    27618 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_config.py
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_construction.py
--rw-r--r--   0        0        0    19693 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_create_model.py
--rw-r--r--   0        0        0    81592 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_dataclasses.py
--rw-r--r--   0        0        0    22681 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_datetime.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_decorators.py
--rw-r--r--   0        0        0    25506 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_deprecated.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_deprecated_fields.py
--rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_deprecated_validate_arguments.py
--rw-r--r--   0        0        0    77509 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_discriminated_union.py
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_docs.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_docs_extraction.py
--rw-r--r--   0        0        0    83734 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_edge_cases.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_errors.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_exports.py
--rwxr-xr-x   0        0        0      935 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_fastapi.sh
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_fastapi_json_schema.py
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_fields.py
--rw-r--r--   0        0        0    30332 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_forward_ref.py
--rw-r--r--   0        0        0    85121 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_generics.py
--rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_internal.py
--rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_json.py
--rw-r--r--   0        0        0   196133 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_json_schema.py
--rw-r--r--   0        0        0    96898 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_main.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_migration.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_model_signature.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_model_validator.py
--rw-r--r--   0        0        0    35324 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_networks.py
--rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_networks_ipaddress.py
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_parse.py
--rw-r--r--   0        0        0     8608 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_pickle.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_plugin_loader.py
--rw-r--r--   0        0        0    16672 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_plugins.py
--rw-r--r--   0        0        0    11378 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_private_attributes.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_pydantic_extra_types.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_pydantic_settings.sh
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_rich_repr.py
--rw-r--r--   0        0        0    18948 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_root_model.py
--rw-r--r--   0        0        0    36361 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_serialize.py
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_serialize_as_any.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_strict.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_structural_pattern_matching.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_tools.py
--rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_type_adapter.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_type_alias_type.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_type_hints.py
--rw-r--r--   0        0        0   211857 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_types.py
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_types_namedtuple.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_types_payment_card_number.py
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_types_self.py
--rw-r--r--   0        0        0    27697 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_types_typeddict.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_typing.py
--rw-r--r--   0        0        0    21237 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_v1.py
--rw-r--r--   0        0        0    24628 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_validate_call.py
--rw-r--r--   0        0        0    83107 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_validators.py
--rwxr-xr-x   0        0        0     4737 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_validators_dataclass.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_version.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/test_warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/benchmarks/basemodel_eq_performance.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/benchmarks/generate_north_star_data.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/benchmarks/test_discriminated_unions.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/benchmarks/test_fastapi_startup_generics.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/benchmarks/test_fastapi_startup_simple.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/benchmarks/test_north_star.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/benchmarks/test_schema_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/__init__.py
--rw-r--r--   0        0        0    11575 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/test_mypy.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/mypy-plugin-strict-no-any.ini
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/mypy-plugin-strict.ini
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/mypy-plugin-very-strict.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/mypy-plugin.ini
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/pyproject-default.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/pyproject-plugin-bad-param.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/pyproject-plugin-no-strict-optional.toml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/pyproject-plugin-strict-equality.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/pyproject-plugin-strict.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/configs/pyproject-plugin.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/computed_fields.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/config_conditional_extra.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/custom_constructor.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/dataclass_no_any.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/fail1.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/fail2.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/fail3.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/fail4.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/fail_defaults.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/generics.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/metaclass_args.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/no_strict_optional.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/plugin_default_factory.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/plugin_fail.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/plugin_optional_inheritance.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/pydantic_settings.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/root_models.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/strict_equality.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/success.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/modules/with_config_decorator.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail2.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py
--rw-r--r--   0        0        0     8716 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict-no-any_ini/dataclass_no_any.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/custom_constructor.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py
--rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_optional_inheritance.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/root_models.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail2.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py
--rw-r--r--   0        0        0     8716 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/with_config_decorator.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-no-strict-optional_toml/no_strict_optional.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict-equality_toml/strict_equality.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_optional_inheritance.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/root_models.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-plugin_ini/root_models.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/root_models.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/with_config_decorator.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-default_ini/root_models.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9194 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_optional_inheritance.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-default_toml/root_models.py
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9194 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_optional_inheritance.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/plugin/example_plugin.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/plugin/pyproject.toml
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/pyright/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.7.1/tests/pyright/pyright_example.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pydantic-2.7.1/.gitignore
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.7.1/LICENSE
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 pydantic-2.7.1/pyproject.toml
--rw-r--r--   0        0        0   107323 2020-02-02 00:00:00.000000 pydantic-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0   200642 2020-02-02 00:00:00.000000 pydantic-2.7.2/HISTORY.md
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pydantic-2.7.2/Makefile
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 pydantic-2.7.2/README.md
+-rw-r--r--   0        0        0    13698 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/__init__.py
+-rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_migration.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/alias_generators.py
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/aliases.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/annotated_handlers.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21493 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/color.py
+-rw-r--r--   0        0        0    32206 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/config.py
+-rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/dataclasses.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/decorator.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/env_settings.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/errors.py
+-rw-r--r--   0        0        0    49922 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/fields.py
+-rw-r--r--   0        0        0    14635 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    24322 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/functional_validators.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/generics.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/json.py
+-rw-r--r--   0        0        0   105243 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/json_schema.py
+-rw-r--r--   0        0        0    69938 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/main.py
+-rw-r--r--   0        0        0    55574 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/mypy.py
+-rw-r--r--   0        0        0    22461 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/networks.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/py.typed
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/root_model.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/schema.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/tools.py
+-rw-r--r--   0        0        0    18834 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    94034 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/typing.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/utils.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/validate_call_decorator.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/validators.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/version.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0    12208 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    24268 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    30623 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    26435 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_docs_extraction.py
+-rw-r--r--   0        0        0    14184 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0   102135 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    22218 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_git.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0    17271 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_mock_val_ser.py
+-rw-r--r--   0        0        0    31789 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_signature.py
+-rw-r--r--   0        0        0    28696 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/plugin/__init__.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/plugin/_loader.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/plugin/_schema_validator.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/config.py
+-rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50485 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44376 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38737 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47614 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35379 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/types.py
+-rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/utils.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/v1.py
+-rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydantic-2.7.2/pydantic/v1/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/__init__.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/check_usage_docs.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/conftest.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_abc.py
+-rw-r--r--   0        0        0    23964 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_aliases.py
+-rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_annotated.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_assert_in_validators.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_callable.py
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_color.py
+-rw-r--r--   0        0        0    22717 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_computed_fields.py
+-rw-r--r--   0        0        0    27618 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_config.py
+-rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_construction.py
+-rw-r--r--   0        0        0    19693 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_create_model.py
+-rw-r--r--   0        0        0    81592 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_dataclasses.py
+-rw-r--r--   0        0        0    22681 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_datetime.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_decorators.py
+-rw-r--r--   0        0        0    25506 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_deprecated.py
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_deprecated_fields.py
+-rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_deprecated_validate_arguments.py
+-rw-r--r--   0        0        0    77509 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_discriminated_union.py
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_docs.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_docs_extraction.py
+-rw-r--r--   0        0        0    83734 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_edge_cases.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_errors.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_exports.py
+-rwxr-xr-x   0        0        0      935 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_fastapi.sh
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_fastapi_json_schema.py
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_fields.py
+-rw-r--r--   0        0        0    30332 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_forward_ref.py
+-rw-r--r--   0        0        0    85121 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_generics.py
+-rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_internal.py
+-rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_json.py
+-rw-r--r--   0        0        0   196133 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_json_schema.py
+-rw-r--r--   0        0        0    96898 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_main.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_migration.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_model_signature.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_model_validator.py
+-rw-r--r--   0        0        0    35324 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_networks.py
+-rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_networks_ipaddress.py
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_parse.py
+-rw-r--r--   0        0        0     8608 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_pickle.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_plugin_loader.py
+-rw-r--r--   0        0        0    16672 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_plugins.py
+-rw-r--r--   0        0        0    11378 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_private_attributes.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_pydantic_extra_types.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_pydantic_settings.sh
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_rich_repr.py
+-rw-r--r--   0        0        0    18948 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_root_model.py
+-rw-r--r--   0        0        0    36361 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_serialize.py
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_serialize_as_any.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_strict.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_structural_pattern_matching.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_tools.py
+-rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_type_adapter.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_type_alias_type.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_type_hints.py
+-rw-r--r--   0        0        0   211857 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_types.py
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_types_namedtuple.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_types_payment_card_number.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_types_self.py
+-rw-r--r--   0        0        0    27697 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_types_typeddict.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_typing.py
+-rw-r--r--   0        0        0    21237 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_v1.py
+-rw-r--r--   0        0        0    24628 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_validate_call.py
+-rw-r--r--   0        0        0    83107 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_validators.py
+-rwxr-xr-x   0        0        0     4737 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_validators_dataclass.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_version.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/test_warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/benchmarks/basemodel_eq_performance.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/benchmarks/generate_north_star_data.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/benchmarks/test_discriminated_unions.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/benchmarks/test_fastapi_startup_generics.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/benchmarks/test_fastapi_startup_simple.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/benchmarks/test_north_star.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/benchmarks/test_schema_build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/__init__.py
+-rw-r--r--   0        0        0    11575 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/test_mypy.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/mypy-plugin-strict-no-any.ini
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/mypy-plugin-strict.ini
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/mypy-plugin-very-strict.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/mypy-plugin.ini
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/pyproject-default.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/pyproject-plugin-bad-param.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/pyproject-plugin-no-strict-optional.toml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/pyproject-plugin-strict-equality.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/pyproject-plugin-strict.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/configs/pyproject-plugin.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/computed_fields.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/config_conditional_extra.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/custom_constructor.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/dataclass_no_any.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/fail1.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/fail2.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/fail3.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/fail4.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/fail_defaults.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/generics.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/metaclass_args.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/no_strict_optional.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/plugin_default_factory.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/plugin_fail.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/plugin_optional_inheritance.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/pydantic_settings.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/root_models.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/strict_equality.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/success.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/modules/with_config_decorator.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/fail2.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py
+-rw-r--r--   0        0        0     8716 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict-no-any_ini/dataclass_no_any.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/custom_constructor.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py
+-rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_optional_inheritance.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/root_models.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail2.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py
+-rw-r--r--   0        0        0     8716 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/with_config_decorator.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-no-strict-optional_toml/no_strict_optional.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict-equality_toml/strict_equality.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_optional_inheritance.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/root_models.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-plugin_ini/root_models.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/pyproject-default_toml/root_models.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.1.1/pyproject-default_toml/with_config_decorator.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-default_ini/root_models.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9194 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_optional_inheritance.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-default_toml/root_models.py
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9194 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_optional_inheritance.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/plugin/example_plugin.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/plugin/pyproject.toml
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/pyright/pyproject.toml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.7.2/tests/pyright/pyright_example.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pydantic-2.7.2/.gitignore
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.7.2/LICENSE
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 pydantic-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0   108504 2020-02-02 00:00:00.000000 pydantic-2.7.2/PKG-INFO
```

### Comparing `pydantic-2.7.1/HISTORY.md` & `pydantic-2.7.2/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,34 @@
+## v2.7.2 (2024-05-28)
+
+[GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.7.2)
+
+### What's Changed
+
+#### Packaging
+
+* Bump `pydantic-core` to `v2.18.3` by @sydney-runkle in [#9515](https://github.com/pydantic/pydantic/pull/9515)
+
+#### Fixes
+
+* Replace `__spec__.parent` with `__package__` by @hramezani in [#9331](https://github.com/pydantic/pydantic/pull/9331)
+* Fix validation of `int`s with leading unary minus by @RajatRajdeep in [pydantic/pydantic-core#1291](https://github.com/pydantic/pydantic-core/pull/1291)
+* Fix `str` subclass validation for enums by @sydney-runkle in [pydantic/pydantic-core#1273]https://github.com/pydantic/pydantic-core/pull/1273
+* Support `BigInt`s in `Literal`s and `Enum`s by @samuelcolvin in [pydantic/pydantic-core#1297]https://github.com/pydantic/pydantic-core/pull/1297
+* Fix: uuid - allow `str` subclass as input by @davidhewitt in [pydantic/pydantic-core#1296]https://github.com/pydantic/pydantic-core/pull/1296
+
 ## v2.7.1 (2024-04-23)
 
 [GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.7.1)
 
 ### What's Changed
 
 #### Packaging
 
-* Bump `pydantic-core` to `v2.18.2` by @sydney-runkle in [#9307](https://github.com/pydantic/pydantic/pull/9307)
+* Bump `pydantic-core` to `v2.18.3` by @sydney-runkle in [#9307](https://github.com/pydantic/pydantic/pull/9307)
 
 #### New Features
 
 * Ftp and Websocket connection strings support by @CherrySuryp in [#9205](https://github.com/pydantic/pydantic/pull/9205)
 
 #### Changes
```

### Comparing `pydantic-2.7.1/Makefile` & `pydantic-2.7.2/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/README.md` & `pydantic-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/__init__.py` & `pydantic-2.7.2/pydantic/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -216,168 +216,168 @@
     'FieldSerializationInfo',
     'SerializerFunctionWrapHandler',
     'OnErrorOmit',
 )
 
 # A mapping of {<member name>: (package, <module name>)} defining dynamic imports
 _dynamic_imports: 'dict[str, tuple[str, str]]' = {
-    'dataclasses': (__package__, '__module__'),
+    'dataclasses': (__spec__.parent, '__module__'),
     # functional validators
-    'field_validator': (__package__, '.functional_validators'),
-    'model_validator': (__package__, '.functional_validators'),
-    'AfterValidator': (__package__, '.functional_validators'),
-    'BeforeValidator': (__package__, '.functional_validators'),
-    'PlainValidator': (__package__, '.functional_validators'),
-    'WrapValidator': (__package__, '.functional_validators'),
-    'SkipValidation': (__package__, '.functional_validators'),
-    'InstanceOf': (__package__, '.functional_validators'),
+    'field_validator': (__spec__.parent, '.functional_validators'),
+    'model_validator': (__spec__.parent, '.functional_validators'),
+    'AfterValidator': (__spec__.parent, '.functional_validators'),
+    'BeforeValidator': (__spec__.parent, '.functional_validators'),
+    'PlainValidator': (__spec__.parent, '.functional_validators'),
+    'WrapValidator': (__spec__.parent, '.functional_validators'),
+    'SkipValidation': (__spec__.parent, '.functional_validators'),
+    'InstanceOf': (__spec__.parent, '.functional_validators'),
     # JSON Schema
-    'WithJsonSchema': (__package__, '.json_schema'),
+    'WithJsonSchema': (__spec__.parent, '.json_schema'),
     # functional serializers
-    'field_serializer': (__package__, '.functional_serializers'),
-    'model_serializer': (__package__, '.functional_serializers'),
-    'PlainSerializer': (__package__, '.functional_serializers'),
-    'SerializeAsAny': (__package__, '.functional_serializers'),
-    'WrapSerializer': (__package__, '.functional_serializers'),
+    'field_serializer': (__spec__.parent, '.functional_serializers'),
+    'model_serializer': (__spec__.parent, '.functional_serializers'),
+    'PlainSerializer': (__spec__.parent, '.functional_serializers'),
+    'SerializeAsAny': (__spec__.parent, '.functional_serializers'),
+    'WrapSerializer': (__spec__.parent, '.functional_serializers'),
     # config
-    'ConfigDict': (__package__, '.config'),
-    'with_config': (__package__, '.config'),
+    'ConfigDict': (__spec__.parent, '.config'),
+    'with_config': (__spec__.parent, '.config'),
     # validate call
-    'validate_call': (__package__, '.validate_call_decorator'),
+    'validate_call': (__spec__.parent, '.validate_call_decorator'),
     # errors
-    'PydanticErrorCodes': (__package__, '.errors'),
-    'PydanticUserError': (__package__, '.errors'),
-    'PydanticSchemaGenerationError': (__package__, '.errors'),
-    'PydanticImportError': (__package__, '.errors'),
-    'PydanticUndefinedAnnotation': (__package__, '.errors'),
-    'PydanticInvalidForJsonSchema': (__package__, '.errors'),
+    'PydanticErrorCodes': (__spec__.parent, '.errors'),
+    'PydanticUserError': (__spec__.parent, '.errors'),
+    'PydanticSchemaGenerationError': (__spec__.parent, '.errors'),
+    'PydanticImportError': (__spec__.parent, '.errors'),
+    'PydanticUndefinedAnnotation': (__spec__.parent, '.errors'),
+    'PydanticInvalidForJsonSchema': (__spec__.parent, '.errors'),
     # fields
-    'Field': (__package__, '.fields'),
-    'computed_field': (__package__, '.fields'),
-    'PrivateAttr': (__package__, '.fields'),
+    'Field': (__spec__.parent, '.fields'),
+    'computed_field': (__spec__.parent, '.fields'),
+    'PrivateAttr': (__spec__.parent, '.fields'),
     # alias
-    'AliasChoices': (__package__, '.aliases'),
-    'AliasGenerator': (__package__, '.aliases'),
-    'AliasPath': (__package__, '.aliases'),
+    'AliasChoices': (__spec__.parent, '.aliases'),
+    'AliasGenerator': (__spec__.parent, '.aliases'),
+    'AliasPath': (__spec__.parent, '.aliases'),
     # main
-    'BaseModel': (__package__, '.main'),
-    'create_model': (__package__, '.main'),
+    'BaseModel': (__spec__.parent, '.main'),
+    'create_model': (__spec__.parent, '.main'),
     # network
-    'AnyUrl': (__package__, '.networks'),
-    'AnyHttpUrl': (__package__, '.networks'),
-    'FileUrl': (__package__, '.networks'),
-    'HttpUrl': (__package__, '.networks'),
-    'FtpUrl': (__package__, '.networks'),
-    'WebsocketUrl': (__package__, '.networks'),
-    'AnyWebsocketUrl': (__package__, '.networks'),
-    'UrlConstraints': (__package__, '.networks'),
-    'EmailStr': (__package__, '.networks'),
-    'NameEmail': (__package__, '.networks'),
-    'IPvAnyAddress': (__package__, '.networks'),
-    'IPvAnyInterface': (__package__, '.networks'),
-    'IPvAnyNetwork': (__package__, '.networks'),
-    'PostgresDsn': (__package__, '.networks'),
-    'CockroachDsn': (__package__, '.networks'),
-    'AmqpDsn': (__package__, '.networks'),
-    'RedisDsn': (__package__, '.networks'),
-    'MongoDsn': (__package__, '.networks'),
-    'KafkaDsn': (__package__, '.networks'),
-    'NatsDsn': (__package__, '.networks'),
-    'MySQLDsn': (__package__, '.networks'),
-    'MariaDBDsn': (__package__, '.networks'),
-    'ClickHouseDsn': (__package__, '.networks'),
-    'validate_email': (__package__, '.networks'),
+    'AnyUrl': (__spec__.parent, '.networks'),
+    'AnyHttpUrl': (__spec__.parent, '.networks'),
+    'FileUrl': (__spec__.parent, '.networks'),
+    'HttpUrl': (__spec__.parent, '.networks'),
+    'FtpUrl': (__spec__.parent, '.networks'),
+    'WebsocketUrl': (__spec__.parent, '.networks'),
+    'AnyWebsocketUrl': (__spec__.parent, '.networks'),
+    'UrlConstraints': (__spec__.parent, '.networks'),
+    'EmailStr': (__spec__.parent, '.networks'),
+    'NameEmail': (__spec__.parent, '.networks'),
+    'IPvAnyAddress': (__spec__.parent, '.networks'),
+    'IPvAnyInterface': (__spec__.parent, '.networks'),
+    'IPvAnyNetwork': (__spec__.parent, '.networks'),
+    'PostgresDsn': (__spec__.parent, '.networks'),
+    'CockroachDsn': (__spec__.parent, '.networks'),
+    'AmqpDsn': (__spec__.parent, '.networks'),
+    'RedisDsn': (__spec__.parent, '.networks'),
+    'MongoDsn': (__spec__.parent, '.networks'),
+    'KafkaDsn': (__spec__.parent, '.networks'),
+    'NatsDsn': (__spec__.parent, '.networks'),
+    'MySQLDsn': (__spec__.parent, '.networks'),
+    'MariaDBDsn': (__spec__.parent, '.networks'),
+    'ClickHouseDsn': (__spec__.parent, '.networks'),
+    'validate_email': (__spec__.parent, '.networks'),
     # root_model
-    'RootModel': (__package__, '.root_model'),
+    'RootModel': (__spec__.parent, '.root_model'),
     # types
-    'Strict': (__package__, '.types'),
-    'StrictStr': (__package__, '.types'),
-    'conbytes': (__package__, '.types'),
-    'conlist': (__package__, '.types'),
-    'conset': (__package__, '.types'),
-    'confrozenset': (__package__, '.types'),
-    'constr': (__package__, '.types'),
-    'StringConstraints': (__package__, '.types'),
-    'ImportString': (__package__, '.types'),
-    'conint': (__package__, '.types'),
-    'PositiveInt': (__package__, '.types'),
-    'NegativeInt': (__package__, '.types'),
-    'NonNegativeInt': (__package__, '.types'),
-    'NonPositiveInt': (__package__, '.types'),
-    'confloat': (__package__, '.types'),
-    'PositiveFloat': (__package__, '.types'),
-    'NegativeFloat': (__package__, '.types'),
-    'NonNegativeFloat': (__package__, '.types'),
-    'NonPositiveFloat': (__package__, '.types'),
-    'FiniteFloat': (__package__, '.types'),
-    'condecimal': (__package__, '.types'),
-    'condate': (__package__, '.types'),
-    'UUID1': (__package__, '.types'),
-    'UUID3': (__package__, '.types'),
-    'UUID4': (__package__, '.types'),
-    'UUID5': (__package__, '.types'),
-    'FilePath': (__package__, '.types'),
-    'DirectoryPath': (__package__, '.types'),
-    'NewPath': (__package__, '.types'),
-    'Json': (__package__, '.types'),
-    'Secret': (__package__, '.types'),
-    'SecretStr': (__package__, '.types'),
-    'SecretBytes': (__package__, '.types'),
-    'StrictBool': (__package__, '.types'),
-    'StrictBytes': (__package__, '.types'),
-    'StrictInt': (__package__, '.types'),
-    'StrictFloat': (__package__, '.types'),
-    'PaymentCardNumber': (__package__, '.types'),
-    'ByteSize': (__package__, '.types'),
-    'PastDate': (__package__, '.types'),
-    'FutureDate': (__package__, '.types'),
-    'PastDatetime': (__package__, '.types'),
-    'FutureDatetime': (__package__, '.types'),
-    'AwareDatetime': (__package__, '.types'),
-    'NaiveDatetime': (__package__, '.types'),
-    'AllowInfNan': (__package__, '.types'),
-    'EncoderProtocol': (__package__, '.types'),
-    'EncodedBytes': (__package__, '.types'),
-    'EncodedStr': (__package__, '.types'),
-    'Base64Encoder': (__package__, '.types'),
-    'Base64Bytes': (__package__, '.types'),
-    'Base64Str': (__package__, '.types'),
-    'Base64UrlBytes': (__package__, '.types'),
-    'Base64UrlStr': (__package__, '.types'),
-    'GetPydanticSchema': (__package__, '.types'),
-    'Tag': (__package__, '.types'),
-    'Discriminator': (__package__, '.types'),
-    'JsonValue': (__package__, '.types'),
-    'OnErrorOmit': (__package__, '.types'),
+    'Strict': (__spec__.parent, '.types'),
+    'StrictStr': (__spec__.parent, '.types'),
+    'conbytes': (__spec__.parent, '.types'),
+    'conlist': (__spec__.parent, '.types'),
+    'conset': (__spec__.parent, '.types'),
+    'confrozenset': (__spec__.parent, '.types'),
+    'constr': (__spec__.parent, '.types'),
+    'StringConstraints': (__spec__.parent, '.types'),
+    'ImportString': (__spec__.parent, '.types'),
+    'conint': (__spec__.parent, '.types'),
+    'PositiveInt': (__spec__.parent, '.types'),
+    'NegativeInt': (__spec__.parent, '.types'),
+    'NonNegativeInt': (__spec__.parent, '.types'),
+    'NonPositiveInt': (__spec__.parent, '.types'),
+    'confloat': (__spec__.parent, '.types'),
+    'PositiveFloat': (__spec__.parent, '.types'),
+    'NegativeFloat': (__spec__.parent, '.types'),
+    'NonNegativeFloat': (__spec__.parent, '.types'),
+    'NonPositiveFloat': (__spec__.parent, '.types'),
+    'FiniteFloat': (__spec__.parent, '.types'),
+    'condecimal': (__spec__.parent, '.types'),
+    'condate': (__spec__.parent, '.types'),
+    'UUID1': (__spec__.parent, '.types'),
+    'UUID3': (__spec__.parent, '.types'),
+    'UUID4': (__spec__.parent, '.types'),
+    'UUID5': (__spec__.parent, '.types'),
+    'FilePath': (__spec__.parent, '.types'),
+    'DirectoryPath': (__spec__.parent, '.types'),
+    'NewPath': (__spec__.parent, '.types'),
+    'Json': (__spec__.parent, '.types'),
+    'Secret': (__spec__.parent, '.types'),
+    'SecretStr': (__spec__.parent, '.types'),
+    'SecretBytes': (__spec__.parent, '.types'),
+    'StrictBool': (__spec__.parent, '.types'),
+    'StrictBytes': (__spec__.parent, '.types'),
+    'StrictInt': (__spec__.parent, '.types'),
+    'StrictFloat': (__spec__.parent, '.types'),
+    'PaymentCardNumber': (__spec__.parent, '.types'),
+    'ByteSize': (__spec__.parent, '.types'),
+    'PastDate': (__spec__.parent, '.types'),
+    'FutureDate': (__spec__.parent, '.types'),
+    'PastDatetime': (__spec__.parent, '.types'),
+    'FutureDatetime': (__spec__.parent, '.types'),
+    'AwareDatetime': (__spec__.parent, '.types'),
+    'NaiveDatetime': (__spec__.parent, '.types'),
+    'AllowInfNan': (__spec__.parent, '.types'),
+    'EncoderProtocol': (__spec__.parent, '.types'),
+    'EncodedBytes': (__spec__.parent, '.types'),
+    'EncodedStr': (__spec__.parent, '.types'),
+    'Base64Encoder': (__spec__.parent, '.types'),
+    'Base64Bytes': (__spec__.parent, '.types'),
+    'Base64Str': (__spec__.parent, '.types'),
+    'Base64UrlBytes': (__spec__.parent, '.types'),
+    'Base64UrlStr': (__spec__.parent, '.types'),
+    'GetPydanticSchema': (__spec__.parent, '.types'),
+    'Tag': (__spec__.parent, '.types'),
+    'Discriminator': (__spec__.parent, '.types'),
+    'JsonValue': (__spec__.parent, '.types'),
+    'OnErrorOmit': (__spec__.parent, '.types'),
     # type_adapter
-    'TypeAdapter': (__package__, '.type_adapter'),
+    'TypeAdapter': (__spec__.parent, '.type_adapter'),
     # warnings
-    'PydanticDeprecatedSince20': (__package__, '.warnings'),
-    'PydanticDeprecatedSince26': (__package__, '.warnings'),
-    'PydanticDeprecationWarning': (__package__, '.warnings'),
+    'PydanticDeprecatedSince20': (__spec__.parent, '.warnings'),
+    'PydanticDeprecatedSince26': (__spec__.parent, '.warnings'),
+    'PydanticDeprecationWarning': (__spec__.parent, '.warnings'),
     # annotated handlers
-    'GetCoreSchemaHandler': (__package__, '.annotated_handlers'),
-    'GetJsonSchemaHandler': (__package__, '.annotated_handlers'),
+    'GetCoreSchemaHandler': (__spec__.parent, '.annotated_handlers'),
+    'GetJsonSchemaHandler': (__spec__.parent, '.annotated_handlers'),
     # generate schema from ._internal
-    'GenerateSchema': (__package__, '._internal._generate_schema'),
+    'GenerateSchema': (__spec__.parent, '._internal._generate_schema'),
     # pydantic_core stuff
     'ValidationError': ('pydantic_core', '.'),
     'ValidationInfo': ('pydantic_core', '.core_schema'),
     'SerializationInfo': ('pydantic_core', '.core_schema'),
     'ValidatorFunctionWrapHandler': ('pydantic_core', '.core_schema'),
     'FieldSerializationInfo': ('pydantic_core', '.core_schema'),
     'SerializerFunctionWrapHandler': ('pydantic_core', '.core_schema'),
     # deprecated, mostly not included in __all__
-    'root_validator': (__package__, '.deprecated.class_validators'),
-    'validator': (__package__, '.deprecated.class_validators'),
-    'BaseConfig': (__package__, '.deprecated.config'),
-    'Extra': (__package__, '.deprecated.config'),
-    'parse_obj_as': (__package__, '.deprecated.tools'),
-    'schema_of': (__package__, '.deprecated.tools'),
-    'schema_json_of': (__package__, '.deprecated.tools'),
+    'root_validator': (__spec__.parent, '.deprecated.class_validators'),
+    'validator': (__spec__.parent, '.deprecated.class_validators'),
+    'BaseConfig': (__spec__.parent, '.deprecated.config'),
+    'Extra': (__spec__.parent, '.deprecated.config'),
+    'parse_obj_as': (__spec__.parent, '.deprecated.tools'),
+    'schema_of': (__spec__.parent, '.deprecated.tools'),
+    'schema_json_of': (__spec__.parent, '.deprecated.tools'),
     'FieldValidationInfo': ('pydantic_core', '.core_schema'),
 }
 
 _getattr_migration = getattr_migration(__name__)
 
 
 def __getattr__(attr_name: str) -> object:
```

### Comparing `pydantic-2.7.1/pydantic/_migration.py` & `pydantic-2.7.2/pydantic/_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/alias_generators.py` & `pydantic-2.7.2/pydantic/alias_generators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/aliases.py` & `pydantic-2.7.2/pydantic/aliases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/annotated_handlers.py` & `pydantic-2.7.2/pydantic/annotated_handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/color.py` & `pydantic-2.7.2/pydantic/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/config.py` & `pydantic-2.7.2/pydantic/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/dataclasses.py` & `pydantic-2.7.2/pydantic/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/errors.py` & `pydantic-2.7.2/pydantic/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/fields.py` & `pydantic-2.7.2/pydantic/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/functional_serializers.py` & `pydantic-2.7.2/pydantic/functional_serializers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/functional_validators.py` & `pydantic-2.7.2/pydantic/functional_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/json_schema.py` & `pydantic-2.7.2/pydantic/json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/main.py` & `pydantic-2.7.2/pydantic/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/mypy.py` & `pydantic-2.7.2/pydantic/mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/networks.py` & `pydantic-2.7.2/pydantic/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/root_model.py` & `pydantic-2.7.2/pydantic/root_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/type_adapter.py` & `pydantic-2.7.2/pydantic/type_adapter.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/types.py` & `pydantic-2.7.2/pydantic/types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/validate_call_decorator.py` & `pydantic-2.7.2/pydantic/validate_call_decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/version.py` & `pydantic-2.7.2/pydantic/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The `version` module holds the version information for Pydantic."""
 from __future__ import annotations as _annotations
 
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '2.7.1'
+VERSION = '2.7.2'
 """The version of Pydantic."""
 
 
 def version_short() -> str:
     """Return the `major.minor` part of Pydantic version.
 
     It returns '2.1' if Pydantic version is '2.1.1'.
```

### Comparing `pydantic-2.7.1/pydantic/warnings.py` & `pydantic-2.7.2/pydantic/warnings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_config.py` & `pydantic-2.7.2/pydantic/_internal/_config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_core_metadata.py` & `pydantic-2.7.2/pydantic/_internal/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_core_utils.py` & `pydantic-2.7.2/pydantic/_internal/_core_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_dataclasses.py` & `pydantic-2.7.2/pydantic/_internal/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_decorators.py` & `pydantic-2.7.2/pydantic/_internal/_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_decorators_v1.py` & `pydantic-2.7.2/pydantic/_internal/_decorators_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_discriminated_union.py` & `pydantic-2.7.2/pydantic/_internal/_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_docs_extraction.py` & `pydantic-2.7.2/pydantic/_internal/_docs_extraction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_fields.py` & `pydantic-2.7.2/pydantic/_internal/_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_forward_ref.py` & `pydantic-2.7.2/pydantic/_internal/_forward_ref.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_generate_schema.py` & `pydantic-2.7.2/pydantic/_internal/_generate_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1652,23 +1652,28 @@
         )
 
     def _unsubstituted_typevar_schema(self, typevar: typing.TypeVar) -> core_schema.CoreSchema:
         assert isinstance(typevar, typing.TypeVar)
 
         bound = typevar.__bound__
         constraints = typevar.__constraints__
-        default = getattr(typevar, '__default__', None)
 
-        if (bound is not None) + (len(constraints) != 0) + (default is not None) > 1:
+        try:
+            typevar_has_default = typevar.has_default()  # type: ignore
+        except AttributeError:
+            # could still have a default if it's an old version of typing_extensions.TypeVar
+            typevar_has_default = getattr(typevar, '__default__', None) is not None
+
+        if (bound is not None) + (len(constraints) != 0) + typevar_has_default > 1:
             raise NotImplementedError(
                 'Pydantic does not support mixing more than one of TypeVar bounds, constraints and defaults'
             )
 
-        if default is not None:
-            return self.generate_schema(default)
+        if typevar_has_default:
+            return self.generate_schema(typevar.__default__)  # type: ignore
         elif constraints:
             return self._union_schema(typing.Union[constraints])  # type: ignore
         elif bound:
             schema = self.generate_schema(bound)
             schema['serialization'] = core_schema.wrap_serializer_function_ser_schema(
                 lambda x, h: h(x), schema=core_schema.any_schema()
             )
```

### Comparing `pydantic-2.7.1/pydantic/_internal/_generics.py` & `pydantic-2.7.2/pydantic/_internal/_generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_git.py` & `pydantic-2.7.2/pydantic/_internal/_git.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_known_annotated_metadata.py` & `pydantic-2.7.2/pydantic/_internal/_known_annotated_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_mock_val_ser.py` & `pydantic-2.7.2/pydantic/_internal/_mock_val_ser.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_model_construction.py` & `pydantic-2.7.2/pydantic/_internal/_model_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_repr.py` & `pydantic-2.7.2/pydantic/_internal/_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_schema_generation_shared.py` & `pydantic-2.7.2/pydantic/_internal/_schema_generation_shared.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_signature.py` & `pydantic-2.7.2/pydantic/_internal/_signature.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_std_types_schema.py` & `pydantic-2.7.2/pydantic/_internal/_std_types_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_typing_extra.py` & `pydantic-2.7.2/pydantic/_internal/_typing_extra.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_utils.py` & `pydantic-2.7.2/pydantic/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_validate_call.py` & `pydantic-2.7.2/pydantic/_internal/_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/_internal/_validators.py` & `pydantic-2.7.2/pydantic/_internal/_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/deprecated/class_validators.py` & `pydantic-2.7.2/pydantic/deprecated/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/deprecated/config.py` & `pydantic-2.7.2/pydantic/deprecated/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/deprecated/copy_internals.py` & `pydantic-2.7.2/pydantic/deprecated/copy_internals.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/deprecated/decorator.py` & `pydantic-2.7.2/pydantic/deprecated/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/deprecated/json.py` & `pydantic-2.7.2/pydantic/deprecated/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/deprecated/parse.py` & `pydantic-2.7.2/pydantic/deprecated/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/deprecated/tools.py` & `pydantic-2.7.2/pydantic/deprecated/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/plugin/__init__.py` & `pydantic-2.7.2/pydantic/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/plugin/_loader.py` & `pydantic-2.7.2/pydantic/plugin/_loader.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/plugin/_schema_validator.py` & `pydantic-2.7.2/pydantic/plugin/_schema_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/__init__.py` & `pydantic-2.7.2/pydantic/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/_hypothesis_plugin.py` & `pydantic-2.7.2/pydantic/v1/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/annotated_types.py` & `pydantic-2.7.2/pydantic/v1/annotated_types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/class_validators.py` & `pydantic-2.7.2/pydantic/v1/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/color.py` & `pydantic-2.7.2/pydantic/v1/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/config.py` & `pydantic-2.7.2/pydantic/v1/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/dataclasses.py` & `pydantic-2.7.2/pydantic/v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/datetime_parse.py` & `pydantic-2.7.2/pydantic/v1/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/decorator.py` & `pydantic-2.7.2/pydantic/v1/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/env_settings.py` & `pydantic-2.7.2/pydantic/v1/env_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/error_wrappers.py` & `pydantic-2.7.2/pydantic/v1/error_wrappers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/errors.py` & `pydantic-2.7.2/pydantic/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/fields.py` & `pydantic-2.7.2/pydantic/v1/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/generics.py` & `pydantic-2.7.2/pydantic/v1/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/json.py` & `pydantic-2.7.2/pydantic/v1/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/main.py` & `pydantic-2.7.2/pydantic/v1/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/mypy.py` & `pydantic-2.7.2/pydantic/v1/mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/networks.py` & `pydantic-2.7.2/pydantic/v1/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/parse.py` & `pydantic-2.7.2/pydantic/v1/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/schema.py` & `pydantic-2.7.2/pydantic/v1/schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/tools.py` & `pydantic-2.7.2/pydantic/v1/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/types.py` & `pydantic-2.7.2/pydantic/v1/types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/typing.py` & `pydantic-2.7.2/pydantic/v1/typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/utils.py` & `pydantic-2.7.2/pydantic/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/v1.py` & `pydantic-2.7.2/pydantic/v1/v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/validators.py` & `pydantic-2.7.2/pydantic/v1/validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pydantic/v1/version.py` & `pydantic-2.7.2/pydantic/v1/version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/check_usage_docs.py` & `pydantic-2.7.2/tests/check_usage_docs.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/conftest.py` & `pydantic-2.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_abc.py` & `pydantic-2.7.2/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_aliases.py` & `pydantic-2.7.2/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_annotated.py` & `pydantic-2.7.2/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_assert_in_validators.py` & `pydantic-2.7.2/tests/test_assert_in_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_callable.py` & `pydantic-2.7.2/tests/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_color.py` & `pydantic-2.7.2/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_computed_fields.py` & `pydantic-2.7.2/tests/test_computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_config.py` & `pydantic-2.7.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_construction.py` & `pydantic-2.7.2/tests/test_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_create_model.py` & `pydantic-2.7.2/tests/test_create_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_dataclasses.py` & `pydantic-2.7.2/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_datetime.py` & `pydantic-2.7.2/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_decorators.py` & `pydantic-2.7.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_deprecated.py` & `pydantic-2.7.2/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_deprecated_fields.py` & `pydantic-2.7.2/tests/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_deprecated_validate_arguments.py` & `pydantic-2.7.2/tests/test_deprecated_validate_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_discriminated_union.py` & `pydantic-2.7.2/tests/test_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_docs.py` & `pydantic-2.7.2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_docs_extraction.py` & `pydantic-2.7.2/tests/test_docs_extraction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_edge_cases.py` & `pydantic-2.7.2/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_errors.py` & `pydantic-2.7.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_exports.py` & `pydantic-2.7.2/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_fastapi.sh` & `pydantic-2.7.2/tests/test_fastapi.sh`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_fastapi_json_schema.py` & `pydantic-2.7.2/tests/test_fastapi_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_fields.py` & `pydantic-2.7.2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_forward_ref.py` & `pydantic-2.7.2/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_generics.py` & `pydantic-2.7.2/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_internal.py` & `pydantic-2.7.2/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_json.py` & `pydantic-2.7.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_json_schema.py` & `pydantic-2.7.2/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_main.py` & `pydantic-2.7.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_migration.py` & `pydantic-2.7.2/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_model_signature.py` & `pydantic-2.7.2/tests/test_model_signature.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_model_validator.py` & `pydantic-2.7.2/tests/test_model_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_networks.py` & `pydantic-2.7.2/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_networks_ipaddress.py` & `pydantic-2.7.2/tests/test_networks_ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_parse.py` & `pydantic-2.7.2/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_pickle.py` & `pydantic-2.7.2/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_plugin_loader.py` & `pydantic-2.7.2/tests/test_plugin_loader.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_plugins.py` & `pydantic-2.7.2/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_private_attributes.py` & `pydantic-2.7.2/tests/test_private_attributes.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_rich_repr.py` & `pydantic-2.7.2/tests/test_rich_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_root_model.py` & `pydantic-2.7.2/tests/test_root_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_serialize.py` & `pydantic-2.7.2/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_serialize_as_any.py` & `pydantic-2.7.2/tests/test_serialize_as_any.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_strict.py` & `pydantic-2.7.2/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_structural_pattern_matching.py` & `pydantic-2.7.2/tests/test_structural_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_tools.py` & `pydantic-2.7.2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_type_adapter.py` & `pydantic-2.7.2/tests/test_type_adapter.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_type_alias_type.py` & `pydantic-2.7.2/tests/test_type_alias_type.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_type_hints.py` & `pydantic-2.7.2/tests/test_type_hints.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_types.py` & `pydantic-2.7.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_types_namedtuple.py` & `pydantic-2.7.2/tests/test_types_namedtuple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_types_payment_card_number.py` & `pydantic-2.7.2/tests/test_types_payment_card_number.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_types_self.py` & `pydantic-2.7.2/tests/test_types_self.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_types_typeddict.py` & `pydantic-2.7.2/tests/test_types_typeddict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_typing.py` & `pydantic-2.7.2/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_utils.py` & `pydantic-2.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_v1.py` & `pydantic-2.7.2/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_validate_call.py` & `pydantic-2.7.2/tests/test_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_validators.py` & `pydantic-2.7.2/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_validators_dataclass.py` & `pydantic-2.7.2/tests/test_validators_dataclass.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_version.py` & `pydantic-2.7.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/test_warnings.py` & `pydantic-2.7.2/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/benchmarks/basemodel_eq_performance.py` & `pydantic-2.7.2/tests/benchmarks/basemodel_eq_performance.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/benchmarks/generate_north_star_data.py` & `pydantic-2.7.2/tests/benchmarks/generate_north_star_data.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/benchmarks/test_discriminated_unions.py` & `pydantic-2.7.2/tests/benchmarks/test_discriminated_unions.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/benchmarks/test_fastapi_startup_generics.py` & `pydantic-2.7.2/tests/benchmarks/test_fastapi_startup_generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/benchmarks/test_fastapi_startup_simple.py` & `pydantic-2.7.2/tests/benchmarks/test_fastapi_startup_simple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/benchmarks/test_north_star.py` & `pydantic-2.7.2/tests/benchmarks/test_north_star.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/benchmarks/test_schema_build.py` & `pydantic-2.7.2/tests/benchmarks/test_schema_build.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/test_mypy.py` & `pydantic-2.7.2/tests/mypy/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/configs/mypy-plugin-strict-no-any.ini` & `pydantic-2.7.2/tests/mypy/configs/mypy-plugin-strict-no-any.ini`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/configs/pyproject-default.toml` & `pydantic-2.7.2/tests/mypy/configs/pyproject-default.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/configs/pyproject-plugin-bad-param.toml` & `pydantic-2.7.2/tests/mypy/configs/pyproject-plugin-bad-param.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/configs/pyproject-plugin-no-strict-optional.toml` & `pydantic-2.7.2/tests/mypy/configs/pyproject-plugin-no-strict-optional.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/configs/pyproject-plugin-strict-equality.toml` & `pydantic-2.7.2/tests/mypy/configs/pyproject-plugin-strict-equality.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/configs/pyproject-plugin-strict.toml` & `pydantic-2.7.2/tests/mypy/configs/pyproject-plugin-strict.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/configs/pyproject-plugin.toml` & `pydantic-2.7.2/tests/mypy/configs/pyproject-plugin.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/computed_fields.py` & `pydantic-2.7.2/tests/mypy/modules/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/fail4.py` & `pydantic-2.7.2/tests/mypy/modules/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/generics.py` & `pydantic-2.7.2/tests/mypy/modules/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/metaclass_args.py` & `pydantic-2.7.2/tests/mypy/modules/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/plugin_default_factory.py` & `pydantic-2.7.2/tests/mypy/modules/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/modules/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/modules/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/plugin_success.py` & `pydantic-2.7.2/tests/mypy/modules/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/plugin_success_baseConfig.py` & `pydantic-2.7.2/tests/mypy/modules/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/modules/success.py` & `pydantic-2.7.2/tests/mypy/modules/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py` & `pydantic-2.7.2/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py` & `pydantic-2.7.2/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py` & `pydantic-2.7.2/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/plugin/example_plugin.py` & `pydantic-2.7.2/tests/plugin/example_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/plugin/test_plugin.py` & `pydantic-2.7.2/tests/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/tests/pyright/pyright_example.py` & `pydantic-2.7.2/tests/pyright/pyright_example.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/.gitignore` & `pydantic-2.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/LICENSE` & `pydantic-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-2.7.1/pyproject.toml` & `pydantic-2.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 requires-python = '>=3.8'
 dependencies = [
     'typing-extensions>=4.6.1',
     'annotated-types>=0.4.0',
-    "pydantic-core==2.18.2",
+    "pydantic-core==2.18.3",
 ]
 dynamic = ['version', 'readme']
 
 [project.optional-dependencies]
 email = ['email-validator>=2.0.0']
 
 [project.urls]
```

### Comparing `pydantic-2.7.1/PKG-INFO` & `pydantic-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydantic
-Version: 2.7.1
+Version: 2.7.2
 Summary: Data validation using Python type hints
 Project-URL: Homepage, https://github.com/pydantic/pydantic
 Project-URL: Documentation, https://docs.pydantic.dev
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic
 Project-URL: Changelog, https://docs.pydantic.dev/latest/changelog/
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Terrence Dorsey <terry@pydantic.dev>, David Montague <david@pydantic.dev>, Serge Matveenko <lig@countzero.co>, Marcelo Trylesinski <marcelotryle@gmail.com>, Sydney Runkle <sydneymarierunkle@gmail.com>, David Hewitt <mail@davidhewitt.io>, Alex Hall <alex.mojaki@gmail.com>
@@ -31,15 +31,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: annotated-types>=0.4.0
-Requires-Dist: pydantic-core==2.18.2
+Requires-Dist: pydantic-core==2.18.3
 Requires-Dist: typing-extensions>=4.6.1
 Provides-Extra: email
 Requires-Dist: email-validator>=2.0.0; extra == 'email'
 Description-Content-Type: text/markdown
 
 # Pydantic
 
@@ -109,23 +109,41 @@
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
 
 ## Changelog
 
+## v2.7.2 (2024-05-28)
+
+[GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.7.2)
+
+### What's Changed
+
+#### Packaging
+
+* Bump `pydantic-core` to `v2.18.3` by [@sydney-runkle](https://github.com/sydney-runkle) in [#9515](https://github.com/pydantic/pydantic/pull/9515)
+
+#### Fixes
+
+* Replace `__spec__.parent` with `__package__` by [@hramezani](https://github.com/hramezani) in [#9331](https://github.com/pydantic/pydantic/pull/9331)
+* Fix validation of `int`s with leading unary minus by [@RajatRajdeep](https://github.com/RajatRajdeep) in [pydantic/pydantic-core#1291](https://github.com/pydantic/pydantic-core/pull/1291)
+* Fix `str` subclass validation for enums by [@sydney-runkle](https://github.com/sydney-runkle) in [pydantic/pydantic-core#1273]https://github.com/pydantic/pydantic-core/pull/1273
+* Support `BigInt`s in `Literal`s and `Enum`s by [@samuelcolvin](https://github.com/samuelcolvin) in [pydantic/pydantic-core#1297]https://github.com/pydantic/pydantic-core/pull/1297
+* Fix: uuid - allow `str` subclass as input by [@davidhewitt](https://github.com/davidhewitt) in [pydantic/pydantic-core#1296]https://github.com/pydantic/pydantic-core/pull/1296
+
 ## v2.7.1 (2024-04-23)
 
 [GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.7.1)
 
 ### What's Changed
 
 #### Packaging
 
-* Bump `pydantic-core` to `v2.18.2` by [@sydney-runkle](https://github.com/sydney-runkle) in [#9307](https://github.com/pydantic/pydantic/pull/9307)
+* Bump `pydantic-core` to `v2.18.3` by [@sydney-runkle](https://github.com/sydney-runkle) in [#9307](https://github.com/pydantic/pydantic/pull/9307)
 
 #### New Features
 
 * Ftp and Websocket connection strings support by [@CherrySuryp](https://github.com/CherrySuryp) in [#9205](https://github.com/pydantic/pydantic/pull/9205)
 
 #### Changes
```

