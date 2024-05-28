# Comparing `tmp/aspose_barcode_cloud-24.4.0.tar.gz` & `tmp/aspose_barcode_cloud-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspose_barcode_cloud-24.4.0.tar", last modified: Mon Apr 29 11:46:20 2024, max compression
+gzip compressed data, was "aspose_barcode_cloud-24.5.0.tar", last modified: Tue May 28 04:33:56 2024, max compression
```

## Comparing `aspose_barcode_cloud-24.4.0.tar` & `aspose_barcode_cloud-24.5.0.tar`

### file list

```diff
@@ -1,117 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15474 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12541 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.122451 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/
--rw-r--r--   0 root         (0) root         (0)     6208 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.122451 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/
--rw-r--r--   0 root         (0) root         (0)      319 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104561 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/barcode_api.py
--rw-r--r--   0 root         (0) root         (0)    23228 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/file_api.py
--rw-r--r--   0 root         (0) root         (0)    21383 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/folder_api.py
--rw-r--r--   0 root         (0) root         (0)    15051 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/storage_api.py
--rw-r--r--   0 root         (0) root         (0)    24950 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api_client.py
--rw-r--r--   0 root         (0) root         (0)     9362 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/
--rw-r--r--   0 root         (0) root         (0)     5753 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/api_error.py
--rw-r--r--   0 root         (0) root         (0)     3505 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/api_error_response.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/australian_post_params.py
--rw-r--r--   0 root         (0) root         (0)     2302 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/auto_size_mode.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/available_graphics_unit.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)    11091 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_params.py
--rw-r--r--   0 root         (0) root         (0)     2324 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
--rw-r--r--   0 root         (0) root         (0)     5156 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/barcode_response.py
--rw-r--r--   0 root         (0) root         (0)     3066 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/barcode_response_list.py
--rw-r--r--   0 root         (0) root         (0)     2344 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/border_dash_style.py
--rw-r--r--   0 root         (0) root         (0)     7246 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/caption_params.py
--rw-r--r--   0 root         (0) root         (0)     2302 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/checksum_validation.py
--rw-r--r--   0 root         (0) root         (0)     2292 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
--rw-r--r--   0 root         (0) root         (0)     5280 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_params.py
--rw-r--r--   0 root         (0) root         (0)     2276 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_symbol.py
--rw-r--r--   0 root         (0) root         (0)     4405 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codablock_params.py
--rw-r--r--   0 root         (0) root         (0)     2330 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_emulation.py
--rw-r--r--   0 root         (0) root         (0)     2388 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3171 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_params.py
--rw-r--r--   0 root         (0) root         (0)     5444 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code16_k_params.py
--rw-r--r--   0 root         (0) root         (0)     2282 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code_location.py
--rw-r--r--   0 root         (0) root         (0)     3169 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/coupon_params.py
--rw-r--r--   0 root         (0) root         (0)     2380 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
--rw-r--r--   0 root         (0) root         (0)     6939 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_bar_params.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
--rw-r--r--   0 root         (0) root         (0)     2458 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)    11710 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_params.py
--rw-r--r--   0 root         (0) root         (0)     4728 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_version.py
--rw-r--r--   0 root         (0) root         (0)     4806 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/decode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     3844 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/disc_usage.py
--rw-r--r--   0 root         (0) root         (0)     2324 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     8325 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/dot_code_params.py
--rw-r--r--   0 root         (0) root         (0)     2960 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/eci_encodings.py
--rw-r--r--   0 root         (0) root         (0)     2286 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/enable_checksum.py
--rw-r--r--   0 root         (0) root         (0)     4404 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/encode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     4901 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/error.py
--rw-r--r--   0 root         (0) root         (0)     3668 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)     7758 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/file_version.py
--rw-r--r--   0 root         (0) root         (0)     2902 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/file_versions.py
--rw-r--r--   0 root         (0) root         (0)     2926 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/files_list.py
--rw-r--r--   0 root         (0) root         (0)     3701 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/files_upload_result.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_mode.py
--rw-r--r--   0 root         (0) root         (0)     4138 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_params.py
--rw-r--r--   0 root         (0) root         (0)     2332 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_style.py
--rw-r--r--   0 root         (0) root         (0)    56510 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/generator_params.py
--rw-r--r--   0 root         (0) root         (0)     4827 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/generator_params_list.py
--rw-r--r--   0 root         (0) root         (0)     2362 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_error_level.py
--rw-r--r--   0 root         (0) root         (0)     6343 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_params.py
--rw-r--r--   0 root         (0) root         (0)     4598 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_version.py
--rw-r--r--   0 root         (0) root         (0)     2338 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/itf14_border_type.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/itf_params.py
--rw-r--r--   0 root         (0) root         (0)     2298 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/macro_character.py
--rw-r--r--   0 root         (0) root         (0)     2328 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     2324 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_mode.py
--rw-r--r--   0 root         (0) root         (0)     4616 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_params.py
--rw-r--r--   0 root         (0) root         (0)     3875 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/object_exist.py
--rw-r--r--   0 root         (0) root         (0)     4681 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/padding.py
--rw-r--r--   0 root         (0) root         (0)     4398 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/patch_code_params.py
--rw-r--r--   0 root         (0) root         (0)     2372 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/patch_format.py
--rw-r--r--   0 root         (0) root         (0)     2338 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_error_level.py
--rw-r--r--   0 root         (0) root         (0)     2312 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
--rw-r--r--   0 root         (0) root         (0)    29407 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_params.py
--rw-r--r--   0 root         (0) root         (0)     3108 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/postal_params.py
--rw-r--r--   0 root         (0) root         (0)     2454 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/preset_type.py
--rw-r--r--   0 root         (0) root         (0)     2390 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     2300 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_encode_type.py
--rw-r--r--   0 root         (0) root         (0)     2312 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_error_level.py
--rw-r--r--   0 root         (0) root         (0)    10984 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_params.py
--rw-r--r--   0 root         (0) root         (0)     3462 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_version.py
--rw-r--r--   0 root         (0) root         (0)    47480 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/reader_params.py
--rw-r--r--   0 root         (0) root         (0)     3471 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/region_point.py
--rw-r--r--   0 root         (0) root         (0)     4647 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/result_image_info.py
--rw-r--r--   0 root         (0) root         (0)     2976 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/storage_exist.py
--rw-r--r--   0 root         (0) root         (0)     5948 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/storage_file.py
--rw-r--r--   0 root         (0) root         (0)     4996 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/structured_append.py
--rw-r--r--   0 root         (0) root         (0)     2288 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/text_alignment.py
--rw-r--r--   0 root         (0) root         (0)    13304 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15474 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4689 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4717 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1848 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_auth.py
--rw-r--r--   0 root         (0) root         (0)     6492 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_barcode_api.py
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1413 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_generate_and_recognize.py
--rw-r--r--   0 root         (0) root         (0)     1803 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_headers.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_load_configuration.py
--rw-r--r--   0 root         (0) root         (0)     2751 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_recognize_bytes.py
--rw-r--r--   0 root         (0) root         (0)     2698 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_recognize_file.py
--rw-r--r--   0 root         (0) root         (0)     1064 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_recognize_url.py
--rw-r--r--   0 root         (0) root         (0)     1401 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_recognize_with_timeout.py
--rw-r--r--   0 root         (0) root         (0)     1133 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_scan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:33:56.107522 aspose_barcode_cloud-24.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15424 2024-05-28 04:33:56.107522 aspose_barcode_cloud-24.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12541 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:33:56.097522 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/
+-rw-r--r--   0 root         (0) root         (0)     6208 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:33:56.097522 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104561 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/barcode_api.py
+-rw-r--r--   0 root         (0) root         (0)    23228 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/file_api.py
+-rw-r--r--   0 root         (0) root         (0)    21383 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    15051 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/storage_api.py
+-rw-r--r--   0 root         (0) root         (0)    24954 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     9362 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:33:56.107522 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/
+-rw-r--r--   0 root         (0) root         (0)     5753 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/api_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/australian_post_params.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/auto_size_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/available_graphics_unit.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/aztec_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)    11091 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/aztec_params.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/barcode_response.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/barcode_response_list.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/border_dash_style.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/caption_params.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/checksum_validation.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5280 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/codabar_params.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/codabar_symbol.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/codablock_params.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code128_emulation.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code128_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3171 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code128_params.py
+-rw-r--r--   0 root         (0) root         (0)     5444 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code16_k_params.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/coupon_params.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
+-rw-r--r--   0 root         (0) root         (0)     6939 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_bar_params.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)    11710 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_matrix_params.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_matrix_version.py
+-rw-r--r--   0 root         (0) root         (0)     4806 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/decode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     3844 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/disc_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/dot_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/eci_encodings.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/enable_checksum.py
+-rw-r--r--   0 root         (0) root         (0)     4404 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/encode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)     7758 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/file_version.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/file_versions.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/files_upload_result.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/font_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4138 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/font_params.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/font_style.py
+-rw-r--r--   0 root         (0) root         (0)    56510 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/generator_params.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/generator_params_list.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/han_xin_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/han_xin_error_level.py
+-rw-r--r--   0 root         (0) root         (0)     6343 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/han_xin_params.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/han_xin_version.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/itf14_border_type.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/itf_params.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/macro_character.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/maxi_code_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/maxi_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/object_exist.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/padding.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/patch_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/patch_format.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/pdf417_error_level.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
+-rw-r--r--   0 root         (0) root         (0)    29407 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/pdf417_params.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/postal_params.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/preset_type.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_encode_type.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_error_level.py
+-rw-r--r--   0 root         (0) root         (0)    10984 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_params.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_version.py
+-rw-r--r--   0 root         (0) root         (0)    47480 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/reader_params.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/region_point.py
+-rw-r--r--   0 root         (0) root         (0)     4647 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/result_image_info.py
+-rw-r--r--   0 root         (0) root         (0)     2976 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/storage_exist.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/storage_file.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/structured_append.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/text_alignment.py
+-rw-r--r--   0 root         (0) root         (0)    13302 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:33:56.107522 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15424 2024-05-28 04:33:56.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4674 2024-05-28 04:33:56.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 04:33:56.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-28 04:33:56.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-28 04:33:56.000000 aspose_barcode_cloud-24.5.0/aspose_barcode_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 04:33:56.107522 aspose_barcode_cloud-24.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4668 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:33:56.107522 aspose_barcode_cloud-24.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_auth.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_barcode_api.py
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_generate_and_recognize.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_headers.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_load_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_recognize_bytes.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_recognize_file.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_recognize_url.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_recognize_with_timeout.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-05-28 04:32:22.000000 aspose_barcode_cloud-24.5.0/tests/test_scan.py
```

### Comparing `aspose_barcode_cloud-24.4.0/LICENSE` & `aspose_barcode_cloud-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/PKG-INFO` & `aspose_barcode_cloud-24.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 24.4.0
+Version: 24.5.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -17,15 +17,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -39,15 +38,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
 [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 24.4.0
+- Package version: 24.5.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -55,15 +54,15 @@
 
 [Aspose.BarCode for Cloud](https://products.aspose.cloud/barcode/) is a REST API for Linear, 2D and postal barcode generation and recognition in the cloud. API recognizes and generates barcode images in a variety of formats. Barcode REST API allows to specify barcode image attributes like image width, height, border style and output image format in order to customize the generation process. Developers can also specify the barcode type and text attributes such as text location and font styles in order to suit the application requirements.
 
 This repository contains Aspose.BarCode Cloud SDK for Python source code. This SDK allows you to work with Aspose.BarCode for Cloud REST APIs in your Python 2 or Python 3 applications quickly and easily.
 
 Supported Python versions:
 
-- Python 3.5+
+- Python 3.6+
 
 To use these SDKs, you will need Client Id and Client Secret which can be looked up at [Aspose Cloud Dashboard](https://dashboard.aspose.cloud/applications) (free registration in Aspose Cloud is required for this).
 
 ## How to use the SDK
 
 The complete source code is available in this repository folder. You can either directly use it in your project via source code or get [from PyPi](https://pypi.org/project/aspose-barcode-cloud/) (recommended).
```

### Comparing `aspose_barcode_cloud-24.4.0/README.md` & `aspose_barcode_cloud-24.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
 [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 24.4.0
+- Package version: 24.5.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -17,15 +17,15 @@
 
 [Aspose.BarCode for Cloud](https://products.aspose.cloud/barcode/) is a REST API for Linear, 2D and postal barcode generation and recognition in the cloud. API recognizes and generates barcode images in a variety of formats. Barcode REST API allows to specify barcode image attributes like image width, height, border style and output image format in order to customize the generation process. Developers can also specify the barcode type and text attributes such as text location and font styles in order to suit the application requirements.
 
 This repository contains Aspose.BarCode Cloud SDK for Python source code. This SDK allows you to work with Aspose.BarCode for Cloud REST APIs in your Python 2 or Python 3 applications quickly and easily.
 
 Supported Python versions:
 
-- Python 3.5+
+- Python 3.6+
 
 To use these SDKs, you will need Client Id and Client Secret which can be looked up at [Aspose Cloud Dashboard](https://dashboard.aspose.cloud/applications) (free registration in Aspose Cloud is required for this).
 
 ## How to use the SDK
 
 The complete source code is available in this repository folder. You can either directly use it in your project via source code or get [from PyPi](https://pypi.org/project/aspose-barcode-cloud/) (recommended).
```

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/__init__.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/barcode_api.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/barcode_api.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/file_api.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/file_api.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/folder_api.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/folder_api.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/storage_api.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api/storage_api.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api_client.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,21 @@
         self.configuration = configuration
 
         # Use the pool property to lazily initialize the ThreadPool.
         self._pool = None
         self.rest_client = RESTClientObject(configuration)
         self.default_headers = {
             "x-aspose-client": "python sdk",
-            "x-aspose-client-version": "24.4.0",
+            "x-aspose-client-version": "24.5.0",
         }
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "Aspose-Barcode-SDK/24.4.0/python"
+        self.user_agent = "Aspose-Barcode-SDK/24.5.0/python"
 
     def __del__(self):
         self.rest_client.close()
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
 
@@ -254,15 +254,15 @@
         :param klass: class literal, or string of class name.
 
         :return: object.
         """
         if data is None:
             return None
 
-        if type(klass) == str:
+        if isinstance(klass, str):
             if klass.startswith("list["):
                 sub_kls = re.match(r"list\[(.*)]", klass).group(1)
                 return [self.__deserialize(sub_data, sub_kls) for sub_data in data]
 
             if klass.startswith("dict("):
                 sub_kls = re.match(r"dict\(([^,]*), (.*)\)", klass).group(2)
                 return {k: self.__deserialize(v, sub_kls) for k, v in six.iteritems(data)}
```

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/configuration.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 3.0\n"
-            "SDK Package Version: 24.4.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 24.5.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     @staticmethod
     def fetch_token(client_id, client_secret, token_url):
         with contextlib.closing(
             RESTClientObject(Configuration(client_id=client_id, client_secret=client_secret, token_url=token_url))
         ) as client:
```

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/__init__.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/api_error.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/api_error.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/api_error_response.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/australian_post_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/australian_post_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/auto_size_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/auto_size_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/available_graphics_unit.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/available_graphics_unit.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_encode_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/aztec_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/aztec_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_symbol_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/aztec_symbol_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/barcode_response.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/barcode_response.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/barcode_response_list.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/barcode_response_list.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/border_dash_style.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/border_dash_style.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/caption_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/caption_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/checksum_validation.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/checksum_validation.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_checksum_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/codabar_checksum_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/codabar_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_symbol.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/codabar_symbol.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codablock_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/codablock_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_emulation.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code128_emulation.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_encode_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code128_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code128_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code16_k_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code16_k_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code_location.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/code_location.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/coupon_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/coupon_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_bar_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_bar_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_matrix_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_version.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/data_matrix_version.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/decode_barcode_type.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/decode_barcode_type.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/disc_usage.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/dot_code_encode_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/dot_code_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/dot_code_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/dot_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/eci_encodings.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/eci_encodings.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/enable_checksum.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/enable_checksum.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/encode_barcode_type.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/encode_barcode_type.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/error.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/error.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/error_details.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/file_version.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/file_versions.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/files_list.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/files_upload_result.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/font_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/font_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_style.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/font_style.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/generator_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/generator_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/generator_params_list.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/generator_params_list.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_encode_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/han_xin_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_error_level.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/han_xin_error_level.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/han_xin_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_version.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/han_xin_version.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/itf14_border_type.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/itf14_border_type.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/itf_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/itf_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/macro_character.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/macro_character.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/maxi_code_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/maxi_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/object_exist.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/padding.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/padding.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/patch_code_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/patch_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/patch_format.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/patch_format.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_error_level.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/pdf417_error_level.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/pdf417_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/postal_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/postal_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/preset_type.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/preset_type.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_encode_mode.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_encode_type.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_encode_type.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_error_level.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_error_level.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_version.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/qr_version.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/reader_params.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/reader_params.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/region_point.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/region_point.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/result_image_info.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/result_image_info.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/storage_exist.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/storage_file.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/structured_append.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/structured_append.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/text_alignment.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/models/text_alignment.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/rest.py` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
         return self.urllib3_response.getheader(name, default)
 
 
 class RESTClientObject(object):
-
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
         # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
         # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
 
@@ -357,15 +356,14 @@
         )
 
     def close(self):
         self.pool_manager.clear()
 
 
 class ApiException(Exception):
-
     def __init__(self, status=0, reason=None, http_resp=None):
         # type: (int, str, RESTResponse) -> None
         if http_resp:
             self.status = http_resp.status
             self.reason = http_resp.reason
             self.body = http_resp.data
         else:
```

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/PKG-INFO` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 24.4.0
+Version: 24.5.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -17,15 +17,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -39,15 +38,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
 [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 24.4.0
+- Package version: 24.5.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -55,15 +54,15 @@
 
 [Aspose.BarCode for Cloud](https://products.aspose.cloud/barcode/) is a REST API for Linear, 2D and postal barcode generation and recognition in the cloud. API recognizes and generates barcode images in a variety of formats. Barcode REST API allows to specify barcode image attributes like image width, height, border style and output image format in order to customize the generation process. Developers can also specify the barcode type and text attributes such as text location and font styles in order to suit the application requirements.
 
 This repository contains Aspose.BarCode Cloud SDK for Python source code. This SDK allows you to work with Aspose.BarCode for Cloud REST APIs in your Python 2 or Python 3 applications quickly and easily.
 
 Supported Python versions:
 
-- Python 3.5+
+- Python 3.6+
 
 To use these SDKs, you will need Client Id and Client Secret which can be looked up at [Aspose Cloud Dashboard](https://dashboard.aspose.cloud/applications) (free registration in Aspose Cloud is required for this).
 
 ## How to use the SDK
 
 The complete source code is available in this repository folder. You can either directly use it in your project via source code or get [from PyPi](https://pypi.org/project/aspose-barcode-cloud/) (recommended).
```

### Comparing `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/SOURCES.txt` & `aspose_barcode_cloud-24.5.0/aspose_barcode_cloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-pyproject.toml
 setup.py
 aspose_barcode_cloud/__init__.py
 aspose_barcode_cloud/api_client.py
 aspose_barcode_cloud/configuration.py
 aspose_barcode_cloud/rest.py
 aspose_barcode_cloud.egg-info/PKG-INFO
 aspose_barcode_cloud.egg-info/SOURCES.txt
```

### Comparing `aspose_barcode_cloud-24.4.0/setup.py` & `aspose_barcode_cloud-24.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import os
 
 from setuptools import setup, find_packages
 
 NAME = "aspose-barcode-cloud"
-VERSION = "24.4.0"
+VERSION = "24.5.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -33,15 +33,14 @@
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_auth.py` & `aspose_barcode_cloud-24.5.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_barcode_api.py` & `aspose_barcode_cloud-24.5.0/tests/test_barcode_api.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_generate_and_recognize.py` & `aspose_barcode_cloud-24.5.0/tests/test_generate_and_recognize.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_headers.py` & `aspose_barcode_cloud-24.5.0/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_load_configuration.py` & `aspose_barcode_cloud-24.5.0/tests/test_load_configuration.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_recognize_bytes.py` & `aspose_barcode_cloud-24.5.0/tests/test_recognize_bytes.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_recognize_file.py` & `aspose_barcode_cloud-24.5.0/tests/test_recognize_file.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_recognize_url.py` & `aspose_barcode_cloud-24.5.0/tests/test_recognize_url.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_recognize_with_timeout.py` & `aspose_barcode_cloud-24.5.0/tests/test_recognize_with_timeout.py`

 * *Files identical despite different names*

### Comparing `aspose_barcode_cloud-24.4.0/tests/test_scan.py` & `aspose_barcode_cloud-24.5.0/tests/test_scan.py`

 * *Files identical despite different names*

