# Comparing `tmp/bioimageio.spec-0.5.2.post5.tar.gz` & `tmp/bioimageio.spec-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.spec-0.5.2.post5.tar", last modified: Wed May 15 11:32:41 2024, max compression
+gzip compressed data, was "bioimageio.spec-0.5.3.tar", last modified: Tue May 28 12:15:13 2024, max compression
```

## Comparing `bioimageio.spec-0.5.2.post5.tar` & `bioimageio.spec-0.5.3.tar`

### file list

```diff
@@ -1,139 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.367090 bioimageio.spec-0.5.2.post5/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.375090 bioimageio.spec-0.5.2.post5/bioimageio/spec/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_build_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.375090 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/_generated_spdx_license_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/common_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/docs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/field_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/field_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    20517 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/packaging_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/root_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validation_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validator_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/warning_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/application/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/application/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/application/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12933 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/v0_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/_v0_2_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/_v0_4_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41555 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)   101042 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/v0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/imjoy/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/imjoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/pretty_validation_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/static/
--rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/static/spdx_licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/static/tag_categories.json
--rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.371090 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.371090 bioimageio.spec-0.5.2.post5/example_descriptions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.371090 bioimageio.spec-0.5.2.post5/example_descriptions/collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/example_descriptions/collections/unet2d_nuclei_broad_coll/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.371090 bioimageio.spec-0.5.2.post5/example_descriptions/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_diff_output_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_fixed_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_fixed_shape/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_multi_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/upsample_test_model/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/upsample_test_model/upsample_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/compare_yaml_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/generate_dtype_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/generate_spec_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/generate_version_submodule_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/report_invalid_rdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/update_spdx_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_bioimageio_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_example_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/tests/test_generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_generic/test_v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_generic/test_v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/tests/test_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_file_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/tests/test_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_model/test_v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_model/test_v0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_specific_reexports_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.431631 bioimageio.spec-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20683 2024-05-28 12:15:13.431631 bioimageio.spec-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19860 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.415631 bioimageio.spec-0.5.3/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.419631 bioimageio.spec-0.5.3/bioimageio/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_build_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.423631 bioimageio.spec-0.5.3/bioimageio/spec/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/_generated_spdx_license_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/common_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/field_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/field_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20517 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/io_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/packaging_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/root_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/validation_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/validator_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_internal/warning_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.423631 bioimageio.spec-0.5.3/bioimageio/spec/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/application/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/application/v0_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.423631 bioimageio.spec-0.5.3/bioimageio/spec/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/dataset/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/dataset/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.423631 bioimageio.spec-0.5.3/bioimageio/spec/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/generic/_v0_2_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/generic/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/generic/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/generic/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.423631 bioimageio.spec-0.5.3/bioimageio/spec/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/model/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/model/_v0_4_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41555 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/model/v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100963 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/model/v0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/bioimageio/spec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/notebook/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/bioimageio/spec/notebook/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/bioimageio/spec/partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/partner_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/bioimageio/spec/partner_utils/imjoy/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/partner_utils/imjoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/pretty_validation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/bioimageio/spec/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   171346 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/static/spdx_licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/static/tag_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/bioimageio/spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.419631 bioimageio.spec-0.5.3/bioimageio.spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20683 2024-05-28 12:15:13.000000 bioimageio.spec-0.5.3/bioimageio.spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-28 12:15:13.000000 bioimageio.spec-0.5.3/bioimageio.spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:15:13.000000 bioimageio.spec-0.5.3/bioimageio.spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 12:15:13.000000 bioimageio.spec-0.5.3/bioimageio.spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 12:15:13.000000 bioimageio.spec-0.5.3/bioimageio.spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.415631 bioimageio.spec-0.5.3/example_descriptions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.415631 bioimageio.spec-0.5.3/example_descriptions/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_diff_output_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_fixed_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_fixed_shape/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_multi_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-28 12:13:09.000000 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_nuclei_broad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/example_descriptions/models/upsample_test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/example_descriptions/models/upsample_test_model/upsample_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.427631 bioimageio.spec-0.5.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/scripts/compare_yaml_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/scripts/generate_dtype_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/scripts/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/scripts/generate_spec_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/scripts/generate_version_submodule_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/scripts/report_invalid_rdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/scripts/update_spdx_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/scripts/update_spdx_licenses_zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:15:13.431631 bioimageio.spec-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.431631 bioimageio.spec-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_bioimageio_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_example_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.431631 bioimageio.spec-0.5.3/tests/test_generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_generic/test_v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_generic/test_v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.431631 bioimageio.spec-0.5.3/tests/test_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_internal/test_version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:13.431631 bioimageio.spec-0.5.3/tests/test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/tests/test_model/test_format_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_model/test_v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/tests/test_model/test_v0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-28 12:13:10.000000 bioimageio.spec-0.5.3/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/tests/test_specific_reexports_generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 12:15:10.000000 bioimageio.spec-0.5.3/tests/test_utils.py
```

### Comparing `bioimageio.spec-0.5.2.post5/LICENSE` & `bioimageio.spec-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/PKG-INFO` & `bioimageio.spec-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.2.post5
+Version: 0.5.3
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -122,14 +122,22 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.3
+
+* remove collection description
+* update SPDX license list
+* update generic description to 0.3.1
+* update model description to 0.5.3
+* add timeout argument to all requests.get calls
+
 #### bioimageio.spec 0.5.2post5
 
 * added more information to validation summary
 * deprioritize `Path` objects in the `FileSource` union
 
 #### bioimageio.spec 0.5.2post4
 
@@ -296,14 +304,19 @@
 
 #### bioimageio.spec 0.4.0.post2
 
 * `load_raw_resource_description` accepts `update_to_format` kwarg
 
 ### Resource Description Format Versions
 
+#### general 0.3.1 and model 0.5.3
+
+* Non-breaking changes
+  * remove `version_number` in favor of using `version`
+
 #### model 0.5.2
 
 * Non-breaking changes
   * added `concatenable` flag to index, time and space input axes
 
 #### model 0.5.1
```

### Comparing `bioimageio.spec-0.5.2.post5/README.md` & `bioimageio.spec-0.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,22 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.3
+
+* remove collection description
+* update SPDX license list
+* update generic description to 0.3.1
+* update model description to 0.5.3
+* add timeout argument to all requests.get calls
+
 #### bioimageio.spec 0.5.2post5
 
 * added more information to validation summary
 * deprioritize `Path` objects in the `FileSource` union
 
 #### bioimageio.spec 0.5.2post4
 
@@ -275,14 +283,19 @@
 
 #### bioimageio.spec 0.4.0.post2
 
 * `load_raw_resource_description` accepts `update_to_format` kwarg
 
 ### Resource Description Format Versions
 
+#### general 0.3.1 and model 0.5.3
+
+* Non-breaking changes
+  * remove `version_number` in favor of using `version`
+
 #### model 0.5.2
 
 * Non-breaking changes
   * added `concatenable` flag to index, time and space input axes
 
 #### model 0.5.1
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/__init__.py` & `bioimageio.spec-0.5.3/bioimageio/spec/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 .. include:: ../../README.md
 """
 
 from . import application as application
-from . import collection as collection
 from . import dataset as dataset
 from . import generic as generic
 from . import model as model
 from ._description import LatestResourceDescr as LatestResourceDescr
 from ._description import ResourceDescr as ResourceDescr
 from ._description import SpecificResourceDescr as SpecificResourceDescr
 from ._description import build_description as build_description
@@ -27,16 +26,14 @@
     save_bioimageio_package_as_folder as save_bioimageio_package_as_folder,
 )
 from ._package import (
     save_bioimageio_package_to_stream as save_bioimageio_package_to_stream,
 )
 from .application import AnyApplicationDescr as AnyApplicationDescr
 from .application import ApplicationDescr as ApplicationDescr
-from .collection import AnyCollectionDescr as AnyCollectionDescr
-from .collection import CollectionDescr as CollectionDescr
 from .dataset import AnyDatasetDescr as AnyDatasetDescr
 from .dataset import DatasetDescr as DatasetDescr
 from .generic import AnyGenericDescr as AnyGenericDescr
 from .generic import GenericDescr as GenericDescr
 from .model import AnyModelDescr as AnyModelDescr
 from .model import ModelDescr as ModelDescr
 from .notebook import AnyNotebookDescr as AnyNotebookDescr
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_build_description.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_build_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_description.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_description.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 from ._internal.common_nodes import InvalidDescr
 from ._internal.io import BioimageioYamlContent, BioimageioYamlSource
 from ._internal.types import FormatVersionPlaceholder
 from ._internal.validation_context import ValidationContext, validation_context_var
 from .application import AnyApplicationDescr, ApplicationDescr
 from .application.v0_2 import ApplicationDescr as ApplicationDescr02
 from .application.v0_3 import ApplicationDescr as ApplicationDescr03
-from .collection import AnyCollectionDescr, CollectionDescr
-from .collection.v0_2 import CollectionDescr as CollectionDescr02
-from .collection.v0_3 import CollectionDescr as CollectionDescr03
 from .dataset import AnyDatasetDescr, DatasetDescr
 from .dataset.v0_2 import DatasetDescr as DatasetDescr02
 from .dataset.v0_3 import DatasetDescr as DatasetDescr03
 from .generic import AnyGenericDescr, GenericDescr
 from .generic.v0_2 import GenericDescr as GenericDescr02
 from .generic.v0_3 import GenericDescr as GenericDescr03
 from .model import AnyModelDescr, ModelDescr
@@ -34,30 +31,28 @@
 """placeholder for the latest available format version"""
 
 
 LatestResourceDescr = Union[
     Annotated[
         Union[
             ApplicationDescr,
-            CollectionDescr,
             DatasetDescr,
             ModelDescr,
             NotebookDescr,
         ],
         Discriminator("type"),
     ],
     GenericDescr,
 ]
 """A resource description following the latest specification format"""
 
 
 SpecificResourceDescr = Annotated[
     Union[
         AnyApplicationDescr,
-        AnyCollectionDescr,
         AnyDatasetDescr,
         AnyModelDescr,
         AnyNotebookDescr,
     ],
     Discriminator("type"),
 ]
 """Any of the implemented, non-generic resource descriptions"""
@@ -95,21 +90,14 @@
         "application": MappingProxyType(
             {
                 "0.2": ApplicationDescr02,
                 "0.3": ApplicationDescr03,
                 None: ApplicationDescr,
             }
         ),
-        "collection": MappingProxyType(
-            {
-                "0.2": CollectionDescr02,
-                "0.3": CollectionDescr03,
-                None: CollectionDescr,
-            }
-        ),
         "dataset": MappingProxyType(
             {
                 "0.2": DatasetDescr02,
                 "0.3": DatasetDescr03,
                 None: DatasetDescr,
             }
         ),
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/_generated_spdx_license_literals.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/_generated_spdx_license_literals.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,565 +1,645 @@
-# This file was generated by scripts/update_spdx_licenses.py
-from typing import Literal
-
-LicenseId = Literal[
-    "0BSD",
-    "AAL",
-    "Abstyles",
-    "AdaCore-doc",
-    "Adobe-2006",
-    "Adobe-Glyph",
-    "ADSL",
-    "AFL-1.1",
-    "AFL-1.2",
-    "AFL-2.0",
-    "AFL-2.1",
-    "AFL-3.0",
-    "Afmparse",
-    "AGPL-1.0-only",
-    "AGPL-1.0-or-later",
-    "AGPL-3.0-only",
-    "AGPL-3.0-or-later",
-    "Aladdin",
-    "AMDPLPA",
-    "AML",
-    "AMPAS",
-    "ANTLR-PD",
-    "ANTLR-PD-fallback",
-    "Apache-1.0",
-    "Apache-1.1",
-    "Apache-2.0",
-    "APAFML",
-    "APL-1.0",
-    "App-s2p",
-    "APSL-1.0",
-    "APSL-1.1",
-    "APSL-1.2",
-    "APSL-2.0",
-    "Arphic-1999",
-    "Artistic-1.0",
-    "Artistic-1.0-cl8",
-    "Artistic-1.0-Perl",
-    "Artistic-2.0",
-    "ASWF-Digital-Assets-1.0",
-    "ASWF-Digital-Assets-1.1",
-    "Baekmuk",
-    "Bahyph",
-    "Barr",
-    "Beerware",
-    "Bitstream-Charter",
-    "Bitstream-Vera",
-    "BitTorrent-1.0",
-    "BitTorrent-1.1",
-    "blessing",
-    "BlueOak-1.0.0",
-    "Boehm-GC",
-    "Borceux",
-    "Brian-Gladman-3-Clause",
-    "BSD-1-Clause",
-    "BSD-2-Clause",
-    "BSD-2-Clause-Patent",
-    "BSD-2-Clause-Views",
-    "BSD-3-Clause",
-    "BSD-3-Clause-Attribution",
-    "BSD-3-Clause-Clear",
-    "BSD-3-Clause-LBNL",
-    "BSD-3-Clause-Modification",
-    "BSD-3-Clause-No-Military-License",
-    "BSD-3-Clause-No-Nuclear-License",
-    "BSD-3-Clause-No-Nuclear-License-2014",
-    "BSD-3-Clause-No-Nuclear-Warranty",
-    "BSD-3-Clause-Open-MPI",
-    "BSD-4-Clause",
-    "BSD-4-Clause-Shortened",
-    "BSD-4-Clause-UC",
-    "BSD-4.3RENO",
-    "BSD-4.3TAHOE",
-    "BSD-Advertising-Acknowledgement",
-    "BSD-Attribution-HPND-disclaimer",
-    "BSD-Protection",
-    "BSD-Source-Code",
-    "BSL-1.0",
-    "BUSL-1.1",
-    "bzip2-1.0.6",
-    "C-UDA-1.0",
-    "CAL-1.0",
-    "CAL-1.0-Combined-Work-Exception",
-    "Caldera",
-    "CATOSL-1.1",
-    "CC-BY-1.0",
-    "CC-BY-2.0",
-    "CC-BY-2.5",
-    "CC-BY-2.5-AU",
-    "CC-BY-3.0",
-    "CC-BY-3.0-AT",
-    "CC-BY-3.0-DE",
-    "CC-BY-3.0-IGO",
-    "CC-BY-3.0-NL",
-    "CC-BY-3.0-US",
-    "CC-BY-4.0",
-    "CC-BY-NC-1.0",
-    "CC-BY-NC-2.0",
-    "CC-BY-NC-2.5",
-    "CC-BY-NC-3.0",
-    "CC-BY-NC-3.0-DE",
-    "CC-BY-NC-4.0",
-    "CC-BY-NC-ND-1.0",
-    "CC-BY-NC-ND-2.0",
-    "CC-BY-NC-ND-2.5",
-    "CC-BY-NC-ND-3.0",
-    "CC-BY-NC-ND-3.0-DE",
-    "CC-BY-NC-ND-3.0-IGO",
-    "CC-BY-NC-ND-4.0",
-    "CC-BY-NC-SA-1.0",
-    "CC-BY-NC-SA-2.0",
-    "CC-BY-NC-SA-2.0-DE",
-    "CC-BY-NC-SA-2.0-FR",
-    "CC-BY-NC-SA-2.0-UK",
-    "CC-BY-NC-SA-2.5",
-    "CC-BY-NC-SA-3.0",
-    "CC-BY-NC-SA-3.0-DE",
-    "CC-BY-NC-SA-3.0-IGO",
-    "CC-BY-NC-SA-4.0",
-    "CC-BY-ND-1.0",
-    "CC-BY-ND-2.0",
-    "CC-BY-ND-2.5",
-    "CC-BY-ND-3.0",
-    "CC-BY-ND-3.0-DE",
-    "CC-BY-ND-4.0",
-    "CC-BY-SA-1.0",
-    "CC-BY-SA-2.0",
-    "CC-BY-SA-2.0-UK",
-    "CC-BY-SA-2.1-JP",
-    "CC-BY-SA-2.5",
-    "CC-BY-SA-3.0",
-    "CC-BY-SA-3.0-AT",
-    "CC-BY-SA-3.0-DE",
-    "CC-BY-SA-3.0-IGO",
-    "CC-BY-SA-4.0",
-    "CC-PDDC",
-    "CC0-1.0",
-    "CDDL-1.0",
-    "CDDL-1.1",
-    "CDL-1.0",
-    "CDLA-Permissive-1.0",
-    "CDLA-Permissive-2.0",
-    "CDLA-Sharing-1.0",
-    "CECILL-1.0",
-    "CECILL-1.1",
-    "CECILL-2.0",
-    "CECILL-2.1",
-    "CECILL-B",
-    "CECILL-C",
-    "CERN-OHL-1.1",
-    "CERN-OHL-1.2",
-    "CERN-OHL-P-2.0",
-    "CERN-OHL-S-2.0",
-    "CERN-OHL-W-2.0",
-    "CFITSIO",
-    "checkmk",
-    "ClArtistic",
-    "Clips",
-    "CMU-Mach",
-    "CNRI-Jython",
-    "CNRI-Python",
-    "CNRI-Python-GPL-Compatible",
-    "COIL-1.0",
-    "Community-Spec-1.0",
-    "Condor-1.1",
-    "copyleft-next-0.3.0",
-    "copyleft-next-0.3.1",
-    "Cornell-Lossless-JPEG",
-    "CPAL-1.0",
-    "CPL-1.0",
-    "CPOL-1.02",
-    "Crossword",
-    "CrystalStacker",
-    "CUA-OPL-1.0",
-    "Cube",
-    "curl",
-    "D-FSL-1.0",
-    "diffmark",
-    "DL-DE-BY-2.0",
-    "DOC",
-    "Dotseqn",
-    "DRL-1.0",
-    "DSDP",
-    "dtoa",
-    "dvipdfm",
-    "ECL-1.0",
-    "ECL-2.0",
-    "EFL-1.0",
-    "EFL-2.0",
-    "eGenix",
-    "Elastic-2.0",
-    "Entessa",
-    "EPICS",
-    "EPL-1.0",
-    "EPL-2.0",
-    "ErlPL-1.1",
-    "etalab-2.0",
-    "EUDatagrid",
-    "EUPL-1.0",
-    "EUPL-1.1",
-    "EUPL-1.2",
-    "Eurosym",
-    "Fair",
-    "FDK-AAC",
-    "Frameworx-1.0",
-    "FreeBSD-DOC",
-    "FreeImage",
-    "FSFAP",
-    "FSFUL",
-    "FSFULLR",
-    "FSFULLRWD",
-    "FTL",
-    "GD",
-    "GFDL-1.1-invariants-only",
-    "GFDL-1.1-invariants-or-later",
-    "GFDL-1.1-no-invariants-only",
-    "GFDL-1.1-no-invariants-or-later",
-    "GFDL-1.1-only",
-    "GFDL-1.1-or-later",
-    "GFDL-1.2-invariants-only",
-    "GFDL-1.2-invariants-or-later",
-    "GFDL-1.2-no-invariants-only",
-    "GFDL-1.2-no-invariants-or-later",
-    "GFDL-1.2-only",
-    "GFDL-1.2-or-later",
-    "GFDL-1.3-invariants-only",
-    "GFDL-1.3-invariants-or-later",
-    "GFDL-1.3-no-invariants-only",
-    "GFDL-1.3-no-invariants-or-later",
-    "GFDL-1.3-only",
-    "GFDL-1.3-or-later",
-    "Giftware",
-    "GL2PS",
-    "Glide",
-    "Glulxe",
-    "GLWTPL",
-    "gnuplot",
-    "GPL-1.0-only",
-    "GPL-1.0-or-later",
-    "GPL-2.0-only",
-    "GPL-2.0-or-later",
-    "GPL-3.0-only",
-    "GPL-3.0-or-later",
-    "Graphics-Gems",
-    "gSOAP-1.3b",
-    "HaskellReport",
-    "Hippocratic-2.1",
-    "HP-1986",
-    "HPND",
-    "HPND-export-US",
-    "HPND-Markus-Kuhn",
-    "HPND-sell-variant",
-    "HPND-sell-variant-MIT-disclaimer",
-    "HTMLTIDY",
-    "IBM-pibs",
-    "ICU",
-    "IEC-Code-Components-EULA",
-    "IJG",
-    "IJG-short",
-    "ImageMagick",
-    "iMatix",
-    "Imlib2",
-    "Info-ZIP",
-    "Inner-Net-2.0",
-    "Intel",
-    "Intel-ACPI",
-    "Interbase-1.0",
-    "IPA",
-    "IPL-1.0",
-    "ISC",
-    "Jam",
-    "JasPer-2.0",
-    "JPL-image",
-    "JPNIC",
-    "JSON",
-    "Kazlib",
-    "Knuth-CTAN",
-    "LAL-1.2",
-    "LAL-1.3",
-    "Latex2e",
-    "Latex2e-translated-notice",
-    "Leptonica",
-    "LGPL-2.0-only",
-    "LGPL-2.0-or-later",
-    "LGPL-2.1-only",
-    "LGPL-2.1-or-later",
-    "LGPL-3.0-only",
-    "LGPL-3.0-or-later",
-    "LGPLLR",
-    "Libpng",
-    "libpng-2.0",
-    "libselinux-1.0",
-    "libtiff",
-    "libutil-David-Nugent",
-    "LiLiQ-P-1.1",
-    "LiLiQ-R-1.1",
-    "LiLiQ-Rplus-1.1",
-    "Linux-man-pages-1-para",
-    "Linux-man-pages-copyleft",
-    "Linux-man-pages-copyleft-2-para",
-    "Linux-man-pages-copyleft-var",
-    "Linux-OpenIB",
-    "LOOP",
-    "LPL-1.0",
-    "LPL-1.02",
-    "LPPL-1.0",
-    "LPPL-1.1",
-    "LPPL-1.2",
-    "LPPL-1.3a",
-    "LPPL-1.3c",
-    "LZMA-SDK-9.11-to-9.20",
-    "LZMA-SDK-9.22",
-    "MakeIndex",
-    "Martin-Birgmeier",
-    "metamail",
-    "Minpack",
-    "MirOS",
-    "MIT",
-    "MIT-0",
-    "MIT-advertising",
-    "MIT-CMU",
-    "MIT-enna",
-    "MIT-feh",
-    "MIT-Festival",
-    "MIT-Modern-Variant",
-    "MIT-open-group",
-    "MIT-Wu",
-    "MITNFA",
-    "Motosoto",
-    "mpi-permissive",
-    "mpich2",
-    "MPL-1.0",
-    "MPL-1.1",
-    "MPL-2.0",
-    "MPL-2.0-no-copyleft-exception",
-    "mplus",
-    "MS-LPL",
-    "MS-PL",
-    "MS-RL",
-    "MTLL",
-    "MulanPSL-1.0",
-    "MulanPSL-2.0",
-    "Multics",
-    "Mup",
-    "NAIST-2003",
-    "NASA-1.3",
-    "Naumen",
-    "NBPL-1.0",
-    "NCGL-UK-2.0",
-    "NCSA",
-    "Net-SNMP",
-    "NetCDF",
-    "Newsletr",
-    "NGPL",
-    "NICTA-1.0",
-    "NIST-PD",
-    "NIST-PD-fallback",
-    "NIST-Software",
-    "NLOD-1.0",
-    "NLOD-2.0",
-    "NLPL",
-    "Nokia",
-    "NOSL",
-    "Noweb",
-    "NPL-1.0",
-    "NPL-1.1",
-    "NPOSL-3.0",
-    "NRL",
-    "NTP",
-    "NTP-0",
-    "O-UDA-1.0",
-    "OCCT-PL",
-    "OCLC-2.0",
-    "ODbL-1.0",
-    "ODC-By-1.0",
-    "OFFIS",
-    "OFL-1.0",
-    "OFL-1.0-no-RFN",
-    "OFL-1.0-RFN",
-    "OFL-1.1",
-    "OFL-1.1-no-RFN",
-    "OFL-1.1-RFN",
-    "OGC-1.0",
-    "OGDL-Taiwan-1.0",
-    "OGL-Canada-2.0",
-    "OGL-UK-1.0",
-    "OGL-UK-2.0",
-    "OGL-UK-3.0",
-    "OGTSL",
-    "OLDAP-1.1",
-    "OLDAP-1.2",
-    "OLDAP-1.3",
-    "OLDAP-1.4",
-    "OLDAP-2.0",
-    "OLDAP-2.0.1",
-    "OLDAP-2.1",
-    "OLDAP-2.2",
-    "OLDAP-2.2.1",
-    "OLDAP-2.2.2",
-    "OLDAP-2.3",
-    "OLDAP-2.4",
-    "OLDAP-2.5",
-    "OLDAP-2.6",
-    "OLDAP-2.7",
-    "OLDAP-2.8",
-    "OLFL-1.3",
-    "OML",
-    "OpenPBS-2.3",
-    "OpenSSL",
-    "OPL-1.0",
-    "OPL-UK-3.0",
-    "OPUBL-1.0",
-    "OSET-PL-2.1",
-    "OSL-1.0",
-    "OSL-1.1",
-    "OSL-2.0",
-    "OSL-2.1",
-    "OSL-3.0",
-    "Parity-6.0.0",
-    "Parity-7.0.0",
-    "PDDL-1.0",
-    "PHP-3.0",
-    "PHP-3.01",
-    "Plexus",
-    "PolyForm-Noncommercial-1.0.0",
-    "PolyForm-Small-Business-1.0.0",
-    "PostgreSQL",
-    "PSF-2.0",
-    "psfrag",
-    "psutils",
-    "Python-2.0",
-    "Python-2.0.1",
-    "Qhull",
-    "QPL-1.0",
-    "QPL-1.0-INRIA-2004",
-    "Rdisc",
-    "RHeCos-1.1",
-    "RPL-1.1",
-    "RPL-1.5",
-    "RPSL-1.0",
-    "RSA-MD",
-    "RSCPL",
-    "Ruby",
-    "SAX-PD",
-    "Saxpath",
-    "SCEA",
-    "SchemeReport",
-    "Sendmail",
-    "Sendmail-8.23",
-    "SGI-B-1.0",
-    "SGI-B-1.1",
-    "SGI-B-2.0",
-    "SGP4",
-    "SHL-0.5",
-    "SHL-0.51",
-    "SimPL-2.0",
-    "SISSL",
-    "SISSL-1.2",
-    "Sleepycat",
-    "SMLNJ",
-    "SMPPL",
-    "SNIA",
-    "snprintf",
-    "Spencer-86",
-    "Spencer-94",
-    "Spencer-99",
-    "SPL-1.0",
-    "SSH-OpenSSH",
-    "SSH-short",
-    "SSPL-1.0",
-    "SugarCRM-1.1.3",
-    "SunPro",
-    "SWL",
-    "Symlinks",
-    "TAPR-OHL-1.0",
-    "TCL",
-    "TCP-wrappers",
-    "TermReadKey",
-    "TMate",
-    "TORQUE-1.1",
-    "TOSL",
-    "TPDL",
-    "TPL-1.0",
-    "TTWL",
-    "TU-Berlin-1.0",
-    "TU-Berlin-2.0",
-    "UCAR",
-    "UCL-1.0",
-    "Unicode-DFS-2015",
-    "Unicode-DFS-2016",
-    "Unicode-TOU",
-    "UnixCrypt",
-    "Unlicense",
-    "UPL-1.0",
-    "Vim",
-    "VOSTROM",
-    "VSL-1.0",
-    "W3C",
-    "W3C-19980720",
-    "W3C-20150513",
-    "w3m",
-    "Watcom-1.0",
-    "Widget-Workshop",
-    "Wsuipa",
-    "WTFPL",
-    "X11",
-    "X11-distribute-modifications-variant",
-    "Xdebug-1.03",
-    "Xerox",
-    "Xfig",
-    "XFree86-1.1",
-    "xinetd",
-    "xlock",
-    "Xnet",
-    "xpp",
-    "XSkat",
-    "YPL-1.0",
-    "YPL-1.1",
-    "Zed",
-    "Zend-2.0",
-    "Zimbra-1.3",
-    "Zimbra-1.4",
-    "Zlib",
-    "zlib-acknowledgement",
-    "ZPL-1.1",
-    "ZPL-2.0",
-    "ZPL-2.1",
-]
-
-DeprecatedLicenseId = Literal[
-    "AGPL-1.0",
-    "AGPL-3.0",
-    "BSD-2-Clause-FreeBSD",
-    "BSD-2-Clause-NetBSD",
-    "bzip2-1.0.5",
-    "eCos-2.0",
-    "GFDL-1.1",
-    "GFDL-1.2",
-    "GFDL-1.3",
-    "GPL-1.0",
-    "GPL-1.0+",
-    "GPL-2.0",
-    "GPL-2.0+",
-    "GPL-2.0-with-autoconf-exception",
-    "GPL-2.0-with-bison-exception",
-    "GPL-2.0-with-classpath-exception",
-    "GPL-2.0-with-font-exception",
-    "GPL-2.0-with-GCC-exception",
-    "GPL-3.0",
-    "GPL-3.0+",
-    "GPL-3.0-with-autoconf-exception",
-    "GPL-3.0-with-GCC-exception",
-    "LGPL-2.0",
-    "LGPL-2.0+",
-    "LGPL-2.1",
-    "LGPL-2.1+",
-    "LGPL-3.0",
-    "LGPL-3.0+",
-    "Nunit",
-    "StandardML-NJ",
-    "wxWindows",
-]
+# This file was generated by scripts/update_spdx_licenses.py
+from typing import Literal
+
+LicenseId = Literal[
+    "0BSD",
+    "AAL",
+    "Abstyles",
+    "AdaCore-doc",
+    "Adobe-2006",
+    "Adobe-Display-PostScript",
+    "Adobe-Glyph",
+    "Adobe-Utopia",
+    "ADSL",
+    "AFL-1.1",
+    "AFL-1.2",
+    "AFL-2.0",
+    "AFL-2.1",
+    "AFL-3.0",
+    "Afmparse",
+    "AGPL-1.0-only",
+    "AGPL-1.0-or-later",
+    "AGPL-3.0-only",
+    "AGPL-3.0-or-later",
+    "Aladdin",
+    "AMDPLPA",
+    "AML",
+    "AML-glslang",
+    "AMPAS",
+    "ANTLR-PD",
+    "ANTLR-PD-fallback",
+    "Apache-1.0",
+    "Apache-1.1",
+    "Apache-2.0",
+    "APAFML",
+    "APL-1.0",
+    "App-s2p",
+    "APSL-1.0",
+    "APSL-1.1",
+    "APSL-1.2",
+    "APSL-2.0",
+    "Arphic-1999",
+    "Artistic-1.0",
+    "Artistic-1.0-cl8",
+    "Artistic-1.0-Perl",
+    "Artistic-2.0",
+    "ASWF-Digital-Assets-1.0",
+    "ASWF-Digital-Assets-1.1",
+    "Baekmuk",
+    "Bahyph",
+    "Barr",
+    "bcrypt-Solar-Designer",
+    "Beerware",
+    "Bitstream-Charter",
+    "Bitstream-Vera",
+    "BitTorrent-1.0",
+    "BitTorrent-1.1",
+    "blessing",
+    "BlueOak-1.0.0",
+    "Boehm-GC",
+    "Borceux",
+    "Brian-Gladman-2-Clause",
+    "Brian-Gladman-3-Clause",
+    "BSD-1-Clause",
+    "BSD-2-Clause",
+    "BSD-2-Clause-Darwin",
+    "BSD-2-Clause-Patent",
+    "BSD-2-Clause-Views",
+    "BSD-3-Clause",
+    "BSD-3-Clause-acpica",
+    "BSD-3-Clause-Attribution",
+    "BSD-3-Clause-Clear",
+    "BSD-3-Clause-flex",
+    "BSD-3-Clause-HP",
+    "BSD-3-Clause-LBNL",
+    "BSD-3-Clause-Modification",
+    "BSD-3-Clause-No-Military-License",
+    "BSD-3-Clause-No-Nuclear-License",
+    "BSD-3-Clause-No-Nuclear-License-2014",
+    "BSD-3-Clause-No-Nuclear-Warranty",
+    "BSD-3-Clause-Open-MPI",
+    "BSD-3-Clause-Sun",
+    "BSD-4-Clause",
+    "BSD-4-Clause-Shortened",
+    "BSD-4-Clause-UC",
+    "BSD-4.3RENO",
+    "BSD-4.3TAHOE",
+    "BSD-Advertising-Acknowledgement",
+    "BSD-Attribution-HPND-disclaimer",
+    "BSD-Inferno-Nettverk",
+    "BSD-Protection",
+    "BSD-Source-beginning-file",
+    "BSD-Source-Code",
+    "BSD-Systemics",
+    "BSD-Systemics-W3Works",
+    "BSL-1.0",
+    "BUSL-1.1",
+    "bzip2-1.0.6",
+    "C-UDA-1.0",
+    "CAL-1.0",
+    "CAL-1.0-Combined-Work-Exception",
+    "Caldera",
+    "Caldera-no-preamble",
+    "CATOSL-1.1",
+    "CC-BY-1.0",
+    "CC-BY-2.0",
+    "CC-BY-2.5",
+    "CC-BY-2.5-AU",
+    "CC-BY-3.0",
+    "CC-BY-3.0-AT",
+    "CC-BY-3.0-AU",
+    "CC-BY-3.0-DE",
+    "CC-BY-3.0-IGO",
+    "CC-BY-3.0-NL",
+    "CC-BY-3.0-US",
+    "CC-BY-4.0",
+    "CC-BY-NC-1.0",
+    "CC-BY-NC-2.0",
+    "CC-BY-NC-2.5",
+    "CC-BY-NC-3.0",
+    "CC-BY-NC-3.0-DE",
+    "CC-BY-NC-4.0",
+    "CC-BY-NC-ND-1.0",
+    "CC-BY-NC-ND-2.0",
+    "CC-BY-NC-ND-2.5",
+    "CC-BY-NC-ND-3.0",
+    "CC-BY-NC-ND-3.0-DE",
+    "CC-BY-NC-ND-3.0-IGO",
+    "CC-BY-NC-ND-4.0",
+    "CC-BY-NC-SA-1.0",
+    "CC-BY-NC-SA-2.0",
+    "CC-BY-NC-SA-2.0-DE",
+    "CC-BY-NC-SA-2.0-FR",
+    "CC-BY-NC-SA-2.0-UK",
+    "CC-BY-NC-SA-2.5",
+    "CC-BY-NC-SA-3.0",
+    "CC-BY-NC-SA-3.0-DE",
+    "CC-BY-NC-SA-3.0-IGO",
+    "CC-BY-NC-SA-4.0",
+    "CC-BY-ND-1.0",
+    "CC-BY-ND-2.0",
+    "CC-BY-ND-2.5",
+    "CC-BY-ND-3.0",
+    "CC-BY-ND-3.0-DE",
+    "CC-BY-ND-4.0",
+    "CC-BY-SA-1.0",
+    "CC-BY-SA-2.0",
+    "CC-BY-SA-2.0-UK",
+    "CC-BY-SA-2.1-JP",
+    "CC-BY-SA-2.5",
+    "CC-BY-SA-3.0",
+    "CC-BY-SA-3.0-AT",
+    "CC-BY-SA-3.0-DE",
+    "CC-BY-SA-3.0-IGO",
+    "CC-BY-SA-4.0",
+    "CC-PDDC",
+    "CC0-1.0",
+    "CDDL-1.0",
+    "CDDL-1.1",
+    "CDL-1.0",
+    "CDLA-Permissive-1.0",
+    "CDLA-Permissive-2.0",
+    "CDLA-Sharing-1.0",
+    "CECILL-1.0",
+    "CECILL-1.1",
+    "CECILL-2.0",
+    "CECILL-2.1",
+    "CECILL-B",
+    "CECILL-C",
+    "CERN-OHL-1.1",
+    "CERN-OHL-1.2",
+    "CERN-OHL-P-2.0",
+    "CERN-OHL-S-2.0",
+    "CERN-OHL-W-2.0",
+    "CFITSIO",
+    "check-cvs",
+    "checkmk",
+    "ClArtistic",
+    "Clips",
+    "CMU-Mach",
+    "CMU-Mach-nodoc",
+    "CNRI-Jython",
+    "CNRI-Python",
+    "CNRI-Python-GPL-Compatible",
+    "COIL-1.0",
+    "Community-Spec-1.0",
+    "Condor-1.1",
+    "copyleft-next-0.3.0",
+    "copyleft-next-0.3.1",
+    "Cornell-Lossless-JPEG",
+    "CPAL-1.0",
+    "CPL-1.0",
+    "CPOL-1.02",
+    "Cronyx",
+    "Crossword",
+    "CrystalStacker",
+    "CUA-OPL-1.0",
+    "Cube",
+    "curl",
+    "D-FSL-1.0",
+    "DEC-3-Clause",
+    "diffmark",
+    "DL-DE-BY-2.0",
+    "DL-DE-ZERO-2.0",
+    "DOC",
+    "Dotseqn",
+    "DRL-1.0",
+    "DRL-1.1",
+    "DSDP",
+    "dtoa",
+    "dvipdfm",
+    "ECL-1.0",
+    "ECL-2.0",
+    "EFL-1.0",
+    "EFL-2.0",
+    "eGenix",
+    "Elastic-2.0",
+    "Entessa",
+    "EPICS",
+    "EPL-1.0",
+    "EPL-2.0",
+    "ErlPL-1.1",
+    "etalab-2.0",
+    "EUDatagrid",
+    "EUPL-1.0",
+    "EUPL-1.1",
+    "EUPL-1.2",
+    "Eurosym",
+    "Fair",
+    "FBM",
+    "FDK-AAC",
+    "Ferguson-Twofish",
+    "Frameworx-1.0",
+    "FreeBSD-DOC",
+    "FreeImage",
+    "FSFAP",
+    "FSFAP-no-warranty-disclaimer",
+    "FSFUL",
+    "FSFULLR",
+    "FSFULLRWD",
+    "FTL",
+    "Furuseth",
+    "fwlw",
+    "GCR-docs",
+    "GD",
+    "GFDL-1.1-invariants-only",
+    "GFDL-1.1-invariants-or-later",
+    "GFDL-1.1-no-invariants-only",
+    "GFDL-1.1-no-invariants-or-later",
+    "GFDL-1.1-only",
+    "GFDL-1.1-or-later",
+    "GFDL-1.2-invariants-only",
+    "GFDL-1.2-invariants-or-later",
+    "GFDL-1.2-no-invariants-only",
+    "GFDL-1.2-no-invariants-or-later",
+    "GFDL-1.2-only",
+    "GFDL-1.2-or-later",
+    "GFDL-1.3-invariants-only",
+    "GFDL-1.3-invariants-or-later",
+    "GFDL-1.3-no-invariants-only",
+    "GFDL-1.3-no-invariants-or-later",
+    "GFDL-1.3-only",
+    "GFDL-1.3-or-later",
+    "Giftware",
+    "GL2PS",
+    "Glide",
+    "Glulxe",
+    "GLWTPL",
+    "gnuplot",
+    "GPL-1.0-only",
+    "GPL-1.0-or-later",
+    "GPL-2.0-only",
+    "GPL-2.0-or-later",
+    "GPL-3.0-only",
+    "GPL-3.0-or-later",
+    "Graphics-Gems",
+    "gSOAP-1.3b",
+    "gtkbook",
+    "HaskellReport",
+    "hdparm",
+    "Hippocratic-2.1",
+    "HP-1986",
+    "HP-1989",
+    "HPND",
+    "HPND-DEC",
+    "HPND-doc",
+    "HPND-doc-sell",
+    "HPND-export-US",
+    "HPND-export-US-modify",
+    "HPND-Fenneberg-Livingston",
+    "HPND-INRIA-IMAG",
+    "HPND-Kevlin-Henney",
+    "HPND-Markus-Kuhn",
+    "HPND-MIT-disclaimer",
+    "HPND-Pbmplus",
+    "HPND-sell-MIT-disclaimer-xserver",
+    "HPND-sell-regexpr",
+    "HPND-sell-variant",
+    "HPND-sell-variant-MIT-disclaimer",
+    "HPND-UC",
+    "HTMLTIDY",
+    "IBM-pibs",
+    "ICU",
+    "IEC-Code-Components-EULA",
+    "IJG",
+    "IJG-short",
+    "ImageMagick",
+    "iMatix",
+    "Imlib2",
+    "Info-ZIP",
+    "Inner-Net-2.0",
+    "Intel",
+    "Intel-ACPI",
+    "Interbase-1.0",
+    "IPA",
+    "IPL-1.0",
+    "ISC",
+    "ISC-Veillard",
+    "Jam",
+    "JasPer-2.0",
+    "JPL-image",
+    "JPNIC",
+    "JSON",
+    "Kastrup",
+    "Kazlib",
+    "Knuth-CTAN",
+    "LAL-1.2",
+    "LAL-1.3",
+    "Latex2e",
+    "Latex2e-translated-notice",
+    "Leptonica",
+    "LGPL-2.0-only",
+    "LGPL-2.0-or-later",
+    "LGPL-2.1-only",
+    "LGPL-2.1-or-later",
+    "LGPL-3.0-only",
+    "LGPL-3.0-or-later",
+    "LGPLLR",
+    "Libpng",
+    "libpng-2.0",
+    "libselinux-1.0",
+    "libtiff",
+    "libutil-David-Nugent",
+    "LiLiQ-P-1.1",
+    "LiLiQ-R-1.1",
+    "LiLiQ-Rplus-1.1",
+    "Linux-man-pages-1-para",
+    "Linux-man-pages-copyleft",
+    "Linux-man-pages-copyleft-2-para",
+    "Linux-man-pages-copyleft-var",
+    "Linux-OpenIB",
+    "LOOP",
+    "LPD-document",
+    "LPL-1.0",
+    "LPL-1.02",
+    "LPPL-1.0",
+    "LPPL-1.1",
+    "LPPL-1.2",
+    "LPPL-1.3a",
+    "LPPL-1.3c",
+    "lsof",
+    "Lucida-Bitmap-Fonts",
+    "LZMA-SDK-9.11-to-9.20",
+    "LZMA-SDK-9.22",
+    "Mackerras-3-Clause",
+    "Mackerras-3-Clause-acknowledgment",
+    "magaz",
+    "mailprio",
+    "MakeIndex",
+    "Martin-Birgmeier",
+    "McPhee-slideshow",
+    "metamail",
+    "Minpack",
+    "MirOS",
+    "MIT",
+    "MIT-0",
+    "MIT-advertising",
+    "MIT-CMU",
+    "MIT-enna",
+    "MIT-feh",
+    "MIT-Festival",
+    "MIT-Modern-Variant",
+    "MIT-open-group",
+    "MIT-testregex",
+    "MIT-Wu",
+    "MITNFA",
+    "MMIXware",
+    "Motosoto",
+    "MPEG-SSG",
+    "mpi-permissive",
+    "mpich2",
+    "MPL-1.0",
+    "MPL-1.1",
+    "MPL-2.0",
+    "MPL-2.0-no-copyleft-exception",
+    "mplus",
+    "MS-LPL",
+    "MS-PL",
+    "MS-RL",
+    "MTLL",
+    "MulanPSL-1.0",
+    "MulanPSL-2.0",
+    "Multics",
+    "Mup",
+    "NAIST-2003",
+    "NASA-1.3",
+    "Naumen",
+    "NBPL-1.0",
+    "NCGL-UK-2.0",
+    "NCSA",
+    "Net-SNMP",
+    "NetCDF",
+    "Newsletr",
+    "NGPL",
+    "NICTA-1.0",
+    "NIST-PD",
+    "NIST-PD-fallback",
+    "NIST-Software",
+    "NLOD-1.0",
+    "NLOD-2.0",
+    "NLPL",
+    "Nokia",
+    "NOSL",
+    "Noweb",
+    "NPL-1.0",
+    "NPL-1.1",
+    "NPOSL-3.0",
+    "NRL",
+    "NTP",
+    "NTP-0",
+    "O-UDA-1.0",
+    "OCCT-PL",
+    "OCLC-2.0",
+    "ODbL-1.0",
+    "ODC-By-1.0",
+    "OFFIS",
+    "OFL-1.0",
+    "OFL-1.0-no-RFN",
+    "OFL-1.0-RFN",
+    "OFL-1.1",
+    "OFL-1.1-no-RFN",
+    "OFL-1.1-RFN",
+    "OGC-1.0",
+    "OGDL-Taiwan-1.0",
+    "OGL-Canada-2.0",
+    "OGL-UK-1.0",
+    "OGL-UK-2.0",
+    "OGL-UK-3.0",
+    "OGTSL",
+    "OLDAP-1.1",
+    "OLDAP-1.2",
+    "OLDAP-1.3",
+    "OLDAP-1.4",
+    "OLDAP-2.0",
+    "OLDAP-2.0.1",
+    "OLDAP-2.1",
+    "OLDAP-2.2",
+    "OLDAP-2.2.1",
+    "OLDAP-2.2.2",
+    "OLDAP-2.3",
+    "OLDAP-2.4",
+    "OLDAP-2.5",
+    "OLDAP-2.6",
+    "OLDAP-2.7",
+    "OLDAP-2.8",
+    "OLFL-1.3",
+    "OML",
+    "OpenPBS-2.3",
+    "OpenSSL",
+    "OpenSSL-standalone",
+    "OpenVision",
+    "OPL-1.0",
+    "OPL-UK-3.0",
+    "OPUBL-1.0",
+    "OSET-PL-2.1",
+    "OSL-1.0",
+    "OSL-1.1",
+    "OSL-2.0",
+    "OSL-2.1",
+    "OSL-3.0",
+    "PADL",
+    "Parity-6.0.0",
+    "Parity-7.0.0",
+    "PDDL-1.0",
+    "PHP-3.0",
+    "PHP-3.01",
+    "Pixar",
+    "Plexus",
+    "pnmstitch",
+    "PolyForm-Noncommercial-1.0.0",
+    "PolyForm-Small-Business-1.0.0",
+    "PostgreSQL",
+    "PSF-2.0",
+    "psfrag",
+    "psutils",
+    "Python-2.0",
+    "Python-2.0.1",
+    "python-ldap",
+    "Qhull",
+    "QPL-1.0",
+    "QPL-1.0-INRIA-2004",
+    "radvd",
+    "Rdisc",
+    "RHeCos-1.1",
+    "RPL-1.1",
+    "RPL-1.5",
+    "RPSL-1.0",
+    "RSA-MD",
+    "RSCPL",
+    "Ruby",
+    "SAX-PD",
+    "SAX-PD-2.0",
+    "Saxpath",
+    "SCEA",
+    "SchemeReport",
+    "Sendmail",
+    "Sendmail-8.23",
+    "SGI-B-1.0",
+    "SGI-B-1.1",
+    "SGI-B-2.0",
+    "SGI-OpenGL",
+    "SGP4",
+    "SHL-0.5",
+    "SHL-0.51",
+    "SimPL-2.0",
+    "SISSL",
+    "SISSL-1.2",
+    "SL",
+    "Sleepycat",
+    "SMLNJ",
+    "SMPPL",
+    "SNIA",
+    "snprintf",
+    "softSurfer",
+    "Soundex",
+    "Spencer-86",
+    "Spencer-94",
+    "Spencer-99",
+    "SPL-1.0",
+    "ssh-keyscan",
+    "SSH-OpenSSH",
+    "SSH-short",
+    "SSLeay-standalone",
+    "SSPL-1.0",
+    "SugarCRM-1.1.3",
+    "Sun-PPP",
+    "SunPro",
+    "SWL",
+    "swrule",
+    "Symlinks",
+    "TAPR-OHL-1.0",
+    "TCL",
+    "TCP-wrappers",
+    "TermReadKey",
+    "TGPPL-1.0",
+    "TMate",
+    "TORQUE-1.1",
+    "TOSL",
+    "TPDL",
+    "TPL-1.0",
+    "TTWL",
+    "TTYP0",
+    "TU-Berlin-1.0",
+    "TU-Berlin-2.0",
+    "UCAR",
+    "UCL-1.0",
+    "ulem",
+    "UMich-Merit",
+    "Unicode-3.0",
+    "Unicode-DFS-2015",
+    "Unicode-DFS-2016",
+    "Unicode-TOU",
+    "UnixCrypt",
+    "Unlicense",
+    "UPL-1.0",
+    "URT-RLE",
+    "Vim",
+    "VOSTROM",
+    "VSL-1.0",
+    "W3C",
+    "W3C-19980720",
+    "W3C-20150513",
+    "w3m",
+    "Watcom-1.0",
+    "Widget-Workshop",
+    "Wsuipa",
+    "WTFPL",
+    "X11",
+    "X11-distribute-modifications-variant",
+    "Xdebug-1.03",
+    "Xerox",
+    "Xfig",
+    "XFree86-1.1",
+    "xinetd",
+    "xkeyboard-config-Zinoviev",
+    "xlock",
+    "Xnet",
+    "xpp",
+    "XSkat",
+    "YPL-1.0",
+    "YPL-1.1",
+    "Zed",
+    "Zeeff",
+    "Zend-2.0",
+    "Zimbra-1.3",
+    "Zimbra-1.4",
+    "Zlib",
+    "zlib-acknowledgement",
+    "ZPL-1.1",
+    "ZPL-2.0",
+    "ZPL-2.1",
+]
+
+DeprecatedLicenseId = Literal[
+    "AGPL-1.0",
+    "AGPL-3.0",
+    "BSD-2-Clause-FreeBSD",
+    "BSD-2-Clause-NetBSD",
+    "bzip2-1.0.5",
+    "eCos-2.0",
+    "GFDL-1.1",
+    "GFDL-1.2",
+    "GFDL-1.3",
+    "GPL-1.0",
+    "GPL-1.0+",
+    "GPL-2.0",
+    "GPL-2.0+",
+    "GPL-2.0-with-autoconf-exception",
+    "GPL-2.0-with-bison-exception",
+    "GPL-2.0-with-classpath-exception",
+    "GPL-2.0-with-font-exception",
+    "GPL-2.0-with-GCC-exception",
+    "GPL-3.0",
+    "GPL-3.0+",
+    "GPL-3.0-with-autoconf-exception",
+    "GPL-3.0-with-GCC-exception",
+    "LGPL-2.0",
+    "LGPL-2.0+",
+    "LGPL-2.1",
+    "LGPL-2.1+",
+    "LGPL-3.0",
+    "LGPL-3.0+",
+    "Nunit",
+    "StandardML-NJ",
+    "wxWindows",
+]
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/_settings.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 
     collection: str = (
         "https://uk1s3.embassy.ebi.ac.uk/public-datasets/bioimage.io/collection.json"
     )
     """url to bioimageio collection.json to resolve collection specific resource IDs.
     """
 
-    collection_staged: str = (
-        "https://uk1s3.embassy.ebi.ac.uk/public-datasets/bioimage.io/collection_staged.json"
+    collection_draft: str = (
+        "https://uk1s3.embassy.ebi.ac.uk/public-datasets/bioimage.io/collection_draft.json"
     )
-    """url to bioimageio collection_staged.json to resolve collection specific, staged
-    resource IDs."""
+    """url to bioimageio collection_draft.json to resolve collection specific draft
+    versions of resources ending with '/draft'."""
 
-    resolve_staged: bool = True
-    """Flag to resolve staged resource versions following the pattern
-    <resource id>/staged/<stage number>.
-    Note that anyone may stage a new resource version and that such a staged version
-    may not have been reviewed.
-    Set this flag to False to avoid this potential security risk."""
+    resolve_draft: bool = True
+    """Flag to resolve draft resource versions following the pattern
+    <resource id>/draft.
+    Note that anyone may stage a new draft and that such a draft version
+    may not have been reviewed yet.
+    Set this flag to False to avoid this potential security risk
+    and disallow loading draft versions."""
 
     perform_io_checks: bool = True
     """wether or not to perform validation that requires file io,
     e.g. downloading a remote files.
 
     Existence of any local absolute file paths is still being checked."""
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/common_nodes.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/common_nodes.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/constants.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 DOI_REGEX = (  # lax DOI regex validating the first 7 DOI characters only
     r"^10\.[0-9]{4}.+$"
 )
 
 IN_PACKAGE_MESSAGE = "∈📦 "
 """DEPRECATED, use ImportantFileSource to indicate that a file source should be included in a package"""
 
-# license file generated with scripts/update_spdx_licenses.py
-with files("bioimageio.spec").joinpath("static/spdx_licenses.json").open(
-    "r", encoding="utf-8"
-) as f:
-    _license_data = json.load(f)
-
 
 SHA256_HINT = """You can drag and drop your file to this
 [online tool](http://emn178.github.io/online-tools/sha256_checksum.html) to generate a SHA256 in your browser.
 Or you can generate a SHA256 checksum with Python's `hashlib`,
 [here is a codesnippet](https://gist.github.com/FynnBe/e64460463df89439cff218bbf59c1100)."""
 
 with files("bioimageio.spec").joinpath("static/tag_categories.json").open(
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/docs_utils.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/docs_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     assert not urlparse(github_file_url).fragment, "unexpected url fragment"
     look_for = {"class": ast.ClassDef, "function": ast.FunctionDef}[type_]
     raw_github_file_url = github_file_url.replace(
         "github.com", "raw.githubusercontent.com"
     ).replace("/blob/", "/")
     try:
-        code = requests.get(raw_github_file_url).text
+        code = requests.get(raw_github_file_url, timeout=5).text
     except requests.RequestException as e:
         warnings.warn(
             f"Could not resolve {github_file_url} due to {e}. Please check your"
             + " internet connection."
         )
         return "URL NOT RESOLVED"
     tree = ast.parse(code)
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/field_validation.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/field_validation.py`

 * *Files 18% similar despite different names*

```diff
@@ -69,21 +69,31 @@
         or not validation_context_var.get().perform_io_checks
     ):
         return username
 
     if username.lower() in KNOWN_INVALID_GH_USERS:
         raise ValueError(f"Known invalid GitHub user '{username}'")
 
-    r = requests.get(
-        f"https://api.github.com/users/{username}", auth=settings.github_auth
-    )
-    if r.status_code == 403 and r.reason == "rate limit exceeded":
+    try:
+        r = requests.get(
+            f"https://api.github.com/users/{username}",
+            auth=settings.github_auth,
+            timeout=3,
+        )
+    except requests.exceptions.Timeout:
         issue_warning(
-            "Could not verify GitHub user '{value}' due to GitHub API rate limit",
+            "Could not verify GitHub user '{value}' due to connection timeout",
             value=username,
         )
-    elif r.status_code != 200:
-        KNOWN_INVALID_GH_USERS.add(username.lower())
-        raise ValueError(f"Could not find GitHub user '{username}'")
+    else:
+        if r.status_code == 403 and r.reason == "rate limit exceeded":
+            issue_warning(
+                "Could not verify GitHub user '{value}' due to GitHub API rate limit",
+                value=username,
+            )
+        elif r.status_code != 200:
+            KNOWN_INVALID_GH_USERS.add(username.lower())
+            raise ValueError(f"Could not find GitHub user '{username}'")
+
+        KNOWN_GH_USERS.add(username.lower())
 
-    KNOWN_GH_USERS.add(username.lower())
     return username
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/field_warning.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/field_warning.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io_basics.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/io_basics.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io_utils.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/io_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,34 +92,34 @@
             or not isinstance(settings.collection, str)
             or "/" not in settings.collection
         ):
             raise
 
         collection = get_collection()
         if source not in collection:
-            if "/staged/" in source:
-                if settings.resolve_staged:
-                    collection_url = settings.collection_staged
+            if isinstance(source, str) and source.endswith("/draft"):
+                if settings.resolve_draft:
+                    collection_url = settings.collection_draft
                 else:
                     collection_url = ""
                     logger.error(
-                        "Did not try to resolve '{}' as BIOIMAGEIO_RESOLVE_STAGED is set to False",
+                        "Did not try to resolve '{}' as BIOIMAGEIO_RESOLVE_DRAFT is set to False",
                         source,
                     )
             else:
                 collection_url = settings.collection
 
             logger.error("'{}' not found in collection {}", source, collection_url)
             raise
 
         entry = collection[source]
         logger.info(
             "{} loading {} {} from {}",
             entry.emoji,
-            entry.id,
+            f"{entry.id}/{entry.version}",
             entry.version,
             entry.url,
         )
         downloaded = download(entry.url, sha256=entry.sha256)
 
     local_source = downloaded.path
     root = downloaded.original_root
@@ -138,105 +138,76 @@
 
 class _CollectionEntry(NamedTuple):
     id: str
     emoji: str
     url: str
     sha256: Optional[Sha256]
     version: str
+    doi: Optional[str]
 
 
 def _get_one_collection(url: str):
     ret: Dict[str, _CollectionEntry] = {}
     if not isinstance(url, str) or "/" not in url:
         logger.error("invalid collection url: {}", url)
     try:
-        collection: List[Dict[Any, Any]] = requests.get(url).json().get("collection")
+        collection: List[Dict[Any, Any]] = (
+            requests.get(url, timeout=5).json().get("collection")
+        )
     except Exception as e:
         logger.error("failed to get {}: {}", url, e)
         return ret
 
     if not isinstance(collection, list):
         logger.error("`collection` field of {} has type {}", url, type(collection))
         return ret
 
-    for entry in collection:
-        if entry["entry_sha256"] is None:
-            logger.debug("skipping {} with entry_sha256=None", entry["id"])
-            continue
-
-        if not isinstance(entry, dict):
-            logger.error("entry has type {}", type(entry))
-            continue
-        if not isinstance(entry["id"], str):
-            logger.error("entry['id'] has type {}", type(entry["id"]))
-            continue
-        if not isinstance(entry["id_emoji"], str):
-            logger.error(
-                "{}.id_emoji has type {}", entry["id"], type(entry["id_emoji"])
+    for raw_entry in collection:
+        try:
+            for i, (v, d) in enumerate(zip(raw_entry["versions"], raw_entry["dois"])):
+                entry = _CollectionEntry(
+                    id=raw_entry["id"],
+                    emoji=raw_entry.get("id_emoji", raw_entry.get("nickname_icon", "")),
+                    url=raw_entry["rdf_source"],
+                    sha256=raw_entry["rdf_sha256"],
+                    version=v,
+                    doi=d,
+                )
+                ret[f"{raw_entry['id']}/{v}"] = entry
+                if i == 0:
+                    # latest version
+                    ret[raw_entry["id"]] = entry
+                    if (concept_doi := raw_entry.get("concept_doi")) is not None:
+                        ret[concept_doi] = entry
+
+                    if (nickname := raw_entry.get("nickname")) is not None:
+                        ret[nickname] = entry
+
+                if d is not None:
+                    ret[d] = entry
+
+        except Exception as e:
+            entry_id = (
+                raw_entry.get("id", "unknown")
+                if isinstance(raw_entry, dict)
+                else "unknown"
             )
-            continue
-        if not isinstance(entry["entry_source"], str):
             logger.error(
-                "{}.entry_source has type {}", entry["id"], type(entry["entry_source"])
+                "failed to parse collection entry with `id={}`: {}", entry_id, e
             )
             continue
-        if not isinstance(entry["entry_sha256"], str):
-            logger.error(
-                "{}.entry_sha256 has type {}", entry["id"], type(entry["entry_sha256"])
-            )
-            continue
-
-        c_entry = _CollectionEntry(
-            entry["id"],
-            entry["id_emoji"],
-            entry["entry_source"],
-            (
-                None
-                if entry.get("entry_sha256") is None
-                else Sha256(entry["entry_sha256"])
-            ),
-            version=str(entry["version_number"]),
-        )
-        # set version specific entry
-        ret[c_entry.id + "/" + str(entry["version_number"])] = c_entry
-
-        # set doi entry
-        doi = entry.get("doi")
-        if doi is not None:
-            ret[doi] = c_entry
-
-        # update 'latest version' entry
-        if c_entry.id not in ret:
-            update = True
-        else:
-            old_v = ret[c_entry.id].version
-            v = c_entry.version
-
-            if old_v.startswith("staged"):
-                update = not v.startswith("staged") or int(
-                    v.replace("staged/", "")
-                ) > int(old_v.replace("staged/", ""))
-            else:
-                update = not v.startswith("staged") and int(v) > int(old_v)
-
-        if update:
-            ret[c_entry.id] = c_entry
-            # set concept doi entry
-            concept_doi = entry.get("concept_doi")
-            if concept_doi is not None:
-                ret[concept_doi] = c_entry
 
     return ret
 
 
 @lru_cache
 def get_collection() -> Mapping[str, _CollectionEntry]:
     try:
-        if settings.resolve_staged:
-            ret = _get_one_collection(settings.collection_staged)
+        if settings.resolve_draft:
+            ret = _get_one_collection(settings.collection_draft)
         else:
             ret = {}
 
         ret.update(_get_one_collection(settings.collection))
         return ret
 
     except Exception as e:
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/license_id.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/node.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/packaging_context.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/packaging_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/root_url.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/root_url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/types.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/url.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         # TODO: improve validation of non-github colab urls
         issue_warning(
             "colab urls currently pass even if the notebook url was not found. Cannot fully validate {value}",
             value=url,
         )
 
     try:
-        response = requests.get(val_url, stream=True, timeout=(3, 3))
+        response = requests.get(val_url, stream=True, timeout=3)
     except (
         requests.exceptions.ChunkedEncodingError,
         requests.exceptions.ContentDecodingError,
         requests.exceptions.InvalidHeader,
         requests.exceptions.InvalidJSONError,
         requests.exceptions.InvalidSchema,
         requests.exceptions.InvalidURL,
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/utils.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validated_string.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validation_context.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/validation_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validator_annotations.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/validator_annotations.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/version_type.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/version_type.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/warning_levels.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_internal/warning_levels.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_io.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/_package.py` & `bioimageio.spec-0.5.3/bioimageio/spec/_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/application/__init__.py` & `bioimageio.spec-0.5.3/bioimageio/spec/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/application/v0_2.py` & `bioimageio.spec-0.5.3/bioimageio/spec/application/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/application/v0_3.py` & `bioimageio.spec-0.5.3/bioimageio/spec/application/v0_3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Literal, Optional
 
 from pydantic import Field
 from typing_extensions import Annotated
 
-from .._internal.common_nodes import Node
 from .._internal.io import FileDescr as FileDescr
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
 from .._internal.io_basics import Sha256 as Sha256
 from .._internal.types import ImportantFileSource
 from .._internal.url import HttpUrl as HttpUrl
 from ..generic.v0_3 import VALID_COVER_IMAGE_EXTENSIONS as VALID_COVER_IMAGE_EXTENSIONS
 from ..generic.v0_3 import Author as Author
 from ..generic.v0_3 import BadgeDescr as BadgeDescr
 from ..generic.v0_3 import CiteEntry as CiteEntry
 from ..generic.v0_3 import Doi as Doi
-from ..generic.v0_3 import GenericDescrBase, ResourceId
+from ..generic.v0_3 import GenericDescrBase, LinkedResourceNode, ResourceId
 from ..generic.v0_3 import LinkedResource as LinkedResource
 from ..generic.v0_3 import Maintainer as Maintainer
 from ..generic.v0_3 import OrcidId as OrcidId
 from ..generic.v0_3 import RelativeFilePath as RelativeFilePath
 from ..generic.v0_3 import Uploader as Uploader
 from ..generic.v0_3 import Version as Version
 
@@ -41,15 +40,12 @@
     source: Annotated[
         Optional[ImportantFileSource],
         Field(description="URL or path to the source of the application"),
     ] = None
     """The primary source of the application"""
 
 
-class LinkedApplication(Node):
+class LinkedApplication(LinkedResourceNode):
     """Reference to a bioimage.io application."""
 
     id: ApplicationId
     """A valid application `id` from the bioimage.io collection."""
-
-    version_number: int
-    """version number (n-th published version, not the semantic version) of linked application"""
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/common.py` & `bioimageio.spec-0.5.3/bioimageio/spec/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/__init__.py` & `bioimageio.spec-0.5.3/bioimageio/spec/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/v0_2.py` & `bioimageio.spec-0.5.3/bioimageio/spec/dataset/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/v0_3.py` & `bioimageio.spec-0.5.3/bioimageio/spec/dataset/v0_3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import TYPE_CHECKING, Any, Dict, Literal, Optional, cast
 
 from pydantic import model_validator
 
-from .._internal.common_nodes import InvalidDescr, Node
+from .._internal.common_nodes import InvalidDescr
 from .._internal.io import FileDescr as FileDescr
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
 from .._internal.io_basics import Sha256 as Sha256
 from .._internal.url import HttpUrl as HttpUrl
 from ..generic.v0_3 import VALID_COVER_IMAGE_EXTENSIONS as VALID_COVER_IMAGE_EXTENSIONS
 from ..generic.v0_3 import Author as Author
 from ..generic.v0_3 import BadgeDescr as BadgeDescr
 from ..generic.v0_3 import CiteEntry as CiteEntry
 from ..generic.v0_3 import (
     DocumentationSource,
     GenericDescrBase,
+    LinkedResourceNode,
     _author_conv,  # pyright: ignore[reportPrivateUsage]
     _maintainer_conv,  # pyright: ignore[reportPrivateUsage]
 )
 from ..generic.v0_3 import Doi as Doi
 from ..generic.v0_3 import LinkedResource as LinkedResource
 from ..generic.v0_3 import Maintainer as Maintainer
 from ..generic.v0_3 import OrcidId as OrcidId
@@ -97,15 +98,12 @@
                     **(old.model_extra or {}),
                 ),
             )
 
         return data
 
 
-class LinkedDataset(Node):
+class LinkedDataset(LinkedResourceNode):
     """Reference to a bioimage.io dataset."""
 
     id: DatasetId
     """A valid dataset `id` from the bioimage.io collection."""
-
-    version_number: int
-    """version number (n-th published version, not the semantic version) of linked dataset"""
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/__init__.py` & `bioimageio.spec-0.5.3/bioimageio/spec/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/_v0_2_converter.py` & `bioimageio.spec-0.5.3/bioimageio/spec/generic/_v0_2_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/_v0_3_converter.py` & `bioimageio.spec-0.5.3/bioimageio/spec/generic/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/v0_2.py` & `bioimageio.spec-0.5.3/bioimageio/spec/generic/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/v0_3.py` & `bioimageio.spec-0.5.3/bioimageio/spec/generic/v0_3.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     YamlValue,
     include_in_package_serializer,
     validate_suffix,
 )
 from .._internal.io import FileDescr as FileDescr
 from .._internal.io_basics import AbsoluteFilePath
 from .._internal.io_basics import Sha256 as Sha256
-from .._internal.license_id import LicenseId
+from .._internal.license_id import DeprecatedLicenseId as DeprecatedLicenseId
+from .._internal.license_id import LicenseId as LicenseId
 from .._internal.types import (
-    DeprecatedLicenseId,
     ImportantFileSource,
     NotEmpty,
 )
 from .._internal.types import RelativeFilePath as RelativeFilePath
 from .._internal.url import HttpUrl as HttpUrl
 from .._internal.validated_string import ValidatedString
 from .._internal.validator_annotations import (
@@ -183,17 +183,14 @@
 
 class LinkedResource(Node):
     """Reference to a bioimage.io resource"""
 
     id: ResourceId
     """A valid resource `id` from the official bioimage.io collection."""
 
-    version_number: int
-    """version number (n-th published version, not the semantic version) of linked resource"""
-
 
 class GenericModelDescrBase(ResourceDescrBase):
     """Base for all resource descriptions including of model descriptions"""
 
     name: Annotated[
         Annotated[
             str, RestrictCharacters(string.ascii_letters + string.digits + "_- ()")
@@ -360,16 +357,22 @@
             )
 
         return value
 
     version: Optional[Version] = None
     """The version of the resource following SemVer 2.0."""
 
-    version_number: Optional[int] = None
-    """version number (n-th published version, not the semantic version)"""
+    @model_validator(mode="before")
+    def _remove_version_number(cls, value: Union[Any, Dict[Any, Any]]):
+        if isinstance(value, dict):
+            vn: Any = value.pop("version_number", None)
+            if vn is not None and "id" in value:
+                value["id"] = f"{value['id']}/{vn}"
+
+        return value
 
 
 class GenericDescrBase(GenericModelDescrBase):
     """Base for all resource descriptions except for the model descriptions"""
 
     format_version: Literal["0.3.0"] = "0.3.0"
     """The **format** version of this resource specification"""
@@ -429,7 +432,19 @@
         if value in KNOWN_SPECIFIC_RESOURCE_TYPES:
             raise ValueError(
                 f"Use the {value} description instead of this generic description for"
                 + f" your '{value}' resource."
             )
 
         return value
+
+
+class LinkedResourceNode(Node):
+
+    @model_validator(mode="before")
+    def _remove_version_number(cls, value: Union[Any, Dict[Any, Any]]):
+        if isinstance(value, dict):
+            vn: Any = value.pop("version_number", None)
+            if vn is not None and "id" in value:
+                value["id"] = f"{value['id']}/{vn}"
+
+        return value
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/__init__.py` & `bioimageio.spec-0.5.3/bioimageio/spec/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/_v0_3_converter.py` & `bioimageio.spec-0.5.3/bioimageio/spec/model/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/_v0_4_converter.py` & `bioimageio.spec-0.5.3/bioimageio/spec/model/_v0_4_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/v0_4.py` & `bioimageio.spec-0.5.3/bioimageio/spec/model/v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/v0_5.py` & `bioimageio.spec-0.5.3/bioimageio/spec/model/v0_5.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 )
 from ..generic.v0_3 import Author as Author
 from ..generic.v0_3 import BadgeDescr as BadgeDescr
 from ..generic.v0_3 import CiteEntry as CiteEntry
 from ..generic.v0_3 import (
     DocumentationSource,
     GenericModelDescrBase,
+    LinkedResourceNode,
     _author_conv,  # pyright: ignore[reportPrivateUsage]
     _maintainer_conv,  # pyright: ignore[reportPrivateUsage]
 )
 from ..generic.v0_3 import Doi as Doi
 from ..generic.v0_3 import LinkedResource as LinkedResource
 from ..generic.v0_3 import Maintainer as Maintainer
 from ..generic.v0_3 import OrcidId as OrcidId
@@ -1971,23 +1972,20 @@
         return self
 
 
 class ModelId(ResourceId):
     pass
 
 
-class LinkedModel(Node):
+class LinkedModel(LinkedResourceNode):
     """Reference to a bioimage.io model."""
 
     id: ModelId
     """A valid model `id` from the bioimage.io collection."""
 
-    version_number: int
-    """version number (n-th published version, not the semantic version) of linked model"""
-
 
 class _DataDepSize(NamedTuple):
     min: int
     max: Optional[int]
 
 
 class _AxisSizes(NamedTuple):
@@ -2005,15 +2003,15 @@
 
 
 class ModelDescr(GenericModelDescrBase, title="bioimage.io model specification"):
     """Specification of the fields used in a bioimage.io-compliant RDF to describe AI models with pretrained weights.
     These fields are typically stored in a YAML file which we call a model resource description file (model RDF).
     """
 
-    format_version: Literal["0.5.0"] = "0.5.0"
+    format_version: Literal["0.5.3"] = "0.5.3"
     """Version of the bioimage.io model description specification used.
     When creating a new model always use the latest micro/patch version described here.
     The `format_version` is important for any consumer software to understand how to parse the fields.
     """
 
     type: Literal["model"] = "model"
     """Specialized resource type 'model'"""
@@ -2591,15 +2589,15 @@
             cite=[
                 {"text": c.text, "doi": c.doi, "url": c.url} for c in src.cite
             ],  # pyright: ignore[reportArgumentType]
             config=src.config,
             covers=src.covers,
             description=src.description,
             documentation=src.documentation,  # pyright: ignore[reportArgumentType]
-            format_version="0.5.0",
+            format_version="0.5.3",
             git_repo=src.git_repo,  # pyright: ignore[reportArgumentType]
             icon=src.icon,
             id=None if src.id is None else ModelId(src.id),
             id_emoji=src.id_emoji,
             license=src.license,  # type: ignore
             links=src.links,
             maintainers=[
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/__init__.py` & `bioimageio.spec-0.5.3/bioimageio/spec/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/v0_2.py` & `bioimageio.spec-0.5.3/bioimageio/spec/notebook/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/v0_3.py` & `bioimageio.spec-0.5.3/bioimageio/spec/notebook/v0_3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Literal, Optional
 
-from .._internal.common_nodes import Node
 from .._internal.io import FileDescr as FileDescr
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
 from .._internal.io_basics import Sha256 as Sha256
 from .._internal.url import HttpUrl as HttpUrl
 from ..generic.v0_3 import VALID_COVER_IMAGE_EXTENSIONS as VALID_COVER_IMAGE_EXTENSIONS
 from ..generic.v0_3 import Author as Author
 from ..generic.v0_3 import BadgeDescr as BadgeDescr
 from ..generic.v0_3 import CiteEntry as CiteEntry
 from ..generic.v0_3 import Doi as Doi
-from ..generic.v0_3 import GenericDescrBase
+from ..generic.v0_3 import GenericDescrBase, LinkedResourceNode
 from ..generic.v0_3 import LinkedResource as LinkedResource
 from ..generic.v0_3 import Maintainer as Maintainer
 from ..generic.v0_3 import OrcidId as OrcidId
 from ..generic.v0_3 import RelativeFilePath as RelativeFilePath
 from ..generic.v0_3 import ResourceId as ResourceId
 from ..generic.v0_3 import Uploader as Uploader
 from ..generic.v0_3 import Version as Version
@@ -36,15 +35,12 @@
     parent: Optional[NotebookId] = None
     """The description from which this one is derived"""
 
     source: NotebookSource
     """The Jupyter notebook"""
 
 
-class LinkedNotebook(Node):
+class LinkedNotebook(LinkedResourceNode):
     """Reference to a bioimage.io notebook."""
 
     id: NotebookId
     """A valid notebook `id` from the bioimage.io collection."""
-
-    version_number: int
-    """version number (n-th published version, not the semantic version) of linked notebook"""
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py` & `bioimageio.spec-0.5.3/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         rdf["authors"] = authors
 
     return rdf
 
 
 def get_plugin_as_rdf(source_url: str) -> Dict[Any, Any]:
     """Get imjoy plugin config in RDF format."""
-    req = requests.get(source_url)
+    req = requests.get(source_url, timeout=5)
     source = req.text
     plugin_config = parse_imjoy_plugin(source)
     rdf = convert_config_to_rdf(plugin_config, source_url)
     return rdf
 
 
 def enrich_partial_rdf_with_imjoy_plugin(
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/pretty_validation_errors.py` & `bioimageio.spec-0.5.3/bioimageio/spec/pretty_validation_errors.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/static/tag_categories.json` & `bioimageio.spec-0.5.3/bioimageio/spec/static/tag_categories.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio/spec/summary.py` & `bioimageio.spec-0.5.3/bioimageio/spec/summary.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/PKG-INFO` & `bioimageio.spec-0.5.3/bioimageio.spec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.2.post5
+Version: 0.5.3
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -122,14 +122,22 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.3
+
+* remove collection description
+* update SPDX license list
+* update generic description to 0.3.1
+* update model description to 0.5.3
+* add timeout argument to all requests.get calls
+
 #### bioimageio.spec 0.5.2post5
 
 * added more information to validation summary
 * deprioritize `Path` objects in the `FileSource` union
 
 #### bioimageio.spec 0.5.2post4
 
@@ -296,14 +304,19 @@
 
 #### bioimageio.spec 0.4.0.post2
 
 * `load_raw_resource_description` accepts `update_to_format` kwarg
 
 ### Resource Description Format Versions
 
+#### general 0.3.1 and model 0.5.3
+
+* Non-breaking changes
+  * remove `version_number` in favor of using `version`
+
 #### model 0.5.2
 
 * Non-breaking changes
   * added `concatenable` flag to index, time and space input axes
 
 #### model 0.5.1
```

### Comparing `bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/SOURCES.txt` & `bioimageio.spec-0.5.3/bioimageio.spec.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,14 @@
 bioimageio/spec/_internal/validation_context.py
 bioimageio/spec/_internal/validator_annotations.py
 bioimageio/spec/_internal/version_type.py
 bioimageio/spec/_internal/warning_levels.py
 bioimageio/spec/application/__init__.py
 bioimageio/spec/application/v0_2.py
 bioimageio/spec/application/v0_3.py
-bioimageio/spec/collection/__init__.py
-bioimageio/spec/collection/v0_2.py
-bioimageio/spec/collection/v0_3.py
 bioimageio/spec/dataset/__init__.py
 bioimageio/spec/dataset/v0_2.py
 bioimageio/spec/dataset/v0_3.py
 bioimageio/spec/generic/__init__.py
 bioimageio/spec/generic/_v0_2_converter.py
 bioimageio/spec/generic/_v0_3_converter.py
 bioimageio/spec/generic/v0_2.py
@@ -65,34 +62,35 @@
 bioimageio/spec/notebook/v0_2.py
 bioimageio/spec/notebook/v0_3.py
 bioimageio/spec/partner_utils/__init__.py
 bioimageio/spec/partner_utils/imjoy/__init__.py
 bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
 bioimageio/spec/static/spdx_licenses.json
 bioimageio/spec/static/tag_categories.json
-example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
 example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
 example_descriptions/models/unet2d_fixed_shape/unet.py
 example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
 example_descriptions/models/unet2d_nuclei_broad/unet2d.py
 example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
 example_descriptions/models/upsample_test_model/upsample_model.py
 scripts/compare_yaml_syntax.py
 scripts/generate_dtype_limits.py
 scripts/generate_json_schemas.py
 scripts/generate_spec_documentation.py
 scripts/generate_version_submodule_imports.py
 scripts/report_invalid_rdfs.py
 scripts/update_spdx_licenses.py
+scripts/update_spdx_licenses_zenodo.py
 tests/test_bioimageio_collection.py
 tests/test_description.py
 tests/test_example_specs.py
 tests/test_io.py
 tests/test_package.py
 tests/test_specific_reexports_generics.py
+tests/test_utils.py
 tests/test_generic/__init__.py
 tests/test_generic/test_v0_2.py
 tests/test_generic/test_v0_3.py
 tests/test_internal/__init__.py
 tests/test_internal/test_base_nodes.py
 tests/test_internal/test_constants.py
 tests/test_internal/test_file_source.py
@@ -101,9 +99,10 @@
 tests/test_internal/test_node.py
 tests/test_internal/test_types.py
 tests/test_internal/test_utils.py
 tests/test_internal/test_validate.py
 tests/test_internal/test_validated_string.py
 tests/test_internal/test_version_type.py
 tests/test_model/__init__.py
+tests/test_model/test_format_version.py
 tests/test_model/test_v0_4.py
 tests/test_model/test_v0_5.py
```

### Comparing `bioimageio.spec-0.5.2.post5/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py` & `bioimageio.spec-0.5.3/example_descriptions/models/unet2d_nuclei_broad/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py` & `bioimageio.spec-0.5.3/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_fixed_shape/unet.py` & `bioimageio.spec-0.5.3/example_descriptions/models/unet2d_fixed_shape/unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py` & `bioimageio.spec-0.5.3/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/unet2d.py` & `bioimageio.spec-0.5.3/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,8 +79,11 @@
         x = self.output(x)
 
         # apply a sigmoid directly if we are in inference mode
         if not self.training:
             # postprocessing
             x = torch.sigmoid(x)
 
-        return x
+        # expand the shape across z
+        out_shape = tuple(x.shape)
+        expanded_shape = out_shape[:2] + (1,) + out_shape[2:]
+        return x.expand(expanded_shape)
```

### Comparing `bioimageio.spec-0.5.2.post5/pyproject.toml` & `bioimageio.spec-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/scripts/compare_yaml_syntax.py` & `bioimageio.spec-0.5.3/scripts/compare_yaml_syntax.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/scripts/generate_json_schemas.py` & `bioimageio.spec-0.5.3/scripts/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/scripts/generate_spec_documentation.py` & `bioimageio.spec-0.5.3/scripts/generate_spec_documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pydantic.alias_generators import to_pascal, to_snake
 from pydantic.fields import FieldInfo
 from pydantic_core import PydanticUndefined
 
 from bioimageio.spec import (
     ResourceDescr,
     application,
-    collection,
     dataset,
     generic,
     model,
     notebook,
 )
 from bioimageio.spec._internal.common_nodes import Node
 from bioimageio.spec._internal.constants import IN_PACKAGE_MESSAGE
@@ -508,15 +507,14 @@
     print(f" copied {latest} as latest")
 
 
 def main(dist: Path):
     dist.mkdir(exist_ok=True, parents=True)
 
     export_module_documentations(dist, application)
-    export_module_documentations(dist, collection)
     export_module_documentations(dist, dataset)
     export_module_documentations(dist, generic)
     export_module_documentations(dist, model)
     export_module_documentations(dist, notebook)
 
 
 def parse_args():
```

### Comparing `bioimageio.spec-0.5.2.post5/scripts/generate_version_submodule_imports.py` & `bioimageio.spec-0.5.3/scripts/generate_version_submodule_imports.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
 
 def main(command: Literal["check", "generate"]):
     for target in [
         "generic",
         "model",
         "dataset",
-        "collection",
         "notebook",
         "application",
     ]:
         process(
             Info(
                 target=target,
                 all_version_modules=get_ordered_version_submodules(target),
```

### Comparing `bioimageio.spec-0.5.2.post5/scripts/report_invalid_rdfs.py` & `bioimageio.spec-0.5.3/scripts/report_invalid_rdfs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/scripts/update_spdx_licenses.py` & `bioimageio.spec-0.5.3/scripts/update_spdx_licenses.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import urllib.request
 from argparse import ArgumentParser
 from pathlib import Path
 
 import black.files
 import black.mode
 
+from bioimageio.spec.utils import SpdxLicenseEntry, SpdxLicenses
+
 PROJECT_ROOT = Path(__file__).parent.parent
 
 URL = (
     "https://raw.githubusercontent.com/spdx/license-list-data/{tag}/json/licenses.json"
 )
 LICENSES_JSON_FILE = PROJECT_ROOT / "bioimageio/spec/static/spdx_licenses.json"
 LICENSE_ID_MODULE_PATH = (
@@ -25,28 +27,43 @@
 
 DeprecatedLicenseId = Literal{deprecated_license_ids}
 """
 
 
 def parse_args():
     p = ArgumentParser(description="script that generates weights formats overview")
-    _ = p.add_argument("tag", nargs="?", default="v3.21")
+    _ = p.add_argument("tag", nargs="?", default="v3.23")
 
     args = p.parse_args()
     return dict(tag=args.tag)
 
 
 def main(*, tag: str):
     url = URL.format(tag=tag)
     print("requesting:", url)
     text = urllib.request.urlopen(url).read().decode("utf-8")
-    _ = LICENSES_JSON_FILE.write_text(text, encoding="utf-8")
+    licenses_full = SpdxLicenses(**json.loads(text))
+    licenses_full["licenses"] = [
+        SpdxLicenseEntry(
+            isDeprecatedLicenseId=lic["isDeprecatedLicenseId"],
+            isOsiApproved=lic["isOsiApproved"],
+            licenseId=lic["licenseId"],
+            name=lic["name"],
+            reference=lic["reference"],
+            isKnownByZenodo=None,  # pyright: ignore[reportArgumentType]
+        )
+        for lic in licenses_full["licenses"]
+    ]
+
+    with LICENSES_JSON_FILE.open("wt", encoding="utf-8") as f:
+        json.dump(licenses_full, f, indent=2)
+
     print(f"Updated {LICENSES_JSON_FILE}")
 
-    licenses = json.loads(text)["licenses"]
+    licenses = licenses_full["licenses"]
     license_ids = [x["licenseId"] for x in licenses if not x["isDeprecatedLicenseId"]]
     deprecated_license_ids = [
         x["licenseId"] for x in licenses if x["isDeprecatedLicenseId"]
     ]
     code = LICENSE_ID_MODULE_TEMPLATE.format(
         license_ids=license_ids, deprecated_license_ids=deprecated_license_ids
     )
```

### Comparing `bioimageio.spec-0.5.2.post5/setup.py` & `bioimageio.spec-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_bioimageio_collection.py` & `bioimageio.spec-0.5.3/tests/test_bioimageio_collection.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_description.py` & `bioimageio.spec-0.5.3/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_example_specs.py` & `bioimageio.spec-0.5.3/tests/test_example_specs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_generic/test_v0_2.py` & `bioimageio.spec-0.5.3/tests/test_generic/test_v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_generic/test_v0_3.py` & `bioimageio.spec-0.5.3/tests/test_generic/test_v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_constants.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_file_source.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_file_source.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_io.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_license_id.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_node.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_types.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_utils.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_validate.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_validate.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_internal/test_validated_string.py` & `bioimageio.spec-0.5.3/tests/test_internal/test_validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_model/test_v0_4.py` & `bioimageio.spec-0.5.3/tests/test_model/test_v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_model/test_v0_5.py` & `bioimageio.spec-0.5.3/tests/test_model/test_v0_5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 from typing import Any, Dict, Union
 
 import pytest
+from pydantic import RootModel, ValidationError
 
 from bioimageio.spec import validate_format
 from bioimageio.spec._internal.io import FileDescr
 from bioimageio.spec._internal.license_id import LicenseId
 from bioimageio.spec._internal.url import HttpUrl
 from bioimageio.spec._internal.validation_context import ValidationContext
 from bioimageio.spec.model.v0_5 import (
@@ -225,15 +226,15 @@
 @pytest.fixture
 def model_data():
     with ValidationContext(perform_io_checks=False):
         model = ModelDescr(
             documentation=UNET2D_ROOT / "README.md",
             license=LicenseId("MIT"),
             git_repo=HttpUrl("https://github.com/bioimage-io/core-bioimage-io-python"),
-            format_version="0.5.0",
+            format_version="0.5.3",
             description="description",
             authors=[
                 Author(name="Author 1", affiliation="Affiliation 1"),
                 Author(name="Author 2"),
             ],
             maintainers=[
                 Maintainer(
@@ -449,15 +450,15 @@
     summary = validate_format(
         model_data, context=ValidationContext(perform_io_checks=False)
     )
     assert summary.status == "failed", summary.format()
 
 
 def test_model_has_parent_with_id(model_data: Dict[str, Any]):
-    model_data["parent"] = dict(id="10.5281/zenodo.5764892", version_number=1)
+    model_data["parent"] = dict(id="10.5281/zenodo.5764892/6647674")
     summary = validate_format(
         model_data, context=ValidationContext(perform_io_checks=False)
     )
     assert summary.status == "passed", summary.format()
 
 
 def test_model_with_expanded_output(model_data: Dict[str, Any]):
@@ -485,7 +486,22 @@
 
 def test_model_does_not_accept_unknown_fields(model_data: Dict[str, Any]):
     model_data["unknown_additional_field"] = "shouldn't be here"
     summary = validate_format(
         model_data, context=ValidationContext(perform_io_checks=False)
     )
     assert summary.status == "failed", summary.format()
+
+
+def test_empty_axis_data():
+    from bioimageio.spec.model.v0_5 import InputAxis as InputAxisUnion
+    from bioimageio.spec.model.v0_5 import OutputAxis as OutputAxisUnion
+
+    InputAxis = RootModel[InputAxisUnion]
+
+    with pytest.raises(ValidationError):
+        _ = InputAxis.model_validate({})
+
+    OutputAxis = RootModel[OutputAxisUnion]
+
+    with pytest.raises(ValidationError):
+        _ = OutputAxis.model_validate({})
```

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_package.py` & `bioimageio.spec-0.5.3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post5/tests/test_specific_reexports_generics.py` & `bioimageio.spec-0.5.3/tests/test_specific_reexports_generics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from types import ModuleType
 from typing import Any, Dict
 
 import pytest
 
-from bioimageio.spec import application, collection, dataset, generic, model, notebook
+from bioimageio.spec import application, dataset, generic, model, notebook
 
 IGNORE_MEMBERS = {
     "AfterValidator",
     "ALERT",
     "annotated_types",
     "Annotated",
     "annotations",
@@ -90,14 +90,15 @@
 
 
 GENERIC_ONLY_MEMBERS = {
     "GenericDescr",
     "GenericDescrBase",
     "GenericModelDescrBase",
     "KNOWN_SPECIFIC_RESOURCE_TYPES",
+    "LinkedResourceNode",
     "ResourceDescrBase",
     "ResourceDescrType",
 }
 
 GENERIC_v0_2_MEMBERS = {
     k: v for k, v in get_members(generic.v0_2).items() if k not in GENERIC_ONLY_MEMBERS
 }
@@ -106,20 +107,18 @@
 }
 
 
 @pytest.mark.parametrize(
     "generic_members,specific",
     [
         (GENERIC_v0_2_MEMBERS, application.v0_2),
-        (GENERIC_v0_2_MEMBERS, collection.v0_2),
         (GENERIC_v0_2_MEMBERS, dataset.v0_2),
         (GENERIC_v0_2_MEMBERS, model.v0_4),
         (GENERIC_v0_2_MEMBERS, notebook.v0_2),
         (GENERIC_v0_3_MEMBERS, application.v0_3),
-        (GENERIC_v0_3_MEMBERS, collection.v0_3),
         (GENERIC_v0_3_MEMBERS, dataset.v0_3),
         (GENERIC_v0_3_MEMBERS, model.v0_5),
         (GENERIC_v0_3_MEMBERS, notebook.v0_3),
     ],
 )
 def test_specific_module_has_all_generic_symbols(
     generic_members: Dict[str, Any], specific: ModuleType
```

