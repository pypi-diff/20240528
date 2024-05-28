# Comparing `tmp/cysecuretools-5.1.0.tar.gz` & `tmp/cysecuretools-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cysecuretools-5.1.0.tar", last modified: Thu Mar 28 12:29:07 2024, max compression
+gzip compressed data, was "cysecuretools-6.0.0.tar", last modified: Tue May 28 15:41:27 2024, max compression
```

## Comparing `cysecuretools-5.1.0.tar` & `cysecuretools-6.0.0.tar`

### file list

```diff
@@ -1,474 +1,471 @@
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.009184 cysecuretools-5.1.0/
--rw-r--r--   0 ihos       (501) staff       (20)     2922 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/CHANGELOG.md
--rw-r--r--   0 ihos       (501) staff       (20)      676 2024-03-28 12:27:45.000000 cysecuretools-5.1.0/LICENSE
--rw-r--r--   0 ihos       (501) staff       (20)      669 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/MANIFEST.in
--rw-r--r--   0 ihos       (501) staff       (20)    10522 2024-03-28 12:29:07.008881 cysecuretools-5.1.0/PKG-INFO
--rw-r--r--   0 ihos       (501) staff       (20)     6814 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/README.md
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.936295 cysecuretools-5.1.0/cysecuretools.egg-info/
--rw-r--r--   0 ihos       (501) staff       (20)    10522 2024-03-28 12:29:06.000000 cysecuretools-5.1.0/cysecuretools.egg-info/PKG-INFO
--rw-r--r--   0 ihos       (501) staff       (20)    17597 2024-03-28 12:29:06.000000 cysecuretools-5.1.0/cysecuretools.egg-info/SOURCES.txt
--rw-r--r--   0 ihos       (501) staff       (20)        1 2024-03-28 12:29:06.000000 cysecuretools-5.1.0/cysecuretools.egg-info/dependency_links.txt
--rw-r--r--   0 ihos       (501) staff       (20)       63 2024-03-28 12:29:06.000000 cysecuretools-5.1.0/cysecuretools.egg-info/entry_points.txt
--rw-r--r--   0 ihos       (501) staff       (20)      164 2024-03-28 12:29:06.000000 cysecuretools-5.1.0/cysecuretools.egg-info/requires.txt
--rw-r--r--   0 ihos       (501) staff       (20)       14 2024-03-28 12:29:06.000000 cysecuretools-5.1.0/cysecuretools.egg-info/top_level.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.938095 cysecuretools-5.1.0/docs/
--rw-r--r--   0 ihos       (501) staff       (20)    40892 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/docs/README_CYW20829.md
--rw-r--r--   0 ihos       (501) staff       (20)    39599 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/docs/README_PSOC64.md
--rw-r--r--   0 ihos       (501) staff       (20)    14181 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/docs/README_XMC7XXX.md
--rw-r--r--   0 ihos       (501) staff       (20)      141 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/pyproject.toml
--rw-r--r--   0 ihos       (501) staff       (20)       38 2024-03-28 12:29:07.009225 cysecuretools-5.1.0/setup.cfg
--rw-r--r--   0 ihos       (501) staff       (20)     2561 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/setup.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.941607 cysecuretools-5.1.0/src/
--rw-r--r--   0 ihos       (501) staff       (20)      762 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/__about__.py
--rw-r--r--   0 ihos       (501) staff       (20)      737 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      700 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/__main__.py
--rw-r--r--   0 ihos       (501) staff       (20)    21227 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/api_common.py
--rw-r--r--   0 ihos       (501) staff       (20)     7177 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/api_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)    18433 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/api_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     3950 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/api_traveo_t2g.py
--rw-r--r--   0 ihos       (501) staff       (20)    22497 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/cli.py
--rw-r--r--   0 ihos       (501) staff       (20)     6605 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/cli_creator.py
--rw-r--r--   0 ihos       (501) staff       (20)    32964 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/cli_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)    27492 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/cli_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     6043 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/cli_traveo_t2g.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.948397 cysecuretools-5.1.0/src/core/
--rw-r--r--   0 ihos       (501) staff       (20)     1217 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1037 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/bitops.py
--rw-r--r--   0 ihos       (501) staff       (20)     5075 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/connect_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     1715 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/crc.py
--rw-r--r--   0 ihos       (501) staff       (20)     2230 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/cy_bootloader_map_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     1259 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/dependecy_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1191 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/deprecated.py
--rw-r--r--   0 ihos       (501) staff       (20)      945 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/entrance_exam_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     1635 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/enums.py
--rw-r--r--   0 ihos       (501) staff       (20)      736 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/exceptions.py
--rw-r--r--   0 ihos       (501) staff       (20)     1469 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/json_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     1674 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/jsonpath.py
--rw-r--r--   0 ihos       (501) staff       (20)     2144 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/key_data.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.949151 cysecuretools-5.1.0/src/core/key_handlers/
--rw-r--r--   0 ihos       (501) staff       (20)     3852 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/key_handlers/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     4417 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/key_handlers/ec_handler.py
--rw-r--r--   0 ihos       (501) staff       (20)     3919 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/key_handlers/pem_key.py
--rw-r--r--   0 ihos       (501) staff       (20)    15654 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/key_handlers/rsa_handler.py
--rw-r--r--   0 ihos       (501) staff       (20)     2422 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/key_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     2472 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/logging_configurator.py
--rw-r--r--   0 ihos       (501) staff       (20)     2453 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/logging_formatter.py
--rw-r--r--   0 ihos       (501) staff       (20)      701 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/memory_area.py
--rw-r--r--   0 ihos       (501) staff       (20)     2253 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/memory_map_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     3161 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/mtb_tools_discovery.py
--rw-r--r--   0 ihos       (501) staff       (20)     2562 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/ocd_settings.py
--rw-r--r--   0 ihos       (501) staff       (20)      840 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/policy_filter_base.py
--rw-r--r--   0 ihos       (501) staff       (20)      911 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/policy_parser_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     1034 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/policy_validator_base.py
--rw-r--r--   0 ihos       (501) staff       (20)      858 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/progress_bar.py
--rw-r--r--   0 ihos       (501) staff       (20)    11374 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/project_base.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.949727 cysecuretools-5.1.0/src/core/provisioning_flows/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/provisioning_flows/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3655 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/provisioning_flows/app_loading_flow.py
--rw-r--r--   0 ihos       (501) staff       (20)     7642 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/provisioning_flows/application.py
--rw-r--r--   0 ihos       (501) staff       (20)     1002 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/ram_app_loader_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     3267 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/register_map_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     4707 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/signtool_base.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.951137 cysecuretools-5.1.0/src/core/strategy_context/
--rw-r--r--   0 ihos       (501) staff       (20)      498 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/strategy_context/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2769 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/strategy_context/cert_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     2735 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/strategy_context/encrypted_programming_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     2534 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/strategy_context/prov_packet_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     2890 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/strategy_context/provisioning_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)      716 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/strops.py
--rw-r--r--   0 ihos       (501) staff       (20)     4629 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/target_builder.py
--rw-r--r--   0 ihos       (501) staff       (20)    12476 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/target_director.py
--rw-r--r--   0 ihos       (501) staff       (20)     5078 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/version_provider.py
--rw-r--r--   0 ihos       (501) staff       (20)      847 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/core/voltage_tool.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.951331 cysecuretools-5.1.0/src/data/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/data/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1579 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/data/cy_bootloader_map.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.951581 cysecuretools-5.1.0/src/data/mxs22/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/data/mxs22/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     4858 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/data/mxs22/mxs22_ram_app_status_codes.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.953323 cysecuretools-5.1.0/src/data/mxs40sv2/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/data/mxs40sv2/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     4698 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.953767 cysecuretools-5.1.0/src/data/mxs40v1/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/data/mxs40v1/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)    13578 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/data/mxs40v1/mxs40v1_sfb_status_codes.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.954407 cysecuretools-5.1.0/src/execute/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.954876 cysecuretools-5.1.0/src/execute/dfuht_commands/
--rw-r--r--   0 ihos       (501) staff       (20)      734 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/dfuht_commands/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     7004 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/dfuht_commands/dfuht_packet.py
--rw-r--r--   0 ihos       (501) staff       (20)     3488 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/dfuht_commands/dfuht_packet_creator.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.955518 cysecuretools-5.1.0/src/execute/image_signing/
--rw-r--r--   0 ihos       (501) staff       (20)      709 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/image_signing/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)    12155 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/image_signing/image.py
--rw-r--r--   0 ihos       (501) staff       (20)     1578 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/image_signing/image_config_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)    13339 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/image_signing/sign_tool.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.956871 cysecuretools-5.1.0/src/execute/imgtool/
--rw-r--r--   0 ihos       (501) staff       (20)      650 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1613 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/boot_record.py
--rw-r--r--   0 ihos       (501) staff       (20)     1208 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/custom_encryptor.py
--rw-r--r--   0 ihos       (501) staff       (20)    26031 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/image.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.958161 cysecuretools-5.1.0/src/execute/imgtool/keys/
--rw-r--r--   0 ihos       (501) staff       (20)     3847 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5388 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/ecdsa.py
--rw-r--r--   0 ihos       (501) staff       (20)     2970 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/ecdsa_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     3090 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/ed25519.py
--rw-r--r--   0 ihos       (501) staff       (20)     3026 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/ed25519_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     1822 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/general.py
--rw-r--r--   0 ihos       (501) staff       (20)     5428 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/rsa.py
--rw-r--r--   0 ihos       (501) staff       (20)     3810 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/rsa_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     3169 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/keys/x25519.py
--rwxr-xr-x   0 ihos       (501) staff       (20)    18219 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/main.py
--rw-r--r--   0 ihos       (501) staff       (20)     1773 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/imgtool/version.py
--rw-r--r--   0 ihos       (501) staff       (20)     4279 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/jwt.py
--rw-r--r--   0 ihos       (501) staff       (20)     3676 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/key_reader.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.958583 cysecuretools-5.1.0/src/execute/keygens/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/keygens/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1753 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/keygens/aes_keygen.py
--rw-r--r--   0 ihos       (501) staff       (20)     4044 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/keygens/ec_keygen.py
--rw-r--r--   0 ihos       (501) staff       (20)     4678 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/keygens/rsa_keygen.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.960474 cysecuretools-5.1.0/src/execute/programmer/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/programmer/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     6799 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/programmer/base.py
--rw-r--r--   0 ihos       (501) staff       (20)     8264 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/programmer/dfuht_runner.py
--rw-r--r--   0 ihos       (501) staff       (20)     8790 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/programmer/dfuht_wrapper.py
--rw-r--r--   0 ihos       (501) staff       (20)    13257 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/programmer/openocd_server.py
--rw-r--r--   0 ihos       (501) staff       (20)     1824 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/execute/programmer/openocd_target_map.json
--rw-r--r--   0 ihos       (501) staff       (20)    22526 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/programmer/openocd_wrapper.py
--rw-r--r--   0 ihos       (501) staff       (20)     1273 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/programmer/programmer.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.960719 cysecuretools-5.1.0/src/execute/project_init/
--rw-r--r--   0 ihos       (501) staff       (20)      729 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/project_init/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     8549 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/project_init/project_init.py
--rw-r--r--   0 ihos       (501) staff       (20)     1089 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/execute/silicon_data_reader.py
--rw-r--r--   0 ihos       (501) staff       (20)     3187 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/main.py
--rw-r--r--   0 ihos       (501) staff       (20)      734 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/pkg_globals.py
--rw-r--r--   0 ihos       (501) staff       (20)      502 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/settings.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.960878 cysecuretools-5.1.0/src/targets/
--rw-r--r--   0 ihos       (501) staff       (20)     4025 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.961634 cysecuretools-5.1.0/src/targets/common/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1561 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/dependencies_validation.py
--rw-r--r--   0 ihos       (501) staff       (20)     3527 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/flow_parser.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.964038 cysecuretools-5.1.0/src/targets/common/mxs40sv2/
--rw-r--r--   0 ihos       (501) staff       (20)     1329 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1336 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/asset.py
--rw-r--r--   0 ihos       (501) staff       (20)     1285 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/asset_builder.py
--rw-r--r--   0 ihos       (501) staff       (20)     3073 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/asset_enums.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.964417 cysecuretools-5.1.0/src/targets/common/mxs40sv2/debug_cert/
--rw-r--r--   0 ihos       (501) staff       (20)      742 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/debug_cert/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3141 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     4365 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_parser_mxs40sv2.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.966079 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1929 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1295 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     2098 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     3387 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1500 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1189 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1828 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependency_validator_mxs40v2.py
--rw-r--r--   0 ihos       (501) staff       (20)     1151 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/enums.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.967074 cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/
--rw-r--r--   0 ihos       (501) staff       (20)      732 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3243 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/encrypt_mxv40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)    17996 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/signtool_mxv40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     1325 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/xip_encryptor_mxs40sv2.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.967735 cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/
--rw-r--r--   0 ihos       (501) staff       (20)    24916 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     2049 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     7972 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)    29537 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/cyw20829_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     4920 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/key_source_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     3282 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/nv_counter_calc.py
--rw-r--r--   0 ihos       (501) staff       (20)    12563 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/policy_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     1713 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/policy_validator_mxs40v2.py
--rw-r--r--   0 ihos       (501) staff       (20)     2018 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/project_init_mxs40sv2.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.968304 cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      802 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     6955 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning/provision_device_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     9446 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning/ram_app_loader_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     7028 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning_packet_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     3981 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/silicon_data_reader_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     2917 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40sv2/version_provider_mxs40sv2.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.971268 cysecuretools-5.1.0/src/targets/common/mxs40v1/
--rw-r--r--   0 ihos       (501) staff       (20)     1510 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3172 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/bootloader_provider_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.972182 cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/
--rw-r--r--   0 ihos       (501) staff       (20)      735 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2561 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/aes_cipher.py
--rw-r--r--   0 ihos       (501) staff       (20)     3830 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/aes_header.py
--rw-r--r--   0 ihos       (501) staff       (20)     5396 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/aes_header_strategy.py
--rw-r--r--   0 ihos       (501) staff       (20)     2957 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/ecc_kdf.py
--rw-r--r--   0 ihos       (501) staff       (20)     3227 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/encrypted_programming.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.972568 cysecuretools-5.1.0/src/targets/common/mxs40v1/entrance_exam/
--rw-r--r--   0 ihos       (501) staff       (20)      778 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/entrance_exam/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     8150 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/entrance_exam/exam_cyb06xx7.py
--rw-r--r--   0 ihos       (501) staff       (20)     8821 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/entrance_exam/exam_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)      839 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/enums.py
--rw-r--r--   0 ihos       (501) staff       (20)     5110 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/image_cert.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.973010 cysecuretools-5.1.0/src/targets/common/mxs40v1/json/
--rw-r--r--   0 ihos       (501) staff       (20)     4452 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/json/policy_template.json
--rw-r--r--   0 ihos       (501) staff       (20)    15796 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/json/schema.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     1977 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/key_reader_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)      825 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/key_source_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     5747 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/policy_filter.py
--rw-r--r--   0 ihos       (501) staff       (20)    15539 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/policy_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)    46181 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/policy_validator.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.973533 cysecuretools-5.1.0/src/targets/common/mxs40v1/prebuilt/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/prebuilt/cy_pub_key.json
--rw-r--r--   0 ihos       (501) staff       (20)      511 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/prebuilt/hsm_state.json
--rw-r--r--   0 ihos       (501) staff       (20)      511 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/prebuilt/oem_state.json
--rw-r--r--   0 ihos       (501) staff       (20)     8014 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/project_init_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.973921 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      742 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)    20588 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning/provision_device_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    22504 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning/sys_call.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.974187 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/
--rw-r--r--   0 ihos       (501) staff       (20)      751 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.975368 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5408 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_crypto.py
--rw-r--r--   0 ihos       (501) staff       (20)     1491 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_customer.py
--rw-r--r--   0 ihos       (501) staff       (20)     3380 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_dev.py
--rw-r--r--   0 ihos       (501) staff       (20)     1822 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_entity.py
--rw-r--r--   0 ihos       (501) staff       (20)     3295 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_hsm.py
--rw-r--r--   0 ihos       (501) staff       (20)     3019 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_oem.py
--rw-r--r--   0 ihos       (501) staff       (20)     1049 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_types.py
--rw-r--r--   0 ihos       (501) staff       (20)     8651 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/provisioning_packet_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    17211 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/signtool_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     1441 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/silicon_data_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     2841 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/silicon_data_reader_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     8744 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/version_provider_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.975742 cysecuretools-5.1.0/src/targets/common/mxs40v1/voltage_tool/
--rw-r--r--   0 ihos       (501) staff       (20)      737 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/voltage_tool/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3215 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/voltage_tool/lvd_voltage_picker.py
--rw-r--r--   0 ihos       (501) staff       (20)     1327 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/voltage_tool/voltage_tool_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    10084 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/mxs40v1/x509_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     4453 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/policy_validator.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.975874 cysecuretools-5.1.0/src/targets/common/prebuilt/
--rw-r--r--   0 ihos       (501) staff       (20)      173 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/prebuilt/bootloader_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.976136 cysecuretools-5.1.0/src/targets/common/traveo_t2g/
--rw-r--r--   0 ihos       (501) staff       (20)      725 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/traveo_t2g/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)    12799 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/common/traveo_t2g/signtool_xmc7xxx.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.976672 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/
--rw-r--r--   0 ihos       (501) staff       (20)     1242 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.976820 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.977175 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1681 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2385 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.977719 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1051 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/packets/cy_auth_512k_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.978649 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     5498 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     5500 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     5111 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     5111 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4_smif.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.930518 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.979377 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/
--rw-r--r--   0 ihos       (501) staff       (20)   134553 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      536 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.980460 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/
--rw-r--r--   0 ihos       (501) staff       (20)   148119 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      540 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     3936 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx5_a1/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.980864 cysecuretools-5.1.0/src/targets/cyb06xx7/
--rw-r--r--   0 ihos       (501) staff       (20)     1548 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.981117 cysecuretools-5.1.0/src/targets/cyb06xx7/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.981425 cysecuretools-5.1.0/src/targets/cyb06xx7/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1991 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2391 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.981873 cysecuretools-5.1.0/src/targets/cyb06xx7/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1031 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.983140 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     5115 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     5115 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     5740 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5739 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     4903 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     4903 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     5531 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5529 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.931001 cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.984022 cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/
--rw-r--r--   0 ihos       (501) staff       (20)   138714 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      543 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.984874 cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/
--rw-r--r--   0 ihos       (501) staff       (20)   150520 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      542 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     3799 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xx7/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.985123 cysecuretools-5.1.0/src/targets/cyb06xxa/
--rw-r--r--   0 ihos       (501) staff       (20)     1147 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.985277 cysecuretools-5.1.0/src/targets/cyb06xxa/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.985621 cysecuretools-5.1.0/src/targets/cyb06xxa/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1682 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2392 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.986121 cysecuretools-5.1.0/src/targets/cyb06xxa/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1051 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.987106 cysecuretools-5.1.0/src/targets/cyb06xxa/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6084 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5800 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5637 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5589 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.931660 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.987980 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/
--rw-r--r--   0 ihos       (501) staff       (20)   158689 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      543 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.989029 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   138738 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      592 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.989792 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/
--rw-r--r--   0 ihos       (501) staff       (20)   172504 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      544 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.990251 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   155454 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      588 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     3802 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyb06xxa/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.990722 cysecuretools-5.1.0/src/targets/cys06xxa/
--rw-r--r--   0 ihos       (501) staff       (20)     1151 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.990927 cysecuretools-5.1.0/src/targets/cys06xxa/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.991378 cysecuretools-5.1.0/src/targets/cys06xxa/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1031 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.992335 cysecuretools-5.1.0/src/targets/cys06xxa/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6084 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5800 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5637 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5589 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.932233 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.992989 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/
--rw-r--r--   0 ihos       (501) staff       (20)   158689 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      543 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.993571 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   138738 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      592 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.994327 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/
--rw-r--r--   0 ihos       (501) staff       (20)   172504 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      544 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.994723 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   155454 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      588 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      804 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cys06xxa/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.995009 cysecuretools-5.1.0/src/targets/cyw20829/
--rw-r--r--   0 ihos       (501) staff       (20)     1196 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.995630 cysecuretools-5.1.0/src/targets/cyw20829/flows/
--rw-r--r--   0 ihos       (501) staff       (20)      179 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/flows/oem_assets.json
--rw-r--r--   0 ihos       (501) staff       (20)      858 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/flows/prov_flows.json
--rw-r--r--   0 ihos       (501) staff       (20)       94 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/flows/reprovisioning_assets.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.996420 cysecuretools-5.1.0/src/targets/cyw20829/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      460 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/keys/pub_hci_0.pem
--rw-r--r--   0 ihos       (501) staff       (20)      460 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/keys/pub_hci_1.pem
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.996665 cysecuretools-5.1.0/src/targets/cyw20829/packets/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.932834 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.997088 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/prov_oem/
--rw-r--r--   0 ihos       (501) staff       (20)      235 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/prov_oem/config.json
--rw-r--r--   0 ihos       (501) staff       (20)     7780 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      375 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/prov_oem/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.998070 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/reprovisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      241 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/reprovisioning/config.json
--rw-r--r--   0 ihos       (501) staff       (20)    28868 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      264 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/reprovisioning/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.998525 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/to_rma/
--rw-r--r--   0 ihos       (501) staff       (20)      269 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/to_rma/config.json
--rw-r--r--   0 ihos       (501) staff       (20)    28676 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      289 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/to_rma/info.txt
--rw-r--r--   0 ihos       (501) staff       (20)      624 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/debug_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)      168 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/packets/rsa_key_tmpl.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.999170 cysecuretools-5.1.0/src/targets/cyw20829/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6135 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_hci_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     6344 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)      374 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_reprovisioning_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     2099 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_reprovisioning_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     8568 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     1288 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw20829/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.999768 cysecuretools-5.1.0/src/targets/cyw20829_a0/
--rw-r--r--   0 ihos       (501) staff       (20)      984 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.000225 cysecuretools-5.1.0/src/targets/cyw20829_a0/flows/
--rw-r--r--   0 ihos       (501) staff       (20)      179 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/flows/oem_assets.json
--rw-r--r--   0 ihos       (501) staff       (20)      858 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/flows/prov_flows.json
--rw-r--r--   0 ihos       (501) staff       (20)       94 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/flows/reprovisioning_assets.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.000455 cysecuretools-5.1.0/src/targets/cyw20829_a0/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      460 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/keys/pub_hci_0.pem
--rw-r--r--   0 ihos       (501) staff       (20)      460 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/keys/pub_hci_1.pem
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.001141 cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     9431 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/asset_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     1052 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     1705 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/register_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     9308 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/reverse_asset_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.001589 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.933539 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.002039 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/prov_oem/
--rw-r--r--   0 ihos       (501) staff       (20)      235 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/prov_oem/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)     7812 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      375 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/prov_oem/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.002451 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      241 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)    28836 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      264 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.003065 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/to_rma/
--rw-r--r--   0 ihos       (501) staff       (20)      269 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/to_rma/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)    28612 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      289 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/to_rma/info.txt
--rw-r--r--   0 ihos       (501) staff       (20)      624 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/debug_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)      168 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/rsa_key_tmpl.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.004168 cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6135 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_hci_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     6344 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)      374 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     1812 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     8281 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     2953 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/policy_generator.py
--rw-r--r--   0 ihos       (501) staff       (20)     4043 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw20829_a0/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.004543 cysecuretools-5.1.0/src/targets/cyw89829/
--rw-r--r--   0 ihos       (501) staff       (20)      980 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.005246 cysecuretools-5.1.0/src/targets/cyw89829/flows/
--rw-r--r--   0 ihos       (501) staff       (20)      179 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/flows/oem_assets.json
--rw-r--r--   0 ihos       (501) staff       (20)      858 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/flows/prov_flows.json
--rw-r--r--   0 ihos       (501) staff       (20)       94 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/flows/reprovisioning_assets.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.005681 cysecuretools-5.1.0/src/targets/cyw89829/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      460 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/keys/pub_hci_0.pem
--rw-r--r--   0 ihos       (501) staff       (20)      460 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/keys/pub_hci_1.pem
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.005921 cysecuretools-5.1.0/src/targets/cyw89829/packets/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:06.934149 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.006309 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/prov_oem/
--rw-r--r--   0 ihos       (501) staff       (20)      235 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/prov_oem/config.json
--rw-r--r--   0 ihos       (501) staff       (20)     7780 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      375 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/prov_oem/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.006950 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/reprovisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      241 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/reprovisioning/config.json
--rw-r--r--   0 ihos       (501) staff       (20)    28868 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      264 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/reprovisioning/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.007374 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/to_rma/
--rw-r--r--   0 ihos       (501) staff       (20)      269 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/to_rma/config.json
--rw-r--r--   0 ihos       (501) staff       (20)    28676 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      289 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/to_rma/info.txt
--rw-r--r--   0 ihos       (501) staff       (20)      624 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/debug_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)      168 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/packets/rsa_key_tmpl.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.008246 cysecuretools-5.1.0/src/targets/cyw89829/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6135 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_hci_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     6344 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)      374 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_reprovisioning_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     2099 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_reprovisioning_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     8568 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     1270 2024-03-28 10:33:29.000000 cysecuretools-5.1.0/src/targets/cyw89829/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-03-28 12:29:07.008635 cysecuretools-5.1.0/src/targets/xmc7xxx/
--rw-r--r--   0 ihos       (501) staff       (20)     1124 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/xmc7xxx/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2544 2024-03-28 10:31:54.000000 cysecuretools-5.1.0/src/targets/xmc7xxx/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.260658 cysecuretools-6.0.0/
+-rw-r--r--   0 ihos       (501) staff       (20)     3129 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/CHANGELOG.md
+-rw-r--r--   0 ihos       (501) staff       (20)    12551 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/EULA
+-rw-r--r--   0 ihos       (501) staff       (20)     9115 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/LICENSE
+-rw-r--r--   0 ihos       (501) staff       (20)      132 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/MANIFEST.in
+-rw-r--r--   0 ihos       (501) staff       (20)    12558 2024-05-28 15:41:27.260310 cysecuretools-6.0.0/PKG-INFO
+-rw-r--r--   0 ihos       (501) staff       (20)     8370 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/README.md
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.258427 cysecuretools-6.0.0/cysecuretools.egg-info/
+-rw-r--r--   0 ihos       (501) staff       (20)    12558 2024-05-28 15:41:27.000000 cysecuretools-6.0.0/cysecuretools.egg-info/PKG-INFO
+-rw-r--r--   0 ihos       (501) staff       (20)    17354 2024-05-28 15:41:27.000000 cysecuretools-6.0.0/cysecuretools.egg-info/SOURCES.txt
+-rw-r--r--   0 ihos       (501) staff       (20)        1 2024-05-28 15:41:27.000000 cysecuretools-6.0.0/cysecuretools.egg-info/dependency_links.txt
+-rw-r--r--   0 ihos       (501) staff       (20)       62 2024-05-28 15:41:27.000000 cysecuretools-6.0.0/cysecuretools.egg-info/entry_points.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      156 2024-05-28 15:41:27.000000 cysecuretools-6.0.0/cysecuretools.egg-info/requires.txt
+-rw-r--r--   0 ihos       (501) staff       (20)       14 2024-05-28 15:41:27.000000 cysecuretools-6.0.0/cysecuretools.egg-info/top_level.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.179967 cysecuretools-6.0.0/docs/
+-rw-r--r--   0 ihos       (501) staff       (20)    50960 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/docs/README_CYW20829.md
+-rw-r--r--   0 ihos       (501) staff       (20)    39599 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/docs/README_PSOC64.md
+-rw-r--r--   0 ihos       (501) staff       (20)    14934 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/docs/README_XMC7XXX.md
+-rw-r--r--   0 ihos       (501) staff       (20)      141 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/pyproject.toml
+-rw-r--r--   0 ihos       (501) staff       (20)       38 2024-05-28 15:41:27.260709 cysecuretools-6.0.0/setup.cfg
+-rw-r--r--   0 ihos       (501) staff       (20)     2555 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/setup.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.184566 cysecuretools-6.0.0/src/
+-rw-r--r--   0 ihos       (501) staff       (20)      762 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/__about__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      737 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      798 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/__main__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    21227 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/api_common.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7177 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/api_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)    18433 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/api_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3955 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/api_traveo_t2g.py
+-rw-r--r--   0 ihos       (501) staff       (20)    22497 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/cli.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6610 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/cli_creator.py
+-rw-r--r--   0 ihos       (501) staff       (20)    32964 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/cli_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)    27492 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/cli_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6048 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/cli_traveo_t2g.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.191629 cysecuretools-6.0.0/src/core/
+-rw-r--r--   0 ihos       (501) staff       (20)     1217 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1037 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/bitops.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5075 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/connect_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1720 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/crc.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2323 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/cy_bootloader_map_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1357 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/dependecy_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1196 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/deprecated.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1043 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/entrance_exam_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1728 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/enums.py
+-rw-r--r--   0 ihos       (501) staff       (20)      834 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/exceptions.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1469 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/json_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1772 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/jsonpath.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2237 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/key_data.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.192250 cysecuretools-6.0.0/src/core/key_handlers/
+-rw-r--r--   0 ihos       (501) staff       (20)     3857 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/key_handlers/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4515 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/key_handlers/ec_handler.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4012 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/key_handlers/pem_key.py
+-rw-r--r--   0 ihos       (501) staff       (20)    15654 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/key_handlers/rsa_handler.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2520 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/key_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2565 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/logging_configurator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2546 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/logging_formatter.py
+-rw-r--r--   0 ihos       (501) staff       (20)      799 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/memory_area.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2346 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/memory_map_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3166 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/mtb_tools_discovery.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2655 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/ocd_settings.py
+-rw-r--r--   0 ihos       (501) staff       (20)      938 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/policy_filter_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)      916 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/policy_parser_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1127 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/policy_validator_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)      951 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/progress_bar.py
+-rw-r--r--   0 ihos       (501) staff       (20)    11467 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/project_base.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.192959 cysecuretools-6.0.0/src/core/provisioning_flows/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/provisioning_flows/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3660 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/provisioning_flows/app_loading_flow.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7647 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/provisioning_flows/application.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1007 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/ram_app_loader_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3360 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/register_map_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4805 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/signtool_base.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.193729 cysecuretools-6.0.0/src/core/strategy_context/
+-rw-r--r--   0 ihos       (501) staff       (20)     1182 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/strategy_context/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2862 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/strategy_context/cert_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2833 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/strategy_context/encrypted_programming_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2534 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/strategy_context/prov_packet_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2983 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/strategy_context/provisioning_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)      814 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/strops.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4722 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/target_builder.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12476 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/target_director.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5083 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/version_provider.py
+-rw-r--r--   0 ihos       (501) staff       (20)      945 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/core/voltage_tool.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.194023 cysecuretools-6.0.0/src/data/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/data/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1579 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/data/cy_bootloader_map.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.194280 cysecuretools-6.0.0/src/data/mxs22/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/data/mxs22/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4956 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/data/mxs22/mxs22_ram_app_status_codes.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.194610 cysecuretools-6.0.0/src/data/mxs40sv2/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/data/mxs40sv2/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4796 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.194941 cysecuretools-6.0.0/src/data/mxs40v1/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/data/mxs40v1/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    13676 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/data/mxs40v1/mxs40v1_sfb_status_codes.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.195906 cysecuretools-6.0.0/src/execute/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.196527 cysecuretools-6.0.0/src/execute/dfuht_commands/
+-rw-r--r--   0 ihos       (501) staff       (20)      739 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/dfuht_commands/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7004 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/dfuht_commands/dfuht_packet.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3488 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/dfuht_commands/dfuht_packet_creator.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.197280 cysecuretools-6.0.0/src/execute/image_signing/
+-rw-r--r--   0 ihos       (501) staff       (20)      709 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/image_signing/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12160 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/image_signing/image.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1676 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/image_signing/image_config_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)    13344 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/image_signing/sign_tool.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.198880 cysecuretools-6.0.0/src/execute/imgtool/
+-rw-r--r--   0 ihos       (501) staff       (20)      650 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1613 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/boot_record.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1213 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/custom_encryptor.py
+-rw-r--r--   0 ihos       (501) staff       (20)    26036 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/image.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.200779 cysecuretools-6.0.0/src/execute/imgtool/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)     3847 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5388 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/ecdsa.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2970 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/ecdsa_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3090 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/ed25519.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3026 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/ed25519_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1822 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/general.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5428 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/rsa.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3810 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/rsa_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3169 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/keys/x25519.py
+-rwxr-xr-x   0 ihos       (501) staff       (20)    18224 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/main.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1773 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/imgtool/version.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4279 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/jwt.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3676 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/key_reader.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.201267 cysecuretools-6.0.0/src/execute/keygens/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/keygens/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1753 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/keygens/aes_keygen.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4044 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/keygens/ec_keygen.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4678 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/keygens/rsa_keygen.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.203333 cysecuretools-6.0.0/src/execute/programmer/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/programmer/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6799 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/programmer/base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8264 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/programmer/dfuht_runner.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8795 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/programmer/dfuht_wrapper.py
+-rw-r--r--   0 ihos       (501) staff       (20)    13257 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/programmer/openocd_server.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1824 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/programmer/openocd_target_map.json
+-rw-r--r--   0 ihos       (501) staff       (20)    22526 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/programmer/openocd_wrapper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1273 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/programmer/programmer.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.203613 cysecuretools-6.0.0/src/execute/project_init/
+-rw-r--r--   0 ihos       (501) staff       (20)      729 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/project_init/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8549 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/project_init/project_init.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1089 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/execute/silicon_data_reader.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3187 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/main.py
+-rw-r--r--   0 ihos       (501) staff       (20)      827 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/pkg_globals.py
+-rw-r--r--   0 ihos       (501) staff       (20)      502 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/settings.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.203794 cysecuretools-6.0.0/src/targets/
+-rw-r--r--   0 ihos       (501) staff       (20)     4025 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.204284 cysecuretools-6.0.0/src/targets/common/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1561 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/dependencies_validation.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3625 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/flow_parser.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.206647 cysecuretools-6.0.0/src/targets/common/mxs40sv2/
+-rw-r--r--   0 ihos       (501) staff       (20)     1329 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1434 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/asset.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1383 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/asset_builder.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3171 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/asset_enums.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.207082 cysecuretools-6.0.0/src/targets/common/mxs40sv2/debug_cert/
+-rw-r--r--   0 ihos       (501) staff       (20)      742 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/debug_cert/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3141 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4463 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_parser_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.208264 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2027 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1393 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2098 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3485 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1598 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1287 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1833 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependency_validator_mxs40v2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1249 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/enums.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.208856 cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/
+-rw-r--r--   0 ihos       (501) staff       (20)      732 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3243 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/encrypt_mxv40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)    17996 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/signtool_mxv40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1325 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/xip_encryptor_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.209711 cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/
+-rw-r--r--   0 ihos       (501) staff       (20)    24916 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     2049 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     7972 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)    29537 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/cyw20829_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     4920 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/key_source_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3380 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/nv_counter_calc.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12661 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/policy_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1718 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/policy_validator_mxs40v2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2018 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/project_init_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.210215 cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      802 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6955 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning/provision_device_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     9446 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning/ram_app_loader_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7028 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning_packet_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3981 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/silicon_data_reader_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2917 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40sv2/version_provider_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.213921 cysecuretools-6.0.0/src/targets/common/mxs40v1/
+-rw-r--r--   0 ihos       (501) staff       (20)     1510 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3172 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/bootloader_provider_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.215647 cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/
+-rw-r--r--   0 ihos       (501) staff       (20)      735 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2561 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_cipher.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3830 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_header.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5396 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_header_strategy.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2957 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/ecc_kdf.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3227 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/encrypted_programming.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.216371 cysecuretools-6.0.0/src/targets/common/mxs40v1/entrance_exam/
+-rw-r--r--   0 ihos       (501) staff       (20)      778 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/entrance_exam/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8150 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/entrance_exam/exam_cyb06xx7.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8821 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/entrance_exam/exam_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)      932 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/enums.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5110 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/image_cert.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.216939 cysecuretools-6.0.0/src/targets/common/mxs40v1/json/
+-rw-r--r--   0 ihos       (501) staff       (20)     4452 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/json/policy_template.json
+-rw-r--r--   0 ihos       (501) staff       (20)    15796 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/json/schema.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     1977 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/key_reader_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)      923 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/key_source_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5840 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/policy_filter.py
+-rw-r--r--   0 ihos       (501) staff       (20)    15632 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/policy_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)    46274 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/policy_validator.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.217471 cysecuretools-6.0.0/src/targets/common/mxs40v1/prebuilt/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/prebuilt/cy_pub_key.json
+-rw-r--r--   0 ihos       (501) staff       (20)      511 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/prebuilt/hsm_state.json
+-rw-r--r--   0 ihos       (501) staff       (20)      511 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/prebuilt/oem_state.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8014 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/project_init_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.218118 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      742 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    20588 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning/provision_device_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    22504 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning/sys_call.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.218546 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/
+-rw-r--r--   0 ihos       (501) staff       (20)      751 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.219867 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5501 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_crypto.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1584 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_customer.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3478 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_dev.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1822 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_entity.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3411 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_hsm.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3112 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_oem.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1147 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_types.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8651 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/provisioning_packet_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    17211 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/signtool_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1441 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/silicon_data_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2934 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/silicon_data_reader_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8744 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/version_provider_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.220248 cysecuretools-6.0.0/src/targets/common/mxs40v1/voltage_tool/
+-rw-r--r--   0 ihos       (501) staff       (20)      737 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/voltage_tool/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3215 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/voltage_tool/lvd_voltage_picker.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1327 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/voltage_tool/voltage_tool_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    10084 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/mxs40v1/x509_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4453 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/policy_validator.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.220389 cysecuretools-6.0.0/src/targets/common/prebuilt/
+-rw-r--r--   0 ihos       (501) staff       (20)      173 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/prebuilt/bootloader_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.220643 cysecuretools-6.0.0/src/targets/common/traveo_t2g/
+-rw-r--r--   0 ihos       (501) staff       (20)      730 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/traveo_t2g/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12804 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/common/traveo_t2g/signtool_xmc7xxx.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.221070 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/
+-rw-r--r--   0 ihos       (501) staff       (20)     1242 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.221212 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.221634 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1681 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2483 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.222203 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1051 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/packets/cy_auth_512k_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.223499 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     5498 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5500 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4_smif.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5111 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5111 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4_smif.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.172121 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.224602 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   134553 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      536 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.228925 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   148119 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      540 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     3936 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx5_a1/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.229539 cysecuretools-6.0.0/src/targets/cyb06xx7/
+-rw-r--r--   0 ihos       (501) staff       (20)     1548 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.229922 cysecuretools-6.0.0/src/targets/cyb06xx7/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.230476 cysecuretools-6.0.0/src/targets/cyb06xx7/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1991 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2484 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.231341 cysecuretools-6.0.0/src/targets/cyb06xx7/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1031 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.232163 cysecuretools-6.0.0/src/targets/cyb06xx7/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     5115 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5115 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4903 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4903 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.172662 cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.233123 cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   138714 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      543 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.233774 cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   150520 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      542 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     3799 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xx7/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.234037 cysecuretools-6.0.0/src/targets/cyb06xxa/
+-rw-r--r--   0 ihos       (501) staff       (20)     1147 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.234171 cysecuretools-6.0.0/src/targets/cyb06xxa/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.234559 cysecuretools-6.0.0/src/targets/cyb06xxa/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1682 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2485 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.235148 cysecuretools-6.0.0/src/targets/cyb06xxa/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1051 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.236451 cysecuretools-6.0.0/src/targets/cyb06xxa/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6084 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5800 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5637 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5589 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.173384 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.236933 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   158689 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      543 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.237346 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   138738 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      592 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.237945 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   172504 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      544 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.238743 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   155454 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      588 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     3802 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyb06xxa/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.239240 cysecuretools-6.0.0/src/targets/cys06xxa/
+-rw-r--r--   0 ihos       (501) staff       (20)     1151 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.239456 cysecuretools-6.0.0/src/targets/cys06xxa/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.240006 cysecuretools-6.0.0/src/targets/cys06xxa/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1031 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.240773 cysecuretools-6.0.0/src/targets/cys06xxa/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6084 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5800 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5637 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5589 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.174021 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.241694 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   158689 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      543 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.242512 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   138738 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      592 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.242934 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   172504 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      544 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.243658 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   155454 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      588 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      804 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cys06xxa/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.243917 cysecuretools-6.0.0/src/targets/cyw20829/
+-rw-r--r--   0 ihos       (501) staff       (20)     1196 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.244307 cysecuretools-6.0.0/src/targets/cyw20829/flows/
+-rw-r--r--   0 ihos       (501) staff       (20)      179 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/flows/oem_assets.json
+-rw-r--r--   0 ihos       (501) staff       (20)      858 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/flows/prov_flows.json
+-rw-r--r--   0 ihos       (501) staff       (20)       94 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/flows/reprovisioning_assets.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.244565 cysecuretools-6.0.0/src/targets/cyw20829/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/keys/pub_hci_0.pem
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/keys/pub_hci_1.pem
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.244825 cysecuretools-6.0.0/src/targets/cyw20829/packets/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.174605 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.245400 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/prov_oem/
+-rw-r--r--   0 ihos       (501) staff       (20)      235 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/prov_oem/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)     7780 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      375 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/prov_oem/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.246057 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/reprovisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      241 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/reprovisioning/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)    28868 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      264 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/reprovisioning/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.246712 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/to_rma/
+-rw-r--r--   0 ihos       (501) staff       (20)      269 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/to_rma/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)    28676 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      289 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/to_rma/info.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      624 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/debug_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)      168 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/packets/rsa_key_tmpl.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.248095 cysecuretools-6.0.0/src/targets/cyw20829/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6135 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_hci_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     6344 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)      374 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_reprovisioning_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     2099 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_reprovisioning_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8568 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1288 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.248663 cysecuretools-6.0.0/src/targets/cyw20829_a0/
+-rw-r--r--   0 ihos       (501) staff       (20)      984 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.249055 cysecuretools-6.0.0/src/targets/cyw20829_a0/flows/
+-rw-r--r--   0 ihos       (501) staff       (20)      179 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/flows/oem_assets.json
+-rw-r--r--   0 ihos       (501) staff       (20)      858 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/flows/prov_flows.json
+-rw-r--r--   0 ihos       (501) staff       (20)       94 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/flows/reprovisioning_assets.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.249316 cysecuretools-6.0.0/src/targets/cyw20829_a0/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/keys/pub_hci_0.pem
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/keys/pub_hci_1.pem
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.250199 cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     9431 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/asset_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1150 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1803 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/register_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     9308 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/reverse_asset_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.250543 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.175305 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.251054 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/
+-rw-r--r--   0 ihos       (501) staff       (20)      235 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)     7812 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      375 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.251711 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      241 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)    28836 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      264 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.252336 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/
+-rw-r--r--   0 ihos       (501) staff       (20)      269 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)    28612 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      289 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/info.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      624 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/debug_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)      168 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/rsa_key_tmpl.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.253499 cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6135 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_hci_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     6344 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)      374 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1812 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8281 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     2953 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/policy_generator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4043 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw20829_a0/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.253954 cysecuretools-6.0.0/src/targets/cyw89829/
+-rw-r--r--   0 ihos       (501) staff       (20)      985 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.254397 cysecuretools-6.0.0/src/targets/cyw89829/flows/
+-rw-r--r--   0 ihos       (501) staff       (20)      179 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/flows/oem_assets.json
+-rw-r--r--   0 ihos       (501) staff       (20)      858 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/flows/prov_flows.json
+-rw-r--r--   0 ihos       (501) staff       (20)       94 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/flows/reprovisioning_assets.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.254702 cysecuretools-6.0.0/src/targets/cyw89829/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/keys/pub_hci_0.pem
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/keys/pub_hci_1.pem
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.254975 cysecuretools-6.0.0/src/targets/cyw89829/packets/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.175903 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.255435 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/prov_oem/
+-rw-r--r--   0 ihos       (501) staff       (20)      235 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/prov_oem/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)     7780 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      375 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/prov_oem/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.256115 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/reprovisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      241 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/reprovisioning/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)    28868 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      264 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/reprovisioning/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.256645 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/to_rma/
+-rw-r--r--   0 ihos       (501) staff       (20)      269 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/to_rma/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)    28676 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      289 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/to_rma/info.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      624 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/debug_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)      168 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/packets/rsa_key_tmpl.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.257710 cysecuretools-6.0.0/src/targets/cyw89829/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6135 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_hci_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     6344 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)      374 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_reprovisioning_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     2099 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_reprovisioning_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8568 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1275 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/cyw89829/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2024-05-28 15:41:27.258184 cysecuretools-6.0.0/src/targets/xmc7xxx/
+-rw-r--r--   0 ihos       (501) staff       (20)     1124 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/xmc7xxx/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2549 2024-05-28 15:22:09.000000 cysecuretools-6.0.0/src/targets/xmc7xxx/target_builder.py
```

### Comparing `cysecuretools-5.1.0/CHANGELOG.md` & `cysecuretools-6.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 6.0.0
+### Added
+- Support for Python 3.12
+
+### Changed
+- Extended package installation instructions
+- Extended CYW20829/CYW89829 readme with usage examples
+- Drop support for Python versions 3.6 and 3.7
+
 ## 5.1.0
 ### Added
 - Support for CYW89829 devices
 
 ## 5.0.0
+### Added
+- Support for XMC7100, XMC7200 devices
+
 ### Changed
 - Removed pyOCD support. OpenOCD is used as a default On-Chip debugger for all platforms
 - High-level API module refactoring
 
-### Added
-- Support for XMC7100, XMC7200 devices
-
 ## 4.2.0
 ### Added
 - Support for CYW20829 B0 silicon revision
 - Multi-image NV counter for CYW20829
 - Transition PSoC 64 devices to RMA LCS
 - Open PSoC 64 devices in RMA LCS for debugging
 - OpenOCD autodiscovery in ModusToolbox directory
```

### Comparing `cysecuretools-5.1.0/LICENSE` & `cysecuretools-6.0.0/src/execute/image_signing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+"""
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
+"""
+from .image import Image
```

### Comparing `cysecuretools-5.1.0/PKG-INFO` & `cysecuretools-6.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,11 @@
-Metadata-Version: 2.1
-Name: cysecuretools
-Version: 5.1.0
-Summary: Python tools for provisioning Cypress/Infineon MCUs
-Home-page: https://github.com/Infineon/cysecuretools
-Author: Cypress Semiconductor Corporation (an Infineon company)
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-This package contains security tools for creating keys, creating certificates, signing user applications, and provisioning Cypress MCUs.
+This package contains security tools for creating keys, creating certificates, signing user applications, and provisioning Cypress/Infineon MCUs.
 
 # Table of Contents
+- [HW/SW compatibility](#hwsw-compatibility)
 - [Prerequisites](#prerequisites)
 - [Documentation](#documentation)
 - [Installing package](#installing-package)
 - [Supported devices](#supported-devices)
 - [Interface and Usage](#interface-and-usage)
     - [PSoC 64](#psoc-64)
     - [CYW20829/CYW89829](#cyw20829cyw89829)
@@ -36,176 +17,197 @@
 
 # HW/SW compatibility
 ## PSoC 64
 <table>
   <thead>
     <tr>
       <td>Target/Kit</td>
-      <td>Silicon Revision<sup>1</sup></td>
       <td>Silicon ID, Silicon Rev., Family ID</td>
       <td>Secure FlashBoot Version</td>
       <td>CyBootloader Version</td>
     </tr>
   </thead>
   <tbody>
     <tr>
       <td colspan="6" style="text-align: center;">512K</td>
     </tr>
     <tr>
       <td>
         cyb06xx5<br>
         cy8cproto&#8209;064b0s3
       </td>
-      <td>A1</td>
       <td>0xE70D, 0x12, 0x105</td>
       <td>4.0.2.1842</td>
       <td>2.0.1.6441</td>
     </tr>
     <tr>
       <td colspan="6" style="text-align: center;">2M</td>
     </tr>
     <tr>
       <td>
         cyb06xxa<br>
         cy8ckit&#8209;064b0s2&#8209;4343w
       </td>
-      <td>A1</td>
       <td>0xE470, 0x12, 0x102</td>
       <td>4.0.3.2319</td>
       <td>2.0.2.8102</td>
     </tr>
     <tr>
       <td>
         cys06xxa<br>
         cy8ckit&#8209;064s0s2&#8209;4343w
       </td>
-      <td>A1</td>
       <td>0xE4A0, 0x12, 0x02</td>
       <td>4.0.3.2319</td>
       <td>2.0.2.8102</td>
     </tr>
     <tr>
       <td colspan="6" style="text-align: center;">1M</td>
     </tr>
     <tr>
       <td>
         cyb06xx7<br>
         cy8cproto&#8209;064s1&#8209;sb<br>
         cy8cproto&#8209;064b0s1&#8209;ble<br>
         cy8cproto&#8209;064b0s1&#8209;ssa
       </td>
-      <td>B3</td>
       <td>
         0xE262, 0x24, 0x100
         0xE261, 0x24, 0x100
       </td>
       <td>4.0.2.1842</td>
       <td>2.0.0.4041</td>
     </tr>
   </tbody>
 </table>
 
-## CYW20829
+## CYW20829 / CYW89829
 <table>
   <thead>
     <tr>
       <td>Target/Kit</td>
-      <td>Silicon Revision<sup>1</sup></td>
       <td>Silicon ID, Silicon Rev., Family ID</td>
       <td>ROM Boot Version</td>
       <td>RAM Applications Version</td>
     </tr>
   </thead>
   <tbody>
   <tr>
     <td>cyw20829</td>
-    <td>A0</td>
-    <td>0xEB40, 0x11, 0x110</td>
-    <td>1.0.0.7120</td>
-    <td>1.0.0.2857</td>
-  </tr>
-  <tr>
-    <td>cyw20829</td>
-    <td>B0</td>
     <td>0xEB43, 0x21, 0x110</td>
     <td>1.2.0.8334</td>
     <td>1.2.0.3073</td>
   </tr>
-  </tbody>
-</table>
-
-<sup>1</sup> Specify `--rev` option for older revision of the silicon (e.g. `$ cysecuretools -t cyw20829 --rev a0 <COMMAND>`). Using the latest revision does not require specifying the option.
-
-## CYW89829
-<table>
-  <thead>
-    <tr>
-      <td>Target/Kit</td>
-      <td>Silicon Revision</td>
-      <td>Silicon ID, Silicon Rev., Family ID</td>
-      <td>ROM Boot Version</td>
-      <td>RAM Applications Version</td>
-    </tr>
-  </thead>
-  <tbody>
   <tr>
     <td>cyw89829</td>
-    <td>B0</td>
     <td>0xEB47, 0x21, 0x110</td>
     <td>1.2.0.8334</td>
     <td>1.2.0.3073</td>
   </tr>
   </tbody>
 </table>
 
 # Prerequisites
 * General
-  * Python 3.6 or later
-  * [Installed Cypress OpenOCD](https://github.com/Infineon/openocd/releases)
-* For PSoC 64 devices
-  * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
-  * Ensure the power selection jumper is set to provide 2.5 V to the power supply pin related to eFuse power. This voltage level is required to blow eFuses
-* For CYW20829/CYW89829 devices
+  * Python 3.8 - 3.12
+  * [Installed Infineon OpenOCD](https://github.com/Infineon/openocd/releases)
+* For PSoC 64 / CYW20829 / CYW89829 devices
   * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
   * Ensure the power selection jumper is set to provide 2.5 V to the power supply pin related to eFuse power. This voltage level is required to blow eFuses
 
 
 # Documentation
 * [PSoC64 Secure MCU Secure Boot SDK User Guide](https://www.cypress.com/documentation/software-and-drivers/psoc-64-secure-mcu-secure-boot-sdk-user-guide)
 * [Changelog](https://github.com/Infineon/cysecuretools/blob/master/CHANGELOG.md)
 
 # Installing Package
-Invoke `pip install` from the command line:
+## Windows
+The installation of ModusToolbox™ Software 3.1 includes the correct version of Python and CySecureTools 5.0.0. The latest version of CySecureTools is 6.0.0.
+To update the package from the ModusToolbox™ shell (for Windows users):
+* In the ModusToolbox™ GUI open the terminal by clicking the **Terminal** tab in the bottom pane.
+* Then, select a project in the **Project Explorer** to open a shell in the project directory.
+* Enter the following command: `$ pip install --upgrade --force-reinstall edgeprotecttools`
+
+## Linux / macOS
+Install Python 3.12 on your computer. You can download it from https://www.python.org/downloads/.
+
+Set up the appropriate environment variable(s) for your operating system.
+
+If Python 2.7 is also installed, make sure that Python312 and Python312\Scripts have higher priority in the
+PATH than CPython27.
+
+### Linux Configuration
+Most distributions of Linux should already have python2 and python3 installed. To verify that python by
+default points to python3 run:
+```bash
+$ python --version
+```
+If python3 is not set as default, run the following commands. The number at the end of each command
+denotes a priority:
+```bash
+$ update-alternatives --install /usr/bin/python python /usr/bin/python2.7 1
+$ update-alternatives --install /usr/bin/python python /usr/bin/python3.12 2
+```
+
+### macOS Configuration
+By default, `python` points to `/usr/bin/python`, which is python2. To make `python` and `pip` resolve to
+python3 versions, execute the following from command line:
+```bash
+$ echo 'alias python=python3' >> ~/.bash_profile
+$ echo 'alias pip=pip3' >> ~/.bash_profile
+$ source ~/.bash_profile
+$ python --version
+Python 3.12.3
+$ pip --version
+pip 24.0 from
+/Library/Frameworks/Python.framework/Versions/3.12/lib/python3.12/site-packages/pip (python 3.12)
+```
+Note: If you use a shell other than bash, update its profile file accordingly. For example `~/.zshrc` if you use zsh instead of `~/.bash_profile`.
+
+### Installing CySecureTools Package
+Make sure that you have the latest version of pip installed, use
+the following command.
+```bash
+$ python -m pip install --upgrade pip
+```
+Run the following command in your terminal window.
 ```bash
-$ pip install cysecuretools
+$ python -m pip install cysecuretools
 ```
+
+### Updating CySecureTools Package
 To update the already installed package:
 ```bash
 $ pip install --upgrade --force-reinstall cysecuretools
 ```
 
+Note 1: During installation, you may see errors saying that cysecuretools requires package version X, but you have package version Y which is incompatible. In most cases, these can be safely ignored.
+
+Note 2: You can use the following command to show the path to the installed package
+`python -m pip show cysecuretools`.
+
 
 # Supported devices
 Use `device-list` command for output of the supported devices list.
 ```bash
 $ cysecuretools device-list
 ```
 
 
 # Interface and Usage
-## PSoC 64
+## PSoC 64 CLI
 See [README_PSOC64.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_PSOC64.md)
-## CYW20829/CYW89829
+## CYW20829/CYW89829 CLI
 See [README_CYW20829.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_CYW20829.md)
-## XMC7100/7200
+## XMC7100/7200 CLI
 See [README_XMC7XXX.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_XMC7XXX.md)
 
 
 # Logging
-Every time the tool is invoked, a new log file is created in the _logs_ directory of the project. By default, the console output has INFO logging severity. The log file contains the DEBUG logging severity.
+Every time the tool is invoked, a new log file is created in the _logs_ directory of the project. By default, the console output has INFO logging severity. The log file has the DEBUG logging severity.
 
 
 # Known issues
 - Using the policy from version 4.0.0 in projects created by version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE error during re-provisioning on PSoC64-2M devices:
 ```
   ...
   ERROR : SFB status: CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid image certificate signature. Check the log for details
@@ -240,110 +242,7 @@
   maintainers to find out if a fix or workaround is available.
 ```
 _Solution:_ Upgrade the `pip` package running the following command from the terminal: `python3 -m pip install --upgrade pip`.
 
 # License and Contributions
 The software is provided under the Apache-2.0 license. Contributions to this project are accepted under the same license.
 This project contains code from other projects. The original license text is included in those source files.
-
-
-# Changelog
-All notable changes to this project will be documented in this file.
-
-## 5.1.0
-### Added
-- Support for CYW89829 devices
-
-## 5.0.0
-### Changed
-- Removed pyOCD support. OpenOCD is used as a default On-Chip debugger for all platforms
-- High-level API module refactoring
-
-### Added
-- Support for XMC7100, XMC7200 devices
-
-## 4.2.0
-### Added
-- Support for CYW20829 B0 silicon revision
-- Multi-image NV counter for CYW20829
-- Transition PSoC 64 devices to RMA LCS
-- Open PSoC 64 devices in RMA LCS for debugging
-- OpenOCD autodiscovery in ModusToolbox directory 
-- Add SW/HW compatibility table to the readme
-
-### Changed
-- Target `cyw20829` is used for the latest silicon revision. For the previous silicon revision (A0) add _--rev_ option in the command line (`-t cyw20829 --rev a0`)
-
-## 4.1.0
-### Added
-- OpenOCD support for PSoC 64 devices
-- Creating update package in the unsigned image (_extend-image_ command)
-
-### Changed
-- Fixed installation failure using pip 22.1
-- CyBootloader 2.0.2.8102 for PSoC 64 2M:
-  - Improved performance of SWAP algorithm
-  - Image certificate signed with the Infineon key (id=3)
-  - Use Infineon key (id=3) for bootloader in the policy files
-
-## 4.0.0
-### Added
-- Support of CYW20829 devices
-- Support Python 3.10
-- Signing images with HSM
-
-### Changed
-- Separated PSoC 64 and CYW20829 devices CLI
-- Updated PSoC 64 CyBootloader for 512k and 2M:
-  - added "reset_after_failure" feature
-  - decreased boot time
-- Protect PSA API from NSPE in PSoC 64 2M-S0 policy
-- Prevent signing of already signed images
-- Change MCUboot image header padding to erase value
-- Use CyBootloader from the project directory if the project exists
-- Updated dependencies packages to the latest versions
-- Use pyocd 0.32.3
-
-## 3.1.1
-### Changed
-- Fixed installation failure on macOS Big Sur and Apple M1 chip
-- Fixed installation failure in Python 3.9
-
-## 3.1.0
-### Added
-- SCRATCH with Status Partition swap mode
-- Small image slots support in the external memory
-
-## 3.0.0
-### Added
-- Image SWAP using Status Partition
-
-### Changed
-- CyBootloader 2.0
-- Secure Flash Boot 4.0.2 support
-
-## 2.1.0
-### Added
-- Support PSoC64 1M
-- New command to read device die ID
-- Optionally add boot record to the signed image
-- New policy validators (address overlaps between images and bootloader, slots address alignment with the SMPU address limits, DAP closure, monotonic counter)
-- Log the device response JWT during the provisioning process
-
-### Changed
-- Fixed issue with using group private key
-- Use pyocd 0.27.3
-
-
-## 2.0.0
-### Added
-- Support PSoC64 2M, PSoC64 512K
-- Command line interface
-- Encrypted programming
-- Single-image and multi-image policy
-
-### Changed
-- Update provisioning according to new Secure Flash Boot functionality (update system calls, reprovisioning, encrypted image support)
-- New CyBootloaders (CY8CKIT-064B0S2-4343W, CY8CKIT-064S0S2-4343W, CY8CPROTO-064B0S3)
-- Use pyocd 0.27.0
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,134 +1,105 @@
-Metadata-Version: 2.1 Name: cysecuretools Version: 5.1.0 Summary: Python tools
-for provisioning Cypress/Infineon MCUs Home-page: https://github.com/Infineon/
-cysecuretools Author: Cypress Semiconductor Corporation (an Infineon company)
-License: Apache 2.0 Platform: UNKNOWN Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
-:: OS Independent Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE This package contains security tools for creating keys, creating
-certificates, signing user applications, and provisioning Cypress MCUs. # Table
-of Contents - [Prerequisites](#prerequisites) - [Documentation](#documentation)
-- [Installing package](#installing-package) - [Supported devices](#supported-
-devices) - [Interface and Usage](#interface-and-usage) - [PSoC 64](#psoc-64) -
-[CYW20829/CYW89829](#cyw20829cyw89829) - [XMC7100/7200](#xmc71007200) -
-[Logging](#logging) - [Installing libusb driver](#installing-libusb-driver) -
-[Known issues](#known-issues) - [License and Contributions](#license-and-
-contributions) # HW/SW compatibility ## PSoC 64
-                      Silicon   Silicon ID,   Secure FlashBoot CyBootloader
-Target/Kit            Revision1 Silicon Rev., Version          Version
-                                Family ID
-                                                      512K
-cyb06xx5              A1        0xE70D, 0x12, 4.0.2.1842       2.0.1.6441
-cy8cproto‑064b0s3               0x105
-                                                       2M
-cyb06xxa              A1        0xE470, 0x12, 4.0.3.2319       2.0.2.8102
-cy8ckit‑064b0s2‑4343w           0x102
-cys06xxa              A1        0xE4A0, 0x12, 4.0.3.2319       2.0.2.8102
-cy8ckit‑064s0s2‑4343w           0x02
-                                                       1M
-cyb06xx7                        0xE262, 0x24,
-cy8cproto‑064s1‑sb    B3        0x100 0xE261, 4.0.2.1842       2.0.0.4041
-cy8cproto‑064b0s1‑ble           0x24, 0x100
+This package contains security tools for creating keys, creating certificates,
+signing user applications, and provisioning Cypress/Infineon MCUs. # Table of
+Contents - [HW/SW compatibility](#hwsw-compatibility) - [Prerequisites]
+(#prerequisites) - [Documentation](#documentation) - [Installing package]
+(#installing-package) - [Supported devices](#supported-devices) - [Interface
+and Usage](#interface-and-usage) - [PSoC 64](#psoc-64) - [CYW20829/CYW89829]
+(#cyw20829cyw89829) - [XMC7100/7200](#xmc71007200) - [Logging](#logging) -
+[Installing libusb driver](#installing-libusb-driver) - [Known issues](#known-
+issues) - [License and Contributions](#license-and-contributions) # HW/SW
+compatibility ## PSoC 64
+Target/Kit            Silicon ID, Silicon Secure FlashBoot CyBootloader
+                      Rev., Family ID     Version          Version
+                                                   512K
+cyb06xx5              0xE70D, 0x12, 0x105 4.0.2.1842       2.0.1.6441
+cy8cproto‑064b0s3
+                                                     2M
+cyb06xxa              0xE470, 0x12, 0x102 4.0.3.2319       2.0.2.8102
+cy8ckit‑064b0s2‑4343w
+cys06xxa              0xE4A0, 0x12, 0x02  4.0.3.2319       2.0.2.8102
+cy8ckit‑064s0s2‑4343w
+                                                     1M
+cyb06xx7
+cy8cproto‑064s1‑sb    0xE262, 0x24, 0x100 4.0.2.1842       2.0.0.4041
+cy8cproto‑064b0s1‑ble 0xE261, 0x24, 0x100
 cy8cproto‑064b0s1‑ssa
-## CYW20829
-                             Silicon ID,                    RAM Applications
-Target/Kit Silicon Revision1 Silicon Rev., ROM Boot Version Version
-                             Family ID
-cyw20829   A0                0xEB40, 0x11, 1.0.0.7120       1.0.0.2857
-                             0x110
-cyw20829   B0                0xEB43, 0x21, 1.2.0.8334       1.2.0.3073
-                             0x110
-1 Specify `--rev` option for older revision of the silicon (e.g. `$
-cysecuretools -t cyw20829 --rev a0 `). Using the latest revision does not
-require specifying the option. ## CYW89829
-                            Silicon ID,                    RAM Applications
-Target/Kit Silicon Revision Silicon Rev., ROM Boot Version Version
-                            Family ID
-cyw89829   B0               0xEB47, 0x21, 1.2.0.8334       1.2.0.3073
-                            0x110
-# Prerequisites * General * Python 3.6 or later * [Installed Cypress OpenOCD]
-(https://github.com/Infineon/openocd/releases) * For PSoC 64 devices * Ensure
-the KitProg3 programming mode is **CMSIS-DAP Bulk** * Ensure the power
-selection jumper is set to provide 2.5 V to the power supply pin related to
-eFuse power. This voltage level is required to blow eFuses * For CYW20829/
+## CYW20829 / CYW89829
+Target/Kit Silicon ID, Silicon Rev., ROM Boot Version RAM Applications Version
+           Family ID
+cyw20829   0xEB43, 0x21, 0x110       1.2.0.8334       1.2.0.3073
+cyw89829   0xEB47, 0x21, 0x110       1.2.0.8334       1.2.0.3073
+# Prerequisites * General * Python 3.8 - 3.12 * [Installed Infineon OpenOCD]
+(https://github.com/Infineon/openocd/releases) * For PSoC 64 / CYW20829 /
 CYW89829 devices * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk** *
 Ensure the power selection jumper is set to provide 2.5 V to the power supply
 pin related to eFuse power. This voltage level is required to blow eFuses #
 Documentation * [PSoC64 Secure MCU Secure Boot SDK User Guide](https://
 www.cypress.com/documentation/software-and-drivers/psoc-64-secure-mcu-secure-
 boot-sdk-user-guide) * [Changelog](https://github.com/Infineon/cysecuretools/
-blob/master/CHANGELOG.md) # Installing Package Invoke `pip install` from the
-command line: ```bash $ pip install cysecuretools ``` To update the already
-installed package: ```bash $ pip install --upgrade --force-reinstall
-cysecuretools ``` # Supported devices Use `device-list` command for output of
-the supported devices list. ```bash $ cysecuretools device-list ``` # Interface
-and Usage ## PSoC 64 See [README_PSOC64.md](https://github.com/Infineon/
-cysecuretools/blob/master/docs/README_PSOC64.md) ## CYW20829/CYW89829 See
-[README_CYW20829.md](https://github.com/Infineon/cysecuretools/blob/master/
-docs/README_CYW20829.md) ## XMC7100/7200 See [README_XMC7XXX.md](https://
-github.com/Infineon/cysecuretools/blob/master/docs/README_XMC7XXX.md) # Logging
-Every time the tool is invoked, a new log file is created in the _logs_
-directory of the project. By default, the console output has INFO logging
-severity. The log file contains the DEBUG logging severity. # Known issues -
-Using the policy from version 4.0.0 in projects created by version 4.1.0 causes
-the CY_FB_INVALID_IMG_JWT_SIGNATURE error during re-provisioning on PSoC64-2M
-devices: ``` ... ERROR : SFB status: CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid
-image certificate signature. Check the log for details ``` _Workaround_: 1.
-Open the policy file. 2. Navigate to section 1 of the `boot_upgrade/firmware`.
-3. Set `boot_auth` and `bootloader_keys` as follows: ``` "boot_auth": [ 3 ],
-"bootloader_keys": [ { "kid": 3, "key": "../keys/cy_pub_key.json" } ] ``` -
-During the installation of the package via _pip_ on Mac OS Big Sur, the
-following exception is raised: ``` ... distutils.errors.DistutilsError: Setup
-script exited with error: SandboxViolation: mkdir('/private/var/root/Library/
-Caches/com.apple.python/private/tmp/easy_install-y8c1npmz', 511) {} The package
-setup script has attempted to modify files on your system that are not within
-the EasyInstall build area, and has been aborted. This package cannot be safely
-installed by EasyInstall, and may not support alternate installation locations
-even if you run its setup script by hand. Please inform the package's author
-and the EasyInstall maintainers to find out if a fix or workaround is
-available. ``` _Solution:_ Upgrade the `pip` package running the following
-command from the terminal: `python3 -m pip install --upgrade pip`. # License
-and Contributions The software is provided under the Apache-2.0 license.
-Contributions to this project are accepted under the same license. This project
-contains code from other projects. The original license text is included in
-those source files. # Changelog All notable changes to this project will be
-documented in this file. ## 5.1.0 ### Added - Support for CYW89829 devices ##
-5.0.0 ### Changed - Removed pyOCD support. OpenOCD is used as a default On-Chip
-debugger for all platforms - High-level API module refactoring ### Added -
-Support for XMC7100, XMC7200 devices ## 4.2.0 ### Added - Support for CYW20829
-B0 silicon revision - Multi-image NV counter for CYW20829 - Transition PSoC 64
-devices to RMA LCS - Open PSoC 64 devices in RMA LCS for debugging - OpenOCD
-autodiscovery in ModusToolbox directory - Add SW/HW compatibility table to the
-readme ### Changed - Target `cyw20829` is used for the latest silicon revision.
-For the previous silicon revision (A0) add _--rev_ option in the command line
-(`-t cyw20829 --rev a0`) ## 4.1.0 ### Added - OpenOCD support for PSoC 64
-devices - Creating update package in the unsigned image (_extend-image_
-command) ### Changed - Fixed installation failure using pip 22.1 - CyBootloader
-2.0.2.8102 for PSoC 64 2M: - Improved performance of SWAP algorithm - Image
-certificate signed with the Infineon key (id=3) - Use Infineon key (id=3) for
-bootloader in the policy files ## 4.0.0 ### Added - Support of CYW20829 devices
-- Support Python 3.10 - Signing images with HSM ### Changed - Separated PSoC 64
-and CYW20829 devices CLI - Updated PSoC 64 CyBootloader for 512k and 2M: -
-added "reset_after_failure" feature - decreased boot time - Protect PSA API
-from NSPE in PSoC 64 2M-S0 policy - Prevent signing of already signed images -
-Change MCUboot image header padding to erase value - Use CyBootloader from the
-project directory if the project exists - Updated dependencies packages to the
-latest versions - Use pyocd 0.32.3 ## 3.1.1 ### Changed - Fixed installation
-failure on macOS Big Sur and Apple M1 chip - Fixed installation failure in
-Python 3.9 ## 3.1.0 ### Added - SCRATCH with Status Partition swap mode - Small
-image slots support in the external memory ## 3.0.0 ### Added - Image SWAP
-using Status Partition ### Changed - CyBootloader 2.0 - Secure Flash Boot 4.0.2
-support ## 2.1.0 ### Added - Support PSoC64 1M - New command to read device die
-ID - Optionally add boot record to the signed image - New policy validators
-(address overlaps between images and bootloader, slots address alignment with
-the SMPU address limits, DAP closure, monotonic counter) - Log the device
-response JWT during the provisioning process ### Changed - Fixed issue with
-using group private key - Use pyocd 0.27.3 ## 2.0.0 ### Added - Support PSoC64
-2M, PSoC64 512K - Command line interface - Encrypted programming - Single-image
-and multi-image policy ### Changed - Update provisioning according to new
-Secure Flash Boot functionality (update system calls, reprovisioning, encrypted
-image support) - New CyBootloaders (CY8CKIT-064B0S2-4343W, CY8CKIT-064S0S2-
-4343W, CY8CPROTO-064B0S3) - Use pyocd 0.27.0
+blob/master/CHANGELOG.md) # Installing Package ## Windows The installation of
+ModusToolboxâ¢ Software 3.1 includes the correct version of Python and
+CySecureTools 5.0.0. The latest version of CySecureTools is 6.0.0. To update
+the package from the ModusToolboxâ¢ shell (for Windows users): * In the
+ModusToolboxâ¢ GUI open the terminal by clicking the **Terminal** tab in the
+bottom pane. * Then, select a project in the **Project Explorer** to open a
+shell in the project directory. * Enter the following command: `$ pip install -
+-upgrade --force-reinstall edgeprotecttools` ## Linux / macOS Install Python
+3.12 on your computer. You can download it from https://www.python.org/
+downloads/. Set up the appropriate environment variable(s) for your operating
+system. If Python 2.7 is also installed, make sure that Python312 and
+Python312\Scripts have higher priority in the PATH than CPython27. ### Linux
+Configuration Most distributions of Linux should already have python2 and
+python3 installed. To verify that python by default points to python3 run:
+```bash $ python --version ``` If python3 is not set as default, run the
+following commands. The number at the end of each command denotes a priority:
+```bash $ update-alternatives --install /usr/bin/python python /usr/bin/
+python2.7 1 $ update-alternatives --install /usr/bin/python python /usr/bin/
+python3.12 2 ``` ### macOS Configuration By default, `python` points to `/usr/
+bin/python`, which is python2. To make `python` and `pip` resolve to python3
+versions, execute the following from command line: ```bash $ echo 'alias
+python=python3' >> ~/.bash_profile $ echo 'alias pip=pip3' >> ~/.bash_profile $
+source ~/.bash_profile $ python --version Python 3.12.3 $ pip --version pip
+24.0 from /Library/Frameworks/Python.framework/Versions/3.12/lib/python3.12/
+site-packages/pip (python 3.12) ``` Note: If you use a shell other than bash,
+update its profile file accordingly. For example `~/.zshrc` if you use zsh
+instead of `~/.bash_profile`. ### Installing CySecureTools Package Make sure
+that you have the latest version of pip installed, use the following command.
+```bash $ python -m pip install --upgrade pip ``` Run the following command in
+your terminal window. ```bash $ python -m pip install cysecuretools ``` ###
+Updating CySecureTools Package To update the already installed package: ```bash
+$ pip install --upgrade --force-reinstall cysecuretools ``` Note 1: During
+installation, you may see errors saying that cysecuretools requires package
+version X, but you have package version Y which is incompatible. In most cases,
+these can be safely ignored. Note 2: You can use the following command to show
+the path to the installed package `python -m pip show cysecuretools`. #
+Supported devices Use `device-list` command for output of the supported devices
+list. ```bash $ cysecuretools device-list ``` # Interface and Usage ## PSoC 64
+CLI See [README_PSOC64.md](https://github.com/Infineon/cysecuretools/blob/
+master/docs/README_PSOC64.md) ## CYW20829/CYW89829 CLI See [README_CYW20829.md]
+(https://github.com/Infineon/cysecuretools/blob/master/docs/README_CYW20829.md)
+## XMC7100/7200 CLI See [README_XMC7XXX.md](https://github.com/Infineon/
+cysecuretools/blob/master/docs/README_XMC7XXX.md) # Logging Every time the tool
+is invoked, a new log file is created in the _logs_ directory of the project.
+By default, the console output has INFO logging severity. The log file has the
+DEBUG logging severity. # Known issues - Using the policy from version 4.0.0 in
+projects created by version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE
+error during re-provisioning on PSoC64-2M devices: ``` ... ERROR : SFB status:
+CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid image certificate signature. Check the
+log for details ``` _Workaround_: 1. Open the policy file. 2. Navigate to
+section 1 of the `boot_upgrade/firmware`. 3. Set `boot_auth` and
+`bootloader_keys` as follows: ``` "boot_auth": [ 3 ], "bootloader_keys": [
+{ "kid": 3, "key": "../keys/cy_pub_key.json" } ] ``` - During the installation
+of the package via _pip_ on Mac OS Big Sur, the following exception is raised:
+``` ... distutils.errors.DistutilsError: Setup script exited with error:
+SandboxViolation: mkdir('/private/var/root/Library/Caches/com.apple.python/
+private/tmp/easy_install-y8c1npmz', 511) {} The package setup script has
+attempted to modify files on your system that are not within the EasyInstall
+build area, and has been aborted. This package cannot be safely installed by
+EasyInstall, and may not support alternate installation locations even if you
+run its setup script by hand. Please inform the package's author and the
+EasyInstall maintainers to find out if a fix or workaround is available. ```
+_Solution:_ Upgrade the `pip` package running the following command from the
+terminal: `python3 -m pip install --upgrade pip`. # License and Contributions
+The software is provided under the Apache-2.0 license. Contributions to this
+project are accepted under the same license. This project contains code from
+other projects. The original license text is included in those source files.
```

### Comparing `cysecuretools-5.1.0/cysecuretools.egg-info/PKG-INFO` & `cysecuretools-6.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: cysecuretools
-Version: 5.1.0
+Version: 6.0.0
 Summary: Python tools for provisioning Cypress/Infineon MCUs
 Home-page: https://github.com/Infineon/cysecuretools
 Author: Cypress Semiconductor Corporation (an Infineon company)
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools==69.5.1
+Requires-Dist: cryptography==36.0.1
+Requires-Dist: click==8.0.4
+Requires-Dist: intelhex==2.3.0
+Requires-Dist: python-jose==3.3.0
+Requires-Dist: jsonschema<=4.22.0,>=4.0.0
+Requires-Dist: cbor==1.0.0
+Requires-Dist: packaging==21.3
+Requires-Dist: lief==0.14.1
 
-This package contains security tools for creating keys, creating certificates, signing user applications, and provisioning Cypress MCUs.
+This package contains security tools for creating keys, creating certificates, signing user applications, and provisioning Cypress/Infineon MCUs.
 
 # Table of Contents
+- [HW/SW compatibility](#hwsw-compatibility)
 - [Prerequisites](#prerequisites)
 - [Documentation](#documentation)
 - [Installing package](#installing-package)
 - [Supported devices](#supported-devices)
 - [Interface and Usage](#interface-and-usage)
     - [PSoC 64](#psoc-64)
     - [CYW20829/CYW89829](#cyw20829cyw89829)
@@ -36,176 +45,197 @@
 
 # HW/SW compatibility
 ## PSoC 64
 <table>
   <thead>
     <tr>
       <td>Target/Kit</td>
-      <td>Silicon Revision<sup>1</sup></td>
       <td>Silicon ID, Silicon Rev., Family ID</td>
       <td>Secure FlashBoot Version</td>
       <td>CyBootloader Version</td>
     </tr>
   </thead>
   <tbody>
     <tr>
       <td colspan="6" style="text-align: center;">512K</td>
     </tr>
     <tr>
       <td>
         cyb06xx5<br>
         cy8cproto&#8209;064b0s3
       </td>
-      <td>A1</td>
       <td>0xE70D, 0x12, 0x105</td>
       <td>4.0.2.1842</td>
       <td>2.0.1.6441</td>
     </tr>
     <tr>
       <td colspan="6" style="text-align: center;">2M</td>
     </tr>
     <tr>
       <td>
         cyb06xxa<br>
         cy8ckit&#8209;064b0s2&#8209;4343w
       </td>
-      <td>A1</td>
       <td>0xE470, 0x12, 0x102</td>
       <td>4.0.3.2319</td>
       <td>2.0.2.8102</td>
     </tr>
     <tr>
       <td>
         cys06xxa<br>
         cy8ckit&#8209;064s0s2&#8209;4343w
       </td>
-      <td>A1</td>
       <td>0xE4A0, 0x12, 0x02</td>
       <td>4.0.3.2319</td>
       <td>2.0.2.8102</td>
     </tr>
     <tr>
       <td colspan="6" style="text-align: center;">1M</td>
     </tr>
     <tr>
       <td>
         cyb06xx7<br>
         cy8cproto&#8209;064s1&#8209;sb<br>
         cy8cproto&#8209;064b0s1&#8209;ble<br>
         cy8cproto&#8209;064b0s1&#8209;ssa
       </td>
-      <td>B3</td>
       <td>
         0xE262, 0x24, 0x100
         0xE261, 0x24, 0x100
       </td>
       <td>4.0.2.1842</td>
       <td>2.0.0.4041</td>
     </tr>
   </tbody>
 </table>
 
-## CYW20829
+## CYW20829 / CYW89829
 <table>
   <thead>
     <tr>
       <td>Target/Kit</td>
-      <td>Silicon Revision<sup>1</sup></td>
       <td>Silicon ID, Silicon Rev., Family ID</td>
       <td>ROM Boot Version</td>
       <td>RAM Applications Version</td>
     </tr>
   </thead>
   <tbody>
   <tr>
     <td>cyw20829</td>
-    <td>A0</td>
-    <td>0xEB40, 0x11, 0x110</td>
-    <td>1.0.0.7120</td>
-    <td>1.0.0.2857</td>
-  </tr>
-  <tr>
-    <td>cyw20829</td>
-    <td>B0</td>
     <td>0xEB43, 0x21, 0x110</td>
     <td>1.2.0.8334</td>
     <td>1.2.0.3073</td>
   </tr>
-  </tbody>
-</table>
-
-<sup>1</sup> Specify `--rev` option for older revision of the silicon (e.g. `$ cysecuretools -t cyw20829 --rev a0 <COMMAND>`). Using the latest revision does not require specifying the option.
-
-## CYW89829
-<table>
-  <thead>
-    <tr>
-      <td>Target/Kit</td>
-      <td>Silicon Revision</td>
-      <td>Silicon ID, Silicon Rev., Family ID</td>
-      <td>ROM Boot Version</td>
-      <td>RAM Applications Version</td>
-    </tr>
-  </thead>
-  <tbody>
   <tr>
     <td>cyw89829</td>
-    <td>B0</td>
     <td>0xEB47, 0x21, 0x110</td>
     <td>1.2.0.8334</td>
     <td>1.2.0.3073</td>
   </tr>
   </tbody>
 </table>
 
 # Prerequisites
 * General
-  * Python 3.6 or later
-  * [Installed Cypress OpenOCD](https://github.com/Infineon/openocd/releases)
-* For PSoC 64 devices
-  * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
-  * Ensure the power selection jumper is set to provide 2.5 V to the power supply pin related to eFuse power. This voltage level is required to blow eFuses
-* For CYW20829/CYW89829 devices
+  * Python 3.8 - 3.12
+  * [Installed Infineon OpenOCD](https://github.com/Infineon/openocd/releases)
+* For PSoC 64 / CYW20829 / CYW89829 devices
   * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
   * Ensure the power selection jumper is set to provide 2.5 V to the power supply pin related to eFuse power. This voltage level is required to blow eFuses
 
 
 # Documentation
 * [PSoC64 Secure MCU Secure Boot SDK User Guide](https://www.cypress.com/documentation/software-and-drivers/psoc-64-secure-mcu-secure-boot-sdk-user-guide)
 * [Changelog](https://github.com/Infineon/cysecuretools/blob/master/CHANGELOG.md)
 
 # Installing Package
-Invoke `pip install` from the command line:
+## Windows
+The installation of ModusToolbox™ Software 3.1 includes the correct version of Python and CySecureTools 5.0.0. The latest version of CySecureTools is 6.0.0.
+To update the package from the ModusToolbox™ shell (for Windows users):
+* In the ModusToolbox™ GUI open the terminal by clicking the **Terminal** tab in the bottom pane.
+* Then, select a project in the **Project Explorer** to open a shell in the project directory.
+* Enter the following command: `$ pip install --upgrade --force-reinstall edgeprotecttools`
+
+## Linux / macOS
+Install Python 3.12 on your computer. You can download it from https://www.python.org/downloads/.
+
+Set up the appropriate environment variable(s) for your operating system.
+
+If Python 2.7 is also installed, make sure that Python312 and Python312\Scripts have higher priority in the
+PATH than CPython27.
+
+### Linux Configuration
+Most distributions of Linux should already have python2 and python3 installed. To verify that python by
+default points to python3 run:
+```bash
+$ python --version
+```
+If python3 is not set as default, run the following commands. The number at the end of each command
+denotes a priority:
 ```bash
-$ pip install cysecuretools
+$ update-alternatives --install /usr/bin/python python /usr/bin/python2.7 1
+$ update-alternatives --install /usr/bin/python python /usr/bin/python3.12 2
 ```
+
+### macOS Configuration
+By default, `python` points to `/usr/bin/python`, which is python2. To make `python` and `pip` resolve to
+python3 versions, execute the following from command line:
+```bash
+$ echo 'alias python=python3' >> ~/.bash_profile
+$ echo 'alias pip=pip3' >> ~/.bash_profile
+$ source ~/.bash_profile
+$ python --version
+Python 3.12.3
+$ pip --version
+pip 24.0 from
+/Library/Frameworks/Python.framework/Versions/3.12/lib/python3.12/site-packages/pip (python 3.12)
+```
+Note: If you use a shell other than bash, update its profile file accordingly. For example `~/.zshrc` if you use zsh instead of `~/.bash_profile`.
+
+### Installing CySecureTools Package
+Make sure that you have the latest version of pip installed, use
+the following command.
+```bash
+$ python -m pip install --upgrade pip
+```
+Run the following command in your terminal window.
+```bash
+$ python -m pip install cysecuretools
+```
+
+### Updating CySecureTools Package
 To update the already installed package:
 ```bash
 $ pip install --upgrade --force-reinstall cysecuretools
 ```
 
+Note 1: During installation, you may see errors saying that cysecuretools requires package version X, but you have package version Y which is incompatible. In most cases, these can be safely ignored.
+
+Note 2: You can use the following command to show the path to the installed package
+`python -m pip show cysecuretools`.
+
 
 # Supported devices
 Use `device-list` command for output of the supported devices list.
 ```bash
 $ cysecuretools device-list
 ```
 
 
 # Interface and Usage
-## PSoC 64
+## PSoC 64 CLI
 See [README_PSOC64.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_PSOC64.md)
-## CYW20829/CYW89829
+## CYW20829/CYW89829 CLI
 See [README_CYW20829.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_CYW20829.md)
-## XMC7100/7200
+## XMC7100/7200 CLI
 See [README_XMC7XXX.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_XMC7XXX.md)
 
 
 # Logging
-Every time the tool is invoked, a new log file is created in the _logs_ directory of the project. By default, the console output has INFO logging severity. The log file contains the DEBUG logging severity.
+Every time the tool is invoked, a new log file is created in the _logs_ directory of the project. By default, the console output has INFO logging severity. The log file has the DEBUG logging severity.
 
 
 # Known issues
 - Using the policy from version 4.0.0 in projects created by version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE error during re-provisioning on PSoC64-2M devices:
 ```
   ...
   ERROR : SFB status: CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid image certificate signature. Check the log for details
@@ -245,26 +275,35 @@
 The software is provided under the Apache-2.0 license. Contributions to this project are accepted under the same license.
 This project contains code from other projects. The original license text is included in those source files.
 
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 6.0.0
+### Added
+- Support for Python 3.12
+
+### Changed
+- Extended package installation instructions
+- Extended CYW20829/CYW89829 readme with usage examples
+- Drop support for Python versions 3.6 and 3.7
+
 ## 5.1.0
 ### Added
 - Support for CYW89829 devices
 
 ## 5.0.0
+### Added
+- Support for XMC7100, XMC7200 devices
+
 ### Changed
 - Removed pyOCD support. OpenOCD is used as a default On-Chip debugger for all platforms
 - High-level API module refactoring
 
-### Added
-- Support for XMC7100, XMC7200 devices
-
 ## 4.2.0
 ### Added
 - Support for CYW20829 B0 silicon revision
 - Multi-image NV counter for CYW20829
 - Transition PSoC 64 devices to RMA LCS
 - Open PSoC 64 devices in RMA LCS for debugging
 - OpenOCD autodiscovery in ModusToolbox directory 
@@ -341,9 +380,7 @@
 - Encrypted programming
 - Single-image and multi-image policy
 
 ### Changed
 - Update provisioning according to new Secure Flash Boot functionality (update system calls, reprovisioning, encrypted image support)
 - New CyBootloaders (CY8CKIT-064B0S2-4343W, CY8CKIT-064S0S2-4343W, CY8CPROTO-064B0S3)
 - Use pyocd 0.27.0
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,134 +1,159 @@
-Metadata-Version: 2.1 Name: cysecuretools Version: 5.1.0 Summary: Python tools
+Metadata-Version: 2.1 Name: cysecuretools Version: 6.0.0 Summary: Python tools
 for provisioning Cypress/Infineon MCUs Home-page: https://github.com/Infineon/
 cysecuretools Author: Cypress Semiconductor Corporation (an Infineon company)
-License: Apache 2.0 Platform: UNKNOWN Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
-:: OS Independent Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE This package contains security tools for creating keys, creating
-certificates, signing user applications, and provisioning Cypress MCUs. # Table
-of Contents - [Prerequisites](#prerequisites) - [Documentation](#documentation)
-- [Installing package](#installing-package) - [Supported devices](#supported-
-devices) - [Interface and Usage](#interface-and-usage) - [PSoC 64](#psoc-64) -
-[CYW20829/CYW89829](#cyw20829cyw89829) - [XMC7100/7200](#xmc71007200) -
-[Logging](#logging) - [Installing libusb driver](#installing-libusb-driver) -
-[Known issues](#known-issues) - [License and Contributions](#license-and-
-contributions) # HW/SW compatibility ## PSoC 64
-                      Silicon   Silicon ID,   Secure FlashBoot CyBootloader
-Target/Kit            Revision1 Silicon Rev., Version          Version
-                                Family ID
-                                                      512K
-cyb06xx5              A1        0xE70D, 0x12, 4.0.2.1842       2.0.1.6441
-cy8cproto‑064b0s3               0x105
-                                                       2M
-cyb06xxa              A1        0xE470, 0x12, 4.0.3.2319       2.0.2.8102
-cy8ckit‑064b0s2‑4343w           0x102
-cys06xxa              A1        0xE4A0, 0x12, 4.0.3.2319       2.0.2.8102
-cy8ckit‑064s0s2‑4343w           0x02
-                                                       1M
-cyb06xx7                        0xE262, 0x24,
-cy8cproto‑064s1‑sb    B3        0x100 0xE261, 4.0.2.1842       2.0.0.4041
-cy8cproto‑064b0s1‑ble           0x24, 0x100
+License: Apache 2.0 Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Operating System :: OS
+Independent Classifier: Topic :: Software Development :: Embedded Systems
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: setuptools==69.5.1 Requires-Dist: cryptography==36.0.1
+Requires-Dist: click==8.0.4 Requires-Dist: intelhex==2.3.0 Requires-Dist:
+python-jose==3.3.0 Requires-Dist: jsonschema<=4.22.0,>=4.0.0 Requires-Dist:
+cbor==1.0.0 Requires-Dist: packaging==21.3 Requires-Dist: lief==0.14.1 This
+package contains security tools for creating keys, creating certificates,
+signing user applications, and provisioning Cypress/Infineon MCUs. # Table of
+Contents - [HW/SW compatibility](#hwsw-compatibility) - [Prerequisites]
+(#prerequisites) - [Documentation](#documentation) - [Installing package]
+(#installing-package) - [Supported devices](#supported-devices) - [Interface
+and Usage](#interface-and-usage) - [PSoC 64](#psoc-64) - [CYW20829/CYW89829]
+(#cyw20829cyw89829) - [XMC7100/7200](#xmc71007200) - [Logging](#logging) -
+[Installing libusb driver](#installing-libusb-driver) - [Known issues](#known-
+issues) - [License and Contributions](#license-and-contributions) # HW/SW
+compatibility ## PSoC 64
+Target/Kit            Silicon ID, Silicon Secure FlashBoot CyBootloader
+                      Rev., Family ID     Version          Version
+                                                   512K
+cyb06xx5              0xE70D, 0x12, 0x105 4.0.2.1842       2.0.1.6441
+cy8cproto‑064b0s3
+                                                     2M
+cyb06xxa              0xE470, 0x12, 0x102 4.0.3.2319       2.0.2.8102
+cy8ckit‑064b0s2‑4343w
+cys06xxa              0xE4A0, 0x12, 0x02  4.0.3.2319       2.0.2.8102
+cy8ckit‑064s0s2‑4343w
+                                                     1M
+cyb06xx7
+cy8cproto‑064s1‑sb    0xE262, 0x24, 0x100 4.0.2.1842       2.0.0.4041
+cy8cproto‑064b0s1‑ble 0xE261, 0x24, 0x100
 cy8cproto‑064b0s1‑ssa
-## CYW20829
-                             Silicon ID,                    RAM Applications
-Target/Kit Silicon Revision1 Silicon Rev., ROM Boot Version Version
-                             Family ID
-cyw20829   A0                0xEB40, 0x11, 1.0.0.7120       1.0.0.2857
-                             0x110
-cyw20829   B0                0xEB43, 0x21, 1.2.0.8334       1.2.0.3073
-                             0x110
-1 Specify `--rev` option for older revision of the silicon (e.g. `$
-cysecuretools -t cyw20829 --rev a0 `). Using the latest revision does not
-require specifying the option. ## CYW89829
-                            Silicon ID,                    RAM Applications
-Target/Kit Silicon Revision Silicon Rev., ROM Boot Version Version
-                            Family ID
-cyw89829   B0               0xEB47, 0x21, 1.2.0.8334       1.2.0.3073
-                            0x110
-# Prerequisites * General * Python 3.6 or later * [Installed Cypress OpenOCD]
-(https://github.com/Infineon/openocd/releases) * For PSoC 64 devices * Ensure
-the KitProg3 programming mode is **CMSIS-DAP Bulk** * Ensure the power
-selection jumper is set to provide 2.5 V to the power supply pin related to
-eFuse power. This voltage level is required to blow eFuses * For CYW20829/
+## CYW20829 / CYW89829
+Target/Kit Silicon ID, Silicon Rev., ROM Boot Version RAM Applications Version
+           Family ID
+cyw20829   0xEB43, 0x21, 0x110       1.2.0.8334       1.2.0.3073
+cyw89829   0xEB47, 0x21, 0x110       1.2.0.8334       1.2.0.3073
+# Prerequisites * General * Python 3.8 - 3.12 * [Installed Infineon OpenOCD]
+(https://github.com/Infineon/openocd/releases) * For PSoC 64 / CYW20829 /
 CYW89829 devices * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk** *
 Ensure the power selection jumper is set to provide 2.5 V to the power supply
 pin related to eFuse power. This voltage level is required to blow eFuses #
 Documentation * [PSoC64 Secure MCU Secure Boot SDK User Guide](https://
 www.cypress.com/documentation/software-and-drivers/psoc-64-secure-mcu-secure-
 boot-sdk-user-guide) * [Changelog](https://github.com/Infineon/cysecuretools/
-blob/master/CHANGELOG.md) # Installing Package Invoke `pip install` from the
-command line: ```bash $ pip install cysecuretools ``` To update the already
-installed package: ```bash $ pip install --upgrade --force-reinstall
-cysecuretools ``` # Supported devices Use `device-list` command for output of
-the supported devices list. ```bash $ cysecuretools device-list ``` # Interface
-and Usage ## PSoC 64 See [README_PSOC64.md](https://github.com/Infineon/
-cysecuretools/blob/master/docs/README_PSOC64.md) ## CYW20829/CYW89829 See
-[README_CYW20829.md](https://github.com/Infineon/cysecuretools/blob/master/
-docs/README_CYW20829.md) ## XMC7100/7200 See [README_XMC7XXX.md](https://
-github.com/Infineon/cysecuretools/blob/master/docs/README_XMC7XXX.md) # Logging
-Every time the tool is invoked, a new log file is created in the _logs_
-directory of the project. By default, the console output has INFO logging
-severity. The log file contains the DEBUG logging severity. # Known issues -
-Using the policy from version 4.0.0 in projects created by version 4.1.0 causes
-the CY_FB_INVALID_IMG_JWT_SIGNATURE error during re-provisioning on PSoC64-2M
-devices: ``` ... ERROR : SFB status: CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid
-image certificate signature. Check the log for details ``` _Workaround_: 1.
-Open the policy file. 2. Navigate to section 1 of the `boot_upgrade/firmware`.
-3. Set `boot_auth` and `bootloader_keys` as follows: ``` "boot_auth": [ 3 ],
-"bootloader_keys": [ { "kid": 3, "key": "../keys/cy_pub_key.json" } ] ``` -
-During the installation of the package via _pip_ on Mac OS Big Sur, the
-following exception is raised: ``` ... distutils.errors.DistutilsError: Setup
-script exited with error: SandboxViolation: mkdir('/private/var/root/Library/
-Caches/com.apple.python/private/tmp/easy_install-y8c1npmz', 511) {} The package
-setup script has attempted to modify files on your system that are not within
-the EasyInstall build area, and has been aborted. This package cannot be safely
-installed by EasyInstall, and may not support alternate installation locations
-even if you run its setup script by hand. Please inform the package's author
-and the EasyInstall maintainers to find out if a fix or workaround is
-available. ``` _Solution:_ Upgrade the `pip` package running the following
-command from the terminal: `python3 -m pip install --upgrade pip`. # License
-and Contributions The software is provided under the Apache-2.0 license.
-Contributions to this project are accepted under the same license. This project
-contains code from other projects. The original license text is included in
-those source files. # Changelog All notable changes to this project will be
-documented in this file. ## 5.1.0 ### Added - Support for CYW89829 devices ##
-5.0.0 ### Changed - Removed pyOCD support. OpenOCD is used as a default On-Chip
-debugger for all platforms - High-level API module refactoring ### Added -
-Support for XMC7100, XMC7200 devices ## 4.2.0 ### Added - Support for CYW20829
-B0 silicon revision - Multi-image NV counter for CYW20829 - Transition PSoC 64
-devices to RMA LCS - Open PSoC 64 devices in RMA LCS for debugging - OpenOCD
-autodiscovery in ModusToolbox directory - Add SW/HW compatibility table to the
-readme ### Changed - Target `cyw20829` is used for the latest silicon revision.
-For the previous silicon revision (A0) add _--rev_ option in the command line
-(`-t cyw20829 --rev a0`) ## 4.1.0 ### Added - OpenOCD support for PSoC 64
-devices - Creating update package in the unsigned image (_extend-image_
-command) ### Changed - Fixed installation failure using pip 22.1 - CyBootloader
-2.0.2.8102 for PSoC 64 2M: - Improved performance of SWAP algorithm - Image
-certificate signed with the Infineon key (id=3) - Use Infineon key (id=3) for
-bootloader in the policy files ## 4.0.0 ### Added - Support of CYW20829 devices
-- Support Python 3.10 - Signing images with HSM ### Changed - Separated PSoC 64
-and CYW20829 devices CLI - Updated PSoC 64 CyBootloader for 512k and 2M: -
-added "reset_after_failure" feature - decreased boot time - Protect PSA API
-from NSPE in PSoC 64 2M-S0 policy - Prevent signing of already signed images -
-Change MCUboot image header padding to erase value - Use CyBootloader from the
-project directory if the project exists - Updated dependencies packages to the
-latest versions - Use pyocd 0.32.3 ## 3.1.1 ### Changed - Fixed installation
-failure on macOS Big Sur and Apple M1 chip - Fixed installation failure in
-Python 3.9 ## 3.1.0 ### Added - SCRATCH with Status Partition swap mode - Small
-image slots support in the external memory ## 3.0.0 ### Added - Image SWAP
-using Status Partition ### Changed - CyBootloader 2.0 - Secure Flash Boot 4.0.2
-support ## 2.1.0 ### Added - Support PSoC64 1M - New command to read device die
-ID - Optionally add boot record to the signed image - New policy validators
-(address overlaps between images and bootloader, slots address alignment with
-the SMPU address limits, DAP closure, monotonic counter) - Log the device
-response JWT during the provisioning process ### Changed - Fixed issue with
-using group private key - Use pyocd 0.27.3 ## 2.0.0 ### Added - Support PSoC64
-2M, PSoC64 512K - Command line interface - Encrypted programming - Single-image
-and multi-image policy ### Changed - Update provisioning according to new
-Secure Flash Boot functionality (update system calls, reprovisioning, encrypted
-image support) - New CyBootloaders (CY8CKIT-064B0S2-4343W, CY8CKIT-064S0S2-
-4343W, CY8CPROTO-064B0S3) - Use pyocd 0.27.0
+blob/master/CHANGELOG.md) # Installing Package ## Windows The installation of
+ModusToolboxâ¢ Software 3.1 includes the correct version of Python and
+CySecureTools 5.0.0. The latest version of CySecureTools is 6.0.0. To update
+the package from the ModusToolboxâ¢ shell (for Windows users): * In the
+ModusToolboxâ¢ GUI open the terminal by clicking the **Terminal** tab in the
+bottom pane. * Then, select a project in the **Project Explorer** to open a
+shell in the project directory. * Enter the following command: `$ pip install -
+-upgrade --force-reinstall edgeprotecttools` ## Linux / macOS Install Python
+3.12 on your computer. You can download it from https://www.python.org/
+downloads/. Set up the appropriate environment variable(s) for your operating
+system. If Python 2.7 is also installed, make sure that Python312 and
+Python312\Scripts have higher priority in the PATH than CPython27. ### Linux
+Configuration Most distributions of Linux should already have python2 and
+python3 installed. To verify that python by default points to python3 run:
+```bash $ python --version ``` If python3 is not set as default, run the
+following commands. The number at the end of each command denotes a priority:
+```bash $ update-alternatives --install /usr/bin/python python /usr/bin/
+python2.7 1 $ update-alternatives --install /usr/bin/python python /usr/bin/
+python3.12 2 ``` ### macOS Configuration By default, `python` points to `/usr/
+bin/python`, which is python2. To make `python` and `pip` resolve to python3
+versions, execute the following from command line: ```bash $ echo 'alias
+python=python3' >> ~/.bash_profile $ echo 'alias pip=pip3' >> ~/.bash_profile $
+source ~/.bash_profile $ python --version Python 3.12.3 $ pip --version pip
+24.0 from /Library/Frameworks/Python.framework/Versions/3.12/lib/python3.12/
+site-packages/pip (python 3.12) ``` Note: If you use a shell other than bash,
+update its profile file accordingly. For example `~/.zshrc` if you use zsh
+instead of `~/.bash_profile`. ### Installing CySecureTools Package Make sure
+that you have the latest version of pip installed, use the following command.
+```bash $ python -m pip install --upgrade pip ``` Run the following command in
+your terminal window. ```bash $ python -m pip install cysecuretools ``` ###
+Updating CySecureTools Package To update the already installed package: ```bash
+$ pip install --upgrade --force-reinstall cysecuretools ``` Note 1: During
+installation, you may see errors saying that cysecuretools requires package
+version X, but you have package version Y which is incompatible. In most cases,
+these can be safely ignored. Note 2: You can use the following command to show
+the path to the installed package `python -m pip show cysecuretools`. #
+Supported devices Use `device-list` command for output of the supported devices
+list. ```bash $ cysecuretools device-list ``` # Interface and Usage ## PSoC 64
+CLI See [README_PSOC64.md](https://github.com/Infineon/cysecuretools/blob/
+master/docs/README_PSOC64.md) ## CYW20829/CYW89829 CLI See [README_CYW20829.md]
+(https://github.com/Infineon/cysecuretools/blob/master/docs/README_CYW20829.md)
+## XMC7100/7200 CLI See [README_XMC7XXX.md](https://github.com/Infineon/
+cysecuretools/blob/master/docs/README_XMC7XXX.md) # Logging Every time the tool
+is invoked, a new log file is created in the _logs_ directory of the project.
+By default, the console output has INFO logging severity. The log file has the
+DEBUG logging severity. # Known issues - Using the policy from version 4.0.0 in
+projects created by version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE
+error during re-provisioning on PSoC64-2M devices: ``` ... ERROR : SFB status:
+CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid image certificate signature. Check the
+log for details ``` _Workaround_: 1. Open the policy file. 2. Navigate to
+section 1 of the `boot_upgrade/firmware`. 3. Set `boot_auth` and
+`bootloader_keys` as follows: ``` "boot_auth": [ 3 ], "bootloader_keys": [
+{ "kid": 3, "key": "../keys/cy_pub_key.json" } ] ``` - During the installation
+of the package via _pip_ on Mac OS Big Sur, the following exception is raised:
+``` ... distutils.errors.DistutilsError: Setup script exited with error:
+SandboxViolation: mkdir('/private/var/root/Library/Caches/com.apple.python/
+private/tmp/easy_install-y8c1npmz', 511) {} The package setup script has
+attempted to modify files on your system that are not within the EasyInstall
+build area, and has been aborted. This package cannot be safely installed by
+EasyInstall, and may not support alternate installation locations even if you
+run its setup script by hand. Please inform the package's author and the
+EasyInstall maintainers to find out if a fix or workaround is available. ```
+_Solution:_ Upgrade the `pip` package running the following command from the
+terminal: `python3 -m pip install --upgrade pip`. # License and Contributions
+The software is provided under the Apache-2.0 license. Contributions to this
+project are accepted under the same license. This project contains code from
+other projects. The original license text is included in those source files. #
+Changelog All notable changes to this project will be documented in this file.
+## 6.0.0 ### Added - Support for Python 3.12 ### Changed - Extended package
+installation instructions - Extended CYW20829/CYW89829 readme with usage
+examples - Drop support for Python versions 3.6 and 3.7 ## 5.1.0 ### Added -
+Support for CYW89829 devices ## 5.0.0 ### Added - Support for XMC7100, XMC7200
+devices ### Changed - Removed pyOCD support. OpenOCD is used as a default On-
+Chip debugger for all platforms - High-level API module refactoring ## 4.2.0
+### Added - Support for CYW20829 B0 silicon revision - Multi-image NV counter
+for CYW20829 - Transition PSoC 64 devices to RMA LCS - Open PSoC 64 devices in
+RMA LCS for debugging - OpenOCD autodiscovery in ModusToolbox directory - Add
+SW/HW compatibility table to the readme ### Changed - Target `cyw20829` is used
+for the latest silicon revision. For the previous silicon revision (A0) add _--
+rev_ option in the command line (`-t cyw20829 --rev a0`) ## 4.1.0 ### Added -
+OpenOCD support for PSoC 64 devices - Creating update package in the unsigned
+image (_extend-image_ command) ### Changed - Fixed installation failure using
+pip 22.1 - CyBootloader 2.0.2.8102 for PSoC 64 2M: - Improved performance of
+SWAP algorithm - Image certificate signed with the Infineon key (id=3) - Use
+Infineon key (id=3) for bootloader in the policy files ## 4.0.0 ### Added -
+Support of CYW20829 devices - Support Python 3.10 - Signing images with HSM ###
+Changed - Separated PSoC 64 and CYW20829 devices CLI - Updated PSoC 64
+CyBootloader for 512k and 2M: - added "reset_after_failure" feature - decreased
+boot time - Protect PSA API from NSPE in PSoC 64 2M-S0 policy - Prevent signing
+of already signed images - Change MCUboot image header padding to erase value -
+Use CyBootloader from the project directory if the project exists - Updated
+dependencies packages to the latest versions - Use pyocd 0.32.3 ## 3.1.1 ###
+Changed - Fixed installation failure on macOS Big Sur and Apple M1 chip - Fixed
+installation failure in Python 3.9 ## 3.1.0 ### Added - SCRATCH with Status
+Partition swap mode - Small image slots support in the external memory ## 3.0.0
+### Added - Image SWAP using Status Partition ### Changed - CyBootloader 2.0 -
+Secure Flash Boot 4.0.2 support ## 2.1.0 ### Added - Support PSoC64 1M - New
+command to read device die ID - Optionally add boot record to the signed image
+- New policy validators (address overlaps between images and bootloader, slots
+address alignment with the SMPU address limits, DAP closure, monotonic counter)
+- Log the device response JWT during the provisioning process ### Changed -
+Fixed issue with using group private key - Use pyocd 0.27.3 ## 2.0.0 ### Added
+- Support PSoC64 2M, PSoC64 512K - Command line interface - Encrypted
+programming - Single-image and multi-image policy ### Changed - Update
+provisioning according to new Secure Flash Boot functionality (update system
+calls, reprovisioning, encrypted image support) - New CyBootloaders (CY8CKIT-
+064B0S2-4343W, CY8CKIT-064S0S2-4343W, CY8CPROTO-064B0S3) - Use pyocd 0.27.0
```

### Comparing `cysecuretools-5.1.0/cysecuretools.egg-info/SOURCES.txt` & `cysecuretools-6.0.0/cysecuretools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.md
+EULA
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 cysecuretools.egg-info/PKG-INFO
 cysecuretools.egg-info/SOURCES.txt
@@ -235,20 +236,16 @@
 src/targets/cyb06xx7/maps/register_map.py
 src/targets/cyb06xx7/packets/control_dap_cert.json
 src/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt
 src/targets/cyb06xx7/packets/ec_key_tmpl.json
 src/targets/cyb06xx7/packets/entrance_exam.jwt
 src/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json
 src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json
-src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json
-src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json
 src/targets/cyb06xx7/policy/policy_single_CM0_CM4.json
 src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json
-src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json
-src/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json
 src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
 src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
 src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
 src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
 src/targets/cyb06xxa/__init__.py
 src/targets/cyb06xxa/target_builder.py
 src/targets/cyb06xxa/keys/cy_pub_key.json
```

### Comparing `cysecuretools-5.1.0/docs/README_CYW20829.md` & `cysecuretools-6.0.0/docs/README_CYW20829.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Table of Contents
 - [Main features](#main-features)
 - [Quick start](#quick-start)
 - [Usage example](#usage-example)
 - [Policy](#policy)
 - [Keys](#keys)
+- [Probe ID](#probe-id)
 - [Command-line interface](#command-line-interface)
     - [Tool help](#tool-help)
     - [Common options](#common-options)
     - [Create key](#create-key)
     - [Provision device](#provision-device)
     - [Reprovision device](#reprovision-device)
     - [Create provisioning data packet](#create-provisioning-data-packet)
@@ -32,15 +33,15 @@
 
 
 # Main features
 * [Create a key](#create-a-key) - Creates an RSA private/public key pair or AES key for image encryption.
 * [Provisioning a device](#provision-a-device) - Provisioning is the act of configuring a device with an authorized set of keys, policies, and optionally certificates.
 * [Sign a user application](#sign-an-image) - Signs a user application with a private key locally or with a Hardware Security Module.
 * [Encrypt a user application](#encrypt-the-user-application) - Signs and encrypts a user application.
-* [Create a debug certificate](#create-debug-certificate) - The debug certificate is used by BootROM to enable CM33-AP and/or Sys-AP when it is temporarily disabled.
+* [Create a debug certificate](#create-debug-certificate) - The debug certificate is used by ROM boot code to enable CM33-AP and/or Sys-AP when it is temporarily disabled.
 
 
 # Quick start
 ## 1. Set a path to the On-Chip debugger
 ```bash
 $ cysecuretools set-ocd --name openocd --path <PATH_TO_OPENOCD_ROOT_DIRECTORY>
 ```
@@ -49,15 +50,15 @@
 
 _Example:_
 ```bash
 $ cysecuretools set-ocd --name openocd --path /Users/username/tools/openocd
 ```
 
 ## 2. Define a target
-Run the following command and find the name of your target in the list of supported targets.
+Run the following command and find the name of your target in the list of supported targets (**cyw20829** or **cyw89829**).
 ```bash
 $ cysecuretools device-list
 ```
 This target name will be used as a `-t` option value with each command.
 
 _Example_:
 ```bash
@@ -85,44 +86,62 @@
 ```bash
 $ cysecuretools -t <TARGET> -p policy/policy_no_secure.json <COMMAND> [OPTIONS]
 ```
 
 ## 5. Create keys (for secure devices only)
 Create a private/public key pair. The public key is used for the provisioning, the private key is used to sign the image with the user application.
 ```bash
-$ cysecuretools -t <TARGET> -p <POLICY> create-key -k 0
+$ cysecuretools -t <TARGET> -p <POLICY> create-key --key-id 0
 ```
 
 ## 6. Provision the device
 ```bash
 $ cysecuretools -t <TARGET> -p <POLICY> provision-device
 ```
 
 ## 7. Sign the image
 ```bash
-$ cysecuretools -t <TARGET> -p <POLICY> sign-image -i image.bin -o image_signed.bin -k 0
+$ cysecuretools -t <TARGET> -p <POLICY> sign-image --image image.bin --output image_signed.bin --key-id 0
 ```
 
 
 # Usage example
 ## Non-secure device
 ```bash
+# Set OpenOCD location
 $ cysecuretools set-ocd --name openocd --path /Users/username/tools/openocd
+
+# Create a project
 $ cysecuretools -t cyw20829 init
+
+# Initiate device provisioning
 $ cysecuretools -t cyw20829 -p policy/policy_no_secure.json provision-device
+
+# Initiate device reprovisioning
 $ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_no_secure.json reprovision-device
 ```
 ## Secure device
 ```bash
+# Set OpenOCD location
 $ cysecuretools set-ocd --name openocd --path /Users/username/tools/openocd
+
+# Create a project
 $ cysecuretools -t cyw20829 init
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json create-key -k 0
+
+# Create an RSA-2048 key pair and save it to the path specified in the policy "oem_priv_key_0" property
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json create-key --key-id 0
+
+# Initiate device provisioning
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json provision-device
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image -i image.bin -o image_signed.bin -k 0
-$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json reprovision-device -k 0
+
+# Sign the user application with the key specified in the policy "oem_priv_key_0" property
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed.bin --key-id 0
+
+# Initiate device reprovisioning with the data previously signed with the key specified in the policy "oem_priv_key_0" property
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json reprovision-device --key-id 0
 ```
 
 
 # Policy
 Policy - is a text file in the JSON format, which contains a set of properties for the device configuration (e.g. enabling/disabling debug access ports, Serial Memory Interface configuration, keys information, etc.)
 
 Policy files are located in the _policy_ directory of the user project and the path to a file is specified when almost any command is run. The user selects a policy file based on their needs.
@@ -145,14 +164,32 @@
 ### OEM key
 During provisioning, the OEM keys are not transferred to a device in their original view. Only a key hash (16 bytes) is provisioned. For the image verification, the image must contain an OEM public key (added automatically by the _sign-image_ command). This public key hash will be compared to the provisioned key hash.
 ### Encryption key
 A 128-bit encryption key is provisioned as is. There is an option to have two OEM keys (_oem_pub_key_0_ and _oem_pub_key_1_). However, if the encryption is used, then only _oem_pub_key_0_ can be used. The encryption key will be placed instead of the second OEM key hash.
 
  _NOTE_: An encryption key can be transferred to a device during provisioning only (NOT reprovisioning). Also, if encryption is used, oem_key_0 cannot be revoked during reprovisioning.
 
+# Probe ID
+If there is more than one device connected it is necessary to provide the probe ID. Otherwise OpenOCD will use the first found. Use `fw-loader` which is one of the ModusToolbox™ tools.
+```bash
+$ ~/ModusToolbox/tools_3.1/fw-loader/bin/fw-loader.exe --device-list
+Infineon Firmware Updater, Version: 3.5.0.2114
+(C) Copyright 2018-2023 by Cypress Semiconductor Corporation (an Infineon company)
+All Rights Reserved
+
+Info: Start the API initialization
+Info: Connected - MiniProg4 CMSIS-DAP BULK-1A1A055A02010400
+Info: Connected - MiniProg4 CMSIS-DAP BULK-151B17B202200400
+Info: The hardware initialization has completed in 428 ms
+The connected supported devices:
+        1: MiniProg4 CMSIS-DAP BULK-1A1A055A02010400    FW Version 2.50.1383
+        2: MiniProg4 CMSIS-DAP BULK-151B17B202200400    FW Version 2.60.1412
+```
+The probe ID is the numeric part of the device name (e.g. 1A1A055A02010400). Specify the option as `--probe-id 1A1A055A02010400`.
+
 
 # Command-line interface
 This section contains the main CLI commands. More commands can be found in the tool help.
 
 ## Tool help
 To see the list of commands supported for a specific target:
 ```bash
@@ -179,52 +216,77 @@
 ### Command: `create-key`
 ### Parameters
 | Name &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Optional/Required  | Description  |
 | --------------------------------|:------------------:| -------------|
 | -k, --key-id [0\|1]             | optional (mutually exclusive with the _--output_ option) | The OEM key ID. This ID defines the paths where the public and private keys will be saved based on the selected policy _pre_build_ and _post_build_ sections. Depending on the selected value 0 or 1, _oem_key_0_ or _oem_key_1_ will be used. |
 | -o, --output [private] [public] | optional (mutually exclusive with the _--key-id_ option) | Key pair output files. This is an alternative option and can be used to create a key in the different from the policy location. If it is specified, the _--key-id_ option will be ignored. However, using _--key-id_ is preferable. It allows avoiding accidental provisioning and signing with a key from the different pairs. As the option value, provide private and public key paths. Specify the option multiple times to create multiple key pairs. |
 | --aes                           | optional (mutually exclusive with the _--key-id_ and _--output_ options)          | Indicates whether to generate an AES key for image encryption. The key will be saved by the path specified in the policy _smif_aes_key_ field.
-| --key-path    | optional        | Used to generate a key into a specific path. Applicable with _--aes_ or _--template_ option. |
-| --overwrite / --no-overwrite    | optional           | Indicates whether overwrite a key if it already exists. |
-| --template    | optional        | A JSON file containing public key modulus and exponent. The option is used for creating a PEM file based on public key modulus and exponent. |
-| --hash-path   | optional        | A path where to save the public key hash.|
+| --key-path    | optional        | Used to generate a key into a specific path. This option should only be used with _--aes_ or _--template_ option to specify location for these type of keys. The option is not applicable to OEM keys. For OEM keys there is the _--key-id_ option. |
+| --overwrite / --no-overwrite    | optional           | Indicates whether overwrite a key if it already exists. If not specified the command prompt would ask for a decision.|
+| --template    | optional        | A JSON file containing public key modulus and exponent. The option is used for creating a PEM file based on public key modulus and exponent. Usually used to convert key public numbers returned by HSM to a standard format key. |
+| --hash-path   | optional        | A path where to save the public key hash if needed.|
 ### Usage example
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json create-key -k 0
+# Generate a new RSA-2048 key pair and save it to the path specified in the "oem_priv_key_0" property in the policy file.
+# Alternatively to the "--key-id" option the "--key-path" option can be used to specify the key path
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json create-key --key-id 0
+
+# Generate a new RSA-2048 key pair and save it to the path specified in the "oem_priv_key_1" property in the policy file
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json create-key --key-id 1
+
+# Generate a 128-bit encryption key and save it to the path specified in the "encrypt_key" property in the policy file
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json create-key --aes
 ```
 
 
 ## Provision device
 Configuring a device with a set of keys and policies.
 ### Command: `provision-device`
 ### Parameters
 | Name &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Optional/Required  | Description  |
 | -------------------|:-----------------:| -------------|
-| --probe-id         | optional          | Probe serial number. |
-| --existing-packet  | optional          | Skip provisioning packet creation and use the existing packet. This may be useful when a packet with RAM application input parameters already exists and the tool does not have to generate it again. |
+| --probe-id         | optional          | Probe serial number. Make sure to specify the probe ID if there is more than one device connected to avoid accidental programming of the wrong device.|
+| --existing-packet  | optional          | Skip provisioning packet creation and use the existing packet. This may be useful when a packet with RAM application input parameters already exists and the tool does not have to generate it again. If not specified, the packet will be generated based on the specified policy.|
 ### Usage example
 ```bash
+# From the specified policy file generate provisioning packet and initiate device provisioning
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json provision-device
+
+# Use the "--probe-id" option if there is more than one device connected
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json provision-device --probe-id 1A1A055A02010400
+
+# Initiate device provisioning, but do not generate/overwrite the existing provisioning packet (packets/apps/prov_oem/in_params.bin)
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json provision-device --existing-packet
 ```
 
 
 ## Reprovision device
 Once a device has been provisioned it can only be reprovisioned. Reprovisioning allows configuring a limited set of settings (e.g. provisioning an additional OEM key, revoking _icv_pubkey_0_ and oem_pubkey_0 keys, changing anti-rollback counter, etc). The _policy_reprovisioning_secure.json_ file contains only those settings that can be changed.
 ### Command: `reprovision-device`
 ### Parameters
 | Name &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Optional/Required  | Description  |
 | --------------------|:------------------:| -------------|
-| -k, --key-id [0\|1] | optional           | The OEM private key ID used to sign the reprovisioning packet. This ID informs the tool about the key location. The tool will use the path specified in the selected policy _post_build_ section. |
+| -k, --key-id [0\|1] | optional           | The OEM private key ID used to sign the reprovisioning packet. This ID informs the tool about the key location. The tool will use the path specified in the selected policy _post_build_ section.|
 | --key-path          | optional           | Sets OEM private key that is used to sign the reprovisioning packet. Overrides --key-id option.|
-| --probe-id          | optional           | Probe serial number. |
-| --existing-packet   | optional           | Skip reprovisioning packet creation and use the existing packet. This may be useful when a packet with RAM application input parameters already exists and the tool does not have to generate it again. |
-| --signature         | optional           | The name of the file containing the signature.|
+| --probe-id          | optional           | Probe serial number. Make sure to specify the probe ID if there is more than one device connected to avoid accidental programming of the wrong device.|
+| --existing-packet   | optional           | Skip reprovisioning packet creation and use the existing packet. This may be useful when a packet with RAM application input parameters already exists and the tool does not have to generate it again. If not specified, the packet will be generated based on the specified policy.|
+| --signature         | optional           | The name of the file containing the signature. Use this option to attach a signature returned by HSM to the unsigned packet. More details in [Signing reprovisioning data packet with HSM](#signing-reprovisioning-data-packet-with-HSM).|
 ### Usage example
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json reprovision-device -k 0
+# From the specified policy file generate a reprovisioning packet and initiate device reprovisioning. The packet is signed with the key specified in the policy "oem_priv_key_0" property. Alternatively to the "--key-id" option the "--key-path" option can be used to specify the key path
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json reprovision-device --key-id 0
+
+# Use the "--probe-id" option if there is more than one device connected
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json reprovision-device --key-id 0 --probe-id 1A1A055A02010400
+
+# Initiate device reprovisioning, but do not generate/overwrite the existing reprovisioning packet. The reprovisioning packet is located in the project directory in packets/apps/reprovisioning/in_params.bin
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json reprovision-device --existing-packet
+
+# Attach a signature to the unsigned reprovisioning packet and initiate device reprovisioning. The unsigned reprovisioning packet must be previously created by the "create-provisioning-packet" command
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json reprovision-device --signature signature.bin
 ```
 
 
 ## Create provisioning data packet
 Creates provisioning/reprovisioning data packet without starting the device provisioning process.
 ### Command: `create-provisioning-packet`
 ### Parameters
@@ -233,166 +295,203 @@
 | -k, --key-id [0\|1] | optional           | The OEM private key ID used to sign the reprovisioning packet. Applicable with reprovisioning policy type only. The ID informs the tool about the key location. The tool will use the path specified in the selected policy _post_build_ section. |
 | --key-path          | optional           | Key file path to sign the reprovisioning packet. Applicable with reprovisioning policy type only. This is an alternative option and can be used to specify different from the policy key file location. If it is specified, the _--key-id_ option will be ignored. However, using _--key-id_ is preferable. It allows avoiding accidental provisioning and signing with keys from the different pairs. |
 | --signature         | optional           | The file path containing the signature. Used to sign the reprovisioning packet by HSM ([Signing reprovisioning data packet with HSM](#signing-reprovisioning-data-packet-with-HSM)). |
 | --pubkey            | optional           | The public key to be added to the reprovisioning packet. Used to sign the reprovisioning packet by HSM ([Signing reprovisioning data packet with HSM](#signing-reprovisioning-data-packet-with-HSM)). |
 | --non-signed        | optional           | The flag indicating that reprovisioning packet will not be signed. Used to create the reprovisioning packet for signing by HSM ([Signing reprovisioning data packet with HSM](#signing-reprovisioning-data-packet-with-HSM)). |
 ### Usage example
 ```bash
+# Create provisioning packet using secure policy
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json create-provisioning-packet
-```
-```bash
-$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json create-provisioning-packet -k 0
+
+# Create reprovisioning packet using secure policy. The packet is signed with the key specified in the policy "oem_priv_key_0" property. Alternatively to the "--key-id" option the "--key-path" option can be used to specify the key path
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json create-provisioning-packet --key-id 0
+
+# Create unsigned reprovisioning packet using secure policy. Used for signing a packet with HSM
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json create-provisioning-packet --non-signed --pubkey keys/pub_oem_0.pem
+
+# Create reprovisioning packet using secure policy and attach the signature. Used for signing a packet with HSM
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json create-provisioning-packet --signature signature.bin
 ```
 
 
 ## Sign image
 Signs a user application with a key. Optionally encrypts the signed application.
 ### Command: `sign-image`
 ### Parameters
 | Name &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Optional/Required  | Description   |
 | ------------------------- |:------------------:| ------------- |
 | -i, --image               | required           | User application file. The output file format is based on the input file extension (bin or hex) |
 | -k, --key-id [0\|1]       | optional (mutually exclusive with the _--key-path_ option) | The OEM key ID. This ID defines the key location based on the selected policy _post_build_ section. Depending on the selected value 0 or 1, _oem_priv_key_0_ or _oem_priv_key_1_ will be used. |
 | --key-path                | optional (mutually exclusive with the _--key-id_ option) | Key file path to sign the image. This is an alternative option and can be used to specify different from the policy key file location. If it is specified, the _--key-id_ option will be ignored. However, using _--key-id_ is preferable. It allows avoiding accidental provisioning and signing with keys from the different pairs. |
-| --signature                | optional           | The name of the file containing the signature. Used to add an existing signature to the image. |
-| -R, --erased-val [0\|0xff] | optional           | The value that is read back from erased flash. |
+| --signature                | optional           | The name of the file containing the signature. Used to add an existing signature generated by HSM to the image. More details in [Signing application with HSM](#signing-application-with-hsm).|
+| -R, --erased-val [0\|0xff] | optional           | The value that is read back from erased flash. The default value is 0.|
 | -o, --output              | optional           | Signed image output file. If not specified, a copy of the input file will be created with the _unsigned_ prefix, then the input file will be signed. |
 | --encrypt                 | optional           | Enable the encryption feature. If present, the image will be encrypted after signing. |
 | --enckey                  | optional           | Path to the AES key. If absent, the key path is taken from the policy _smif_aes_key_ field. |
-| --hex-addr                | optional           | Adjusts address in .hex output file. The default value is 0. Ignored for output images in .bin format|
+| --hex-addr                | optional           | Adjusts start address in .hex output file. The default value is 0. Ignored for output images in .bin format.|
 | --app-addr                | optional           | The address of the application to encrypt. Accepts values as hexadecimal or decimal numbers. The default value is 0. |
-| -f, --image-format        | optional           | The image format defines the image header size, signing and encryption algorithms. Values: _bootrom_ram_app_ - RAM application started by BootROM; _bootrom_next_app_ - external memory application started by BootROM (e.g. MCUBoot); _mcuboot_user_app_ - application started by MCUBoot. The default value is _mcuboot_user_app_. |
+| -f, --image-format        | optional           | The image format defines the image header size, signing and encryption algorithms. Values: _bootrom_ram_app_ - RAM application started by ROM boot code; _bootrom_next_app_ - external memory application started by ROM boot code (e.g. [MCUBoot](#https://docs.mcuboot.com/)); _mcuboot_user_app_ - application started by MCUBoot. The default value is _mcuboot_user_app_. |
 | -H, --header-size         | optional           | Sets image header size. Overrides header size defined by the --image-format option. |
 | -S, --slot-size           | optional           | Sets maximum slot size. The default value is 0x20000.
-| --pad                     | optional           | Adds padding to the image trailer up to maximum slot size. Adds padding to 32-byte Boot Magic to the end of the trailer. Needed for MCUBoot image upgrade.|
-| --confirm                 | optional           | Adds Image OK byte to image trailer. Needed for MCUBoot image upgrade.|
-| --overwrite-only          | optional           | Sets Overwrite mode in MCUBoot image header instead of Swap.|
-| --update-key-id [0\|1]    | optional           | Sets OEM private key ID used to sign the update data packet.|
-| --update-key-path         | optional           | The key used to sign the update data packet. Overrides the --update-key-id option.|
-| --min-erase-size          | optional           | Sets minimum erase size.|
+| --pad                     | optional           | Adds padding to the image trailer. Pads the image from the end of the TLV area up to the slot size. _boot_magic_ is always at the very end after the padding. Needed for [MCUBoot](#https://docs.mcuboot.com/) image upgrade.|
+| --confirm                 | optional           | Adds image OK status to the trailer. Pads the image from the end of the TLV area up to the slot size and sets the image OK byte to 0x01 (the eighth byte from the end). The padding is required for this feature and is always applied. _boot_magic_ is always at the very end after the padding. Needed for [MCUBoot](#https://docs.mcuboot.com/) image upgrade.|
+| --overwrite-only          | optional           | Sets Overwrite mode in [MCUBoot](#https://docs.mcuboot.com/) image header instead of Swap.|
+| --update-key-id [0\|1]    | optional           | Sets OEM private key ID used to sign the update data packet. Used to add the update packet with the NV counter to the protected TLV.|
+| --update-key-path         | optional           | The alternative option to _--update-key-id_ used to sign the update data packet. Overrides the --update-key-id option.|
+| --min-erase-size          | optional           | Sets minimum erase size. The default value is 0x1000.|
 | --align [1\|2\|4\|8]      | optional           | Sets flash alignment. The default value is 8.|
-| -v, --version             | optional           | Sets image version in the image header.|
+| -v, --version             | optional           | Sets image version in the image header. The default value is 0.1.|
 | -d, --dependencies        | optional           | Add dependency on another image, format: "(<image_ID>,<image_version>), ... ".|
 | --image-id                | optional           | Image ID. The value is used to update NV counter. The default value is 0.|
 ### Usage example
-#### Sign without encryption:
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed.bin --key-id 0 --image-type APP_PC0
-```
-#### Sign and encrypt:
-```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed.bin --key-id 0 --image-type APP_PC0--encrypt --app-addr 0x08000200
+# Sign the image with the "oem_priv_key_0" specified in the policy
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed.bin --key-id 0
+
+# Sign the image with the "oem_priv_key_0" specified in the policy. Save the output file in the Intel hex format and set the final hex address to 0x60020000
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed.hex --key-id 0 --hex-addr 0x60020000
+
+# Sign the image with the "oem_priv_key_0" specified in the policy. Pad the image with 0xFF value up to the slot size.
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed.bin --key-id 0 --pad --overwrite-only --slot-size 0x10000 --header-size 0x400 --erased-val 0xFF
+
+# Sign the image with the "oem_priv_key_0" specified in the policy. Encrypt the image with a new random encryption key and use device public key ("--enckey" option) for the ECIES schema (https://docs.mcuboot.com/encrypted_images.html). The "--app-addr" option specifies the start address of the application to be encrypted
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed_encrypted.bin --key-id 0 --encrypt --enckey keys/ec256_pub_key.pem --header-size 1024 --app-addr 0x08000200 --hex-addr 0x60020000
 ```
 Refer to [Encrypt the user application](#encrypt-the-user-application) for more details about image encryption.
 
 
 ## Extend image
-Extends a firmware image with the protected TLV area and [mcuboot header](https://github.com/mcu-tools/mcuboot/blob/master/docs/design.md#image-format), but does not sign the image. Usually, this command is useful for [signing and image with a Hardware Security Module](#signing-application-with-hsm).
+Extends a firmware image with the [protected TLV](https://docs.mcuboot.com/design.html#protected-tlvs) area and [mcuboot header](https://github.com/mcu-tools/mcuboot/blob/master/docs/design.md#image-format), but does not sign the image. Usually, this command is useful for [signing and image with a Hardware Security Module](#signing-application-with-hsm).
 ### Command: `extend-image`
 ### Parameters
 | Name &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Optional/Required | Description |
 | ----------------------------- |:------------------:| ------------- |
 | -i, --image                   | required           | User application file. The output file format is based on the input file extension (bin or hex). |
 | --pubkey                      | optional           | The public key to be added to the image. Necessary for the image further verification. |
-| -R, --erased-val [0\|0xff]    | optional           | The value that is read back from erased flash.    |
+| -R, --erased-val [0\|0xff]    | optional           | The value that is read back from erased flash. The default value is 0.|
 | -o, --output                  | optional           | Extended image output file. If not specified, a copy of the input file will be created with the _orig_ prefix, then the input file will be processed.|
 | --protected-tlv [tag] [value] | optional           | Custom TLV that will be placed into a protected area. Basically, this is the user's custom data. Add the "0x" prefix if the value should be interpreted as an integer, otherwise, it will be interpreted as a string. Specify the option multiple times to add multiple TLVs. |
-| -f, --image-format        | optional           | The image format defines the image header size, signing and encryption algorithms. Values: _bootrom_ram_app_ - RAM application started by BootROM; _bootrom_next_app_ - external memory application started by BootROM (e.g. MCUBoot); _mcuboot_user_app_ - application started by MCUBoot. The default value is _mcuboot_user_app_. |
+| -f, --image-format        | optional           | The image format defines the image header size, signing and encryption algorithms. Values: _bootrom_ram_app_ - RAM application started by ROM boot code; _bootrom_next_app_ - external memory application started by ROM boot code (e.g. [MCUBoot](#https://docs.mcuboot.com/)); _mcuboot_user_app_ - application started by MCUBoot. The default value is _mcuboot_user_app_. |
 | -H, --header-size         | optional           | Sets image header size. Overrides header size defined by the --image-format option. |
 | -S, --slot-size           | optional           | Sets maximum slot size. The default value is 0x20000.|
-| --pad                     | optional           | Adds padding to the image trailer up to maximum slot size. Adds padding to 32-byte Boot Magic to the end of the trailer. Needed for MCUBoot image upgrade.|
-| --confirm                 | optional           | Adds Image OK byte to image trailer. Needed for MCUBoot image upgrade.|
-| --overwrite-only          | optional           | Sets Overwrite mode in MCUBoot image header instead of Swap.|
+| --pad                     | optional           | Adds padding to the image trailer. Pads the image from the end of the TLV area up to the slot size. _boot_magic_ is always at the very end after the padding. Needed for [MCUBoot](#https://docs.mcuboot.com/) image upgrade.|
+| --confirm                 | optional           | Adds image OK status to the trailer. Pads the image from the end of the TLV area up to the slot size and sets the image OK byte to 0x01 (the eighth byte from the end). The padding is required for this feature and is always applied. _boot_magic_ is always at the very end after the padding. Needed for [MCUBoot](#https://docs.mcuboot.com/) image upgrade.|
+| --overwrite-only          | optional           | Sets Overwrite mode in [MCUBoot](#https://docs.mcuboot.com/) image header instead of Swap.|
 | --align [1\|2\|4\|8]      | optional           | Sets flash alignment. The default value is 8.|
-| --update-key-id [0\|1]    | optional           | Sets OEM private key ID used to sign the update data packet.|
-| --update-key-path         | optional           | The key used to sign the update data packet. Overrides the --update-key-id option.|
+| --update-key-id [0\|1]    | optional           | Sets OEM private key ID used to sign the update data packet. Used to add the update packet with the NV counter to the protected TLV.|
+| --update-key-path         | optional           | The alternative option to _--update-key-id_ used to sign the update data packet. Overrides the --update-key-id option.|
 | --image-id                | optional           | Image ID. The value is used to update NV counter. The default value is 0.|
 ### Usage example
-#### Unsigned image with metadata:
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json extend-image -i image.bin -o image_extended.bin --protected-tlv 0x1A 0x1000 --protected-tlv 0x3E 0123456789 --pubkey keys/pub_key.pem
-```
-#### Unsigned image with metadata and update package:
-```bash
-$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json extend-image -i image.bin -o image_extended.bin --pubkey keys/pub_key.pem --update-key-id 0 --image-id 1
+# Unsigned image with MCUboot metadata with the additional protected TLVs
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json extend-image --image image.bin --output image_extended.bin --protected-tlv 0x1A 0x1000 --protected-tlv 0x3E 0123456789 --pubkey keys/pub_key.pem
+
+# Create an unsigned MCUboot format image with the updated NV counter. The "--update-key-id 0" option specifies that the policy "oem_priv_key_0" is used to sign the update packet with the NV counter
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json extend-image --image image.bin --output image_extended.bin --pubkey keys/pub_key.pem --update-key-id 0 --image-id 1
 ```
 
 
 ## Convert bin to hex
 Converts image of bin format to hex format.
 ### Command: `bin2hex`
 ### Parameters
 | Name          | Optional/Required  | Description     |
 | ------------- |:------------------:| --------------- |
 | --image       | required           | Input bin file  |
 | -o, --output  | required           | Output hex file |
 | --offset      | optional           | Starting address offset for loading bin |
 ### Usage example
 ```bash
+# Convert binary to Intel hex format with the start address 0x20000
 $ cysecuretools bin2hex --image image.bin --output image.hex --offset 0x20000
 ```
 
 
 ## Create debug certificate
-The debug certificate is used by BootROM to enable CM33-AP and/or Sys-AP when it is temporarily disabled. Note that the certificate cannot enable an access port that is permanently disabled by the access restrictions. Also, the debug certificate can be used to enable/disable invasive or non-invasive debug for CM33-AP.
+The debug certificate is used by ROM boot code to enable CM33-AP and/or Sys-AP when it is temporarily disabled. Note that the certificate cannot enable an access port that is permanently disabled by the access restrictions. Also, the debug certificate can be used to enable/disable invasive or non-invasive debug for CM33-AP.
 
 The command creates a debug or RMA certificate binary based on the template. The certificate must contain a public key for further verification. If it is signed using the local private key then the public key is extracted from the private. If the certificate is going to be signed using HSM, then create a non-signed certificate and specify the public key.
 ### Command: `debug-certificate`
 ### Parameters
 | Name &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Optional/Required  | Description   |
 | ------------------------- |:------------------:| ------------- |
-| --non-signed              | optional           | The flag indicating that debug certificate will not be signed. |
-| -t, --template            | optional           | The path to the certificate template in the JSON format. |
+| --non-signed              | optional           | The flag indicating that debug certificate will not be signed. Otherwise, a private key must be specified.|
+| -t, --template            | optional           | The path to the certificate template in the JSON format. Can be found in the _packets_ directory of the project. |
 | -k, --key-id [0\|1]       | optional (mutually exclusive with the _--key-path_ option) | The OEM private key ID used to sign the certificate. This ID defines the key location based on the selected policy _post_build_ section. Depending on the selected value 0 or 1, _oem_priv_key_0_ or _oem_priv_key_1_ will be used. |
 | --key-path                | optional (mutually exclusive with the _--key-id_ option) | Either a private key path for signing the certificate or a public key to be added to the certificate. This is an alternative option and can be used to specify different from the policy key file location. If it is specified, the _--key-id_ option will be ignored. |
-| --sign [cert] [signature] | optional           | The option for signing an existing certificate using existing signature file. |
+| --sign [cert] [signature] | optional           | The option for signing an existing certificate using existing signature file generated by HSM. More details in [Creation and signing debug certificate with HSM](#creation-and-signing-a-debug-certificate-with-hsm). |
 | -o, --output              | required           | The file where to save the debug certificate. |
 
-The certificate template is located in the _packets_ directory of the project (_debug_cert.json_). By default, the template is configured to be applicable for any die ID. See the [Read die id](#read-die-id) section to the find die ID of your device. See the [Get device info](#get-a-device-info) section to find silicon ID, family ID, and revision ID needed to create a certificate.
+### Edit certificate template
+The certificate template is located in the _packets_ directory of the project (_debug_cert.json_). 
+
+Silicon ID, family ID, revision ID, and die ID are necessary to create the certificate.
+1. Use [device-info](#get-device-info) command to read the device ID. 
+```bash
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json device-info
+```
+2. Specify `silicon_id`, `family_id`, `revision_id` retrieved from the device in the certificate template.
+3. By default, the template is configured to be applicable for any die ID. Use [read-die-id](#read-die-id) command to retrieve the device die ID.
+```bash
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json read-die-id
+```
+4. Specify `die_id` retrieved from the device in the certificate template.
+
+Keep `"rma": "Enable"` to generate transit to RMA certificate or change it to `Disable` to generate debug certificate.
 ### Usage example
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json debug-certificate -t packets/debug_cert.json -o packets/debug_cert.bin -k 0
+# Generate debug or transit to RMA certificate and sign it with the "oem_priv_key_0" specified in the policy
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json debug-certificate --template packets/debug_cert.json --output packets/debug_cert.bin --key-id 0
+
+# Generate unsigned debug or transit to RMA certificate. Since the private key is not provided, the public key must be provided explicitly
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json debug-certificate --template packets/debug_cert.json --key-path keys/pub_oem_0.pem --output packets/debug_cert_unsigned.bin --non-signed
+
+# Attach the existing signature to the certificate. Usually needed to sign the certificate with HSM
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json debug-certificate --sign packets/debug_cert_unsigned.bin signature.bin --output packets/debug_cert_signed.bin
 ```
 
 
 ## Read die ID
 Reads the die ID from device.
 ### Command: `read-die-id`
 ### Parameters
 | Name           | Optional/Required  | Description   |
 | -------------- |:------------------:| ------------- |
 | -o, --out-file | optional           | The name of the file where to save the die ID. If not specified, the information will be displayed in the console. |
-| --probe-id     | optional           | Probe serial number. |
+| --probe-id     | optional           | Probe serial number. Make sure to specify the probe ID if there is more than one device connected.|
 ### Usage example
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json read-die-id
+# Print device die ID and save it to the file
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json read-die-id -o die_id.json
+
+# Print the device die ID, which probe ID is 1A1A055A02010400
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json read-die-id --probe-id 1A1A055A02010400
 ```
 
 
 ## Get firmware version
-Shows BootROM version and RAM applications version used for provisioning.
+Shows ROM boot code version and RAM applications version used for provisioning.
 ### Command: `version`
 ### Parameters
 | Name           | Optional/Required  | Description   |
 | -------------- |:------------------:| ------------- |
-| --probe-id     | optional           | Probe serial number. |
+| --probe-id     | optional           | Probe serial number. Make sure to specify the probe ID if there is more than one device connected.|
 ### Usage example
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json version
 ```
 
 
 ## Get device info
 Gets device information - silicon ID, silicon revision, and family ID.
 ### Command: `device-info`
 ### Parameters
 | Name           | Optional/Required  | Description   |
 | -------------- |:------------------:| ------------- |
-| --probe-id     | optional           | Probe serial number. |
-| --ap [cm33\|sysap] | optional       | The access port used to read the data. The default value is sysap.|
+| --probe-id     | optional           | Probe serial number. Make sure to specify the probe ID if there is more than one device connected.|
 ### Usage example
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json device-info
 ```
 
 
 ## Converting binary packet to policy
@@ -412,18 +511,18 @@
 ## Return Merchandise Authorization (RMA)
 The command advances the device lifecycle stage to RMA. If the device is in the SECURE LCS the transition process requires a certificate. Use debug certificate with the RMA flag enabled (refer to [Create debug certificate](#create-debug-certificate)). The certificate must be signed with the OEM private key.
 ### Command: `convert-to-rma`
 ### Parameters
 | Name          | Optional/Required  | Description   |
 | ------------- |:------------------:| ------------- |
 | -c, --cert    | optional           | Debug certificate with the RMA flag enabled. Signed with the OEM private key. |
-| --probe-id    | optional           | Probe serial number. |
+| --probe-id    | optional           | Probe serial number. Make sure to specify the probe ID if there is more than one device connected to avoid accidental programming of the wrong device.|
 ### Usage example
 ```bash
-$ cysecuretools -t cyw20829 convert-to-rma --cert packets/debug_cert.bin
+$ cysecuretools -t cyw20829 convert-to-rma --cert packets/debug_cert.bin --probe-id 1A1A055A02010400
 ```
 
 
 # Using package together with HSM
 To protect your private keys, the cryptographic operations can be delegated to a Hardware Security Module (HSM). The flow of using the package with an HSM is different from the standard flow because of the necessity to sign the image on the remote machine. The HSM machine gets an image as an input, then signs it, and returns a signature without a payload. Then this signature has to be added to the payload in a specific format.
 
 ## Signing application with HSM
@@ -437,22 +536,22 @@
 ### Step 1
 Using the tools provided by your HSM provider, export the HSM public key to a file. The key will be added to the image for further verification.
 ### Step 2
 If your HSM provider allows exporting public keys directly to the PEM format, then this step can be skipped. However, if the HSM provider exports the public part of the key as a modulus and exponent, this data must be converted to the PEM format (see [Converting RSA key public numbers to PEM](#converting-rsa-key-public-numbers-to-pem)).
 ### Step 3
 Add the data that have to be signed - protected TLV, the public key, and [mcuboot header](https://github.com/mcu-tools/mcuboot/blob/master/docs/design.md#image-format) (added by default).
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json extend-image -i image.bin -o image_extended.bin --protected-tlv 0x1A 0x1000 --protected-tlv 0x3E 0123456789 --pubkey keys/pub_key.pem
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json extend-image --image image.bin --output image_extended.bin --protected-tlv 0x1A 0x1000 --protected-tlv 0x3E 0123456789 --pubkey keys/pub_key.pem
 ```
 ### Step 4
 Use the tools provided by your HSM provider to sign the extended image on the HSM machine. Save the signature returned by the HSM to a file.
 ### Step 5
 Run the _sign-image_ command with the _--signature_ parameter and provide the signature file created by the HSM. Use the extended image, which was sent to the HSM.
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image -i image_extended.bin -o image_signed.bin --signature signature.sig
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image_extended.bin --output image_signed.bin --signature signature.sig
 ```
 
 ## Creation and signing a debug certificate with HSM
 The flow:
 1. Export the HSM public key to a file.
 2. Convert the exported key to the PEM format.
 3. Create a non-signed debug certificate.
@@ -460,15 +559,15 @@
 5. Add a signature returned by the HSM to the certificate.
 
 ### Step 1
 Using the tools provided by your HSM provider, export the HSM public key to a file. The key will be added to the image for further verification.
 ### Step 2
 If your HSM provider allows exporting public keys directly to the PEM format then this step can be skipped. However, if the HSM provider exports the public part of the key as a modulus and exponent, this data must be converted to the PEM format (see [Converting RSA key public numbers to PEM](#converting-rsa-key-public-numbers-to-pem)).
 ### Step 3
-Create a certificate using _--non-signed_ option.
+Create a certificate using _--non-signed_ option. Specify the active OEM public key in the _--key-path_ option.
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json debug-certificate --template packets/debug_cert.json --non-signed --key-path keys/pub_key.pem --output packets/cert_unsigned.bin
 ```
 ### Step 4
 Use the tools provided by your HSM provider to sign the extended image on the HSM machine. Save the signature returned by the HSM to a file.
 ### Step 5
 Run the _debug-certificate_ command with the _--sign_ parameter and provide the unsigned certificate and the signature file created by the HSM.
@@ -486,30 +585,30 @@
 5. Add a signature returned by the HSM to the data packet.
 
 ### Step 1
 Using the tools provided by your HSM provider, export the HSM public key to a file. The key will be added to the image for further verification.
 ### Step 2
 If your HSM provider allows exporting public keys directly to the PEM format then this step can be skipped. However, if the HSM provider exports the public part of the key as a modulus and exponent, this data must be converted to the PEM format (see [Converting RSA key public numbers to PEM](#converting-rsa-key-public-numbers-to-pem)).
 ### Step 3
-Create a reprovisioning data packet using _--non-signed_ option. Also, add the public key to for the packet further verification.
+Create a reprovisioning data packet using _--non-signed_ option and add the public key for the packet further verification.
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json create-provisioning-packet --non-signed --pubkey keys/pub_key.pem
 ```
 ### Step 4
 Use the tools provided by your HSM provider to sign the data packet on the HSM machine. You can find the packet location in the previous step output. Save the signature returned by the HSM to a file.
 ### Step 5
 Run the same command with the _--signature_ parameter and provide the unsigned packet and the signature file created by the HSM.
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json create-provisioning-packet --signature keys/hsm_signature.bin
 ```
-Now, you can run the _reprovision-device_ command and the _--existing-packet_ option to make the tool not generate the packet again.
+The reprovisioning packet is generated to _packets/apps/reprovisioning/in_params.bin_ in the project directory.
 
-Or you can skip adding the signature to the packet as a separate step and directly run the _reprovision-device_ command with the _--signature_ option.
+Now, you can run the _reprovision-device_ command and the _--existing-packet_ option to make the tool not generate the packet again.
 ```bash
-$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json reprovision-device --signature keys/hsm_signature.bin
+$ cysecuretools -t cyw20829 -p policy/policy_reprovisioning_secure.json reprovision-device --existing-packet
 ```
 __IMPORTANT:__ Make sure not to add the signature more than one time for further reprovisioning.
 
 
 ## Converting RSA key public numbers to PEM
 If the HSM provider exports public part of the key as a modulus and exponent, this data must be converted to the PEM format.
 
@@ -522,19 +621,19 @@
 Copy the modulus and exponent from the exported key to the _rsa_key_tmpl.json_ file located in the _packets_ directory of your project and convert it to PEM:
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json create-key --template packets/rsa_key_tmpl.json --key-path keys/pub_key.pem
 ```
 
 
 # Encrypt the user application
-Protect confidential images by encrypting an image before transmissioning it to the device.
+Protect confidential images by encrypting an image before transmitting it to the device.
 
-There must be a 128-bit encryption key that has to be provisioned to the device. Then user's application must be signed with a private key and encrypted with this encryption key.
+There must be a 128-bit encryption key that has to be provisioned to the device. Then user's application must be encrypted with this encryption key and signed.
 
-The following example shows how to create an encryption key, provision it to the device and encrypt the image:
+The below sections show how to create an encryption key, provision it to the device and encrypt the image.
 ## Create encryption key
 This example creates a binary file containing a 128-bit encryption key in the _keys_ directory of the project.
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json create-key --aes --key-path keys/encrypt_key.bin
 ```
 ## Program encryption key
 The device must be able to decrypt the image. Therefore, the encryption key must be specified in the provisioning policy. The entire encryption key is provisioned to a device unlike the OEM key, where only a hash of the key is provisioned.
@@ -579,19 +678,19 @@
 Then run a device provisioning.
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json provision-device
 ```
 
 ## Sign and encrypt an image
 The image encryption process is similar to signing but with the additional option _--encrypt_. Another important option that needs to be specified is _--app-addr_. This is the image base address in the external memory. Points to the address from where the image needs to be encrypted:
- - for L1 application (mcuboot) - TOC2 address + TOC2 size + L1 application descriptor size.
+ - for L1 application ([MCUBoot](#https://docs.mcuboot.com/)) - TOC2 address + TOC2 size + L1 application descriptor size.
  - for the next user applications - user application base address
 
-Example for BootROM next application - the external memory application started by BootROM:
+Example for signing the external memory application executed by ROM boot code:
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed.bin --key-id 0 --image-format bootrom_next_app --encrypt --app-addr 0x08000030
 ```
-Example for MCUboot user application - the application started by MCUboot:
+Example for the application started by MCUboot:
 ```bash
 $ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image image.bin --output image_signed.hex --key-path keys/p256_priv_key.pem --encrypt --enckey keys/ec256_pub_key.pem --image-format mcuboot_user_app --app-addr 0x08020000 --hex-addr 0x60020000
 ```
 __NOTE:__ RSA key is not supported for MCUboot user application encryption. Use ECDSA key.
```

### Comparing `cysecuretools-5.1.0/docs/README_PSOC64.md` & `cysecuretools-6.0.0/docs/README_PSOC64.md`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/docs/README_XMC7XXX.md` & `cysecuretools-6.0.0/docs/README_XMC7XXX.md`

 * *Files 12% similar despite different names*

```diff
@@ -38,15 +38,18 @@
 ## 3. Sign the image
 ```bash
 $ cysecuretools -t <TARGET> sign-image --image <IMAGE_PATH> --output <OUTPUT_PATH> --key-path <KEY_PATH> [OPTIONS]
 ```
 
 # Usage example
 ```bash
+# Generate a new RSA-2048 key pair in the PEM format
 $ cysecuretools -t xmc7200 create-key --key-type rsa2048 --output private.pem public.pem --format PEM
+
+# Sign the image
 $ cysecuretools -t xmc7200 sign-image --key-path private.pem --image example-blinky.hex --output example-blinky-signed.hex 
 ```
 
 # Command-line interface
 This section contains the main CLI commands. More commands can be found in the tool help.
 
 ## Tool help
@@ -79,15 +82,19 @@
 |----------------------------------------------------------------|:-----------------:|----------------------------------------------------------|
 | --key-type [RSA2048&#124;RSA3072&#124;RSA4096&#124;ECDSA-P256] |     required      | Key type.                                                |
 | -o, --output                                                   |     required      | The output paths for generated private and public key.   |
 | --format [PEM&#124;DER&#124;JWK]                               |     optional      | Key format.                                              |
 
 ### Usage example
 ```bash
+# Generate a new ECDSA-P256 key pair in the JSON Web Key format
 $ cysecuretools -t xmc7100 create-key --key-type ecdsa-p256 --output private.jwk public.jwk --format JWK
+
+# Generate a new RSA-4096 key pair in the PEM format
+$ cysecuretools -t xmc7100 create-key --key-type rsa4096 --output private.jwk public.jwk --format PEM
 ```
 
 ## Sign image
 Signs the user application with a key.
 
 The file specified in the `--image` option will be signed and saved to the file specified in the `--output` option. 
 ### Command: `sign-image`
@@ -95,28 +102,32 @@
 | Name                             | Optional/Required | Description                                                                                                                                                                                                                           |
 |----------------------------------|:-----------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | -i,--image                       |     required      | User application image (hex or bin).                                                                                                                                                                                                  |
 | --key-path                       |     required      | The key used to sign the image.                                                                                                                                                                                                       |
 | -R, --erased-val                 |     optional      | The value that is read back from erased flash.                                                                                                                                                                                        |
 | -o, --output                     |     required      | Signed image output file.                                                                                                                                                                                                             |
 | -H, --header-size                |     optional      | Sets image header size.                                                                                                                                                                                                               |
-| -S, --slot-size                  |     optional      | Sets maximum slot size.                                                                                                                                                                                                               |
+| -S, --slot-size                  |     optional      | Sets maximum slot size. The default value is 0x20000 (=128KB).                                                                                                                                                                        |
 | --hex-addr                       |     optional      | Adjust address in hex output file.                                                                                                                                                                                                    |
 | --pad                            |     optional      | Add padding to the image trailer.                                                                                                                                                                                                     |
 | --overwrite-only                 |     optional      | Use Overwrite mode instead of Swap.                                                                                                                                                                                                   |
 | -v, --version                    |     optional      | Sets image version in the image header.                                                                                                                                                                                               |
 | -d, --dependencies               |     optional      | Add dependence on another image, format: "(<image_ID>,<image_version>), ... "                                                                                                                                                         |
 | --align [1&#124;2&#124;4&#124;8] |     optional      | Sets flash alignment. The default value is 8.                                                                                                                                                                                         |
-| --min-erase-size                 |     optional      | Sets minimum erase size. Note that this parameter is only applicable for external memory.                                                                                                                                             |
-| --protected-tlv                  |     optional      | Custom TLV that will be placed into a protected area. Add the "0x" prefix if the value should be interpreted as an integer, otherwise it will be interpreted as a string. Specify the option multiple times to add multiple TLVs      |
-| --tlv                            |     optional      | Custom TLV that will be placed into a non-protected area. Add the "0x" prefix if the value should be interpreted as an integer, otherwise it will be interpreted as a string. Specify the option multiple times to add multiple TLVs. |
+| --min-erase-size                 |     optional      | Sets minimum erase size of memory. The default value is 0x8000 (=32KB).                                                                                                                                                               |
+| --protected-tlv                  |     optional      | Custom TLV that will be placed into a protected area. Add the "0x" prefix if the value should be interpreted as an integer, otherwise it will be interpreted as a string. Specify the option multiple times to add multiple [TLVs](https://docs.mcuboot.com/design.html#protected-tlvs). |
+| --tlv                            |     optional      | Custom TLV that will be placed into a non-protected area. Add the "0x" prefix if the value should be interpreted as an integer, otherwise it will be interpreted as a string. Specify the option multiple times to add multiple [TLVs](https://docs.mcuboot.com/design.html#protected-tlvs). |
 
 ### Usage example
 ```bash
+# Sign the image with the additional protected and non-protected TLVs
 $ cysecuretools -t xmc7200 sign-image --key-path private.jwk --image example-blinky.hex --output example-blinky-signed.hex  --tlv 0xbb 0xdddddddd --tlv 0xaa 0xff --protected-tlv 0xee 0x12345678
+
+# Sign the image and pad it with zeros up to the slot size
+$ cysecuretools -t cyw20829 -p policy/policy_secure.json sign-image --image example-blinky.hex --output example-blinky-signed.hex --key-path private.pem --pad --overwrite-only --slot-size 0x10000 --header-size 0x400
 ```
 
 ## Signing the image in the CySAF format
 Signs the application in Infineon secure application format (CySAF)
 
 The ELF file specified in the `--image` option will be signed and saved to the ELF file specified in the `--output` option. 
 
@@ -135,15 +146,15 @@
 | -i,--image                | required          | User application image in CySAF format (ELF only). |
 | --key-path                | required          | The RSA key used to sign the image.                |
 | -o, --output              | required          | The signed image output file.                      |
 
 
 ### Usage example
 ```bash
-$ cysecuretools -t xmc7100 sign-cysaf --image image.elf --output image_signed.elf --key-path private.pem 
+$ cysecuretools -t xmc7100 sign-cysaf --image image.elf --output image_signed.elf --key-path private.pem
 ```
 
 ## Convert bin to hex
 Converts image of bin format to hex format.
 ### Command: `bin2hex`
 ### Parameters
 | Name          | Optional/Required  | Description                             |
@@ -228,13 +239,16 @@
 |----------------|:-----------------:|------------------------------------------------------------------------------------|
 | -k, --key-path |     required      | Input key path (supports keys in PEM, DER, JWK formats)                            |
 | -o, --output   |     required      | Output file                                                                        |
 | -f, --fmt      |     required      | Output key format. Available values: "pem", "der", "jwk", "secure_boot", "c_array" |
 | --endian       |     optional      | Byte order. Available values: "little", "big" (default: "little")                  |
 ### Usage example
 ```bash
+# Convert key in JWK format to PEM format
 $ cysecuretools convert-key --key-path private.json --output private.pem --fmt pem
-$ cysecuretools convert-key --key-path private.pem --output private.der --fmt der
-$ cysecuretools convert-key --key-path public.der --output public.json --fmt jwk
+
+# Represents a key as a C structure to include it into application
 $ cysecuretools convert-key --key-path public.der --output secure_boot_key.c --fmt secure_boot
+
+# Represents a key as a C array to include it into application
 $ cysecuretools convert-key --key-path public.jwk --output array_key.c --fmt c_array
 ```
```

### Comparing `cysecuretools-5.1.0/setup.py` & `cysecuretools-6.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -32,39 +32,39 @@
 
 setup(
     name=package_name,
     version=version,
     packages=[package_name],
     package_dir={package_name: 'src'},
     install_requires=[
-        'setuptools==59.6.0',
+        'setuptools==69.5.1',
         'cryptography==36.0.1',
         'click==8.0.4',
         'intelhex==2.3.0',
         'python-jose==3.3.0',
-        'jsonschema>=4.0.0,<=4.4.0',
+        'jsonschema>=4.0.0,<=4.22.0',
         'cbor==1.0.0',
         'packaging==21.3',
-        'lief>=0.12.3,<=0.13.1'
+        'lief==0.14.1'
         ],
     description='Python tools for provisioning Cypress/Infineon MCUs',
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/markdown',
     author='Cypress Semiconductor Corporation (an Infineon company)',
     url='https://github.com/Infineon/cysecuretools',
     license='Apache 2.0',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     include_package_data=True,  # include files from MANIFEST.in
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Embedded Systems',
     ],
     entry_points={
         'console_scripts': [
             f'cysecuretools = {package_name}.__main__:main',
         ],
```

### Comparing `cysecuretools-5.1.0/src/__about__.py` & `cysecuretools-6.0.0/src/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -11,9 +11,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 __pkg_name__ = 'CySecureTools'
-__version__ = '5.1.0'
+__version__ = '6.0.0'
 __pkg_short_name__ = 'C'
```

### Comparing `cysecuretools-5.1.0/src/__init__.py` & `cysecuretools-6.0.0/src/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/__main__.py` & `cysecuretools-6.0.0/src/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/api_common.py` & `cysecuretools-6.0.0/src/api_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/api_mxs40sv2.py` & `cysecuretools-6.0.0/src/api_mxs40sv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/api_mxs40v1.py` & `cysecuretools-6.0.0/src/api_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/api_traveo_t2g.py` & `cysecuretools-6.0.0/src/api_traveo_t2g.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/cli.py` & `cysecuretools-6.0.0/src/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/cli_creator.py` & `cysecuretools-6.0.0/src/cli_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/cli_mxs40sv2.py` & `cysecuretools-6.0.0/src/cli_mxs40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/cli_mxs40v1.py` & `cysecuretools-6.0.0/src/cli_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/cli_traveo_t2g.py` & `cysecuretools-6.0.0/src/cli_traveo_t2g.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/__init__.py` & `cysecuretools-6.0.0/src/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/bitops.py` & `cysecuretools-6.0.0/src/core/bitops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/connect_helper.py` & `cysecuretools-6.0.0/src/core/connect_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/crc.py` & `cysecuretools-6.0.0/src/core/crc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/cy_bootloader_map_parser.py` & `cysecuretools-6.0.0/src/core/cy_bootloader_map_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/dependecy_validator.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from abc import ABC, abstractmethod
+from .....core.dependecy_validator import DependencyValidator
 
 
-class DependencyValidator(ABC):
-    """ Base class for the classes that do dependency validation """
-
-    class Message:
-        def __init__(self, msg, severity):
-            self.severity = severity
-            self.message = msg
-
-    def __init__(self, policy_parser):
-        self.policy_parser = policy_parser
-        self.messages = list()
-
-    @property
-    def is_valid(self):
-        return not any(m.severity == 'error' for m in self.messages)
-
-    @abstractmethod
-    def validate(self): pass
-
-    def add_msg(self, msg, severity='error'):
-        message = self.Message(msg, severity)
-        self.messages.append(message)
+class RevocationAndEncryptionValidator(DependencyValidator):
+    def validate(self):
+        _pp = self.policy_parser
+
+        encryption = _pp.get_encryption()
+        revoke = _pp.get_revoke_oem_pubkey_0()
+
+        if revoke and encryption:
+            self.add_msg('Either the "revoke_oem_pubkey_0" or the '
+                         '"encryption" can be used. '
+                         '"revoke_oem_pubkey_0" and "encryption" '
+                         'can not be enabled at once. '
+                         'Please edit the policy')
```

### Comparing `cysecuretools-5.1.0/src/core/deprecated.py` & `cysecuretools-6.0.0/src/core/deprecated.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/entrance_exam_base.py` & `cysecuretools-6.0.0/src/core/policy_filter_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,23 +13,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from abc import ABC, abstractmethod
 
 
-class EntranceExam(ABC):
+class PolicyFilterBase(ABC):
+    """
+    Base class for policy filter.
+    Each device-specific policy filter class should implement its methods.
+    """
     @abstractmethod
-    def __init__(self, target, **kwargs):
-        pass
-
-    @abstractmethod
-    def execute(self, tool, **kwargs):
-        pass
-
-    @abstractmethod
-    def read_sfb_version(self, tool):
-        pass
-
-    @abstractmethod
-    def log_protection_state(self, tool):
+    def filter_policy(self):
         pass
```

### Comparing `cysecuretools-5.1.0/src/core/enums.py` & `cysecuretools-6.0.0/src/core/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2018-2021 Cypress Semiconductor Corporation
+Copyright 2018-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/exceptions.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
-
-class ValidationError(Exception):
-    def __init__(self, message=None, errors=None):
-        super().__init__(message)
-        self.errors = errors
+from .provisioning_packet_mxs40v1 import ProvisioningPacketMXS40v1
```

### Comparing `cysecuretools-5.1.0/src/core/json_helper.py` & `cysecuretools-6.0.0/src/core/json_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/jsonpath.py` & `cysecuretools-6.0.0/src/core/jsonpath.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/key_data.py` & `cysecuretools-6.0.0/src/core/key_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2022 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/key_handlers/__init__.py` & `cysecuretools-6.0.0/src/core/key_handlers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/key_handlers/ec_handler.py` & `cysecuretools-6.0.0/src/core/key_handlers/ec_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/key_handlers/pem_key.py` & `cysecuretools-6.0.0/src/core/key_handlers/pem_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2022 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/key_handlers/rsa_handler.py` & `cysecuretools-6.0.0/src/core/key_handlers/rsa_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/key_helper.py` & `cysecuretools-6.0.0/src/core/key_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/logging_configurator.py` & `cysecuretools-6.0.0/src/core/logging_configurator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/logging_formatter.py` & `cysecuretools-6.0.0/src/core/logging_formatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/memory_area.py` & `cysecuretools-6.0.0/src/core/memory_area.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/memory_map_base.py` & `cysecuretools-6.0.0/src/core/memory_map_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/mtb_tools_discovery.py` & `cysecuretools-6.0.0/src/core/mtb_tools_discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/ocd_settings.py` & `cysecuretools-6.0.0/src/core/ocd_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021-2022 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/policy_filter_base.py` & `cysecuretools-6.0.0/src/core/policy_parser_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,15 +13,13 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from abc import ABC, abstractmethod
 
 
-class PolicyFilterBase(ABC):
-    """
-    Base class for policy filter.
-    Each device-specific policy filter class should implement its methods.
-    """
+class PolicyParserBase(ABC):
+    """Base class for the classes that implement policy parser"""
+
     @abstractmethod
-    def filter_policy(self):
-        pass
+    def policy_type(self):
+        """Gets a value of policy type property"""
```

### Comparing `cysecuretools-5.1.0/src/core/policy_parser_base.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 """
-Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from abc import ABC, abstractmethod
-
-
-class PolicyParserBase(ABC):
-    """Base class for the classes that implement policy parser"""
-
-    @abstractmethod
-    def policy_type(self):
-        """Gets a value of policy type property"""
+from .aes_header_strategy import AesHeaderStrategy
```

### Comparing `cysecuretools-5.1.0/src/core/policy_validator_base.py` & `cysecuretools-6.0.0/src/core/policy_validator_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/progress_bar.py` & `cysecuretools-6.0.0/src/targets/common/traveo_t2g/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 """
-Copyright (c) 2020-2022 Cypress Semiconductor Corporation
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import sys
-
-
-def update_progress(progress):
-    """Prints a single-line progress bar with the specified progress"""
-    sys.stdout.write(
-        f'\r[ {"#" * progress}{" " * int(100 - progress)} ] {progress}%')
-    if progress == 100:
-        sys.stdout.write('\n')
+from .signtool_xmc7xxx import SignToolXMC7xxx
```

### Comparing `cysecuretools-5.1.0/src/core/project_base.py` & `cysecuretools-6.0.0/src/core/project_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2021 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/provisioning_flows/app_loading_flow.py` & `cysecuretools-6.0.0/src/core/provisioning_flows/app_loading_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/provisioning_flows/application.py` & `cysecuretools-6.0.0/src/core/provisioning_flows/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/ram_app_loader_base.py` & `cysecuretools-6.0.0/src/core/ram_app_loader_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/register_map_base.py` & `cysecuretools-6.0.0/src/core/register_map_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/signtool_base.py` & `cysecuretools-6.0.0/src/core/signtool_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/strategy_context/cert_strategy_ctx.py` & `cysecuretools-6.0.0/src/core/strategy_context/cert_strategy_ctx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2022 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/strategy_context/encrypted_programming_strategy_ctx.py` & `cysecuretools-6.0.0/src/core/strategy_context/encrypted_programming_strategy_ctx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/strategy_context/prov_packet_strategy_ctx.py` & `cysecuretools-6.0.0/src/core/strategy_context/prov_packet_strategy_ctx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/strategy_context/provisioning_strategy_ctx.py` & `cysecuretools-6.0.0/src/core/strategy_context/provisioning_strategy_ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2023 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/strops.py` & `cysecuretools-6.0.0/src/core/strops.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/target_builder.py` & `cysecuretools-6.0.0/src/core/target_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/target_director.py` & `cysecuretools-6.0.0/src/core/target_director.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/version_provider.py` & `cysecuretools-6.0.0/src/core/version_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/core/voltage_tool.py` & `cysecuretools-6.0.0/src/core/voltage_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/data/cy_bootloader_map.json` & `cysecuretools-6.0.0/src/data/cy_bootloader_map.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/data/mxs22/mxs22_ram_app_status_codes.py` & `cysecuretools-6.0.0/src/data/mxs22/mxs22_ram_app_status_codes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py` & `cysecuretools-6.0.0/src/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/data/mxs40v1/mxs40v1_sfb_status_codes.py` & `cysecuretools-6.0.0/src/data/mxs40v1/mxs40v1_sfb_status_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/dfuht_commands/__init__.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/entrance_exam/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .dfuht_packet_creator import DfuhtCommandsCreator
+from .exam_mxs40v1 import EntranceExamMXS40v1
+from .exam_cyb06xx7 import EntranceExamCyb06xx7
```

### Comparing `cysecuretools-5.1.0/src/execute/dfuht_commands/dfuht_packet.py` & `cysecuretools-6.0.0/src/execute/dfuht_commands/dfuht_packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/dfuht_commands/dfuht_packet_creator.py` & `cysecuretools-6.0.0/src/execute/dfuht_commands/dfuht_packet_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/image_signing/__init__.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .image import Image
+from enum import IntEnum
+
+
+class ProtectionState(IntEnum):
+    """ Device protection states """
+    unknown = 0
+    virgin = 1
+    normal = 2
+    secure = 3
+    dead = 4
+
+
+class KeyId(IntEnum):
+    HSM = 4
+    OEM = 5
+    DEVICE = 1
+    GROUP = 12
```

### Comparing `cysecuretools-5.1.0/src/execute/image_signing/image.py` & `cysecuretools-6.0.0/src/execute/image_signing/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/image_signing/image_config_parser.py` & `cysecuretools-6.0.0/src/execute/image_signing/image_config_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/image_signing/sign_tool.py` & `cysecuretools-6.0.0/src/execute/image_signing/sign_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/__init__.py` & `cysecuretools-6.0.0/src/execute/imgtool/__init__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/boot_record.py` & `cysecuretools-6.0.0/src/execute/imgtool/boot_record.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/custom_encryptor.py` & `cysecuretools-6.0.0/src/execute/imgtool/custom_encryptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python3
 #
-# Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+# Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 # or an affiliate of Cypress Semiconductor Corporation.  All rights reserved.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
```

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/image.py` & `cysecuretools-6.0.0/src/execute/imgtool/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2018 Nordic Semiconductor ASA
 # Copyright 2017-2020 Linaro Limited
 # Copyright 2019-2020 Arm Limited
-# Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+# Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 # or an affiliate of Cypress Semiconductor Corporation.  All rights reserved.
 #     Changes made to the original file:
 #     [Oct 6 2021]
 #         - Added image encryption scheme with random salt and AES
 #           initial vectors from HKDF tag
 #         - Added custom non-protected TLV support
 #         - Added option to skip adding non-protected TLV to
```

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/__init__.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/ecdsa.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/ecdsa.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/ecdsa_test.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/ecdsa_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/ed25519.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/ed25519.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/ed25519_test.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/ed25519_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/general.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/general.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/rsa.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/rsa.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/rsa_test.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/rsa_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/keys/x25519.py` & `cysecuretools-6.0.0/src/execute/imgtool/keys/x25519.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/main.py` & `cysecuretools-6.0.0/src/execute/imgtool/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python3
 #
 # Copyright 2017-2020 Linaro Limited
 # Copyright 2019-2020 Arm Limited
-# Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+# Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 # or an affiliate of Cypress Semiconductor Corporation.  All rights reserved.
 #     Changes made to the original file:
 #     [Feb 26 2021]
 #         - Added image encryption scheme with random salt and AES
 #           initial vectors from HKDF tag
 #         - Added custom non-protected TLV support
 #         - Added extend_image function
```

### Comparing `cysecuretools-5.1.0/src/execute/imgtool/version.py` & `cysecuretools-6.0.0/src/execute/imgtool/version.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/jwt.py` & `cysecuretools-6.0.0/src/execute/jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/key_reader.py` & `cysecuretools-6.0.0/src/execute/key_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/keygens/aes_keygen.py` & `cysecuretools-6.0.0/src/execute/keygens/aes_keygen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/keygens/ec_keygen.py` & `cysecuretools-6.0.0/src/execute/keygens/ec_keygen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/keygens/rsa_keygen.py` & `cysecuretools-6.0.0/src/execute/keygens/rsa_keygen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/programmer/base.py` & `cysecuretools-6.0.0/src/execute/programmer/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/programmer/dfuht_runner.py` & `cysecuretools-6.0.0/src/execute/programmer/dfuht_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/programmer/dfuht_wrapper.py` & `cysecuretools-6.0.0/src/execute/programmer/dfuht_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/programmer/openocd_server.py` & `cysecuretools-6.0.0/src/execute/programmer/openocd_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/programmer/openocd_target_map.json` & `cysecuretools-6.0.0/src/execute/programmer/openocd_target_map.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/execute/programmer/openocd_wrapper.py` & `cysecuretools-6.0.0/src/execute/programmer/openocd_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/programmer/programmer.py` & `cysecuretools-6.0.0/src/execute/programmer/programmer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/project_init/__init__.py` & `cysecuretools-6.0.0/src/execute/project_init/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/project_init/project_init.py` & `cysecuretools-6.0.0/src/execute/project_init/project_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/execute/silicon_data_reader.py` & `cysecuretools-6.0.0/src/execute/silicon_data_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/main.py` & `cysecuretools-6.0.0/src/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/pkg_globals.py` & `cysecuretools-6.0.0/src/pkg_globals.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/__init__.py` & `cysecuretools-6.0.0/src/targets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/dependencies_validation.py` & `cysecuretools-6.0.0/src/targets/common/dependencies_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/flow_parser.py` & `cysecuretools-6.0.0/src/targets/common/flow_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/__init__.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/asset.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/asset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/asset_builder.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/asset_builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/asset_enums.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/asset_enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/debug_cert/__init__.py` & `cysecuretools-6.0.0/src/core/entrance_exam_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .debug_cert_mxs40sv2 import DebugCertificateMXS40Sv2
+from abc import ABC, abstractmethod
+
+
+class EntranceExam(ABC):
+    @abstractmethod
+    def __init__(self, target, **kwargs):
+        pass
+
+    @abstractmethod
+    def execute(self, tool, **kwargs):
+        pass
+
+    @abstractmethod
+    def read_sfb_version(self, tool):
+        pass
+
+    @abstractmethod
+    def log_protection_state(self, tool):
+        pass
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_mxs40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_parser_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_parser_mxs40sv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/dependency_validator_mxs40v2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/dependency_validator_mxs40v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/enums.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/__init__.py` & `cysecuretools-6.0.0/src/core/progress_bar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .signtool_mxv40sv2 import SignToolMXS40Sv2
+import sys
+
+
+def update_progress(progress):
+    """Prints a single-line progress bar with the specified progress"""
+    sys.stdout.write(
+        f'\r[ {"#" * progress}{" " * int(100 - progress)} ] {progress}%')
+    if progress == 100:
+        sys.stdout.write('\n')
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/encrypt_mxv40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/encrypt_mxv40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/signtool_mxv40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/signtool_mxv40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/image_signing/xip_encryptor_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/xip_encryptor_mxs40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/json/cyw20829_secure.json_schema` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/json/cyw20829_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/key_source_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/key_source_mxs40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/nv_counter_calc.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/nv_counter_calc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/policy_parser.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/policy_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/policy_validator_mxs40v2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/policy_validator_mxs40v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/project_init_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/project_init_mxs40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning/__init__.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning/provision_device_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning/provision_device_mxs40sv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning/ram_app_loader_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning/ram_app_loader_mxs40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/provisioning_packet_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/provisioning_packet_mxs40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/silicon_data_reader_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/silicon_data_reader_mxs40sv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40sv2/version_provider_mxs40sv2.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/version_provider_mxs40sv2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/__init__.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/bootloader_provider_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/bootloader_provider_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/__init__.py` & `cysecuretools-6.0.0/src/core/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .aes_header_strategy import AesHeaderStrategy
+
+
+class ValidationError(Exception):
+    def __init__(self, message=None, errors=None):
+        super().__init__(message)
+        self.errors = errors
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/aes_cipher.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_cipher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/aes_header.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/aes_header_strategy.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_header_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/ecc_kdf.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/ecc_kdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/encrypted_programming/encrypted_programming.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/encrypted_programming/encrypted_programming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/entrance_exam/__init__.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .exam_mxs40v1 import EntranceExamMXS40v1
-from .exam_cyb06xx7 import EntranceExamCyb06xx7
+from .provision_device_mxs40v1 import ProvisioningMXS40v1
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/entrance_exam/exam_cyb06xx7.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/entrance_exam/exam_cyb06xx7.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/entrance_exam/exam_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/entrance_exam/exam_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/image_cert.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/image_cert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2018-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2018-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/json/policy_template.json` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/json/policy_template.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/json/schema.json_schema` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/json/schema.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/key_reader_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/key_reader_mxs40v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/key_source_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/key_source_mxs40v1.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/policy_filter.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/policy_filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/policy_parser.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/policy_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/policy_validator.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/policy_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/project_init_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/project_init_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning/__init__.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/voltage_tool/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .provision_device_mxs40v1 import ProvisioningMXS40v1
+from .voltage_tool_mxs40v1 import VoltageToolMXS40v1
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning/provision_device_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning/provision_device_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2018-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2018-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning/sys_call.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning/sys_call.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2018-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2018-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_crypto.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_crypto.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_customer.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_customer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_dev.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_dev.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_entity.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_hsm.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_hsm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -59,15 +60,15 @@
                                 x509.load_pem_x509_certificate(bytes(barr), default_backend())
                             except ValueError as e:
                                 raise ValueError(f'{e} Invalid certificate \'{cert_file}\'') from e
                         except UnicodeDecodeError:
                             sequence.append(self.der_to_pem(cert_file))
                     payload[k] = sequence
                 else:
-                    if os.path.isfile(v):
+                    if isinstance(v, str) and os.path.isfile(v):
                         payload[k] = Crypto.read_jwt(v)
                     else:
                         payload[k] = v
 
         payload['type'] = Types.HSM_PROV_CMD
 
         hsm_priv_key = self.state['hsm_priv_key']
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_oem.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_oem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_types.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/provisioning_packet/provisioning_packet_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/provisioning_packet/provisioning_packet_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/signtool_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/signtool_mxs40v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/silicon_data_parser.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/silicon_data_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/silicon_data_reader_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/silicon_data_reader_mxs40v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2021 Cypress Semiconductor Corporation
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/version_provider_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/version_provider_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/voltage_tool/__init__.py` & `cysecuretools-6.0.0/src/targets/common/mxs40sv2/image_signing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .voltage_tool_mxs40v1 import VoltageToolMXS40v1
+from .signtool_mxv40sv2 import SignToolMXS40Sv2
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/voltage_tool/lvd_voltage_picker.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/voltage_tool/lvd_voltage_picker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/voltage_tool/voltage_tool_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/voltage_tool/voltage_tool_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/mxs40v1/x509_mxs40v1.py` & `cysecuretools-6.0.0/src/targets/common/mxs40v1/x509_mxs40v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/policy_validator.py` & `cysecuretools-6.0.0/src/targets/common/policy_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/common/traveo_t2g/__init__.py` & `cysecuretools-6.0.0/src/targets/cyw89829/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .signtool_xmc7xxx import SignToolXMC7xxx
+from .target_builder import CYW89829Builder
+
+target_map = {
+    'cyw89829': {
+        'default': {
+            'class': CYW89829Builder,
+            'family': 'MXS40Sv2 Family',
+            'display_name': 'CYW89829',
+            'type': 'family',
+            'platform': 'mxs40sv2'
+        }
+    }
+}
```

### Comparing `cysecuretools-5.1.0/src/targets/common/traveo_t2g/signtool_xmc7xxx.py` & `cysecuretools-6.0.0/src/targets/common/traveo_t2g/signtool_xmc7xxx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/__init__.py` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/maps/memory_map.py` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/maps/memory_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/maps/register_map.py` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/maps/register_map.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/packets/cy_auth_512k_b0_sample.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/packets/cy_auth_512k_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/packets/entrance_exam.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4.json` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4_smif.json` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4_smif.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4.json` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4_smif.json` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4_smif.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx5_a1/target_builder.py` & `cysecuretools-6.0.0/src/targets/cyb06xx5_a1/target_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/__init__.py` & `cysecuretools-6.0.0/src/targets/cyb06xx7/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/maps/memory_map.py` & `cysecuretools-6.0.0/src/targets/cyb06xx7/maps/memory_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/maps/register_map.py` & `cysecuretools-6.0.0/src/targets/cyb06xx7/maps/register_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/packets/entrance_exam.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xx7/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json` & `cysecuretools-6.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json` & `cysecuretools-6.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-6.0.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724746729269755%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'boot_auth': [3], 'bootloader_keys': {0: {'kid': 3, 'key': "*

 * *                   "'../keys/cy_pub_key.json'}}, 'protect_flags': 3, 'resources': {0: {'address': "*

 * *                   "270336000}, 1: {'address': 135135232}, 2: {'address': 135184384}, 3: "*

 * *                   "{'address': 270303232}, 4: {'address': 405012480}}, 'reset_after_failure': 0}, "*

 * *                   "1: {'resources': {0: {'size': 1867776}, 1: {'address': 402883584, 'size': "*

 * *                   "18677 […]*

```diff
@@ -1,49 +1,50 @@
 {
     "boot_upgrade": {
         "firmware": [
             {
                 "acq_win": 100,
                 "boot_auth": [
-                    5
+                    3
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/prebuilt/oem_state.json",
-                        "kid": 5
+                        "key": "../keys/cy_pub_key.json",
+                        "kid": 3
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
-                "protect_flags": 1,
+                "protect_flags": 3,
+                "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 269287424,
+                        "address": 270336000,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
-                        "address": 134348800,
+                        "address": 135135232,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
-                        "address": 134397952,
+                        "address": 135184384,
                         "size": 16384,
                         "type": "SRAM_DAP"
                     },
                     {
-                        "address": 269254656,
+                        "address": 270303232,
                         "size": 32768,
                         "type": "STATUS_PARTITION"
                     },
                     {
-                        "address": 404226048,
+                        "address": 405012480,
                         "size": 786432,
                         "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
                 "upgrade_mode": "swap",
                 "wdt_enable": true,
@@ -60,31 +61,32 @@
                         "kid": 8
                     }
                 ],
                 "encrypt": false,
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
+                "launch": 16,
                 "monotonic": 0,
-                "multi_image": 1,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 262144,
+                        "size": 1867776,
                         "type": "BOOT"
                     },
                     {
-                        "address": 402653696,
-                        "size": 262144,
+                        "address": 402883584,
+                        "size": 1867776,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "set_img_ok": true,
                 "smif_id": 1,
+                "smif_sector_size": 262144,
                 "upgrade": true,
                 "version": "0.1",
                 "wdt_enable": false,
                 "wdt_timeout": 4000
             },
             {
                 "boot_auth": [
@@ -97,37 +99,31 @@
                     }
                 ],
                 "encrypt": false,
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
-                "multi_image": 2,
                 "resources": [
                     {
-                        "address": 268697600,
-                        "size": 557056,
+                        "address": 268500992,
+                        "size": 1802240,
                         "type": "BOOT"
-                    },
-                    {
-                        "address": 403407360,
-                        "size": 557056,
-                        "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
-                "smif_id": 1,
-                "upgrade": true,
+                "smif_id": 0,
+                "upgrade": false,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 269287424
+                "start": 270336000
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -171,21 +167,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json` & `cysecuretools-6.0.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735989347662141%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'boot_auth': [3], 'bootloader_keys': {0: {'kid': 3, 'key': "*

 * *                   "'../keys/cy_pub_key.json'}}, 'protect_flags': 3, 'resources': {0: {'address': "*

 * *                   "270336000}, 1: {'address': 135135232}, 2: {'address': 135184384}, 3: "*

 * *                   "{'address': 270303232}, 4: {'address': 270270464}}, 'reset_after_failure': 0}, "*

 * *                   "1: {'resources': {0: {'size': 458752}, 1: {'address': 268894208, 'size': "*

 * *                   "458752 […]*

```diff
@@ -1,49 +1,50 @@
 {
     "boot_upgrade": {
         "firmware": [
             {
                 "acq_win": 100,
                 "boot_auth": [
-                    5
+                    3
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/prebuilt/oem_state.json",
-                        "kid": 5
+                        "key": "../keys/cy_pub_key.json",
+                        "kid": 3
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
-                "protect_flags": 1,
+                "protect_flags": 3,
+                "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 269287424,
+                        "address": 270336000,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
-                        "address": 134348800,
+                        "address": 135135232,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
-                        "address": 134397952,
+                        "address": 135184384,
                         "size": 16384,
                         "type": "SRAM_DAP"
                     },
                     {
-                        "address": 269254656,
+                        "address": 270303232,
                         "size": 32768,
                         "type": "STATUS_PARTITION"
                     },
                     {
-                        "address": 269221888,
+                        "address": 270270464,
                         "size": 32768,
                         "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
                 "upgrade_mode": "swap",
                 "wdt_enable": true,
@@ -65,20 +66,20 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "monotonic": 0,
                 "multi_image": 1,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 196608,
+                        "size": 458752,
                         "type": "BOOT"
                     },
                     {
-                        "address": 268632064,
-                        "size": 196608,
+                        "address": 268894208,
+                        "size": 458752,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "set_img_ok": true,
                 "smif_id": 0,
                 "upgrade": true,
@@ -100,34 +101,34 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "multi_image": 2,
                 "resources": [
                     {
-                        "address": 268828672,
-                        "size": 196608,
+                        "address": 269352960,
+                        "size": 458752,
                         "type": "BOOT"
                     },
                     {
-                        "address": 269025280,
-                        "size": 196608,
+                        "address": 269811712,
+                        "size": 458752,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": true,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 269287424
+                "start": 270336000
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -171,21 +172,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4.json` & `cysecuretools-6.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json` & `cysecuretools-6.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json` & `cysecuretools-6.0.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735089464026352%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'boot_auth': [3], 'bootloader_keys': {0: {'kid': 3, 'key': "*

 * *                   "'../keys/cy_pub_key.json'}}, 'protect_flags': 3, 'resources': {0: {'address': "*

 * *                   "270336000}, 1: {'address': 135135232}, 2: {'address': 135184384}, 3: "*

 * *                   "{'address': 270319616, 'size': 16384}, 4: {'address': 270270464, 'size': "*

 * *                   "49152}}, 'reset_after_failure': 0}, 1: {'smif_id': 0, 'resources': {0: "*

 * *                   "{'size': 91750 […]*

```diff
@@ -1,50 +1,51 @@
 {
     "boot_upgrade": {
         "firmware": [
             {
                 "acq_win": 100,
                 "boot_auth": [
-                    5
+                    3
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/prebuilt/oem_state.json",
-                        "kid": 5
+                        "key": "../keys/cy_pub_key.json",
+                        "kid": 3
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
-                "protect_flags": 1,
+                "protect_flags": 3,
+                "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 269287424,
+                        "address": 270336000,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
-                        "address": 134348800,
+                        "address": 135135232,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
-                        "address": 134397952,
+                        "address": 135184384,
                         "size": 16384,
                         "type": "SRAM_DAP"
                     },
                     {
-                        "address": 269254656,
-                        "size": 32768,
+                        "address": 270319616,
+                        "size": 16384,
                         "type": "STATUS_PARTITION"
                     },
                     {
-                        "address": 403963904,
-                        "size": 1048576,
+                        "address": 270270464,
+                        "size": 49152,
                         "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
                 "upgrade_mode": "swap",
                 "wdt_enable": true,
                 "wdt_timeout": 4000
@@ -65,26 +66,26 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "launch": 16,
                 "monotonic": 0,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 819200,
+                        "size": 917504,
                         "type": "BOOT"
                     },
                     {
-                        "address": 402883072,
-                        "size": 819200,
+                        "address": 269352960,
+                        "size": 917504,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "set_img_ok": true,
-                "smif_id": 1,
+                "smif_id": 0,
                 "upgrade": true,
                 "version": "0.1",
                 "wdt_enable": false,
                 "wdt_timeout": 4000
             },
             {
                 "boot_auth": [
@@ -100,28 +101,28 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "resources": [
                     {
                         "address": 268500992,
-                        "size": 753664,
+                        "size": 851968,
                         "type": "BOOT"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": false,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 269287424
+                "start": 270336000
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -165,21 +166,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json` & `cysecuretools-6.0.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9734471450617285%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'boot_auth': [3], 'bootloader_keys': {0: {'kid': 3, 'key': "*

 * *                   "'../keys/cy_pub_key.json'}}, 'resources': {0: {'address': 270336000}, 1: "*

 * *                   "{'address': 135135232}, 2: {'address': 135184384}, 3: {'address': 270303232, "*

 * *                   "'size': 32768}, 4: {'address': 405012480, 'size': 786432}}, "*

 * *                   "'reset_after_failure': 0}, 1: {'smif_id': 1, 'resources': {0: {'size': "*

 * *                   "1867776}, 1: {'address': […]*

```diff
@@ -1,50 +1,51 @@
 {
     "boot_upgrade": {
         "firmware": [
             {
                 "acq_win": 100,
                 "boot_auth": [
-                    5
+                    3
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/prebuilt/oem_state.json",
-                        "kid": 5
+                        "key": "../keys/cy_pub_key.json",
+                        "kid": 3
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
                 "protect_flags": 1,
+                "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 269287424,
+                        "address": 270336000,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
-                        "address": 134348800,
+                        "address": 135135232,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
-                        "address": 134397952,
+                        "address": 135184384,
                         "size": 16384,
                         "type": "SRAM_DAP"
                     },
                     {
-                        "address": 269271040,
-                        "size": 16384,
+                        "address": 270303232,
+                        "size": 32768,
                         "type": "STATUS_PARTITION"
                     },
                     {
-                        "address": 269221888,
-                        "size": 49152,
+                        "address": 405012480,
+                        "size": 786432,
                         "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
                 "upgrade_mode": "swap",
                 "wdt_enable": true,
                 "wdt_timeout": 4000
@@ -65,26 +66,27 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "launch": 16,
                 "monotonic": 0,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 393216,
+                        "size": 1867776,
                         "type": "BOOT"
                     },
                     {
-                        "address": 268828672,
-                        "size": 393216,
+                        "address": 402883584,
+                        "size": 1867776,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "set_img_ok": true,
-                "smif_id": 0,
+                "smif_id": 1,
+                "smif_sector_size": 262144,
                 "upgrade": true,
                 "version": "0.1",
                 "wdt_enable": false,
                 "wdt_timeout": 4000
             },
             {
                 "boot_auth": [
@@ -100,28 +102,28 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "resources": [
                     {
                         "address": 268500992,
-                        "size": 327680,
+                        "size": 1802240,
                         "type": "BOOT"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": false,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 269287424
+                "start": 270336000
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -165,21 +167,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_2m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xx7/target_builder.py` & `cysecuretools-6.0.0/src/targets/cyb06xx7/target_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/__init__.py` & `cysecuretools-6.0.0/src/targets/cyb06xxa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/maps/memory_map.py` & `cysecuretools-6.0.0/src/targets/cyb06xxa/maps/memory_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/maps/register_map.py` & `cysecuretools-6.0.0/src/targets/cyb06xxa/maps/register_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/packets/entrance_exam.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xxa/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-6.0.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json` & `cysecuretools-6.0.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json` & `cysecuretools-6.0.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996458884479718%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'resources': {3: {'address': 270319616, 'size': 16384}, 4: "*

 * *                   "{'address': 270270464, 'size': 49152}}}, 1: {'smif_id': 0, 'resources': {0: "*

 * *                   "{'size': 917504}, 1: {'address': 269352960, 'size': 917504}}, delete: "*

 * *                   "['smif_sector_size']}, 2: {'resources': {0: {'size': 851968}}}}}"}*

```diff
@@ -31,21 +31,21 @@
                     },
                     {
                         "address": 135184384,
                         "size": 16384,
                         "type": "SRAM_DAP"
                     },
                     {
-                        "address": 270303232,
-                        "size": 32768,
+                        "address": 270319616,
+                        "size": 16384,
                         "type": "STATUS_PARTITION"
                     },
                     {
-                        "address": 405012480,
-                        "size": 786432,
+                        "address": 270270464,
+                        "size": 49152,
                         "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
                 "upgrade_mode": "swap",
                 "wdt_enable": true,
                 "wdt_timeout": 4000
@@ -66,27 +66,26 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "launch": 16,
                 "monotonic": 0,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 1867776,
+                        "size": 917504,
                         "type": "BOOT"
                     },
                     {
-                        "address": 402883584,
-                        "size": 1867776,
+                        "address": 269352960,
+                        "size": 917504,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "set_img_ok": true,
-                "smif_id": 1,
-                "smif_sector_size": 262144,
+                "smif_id": 0,
                 "upgrade": true,
                 "version": "0.1",
                 "wdt_enable": false,
                 "wdt_timeout": 4000
             },
             {
                 "boot_auth": [
@@ -102,15 +101,15 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "resources": [
                     {
                         "address": 268500992,
-                        "size": 1802240,
+                        "size": 851968,
                         "type": "BOOT"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": false,
                 "version": "0.1"
```

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyb06xxa/target_builder.py` & `cysecuretools-6.0.0/src/targets/cyb06xxa/target_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/__init__.py` & `cysecuretools-6.0.0/src/targets/cys06xxa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt` & `cysecuretools-6.0.0/src/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/packets/entrance_exam.jwt` & `cysecuretools-6.0.0/src/targets/cys06xxa/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-6.0.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex` & `cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-6.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cys06xxa/target_builder.py` & `cysecuretools-6.0.0/src/targets/cys06xxa/target_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/__init__.py` & `cysecuretools-6.0.0/src/targets/cyw20829/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/flows/prov_flows.json` & `cysecuretools-6.0.0/src/targets/cyw20829/flows/prov_flows.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/packets/debug_cert.json` & `cysecuretools-6.0.0/src/targets/cyw20829/packets/debug_cert.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_hci_secure.json` & `cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_hci_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_no_secure.json` & `cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_no_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_reprovisioning_secure.json` & `cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_reprovisioning_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/policy/policy_secure.json` & `cysecuretools-6.0.0/src/targets/cyw20829/policy/policy_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829/target_builder.py` & `cysecuretools-6.0.0/src/targets/cyw20829/target_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/__init__.py` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/flows/prov_flows.json` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/flows/prov_flows.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/asset_map.py` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/asset_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/memory_map.py` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/memory_map.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/register_map.py` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/register_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/maps/reverse_asset_map.py` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/maps/reverse_asset_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/packets/debug_cert.json` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/packets/debug_cert.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_hci_secure.json` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_hci_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_no_secure.json` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_no_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/policy/policy_secure.json` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/policy/policy_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/policy_generator.py` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/policy_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2021-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw20829_a0/target_builder.py` & `cysecuretools-6.0.0/src/targets/cyw20829_a0/target_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2020-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/flows/prov_flows.json` & `cysecuretools-6.0.0/src/targets/cyw89829/flows/prov_flows.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin` & `cysecuretools-6.0.0/src/targets/cyw89829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/packets/debug_cert.json` & `cysecuretools-6.0.0/src/targets/cyw89829/packets/debug_cert.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_hci_secure.json` & `cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_hci_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_no_secure.json` & `cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_no_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_reprovisioning_secure.json` & `cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_reprovisioning_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/policy/policy_secure.json` & `cysecuretools-6.0.0/src/targets/cyw89829/policy/policy_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-5.1.0/src/targets/cyw89829/target_builder.py` & `cysecuretools-6.0.0/src/targets/cyw89829/target_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/xmc7xxx/__init__.py` & `cysecuretools-6.0.0/src/targets/xmc7xxx/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-5.1.0/src/targets/xmc7xxx/target_builder.py` & `cysecuretools-6.0.0/src/targets/xmc7xxx/target_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2023-2024 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

