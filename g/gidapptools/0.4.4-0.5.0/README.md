# Comparing `tmp/gidapptools-0.4.4.tar.gz` & `tmp/gidapptools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gidapptools-0.4.4.tar", last modified: Sat Nov 26 22:23:18 2022, max compression
+gzip compressed data, was "gidapptools-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gidapptools-0.4.4.tar` & `gidapptools-0.5.0.tar`

### file list

```diff
@@ -1,196 +1,226 @@
--rw-r--r--   0        0        0     1064 2021-08-31 18:36:20.520000 gidapptools-0.4.4/LICENSE
--rw-r--r--   0        0        0      148 2022-08-06 19:27:50.440341 gidapptools-0.4.4/README.rst
--rw-r--r--   0        0        0      505 2022-11-26 22:22:58.651809 gidapptools-0.4.4/gidapptools/__init__.py
--rw-r--r--   0        0        0      660 2022-11-02 13:03:46.993653 gidapptools-0.4.4/gidapptools/__main__.py
--rw-r--r--   0        0        0      106 2021-09-20 21:57:04.325557 gidapptools-0.4.4/gidapptools/abstract_classes/__init__.py
--rw-r--r--   0        0        0     2093 2022-11-02 13:03:47.013599 gidapptools-0.4.4/gidapptools/abstract_classes/abstract_meta_factory.py
--rw-r--r--   0        0        0     1319 2022-11-02 13:03:47.032548 gidapptools-0.4.4/gidapptools/abstract_classes/abstract_meta_item.py
--rw-r--r--   0        0        0      580 2022-11-02 13:03:46.929061 gidapptools-0.4.4/gidapptools/cli_info.py
--rw-r--r--   0        0        0      695 2022-11-02 13:03:46.943024 gidapptools-0.4.4/gidapptools/custom_types.py
--rw-r--r--   0        0        0       69 2022-01-12 13:50:02.703044 gidapptools-0.4.4/gidapptools/data/__init__.py
--rw-r--r--   0        0        0     1453 2022-11-02 13:03:47.054491 gidapptools-0.4.4/gidapptools/data/conversion_data.py
--rw-r--r--   0        0        0      126 2022-11-02 13:03:47.066458 gidapptools-0.4.4/gidapptools/data/general_data.py
--rw-r--r--   0        0        0     1035 2022-03-20 03:11:40.597216 gidapptools-0.4.4/gidapptools/data/gifs/__init__.py
--rw-r--r--   0        0        0    21837 2022-03-04 16:17:21.627813 gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_1.gif
--rw-r--r--   0        0        0    28904 2022-03-04 16:31:53.112866 gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_2.gif
--rw-r--r--   0        0        0   780846 2022-03-04 16:16:38.588118 gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_3.gif
--rw-r--r--   0        0        0   126652 2022-03-04 16:35:31.028357 gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_4.gif
--rw-r--r--   0        0        0    72232 2022-03-05 00:49:16.857127 gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_5.gif
--rw-r--r--   0        0        0    77029 2022-03-05 00:49:38.490391 gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_6.gif
--rw-r--r--   0        0        0    75110 2022-03-05 00:49:54.683726 gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_7.gif
--rw-r--r--   0        0        0    24880 2022-03-05 00:48:39.458832 gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_cat.gif
--rw-r--r--   0        0        0       80 2021-12-14 11:09:57.360075 gidapptools-0.4.4/gidapptools/data/json/__init__.py
--rw-r--r--   0        0        0    16646 2021-12-14 11:02:54.001076 gidapptools-0.4.4/gidapptools/data/json/webcolors.json
--rw-r--r--   0        0        0    12516 2022-11-21 20:01:58.476636 gidapptools-0.4.4/gidapptools/errors.py
--rw-r--r--   0        0        0        0 2022-04-28 02:40:17.435746 gidapptools-0.4.4/gidapptools/general_helper/__init__.py
--rw-r--r--   0        0        0      681 2022-11-02 13:03:47.079424 gidapptools-0.4.4/gidapptools/general_helper/checker.py
--rw-r--r--   0        0        0     2602 2022-11-02 13:03:47.098373 gidapptools-0.4.4/gidapptools/general_helper/class_helper.py
--rw-r--r--   0        0        0        0 2021-10-04 15:25:35.923246 gidapptools-0.4.4/gidapptools/general_helper/color/__init__.py
--rw-r--r--   0        0        0     2309 2022-11-02 13:03:47.735521 gidapptools-0.4.4/gidapptools/general_helper/color/color.py
--rw-r--r--   0        0        0    12017 2022-11-02 13:03:47.781420 gidapptools-0.4.4/gidapptools/general_helper/color/color_item.py
--rw-r--r--   0        0        0        0 2021-12-14 11:01:49.256730 gidapptools-0.4.4/gidapptools/general_helper/color/preset_colors/__init__.py
--rw-r--r--   0        0        0     1241 2022-11-02 13:03:47.796165 gidapptools-0.4.4/gidapptools/general_helper/color/preset_colors/web_colors.py
--rw-r--r--   0        0        0     1307 2022-11-02 13:03:47.116325 gidapptools-0.4.4/gidapptools/general_helper/compress.py
--rw-r--r--   0        0        0        0 2021-11-20 18:26:05.665295 gidapptools-0.4.4/gidapptools/general_helper/concurrency/__init__.py
--rw-r--r--   0        0        0     1065 2022-11-02 13:03:47.811102 gidapptools-0.4.4/gidapptools/general_helper/concurrency/events.py
--rw-r--r--   0        0        0     2677 2022-11-02 13:03:47.829053 gidapptools-0.4.4/gidapptools/general_helper/concurrency/locks.py
--rw-r--r--   0        0        0     1703 2022-11-02 13:03:47.859001 gidapptools-0.4.4/gidapptools/general_helper/concurrency/switch.py
--rw-r--r--   0        0        0      491 2022-11-02 13:03:47.875928 gidapptools-0.4.4/gidapptools/general_helper/concurrency/threadpools.py
--rw-r--r--   0        0        0    14962 2022-11-02 13:03:47.190203 gidapptools-0.4.4/gidapptools/general_helper/conversion.py
--rw-r--r--   0        0        0     4773 2022-11-21 20:18:31.781609 gidapptools-0.4.4/gidapptools/general_helper/date_time.py
--rw-r--r--   0        0        0   254882 2022-10-25 22:47:39.001650 gidapptools-0.4.4/gidapptools/general_helper/development/QMenu.html
--rw-r--r--   0        0        0       60 2022-03-03 04:10:34.793253 gidapptools-0.4.4/gidapptools/general_helper/development/__init__.py
--rw-r--r--   0        0        0    11342 2022-11-02 13:03:47.941752 gidapptools-0.4.4/gidapptools/general_helper/development/inspect_helpers.py
--rw-r--r--   0        0        0     3406 2022-11-02 13:03:47.976686 gidapptools-0.4.4/gidapptools/general_helper/development/misc.py
--rw-r--r--   0        0        0    15126 2022-11-02 13:03:47.377100 gidapptools-0.4.4/gidapptools/general_helper/dict_helper.py
--rw-r--r--   0        0        0     5285 2022-11-02 13:03:47.400039 gidapptools-0.4.4/gidapptools/general_helper/dispatch_table.py
--rw-r--r--   0        0        0     2277 2022-11-02 13:03:47.417990 gidapptools-0.4.4/gidapptools/general_helper/enums.py
--rw-r--r--   0        0        0     5864 2022-11-02 13:03:47.455914 gidapptools-0.4.4/gidapptools/general_helper/general.py
--rw-r--r--   0        0        0     3111 2022-11-02 13:03:47.481819 gidapptools-0.4.4/gidapptools/general_helper/general_classes.py
--rw-r--r--   0        0        0     1663 2022-11-02 13:03:47.526700 gidapptools-0.4.4/gidapptools/general_helper/hashing.py
--rw-r--r--   0        0        0     2168 2022-11-02 13:03:47.546646 gidapptools-0.4.4/gidapptools/general_helper/import_helper.py
--rw-r--r--   0        0        0     2823 2022-11-02 13:03:47.565597 gidapptools-0.4.4/gidapptools/general_helper/io_helper.py
--rw-r--r--   0        0        0        0 2022-08-06 19:27:50.929033 gidapptools-0.4.4/gidapptools/general_helper/meta_helper/__init__.py
--rw-r--r--   0        0        0     3369 2022-11-02 13:03:48.019544 gidapptools-0.4.4/gidapptools/general_helper/meta_helper/single_running_instance.py
--rw-r--r--   0        0        0        0 2021-09-27 16:39:28.396464 gidapptools-0.4.4/gidapptools/general_helper/mixins/__init__.py
--rw-r--r--   0        0        0     8400 2022-11-02 13:03:48.054450 gidapptools-0.4.4/gidapptools/general_helper/mixins/file_mixin.py
--rw-r--r--   0        0        0      188 2022-03-31 12:52:12.827634 gidapptools-0.4.4/gidapptools/general_helper/output_helper/__init__.py
--rw-r--r--   0        0        0     4443 2022-11-02 13:03:48.094372 gidapptools-0.4.4/gidapptools/general_helper/output_helper/rich_helper.py
--rw-r--r--   0        0        0      491 2022-11-02 13:03:48.107309 gidapptools-0.4.4/gidapptools/general_helper/output_helper/rich_styles.py
--rw-r--r--   0        0        0     4419 2022-11-02 13:03:47.600502 gidapptools-0.4.4/gidapptools/general_helper/path_helper.py
--rw-r--r--   0        0        0        0 2021-10-27 16:15:21.832963 gidapptools-0.4.4/gidapptools/general_helper/regex/__init__.py
--rw-r--r--   0        0        0     1749 2022-11-02 13:03:48.119277 gidapptools-0.4.4/gidapptools/general_helper/regex/datetime_regex.py
--rw-r--r--   0        0        0      491 2022-11-02 13:03:47.616460 gidapptools-0.4.4/gidapptools/general_helper/ressource_classes.py
--rw-r--r--   0        0        0    16012 2022-11-02 13:03:47.658348 gidapptools-0.4.4/gidapptools/general_helper/string_helper.py
--rw-r--r--   0        0        0     4909 2022-11-02 13:03:47.687648 gidapptools-0.4.4/gidapptools/general_helper/timing.py
--rw-r--r--   0        0        0     1020 2022-11-02 13:03:47.703604 gidapptools-0.4.4/gidapptools/general_helper/typing_helper.py
--rw-r--r--   0        0        0      953 2022-11-02 13:03:47.718573 gidapptools-0.4.4/gidapptools/general_helper/web_helper.py
--rw-r--r--   0        0        0       61 2022-09-23 14:25:48.373107 gidapptools-0.4.4/gidapptools/gid_argparse/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 13:44:44.191704 gidapptools-0.4.4/gidapptools/gid_argparse/custom_actions/__init__.py
--rw-r--r--   0        0        0      491 2022-11-02 13:03:49.005085 gidapptools-0.4.4/gidapptools/gid_argparse/custom_actions/base_actions.py
--rw-r--r--   0        0        0     5670 2022-11-02 13:03:48.984145 gidapptools-0.4.4/gidapptools/gid_argparse/custom_parser.py
--rw-r--r--   0        0        0      669 2022-10-08 05:04:32.804406 gidapptools-0.4.4/gidapptools/gid_config/__init__.py
--rw-r--r--   0        0        0        0 2021-09-23 00:22:27.273740 gidapptools-0.4.4/gidapptools/gid_config/conversion/__init__.py
--rw-r--r--   0        0        0    11432 2022-11-02 13:03:49.115428 gidapptools-0.4.4/gidapptools/gid_config/conversion/base_converters.py
--rw-r--r--   0        0        0     3108 2022-11-02 13:03:49.138665 gidapptools-0.4.4/gidapptools/gid_config/conversion/conversion_table.py
--rw-r--r--   0        0        0     3078 2022-11-02 13:03:49.158612 gidapptools-0.4.4/gidapptools/gid_config/conversion/converter_grammar.py
--rw-r--r--   0        0        0     1360 2022-11-02 13:03:49.173572 gidapptools-0.4.4/gidapptools/gid_config/conversion/extra_base_typus.py
--rw-r--r--   0        0        0     7840 2022-11-02 13:03:49.205511 gidapptools-0.4.4/gidapptools/gid_config/conversion/spec_data.py
--rw-r--r--   0        0        0     4890 2022-11-02 13:03:49.230421 gidapptools-0.4.4/gidapptools/gid_config/conversion/spec_item.py
--rw-r--r--   0        0        0      608 2022-11-02 13:03:49.016034 gidapptools-0.4.4/gidapptools/gid_config/enums.py
--rw-r--r--   0        0        0    11933 2022-11-02 13:03:49.055956 gidapptools-0.4.4/gidapptools/gid_config/interface.py
--rw-r--r--   0        0        0        0 2021-09-23 00:22:27.273740 gidapptools-0.4.4/gidapptools/gid_config/parser/__init__.py
--rw-r--r--   0        0        0     9756 2022-11-02 13:03:49.297264 gidapptools-0.4.4/gidapptools/gid_config/parser/config_data.py
--rw-r--r--   0        0        0     4548 2022-11-02 13:03:49.317717 gidapptools-0.4.4/gidapptools/gid_config/parser/grammar.py
--rw-r--r--   0        0        0     5992 2022-11-02 13:03:49.339659 gidapptools-0.4.4/gidapptools/gid_config/parser/ini_parser.py
--rw-r--r--   0        0        0     4792 2022-11-02 13:03:49.368610 gidapptools-0.4.4/gidapptools/gid_config/parser/tokens.py
--rw-r--r--   0        0        0        0 2022-09-23 03:58:23.085387 gidapptools-0.4.4/gidapptools/gid_database/__init__.py
--rw-r--r--   0        0        0      145 2022-09-23 04:02:35.172766 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/__init__.py
--rw-r--r--   0        0        0      153 2022-09-23 03:59:53.337430 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/__init__.py
--rw-r--r--   0        0        0    14208 2022-11-02 13:03:49.444743 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/apsw_database.py
--rw-r--r--   0        0        0     1515 2022-11-02 13:03:49.464213 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/constants.py
--rw-r--r--   0        0        0        0 2022-09-23 10:53:55.853779 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/custom_base_models/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 11:29:26.257182 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/custom_fields/__init__.py
--rw-r--r--   0        0        0        0 2022-10-08 05:05:38.373765 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/__init__.py
--rw-r--r--   0        0        0      665 2022-11-02 13:03:49.531035 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/commit_hook_functions.py
--rw-r--r--   0        0        0     1066 2022-11-02 13:03:49.552976 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/profile_hook_functions.py
--rw-r--r--   0        0        0      665 2022-11-02 13:03:49.571927 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/rollback_hook_functions.py
--rw-r--r--   0        0        0      665 2022-11-02 13:03:49.591873 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/update_hook_functions.py
--rw-r--r--   0        0        0      665 2022-11-02 13:03:49.609848 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/wal_hook_functions.py
--rw-r--r--   0        0        0     7469 2022-11-02 13:03:49.509116 gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/pragma_info.py
--rw-r--r--   0        0        0        0 2021-11-04 00:01:05.741311 gidapptools-0.4.4/gidapptools/gid_logger/__init__.py
--rw-r--r--   0        0        0     4641 2022-11-02 13:03:49.630768 gidapptools-0.4.4/gidapptools/gid_logger/enums.py
--rw-r--r--   0        0        0    10628 2022-11-02 13:03:49.681634 gidapptools-0.4.4/gidapptools/gid_logger/fake_logger.py
--rw-r--r--   0        0        0    16733 2022-11-02 13:03:49.740501 gidapptools-0.4.4/gidapptools/gid_logger/formatter.py
--rw-r--r--   0        0        0     8170 2022-11-02 13:03:49.821401 gidapptools-0.4.4/gidapptools/gid_logger/handler.py
--rw-r--r--   0        0        0    10997 2022-11-02 13:03:49.860083 gidapptools-0.4.4/gidapptools/gid_logger/logger.py
--rw-r--r--   0        0        0     4060 2022-11-02 13:03:49.884011 gidapptools-0.4.4/gidapptools/gid_logger/misc.py
--rw-r--r--   0        0        0     3608 2022-11-02 13:03:49.903938 gidapptools-0.4.4/gidapptools/gid_logger/records.py
--rw-r--r--   0        0        0      149 2022-08-06 19:27:51.411743 gidapptools-0.4.4/gidapptools/gid_parsing/__init__.py
--rw-r--r--   0        0        0     4216 2022-11-02 13:03:49.929869 gidapptools-0.4.4/gidapptools/gid_parsing/py_log_parsing.py
--rw-r--r--   0        0        0        0 2022-01-15 19:38:52.874584 gidapptools-0.4.4/gidapptools/gid_parsing/tokens/__init__.py
--rw-r--r--   0        0        0     1166 2022-11-02 13:03:49.999989 gidapptools-0.4.4/gidapptools/gid_parsing/tokens/base_tokens.py
--rw-r--r--   0        0        0        0 2022-01-15 19:38:52.874584 gidapptools-0.4.4/gidapptools/gid_parsing/universal/__init__.py
--rw-r--r--   0        0        0     2966 2022-11-02 13:03:50.019940 gidapptools-0.4.4/gidapptools/gid_parsing/universal/character_elements.py
--rw-r--r--   0        0        0     4571 2022-11-02 13:03:50.049832 gidapptools-0.4.4/gidapptools/gid_parsing/universal/datetime_elements.py
--rw-r--r--   0        0        0        0 2022-08-06 19:27:51.547380 gidapptools-0.4.4/gidapptools/gid_pytest/__init__.py
--rw-r--r--   0        0        0      487 2022-11-02 13:03:50.062822 gidapptools-0.4.4/gidapptools/gid_pytest/parameter.py
--rw-r--r--   0        0        0        0 2021-09-29 21:44:28.330981 gidapptools-0.4.4/gidapptools/gid_signal/__init__.py
--rw-r--r--   0        0        0     1413 2022-11-02 13:03:50.081748 gidapptools-0.4.4/gidapptools/gid_signal/interface.py
--rw-r--r--   0        0        0     1674 2022-11-02 13:03:50.099700 gidapptools-0.4.4/gidapptools/gid_signal/signal_registry.py
--rw-r--r--   0        0        0        0 2021-09-29 21:44:28.330981 gidapptools-0.4.4/gidapptools/gid_signal/signals/__init__.py
--rw-r--r--   0        0        0     3446 2022-11-02 13:03:50.121642 gidapptools-0.4.4/gidapptools/gid_signal/signals/abstract_signal.py
--rw-r--r--   0        0        0     2340 2022-11-02 13:03:50.146574 gidapptools-0.4.4/gidapptools/gid_signal/signals/basic_signal.py
--rw-r--r--   0        0        0      491 2022-11-02 13:03:50.158542 gidapptools-0.4.4/gidapptools/gid_signal/signals/qt_signal.py
--rw-r--r--   0        0        0       29 2022-03-11 23:29:54.398628 gidapptools-0.4.4/gidapptools/gid_utility/__init__.py
--rw-r--r--   0        0        0     3768 2022-11-02 13:03:50.177491 gidapptools-0.4.4/gidapptools/gid_utility/version_item.py
--rw-r--r--   0        0        0        0 2022-03-21 03:01:51.190903 gidapptools-0.4.4/gidapptools/gid_warning/__init__.py
--rw-r--r--   0        0        0     3373 2022-11-02 13:03:50.199462 gidapptools-0.4.4/gidapptools/gid_warning/deprecation.py
--rw-r--r--   0        0        0     1295 2022-11-02 13:03:50.213420 gidapptools-0.4.4/gidapptools/gid_warning/experimental.py
--rw-r--r--   0        0        0      229 2022-04-18 18:34:33.321765 gidapptools-0.4.4/gidapptools/gidapptools_qt/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 20:52:02.729934 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/__init__.py
--rw-r--r--   0        0        0     1244 2022-08-18 05:21:57.885946 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/images/__init__.py
--rw-r--r--   0        0        0    12608 2022-08-18 05:21:13.655846 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/images/default_app_icon.png
--rw-r--r--   0        0        0   134024 2021-12-11 23:04:26.441608 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/images/placeholder.png
--rw-r--r--   0        0        0      421 2022-08-24 18:17:31.865700 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/templates/__init__.py
--rw-r--r--   0        0        0      220 2022-08-24 18:35:31.118550 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/templates/about_stylesheet.css
--rw-r--r--   0        0        0      598 2022-08-24 18:40:47.966025 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/templates/about_template.jinja_html
--rw-r--r--   0        0        0      826 2022-08-24 18:14:01.808478 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/templates/arg_doc_html_template.jinja_html
--rw-r--r--   0        0        0      218 2022-08-24 18:15:48.522228 gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/templates/arg_doc_markdown_template.jinja_md
--rw-r--r--   0        0        0        0 2021-11-25 19:55:33.355786 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/__init__.py
--rw-r--r--   0        0        0    27392 2022-11-02 13:03:48.277854 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/application.py
--rw-r--r--   0        0        0     1063 2022-11-02 13:03:48.296803 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/application_info.py
--rw-r--r--   0        0        0     1607 2022-11-02 13:03:48.337693 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/application_new.py
--rw-r--r--   0        0        0      491 2022-11-02 13:03:48.351684 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/command_line_parser.py
--rw-r--r--   0        0        0     2825 2022-11-02 13:03:48.370629 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/main_window.py
--rw-r--r--   0        0        0     5824 2022-11-02 13:03:48.398531 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/menu_bar.py
--rw-r--r--   0        0        0     1447 2022-11-02 13:03:48.416483 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/status_bar.py
--rw-r--r--   0        0        0     6470 2022-11-02 13:03:48.448427 gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/sys_tray.py
--rw-r--r--   0        0        0        0 2022-01-06 22:29:45.436190 gidapptools-0.4.4/gidapptools/gidapptools_qt/debug/__init__.py
--rw-r--r--   0        0        0     7216 2022-11-02 13:03:48.477898 gidapptools-0.4.4/gidapptools/gidapptools_qt/debug/event_analyzer.py
--rw-r--r--   0        0        0        0 2021-12-07 00:05:58.701876 gidapptools-0.4.4/gidapptools/gidapptools_qt/dialogs/__init__.py
--rw-r--r--   0        0        0     1786 2022-11-02 13:03:48.501654 gidapptools-0.4.4/gidapptools/gidapptools_qt/dialogs/app_info_dialog.py
--rw-r--r--   0        0        0        0 2021-12-07 22:19:08.564742 gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/__init__.py
--rw-r--r--   0        0        0        0 2021-12-07 22:19:08.564742 gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/command_line_parser/__init__.py
--rw-r--r--   0        0        0     1488 2022-11-02 13:03:48.620606 gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/command_line_parser/parser.py
--rw-r--r--   0        0        0     1158 2022-11-02 13:03:48.518708 gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/misc.py
--rw-r--r--   0        0        0      742 2022-11-02 13:03:48.532488 gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/object_name.py
--rw-r--r--   0        0        0      491 2022-11-02 13:03:48.545431 gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/signal_bridge.py
--rw-r--r--   0        0        0     1284 2022-11-02 13:03:48.577293 gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/window_geometry_helper.py
--rw-r--r--   0        0        0     2514 2022-11-02 13:03:48.599707 gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/window_reference_keeper.py
--rw-r--r--   0        0        0        0 2022-02-27 16:36:21.918865 gidapptools-0.4.4/gidapptools/gidapptools_qt/layouts/__init__.py
--rw-r--r--   0        0        0      818 2022-11-02 13:03:48.635465 gidapptools-0.4.4/gidapptools/gidapptools_qt/layouts/vertical_form_layout.py
--rw-r--r--   0        0        0        0 2021-12-02 11:38:53.174893 gidapptools-0.4.4/gidapptools/gidapptools_qt/models/__init__.py
--rw-r--r--   0        0        0     1793 2022-11-02 13:03:48.655270 gidapptools-0.4.4/gidapptools/gidapptools_qt/models/basic_model.py
--rw-r--r--   0        0        0        0 2022-01-06 22:01:16.199629 gidapptools-0.4.4/gidapptools/gidapptools_qt/resources/__init__.py
--rw-r--r--   0        0        0     1623 2022-11-02 13:03:48.673555 gidapptools-0.4.4/gidapptools/gidapptools_qt/resources/placeholder.py
--rw-r--r--   0        0        0     5389 2022-11-02 13:03:48.728996 gidapptools-0.4.4/gidapptools/gidapptools_qt/resources/resources_helper.py
--rw-r--r--   0        0        0        0 2021-12-02 11:32:36.936086 gidapptools-0.4.4/gidapptools/gidapptools_qt/views/__init__.py
--rw-r--r--   0        0        0      493 2022-11-02 13:03:48.742961 gidapptools-0.4.4/gidapptools/gidapptools_qt/views/basic_view.py
--rw-r--r--   0        0        0        0 2021-12-07 00:05:58.701876 gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/__init__.py
--rw-r--r--   0        0        0    11646 2022-11-02 13:03:48.781422 gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/app_log_viewer.py
--rw-r--r--   0        0        0    10932 2022-11-02 13:03:48.820172 gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/category_select_widget.py
--rw-r--r--   0        0        0     1987 2022-11-02 13:03:48.842080 gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/hyperlink_label.py
--rw-r--r--   0        0        0     3556 2022-11-02 13:03:48.865822 gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/icon_text_button.py
--rw-r--r--   0        0        0     1061 2022-11-02 13:03:48.880778 gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/json_editor.py
--rw-r--r--   0        0        0     5492 2022-11-02 13:03:48.906550 gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/spinner_widget.py
--rw-r--r--   0        0        0     6640 2022-11-02 13:03:48.934815 gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/std_stream_widget.py
--rw-r--r--   0        0        0       96 2021-09-14 19:29:19.689941 gidapptools-0.4.4/gidapptools/meta_data/__init__.py
--rw-r--r--   0        0        0     2811 2022-11-02 13:03:50.235365 gidapptools-0.4.4/gidapptools/meta_data/config_kwargs.py
--rw-r--r--   0        0        0     7497 2022-11-02 13:03:50.266254 gidapptools-0.4.4/gidapptools/meta_data/interface.py
--rw-r--r--   0        0        0       65 2021-09-19 15:57:06.694208 gidapptools-0.4.4/gidapptools/meta_data/meta_info/__init__.py
--rw-r--r--   0        0        0     6330 2022-11-02 13:03:50.296176 gidapptools-0.4.4/gidapptools/meta_data/meta_info/meta_info_factory.py
--rw-r--r--   0        0        0     5969 2022-11-02 13:03:50.344074 gidapptools-0.4.4/gidapptools/meta_data/meta_info/meta_info_item.py
--rw-r--r--   0        0        0       67 2021-09-19 15:57:36.351976 gidapptools-0.4.4/gidapptools/meta_data/meta_paths/__init__.py
--rw-r--r--   0        0        0     2415 2022-11-02 13:03:50.362001 gidapptools-0.4.4/gidapptools/meta_data/meta_paths/appdirs_implementations.py
--rw-r--r--   0        0        0     2938 2022-11-02 13:03:50.380349 gidapptools-0.4.4/gidapptools/meta_data/meta_paths/meta_paths_factory.py
--rw-r--r--   0        0        0     6151 2022-11-02 13:03:50.412266 gidapptools-0.4.4/gidapptools/meta_data/meta_paths/meta_paths_item.py
--rw-r--r--   0        0        0        0 2021-09-22 03:09:38.138175 gidapptools-0.4.4/gidapptools/utility/__init__.py
--rw-r--r--   0        0        0     3024 2022-11-02 13:03:50.430245 gidapptools-0.4.4/gidapptools/utility/enums.py
--rw-r--r--   0        0        0     8393 2022-11-02 13:03:50.475174 gidapptools-0.4.4/gidapptools/utility/helper.py
--rw-r--r--   0        0        0     2524 2022-11-02 13:03:50.496865 gidapptools-0.4.4/gidapptools/utility/kwarg_dict.py
--rw-r--r--   0        0        0        0 2022-08-06 21:26:08.033946 gidapptools-0.4.4/gidapptools/vendored/__init__.py
--rw-r--r--   0        0        0     7128 2022-11-02 13:03:50.593217 gidapptools-0.4.4/gidapptools/vendored/atomic_writes.py
--rw-r--r--   0        0        0     1069 2022-06-30 02:44:23.800813 gidapptools-0.4.4/gidapptools/vendored/atomic_writes_LICENSE
--rw-r--r--   0        0        0     3118 2022-11-26 21:56:08.074098 gidapptools-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 gidapptools-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-08-31 18:36:20.520000 gidapptools-0.5.0/LICENSE
+-rw-r--r--   0        0        0      649 2023-04-07 20:25:45.102049 gidapptools-0.5.0/README.rst
+-rw-r--r--   0        0        0      716 2024-05-27 23:51:56.629160 gidapptools-0.5.0/gidapptools/__init__.py
+-rw-r--r--   0        0        0      667 2023-01-07 14:13:33.733996 gidapptools-0.5.0/gidapptools/__main__.py
+-rw-r--r--   0        0        0      106 2021-09-20 21:57:04.325557 gidapptools-0.5.0/gidapptools/abstract_classes/__init__.py
+-rw-r--r--   0        0        0     2098 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/abstract_classes/abstract_meta_factory.py
+-rw-r--r--   0        0        0     1324 2023-01-07 14:13:46.164752 gidapptools-0.5.0/gidapptools/abstract_classes/abstract_meta_item.py
+-rw-r--r--   0        0        0      585 2023-01-07 14:13:32.664855 gidapptools-0.5.0/gidapptools/cli_info.py
+-rw-r--r--   0        0        0       21 2024-04-25 20:13:17.822555 gidapptools-0.5.0/gidapptools/code_generation/__init__.py
+-rw-r--r--   0        0        0     5890 2024-04-25 21:29:19.094195 gidapptools-0.5.0/gidapptools/code_generation/python.py
+-rw-r--r--   0        0        0      769 2023-06-19 19:52:38.610215 gidapptools-0.5.0/gidapptools/custom_types.py
+-rw-r--r--   0        0        0       69 2022-01-12 13:50:02.703044 gidapptools-0.5.0/gidapptools/data/__init__.py
+-rw-r--r--   0        0        0     3374 2023-08-16 03:08:15.130796 gidapptools-0.5.0/gidapptools/data/conversion_data.py
+-rw-r--r--   0        0        0      126 2022-11-02 13:03:47.066458 gidapptools-0.5.0/gidapptools/data/general_data.py
+-rw-r--r--   0        0        0     1035 2022-03-20 03:11:40.597216 gidapptools-0.5.0/gidapptools/data/gifs/__init__.py
+-rw-r--r--   0        0        0    21837 2022-03-04 16:17:21.627813 gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_1.gif
+-rw-r--r--   0        0        0    28904 2022-03-04 16:31:53.112866 gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_2.gif
+-rw-r--r--   0        0        0   780846 2022-03-04 16:16:38.588118 gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_3.gif
+-rw-r--r--   0        0        0   126652 2022-03-04 16:35:31.028357 gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_4.gif
+-rw-r--r--   0        0        0    72232 2022-03-05 00:49:16.857127 gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_5.gif
+-rw-r--r--   0        0        0    77029 2022-03-05 00:49:38.490391 gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_6.gif
+-rw-r--r--   0        0        0    75110 2022-03-05 00:49:54.683726 gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_7.gif
+-rw-r--r--   0        0        0    24880 2022-03-05 00:48:39.458832 gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_cat.gif
+-rw-r--r--   0        0        0      115 2023-04-02 21:48:20.214187 gidapptools-0.5.0/gidapptools/data/json/__init__.py
+-rw-r--r--   0        0        0    23364 2023-04-13 23:13:08.036055 gidapptools-0.5.0/gidapptools/data/json/webcolors.json
+-rw-r--r--   0        0        0       80 2021-12-14 11:09:57.360075 gidapptools-0.5.0/gidapptools/data/py/__init__.py
+-rw-r--r--   0        0        0    13608 2024-05-27 23:40:41.217006 gidapptools-0.5.0/gidapptools/errors.py
+-rw-r--r--   0        0        0        0 2023-04-02 21:48:15.322224 gidapptools-0.5.0/gidapptools/general_helper/__init__.py
+-rw-r--r--   0        0        0     2949 2023-03-29 11:24:17.430146 gidapptools-0.5.0/gidapptools/general_helper/ast_helper.py
+-rw-r--r--   0        0        0      686 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/general_helper/checker.py
+-rw-r--r--   0        0        0     2607 2023-01-07 14:13:33.733996 gidapptools-0.5.0/gidapptools/general_helper/class_helper.py
+-rw-r--r--   0        0        0     1341 2023-03-25 00:28:35.426969 gidapptools-0.5.0/gidapptools/general_helper/compress.py
+-rw-r--r--   0        0        0        0 2021-11-20 18:26:05.665295 gidapptools-0.5.0/gidapptools/general_helper/concurrency/__init__.py
+-rw-r--r--   0        0        0     1197 2023-04-16 18:59:55.715194 gidapptools-0.5.0/gidapptools/general_helper/concurrency/events.py
+-rw-r--r--   0        0        0     2244 2023-06-19 19:55:25.461422 gidapptools-0.5.0/gidapptools/general_helper/concurrency/locks.py
+-rw-r--r--   0        0        0     1708 2023-01-07 14:13:33.733996 gidapptools-0.5.0/gidapptools/general_helper/concurrency/switch.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:32.741650 gidapptools-0.5.0/gidapptools/general_helper/concurrency/threadpools.py
+-rw-r--r--   0        0        0    15290 2024-05-25 23:05:36.995810 gidapptools-0.5.0/gidapptools/general_helper/conversion.py
+-rw-r--r--   0        0        0    10469 2023-09-16 19:31:46.401660 gidapptools-0.5.0/gidapptools/general_helper/date_time.py
+-rw-r--r--   0        0        0       60 2022-03-03 04:10:34.793253 gidapptools-0.5.0/gidapptools/general_helper/development/__init__.py
+-rw-r--r--   0        0        0     6454 2023-09-03 21:09:48.923621 gidapptools-0.5.0/gidapptools/general_helper/development/class_hierachy_inspect.py
+-rw-r--r--   0        0        0    11546 2023-04-02 21:27:25.104771 gidapptools-0.5.0/gidapptools/general_helper/development/inspect_helpers.py
+-rw-r--r--   0        0        0     3411 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/general_helper/development/misc.py
+-rw-r--r--   0        0        0    15131 2023-01-07 14:13:32.741650 gidapptools-0.5.0/gidapptools/general_helper/dict_helper.py
+-rw-r--r--   0        0        0     5290 2023-01-07 14:12:32.946563 gidapptools-0.5.0/gidapptools/general_helper/dispatch_table.py
+-rw-r--r--   0        0        0     2282 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/general_helper/enums.py
+-rw-r--r--   0        0        0        0 2023-03-18 16:54:11.952129 gidapptools-0.5.0/gidapptools/general_helper/font/__init__.py
+-rw-r--r--   0        0        0     7904 2023-03-25 00:44:51.605615 gidapptools-0.5.0/gidapptools/general_helper/font/font_locating.py
+-rw-r--r--   0        0        0     5995 2023-03-25 00:41:16.101915 gidapptools-0.5.0/gidapptools/general_helper/general.py
+-rw-r--r--   0        0        0     3116 2023-01-07 14:13:32.742648 gidapptools-0.5.0/gidapptools/general_helper/general_classes.py
+-rw-r--r--   0        0        0     1748 2023-06-13 19:40:27.991615 gidapptools-0.5.0/gidapptools/general_helper/hashing.py
+-rw-r--r--   0        0        0     2921 2023-06-17 04:04:12.834423 gidapptools-0.5.0/gidapptools/general_helper/import_helper.py
+-rw-r--r--   0        0        0     2828 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/general_helper/io_helper.py
+-rw-r--r--   0        0        0        0 2022-08-06 19:27:50.929033 gidapptools-0.5.0/gidapptools/general_helper/meta_helper/__init__.py
+-rw-r--r--   0        0        0     5641 2023-04-29 22:15:25.791172 gidapptools-0.5.0/gidapptools/general_helper/meta_helper/single_running_instance.py
+-rw-r--r--   0        0        0        0 2021-09-27 16:39:28.396464 gidapptools-0.5.0/gidapptools/general_helper/mixins/__init__.py
+-rw-r--r--   0        0        0     8434 2023-03-25 00:18:50.510201 gidapptools-0.5.0/gidapptools/general_helper/mixins/file_mixin.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:10:07.945114 gidapptools-0.5.0/gidapptools/general_helper/output_helper/__init__.py
+-rw-r--r--   0        0        0    10403 2024-04-27 18:44:31.954748 gidapptools-0.5.0/gidapptools/general_helper/output_helper/console_colors.py
+-rw-r--r--   0        0        0      188 2022-03-31 12:52:12.827634 gidapptools-0.5.0/gidapptools/general_helper/output_helper/rich_helper/__init__.py
+-rw-r--r--   0        0        0     4545 2023-02-15 16:01:15.425910 gidapptools-0.5.0/gidapptools/general_helper/output_helper/rich_helper/rich_helper.py
+-rw-r--r--   0        0        0      621 2023-05-24 23:00:14.061622 gidapptools-0.5.0/gidapptools/general_helper/output_helper/rich_helper/rich_styles.py
+-rw-r--r--   0        0        0     4350 2023-05-25 07:17:35.605342 gidapptools-0.5.0/gidapptools/general_helper/output_helper/rich_helper/rich_themes.py
+-rw-r--r--   0        0        0     5112 2023-04-29 21:16:12.721551 gidapptools-0.5.0/gidapptools/general_helper/path_helper.py
+-rw-r--r--   0        0        0        0 2021-10-27 16:15:21.832963 gidapptools-0.5.0/gidapptools/general_helper/regex/__init__.py
+-rw-r--r--   0        0        0     1754 2023-01-07 14:13:32.664855 gidapptools-0.5.0/gidapptools/general_helper/regex/datetime_regex.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:32.742648 gidapptools-0.5.0/gidapptools/general_helper/ressource_classes.py
+-rw-r--r--   0        0        0    16114 2023-06-13 19:16:50.176014 gidapptools-0.5.0/gidapptools/general_helper/string_helper.py
+-rw-r--r--   0        0        0     4965 2023-01-07 15:48:23.927013 gidapptools-0.5.0/gidapptools/general_helper/timing.py
+-rw-r--r--   0        0        0     1025 2023-01-07 14:13:32.665853 gidapptools-0.5.0/gidapptools/general_helper/typing_helper.py
+-rw-r--r--   0        0        0      752 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/general_helper/web_helper.py
+-rw-r--r--   0        0        0       61 2022-09-23 14:25:48.373107 gidapptools-0.5.0/gidapptools/gid_argparse/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-23 13:44:44.191704 gidapptools-0.5.0/gidapptools/gid_argparse/custom_actions/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gid_argparse/custom_actions/base_actions.py
+-rw-r--r--   0        0        0     5675 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gid_argparse/custom_parser.py
+-rw-r--r--   0        0        0      669 2022-10-08 05:04:32.804406 gidapptools-0.5.0/gidapptools/gid_config/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-23 00:22:27.273740 gidapptools-0.5.0/gidapptools/gid_config/conversion/__init__.py
+-rw-r--r--   0        0        0    13101 2024-05-27 23:40:05.042182 gidapptools-0.5.0/gidapptools/gid_config/conversion/base_converters.py
+-rw-r--r--   0        0        0     3113 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/gid_config/conversion/conversion_table.py
+-rw-r--r--   0        0        0     3083 2023-02-26 14:34:28.683848 gidapptools-0.5.0/gidapptools/gid_config/conversion/converter_grammar.py
+-rw-r--r--   0        0        0     1365 2023-01-07 14:13:32.660866 gidapptools-0.5.0/gidapptools/gid_config/conversion/extra_base_typus.py
+-rw-r--r--   0        0        0     7978 2024-05-26 17:01:31.981447 gidapptools-0.5.0/gidapptools/gid_config/conversion/spec_data.py
+-rw-r--r--   0        0        0     4895 2023-01-07 14:13:33.733996 gidapptools-0.5.0/gidapptools/gid_config/conversion/spec_item.py
+-rw-r--r--   0        0        0      613 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/gid_config/enums.py
+-rw-r--r--   0        0        0    12005 2024-05-26 17:25:49.550783 gidapptools-0.5.0/gidapptools/gid_config/interface.py
+-rw-r--r--   0        0        0        0 2021-09-23 00:22:27.273740 gidapptools-0.5.0/gidapptools/gid_config/parser/__init__.py
+-rw-r--r--   0        0        0     9761 2024-05-26 17:25:01.962688 gidapptools-0.5.0/gidapptools/gid_config/parser/config_data.py
+-rw-r--r--   0        0        0     4553 2023-01-07 14:13:32.741650 gidapptools-0.5.0/gidapptools/gid_config/parser/grammar.py
+-rw-r--r--   0        0        0     6121 2023-02-26 14:34:28.689832 gidapptools-0.5.0/gidapptools/gid_config/parser/ini_parser.py
+-rw-r--r--   0        0        0     4797 2023-02-26 14:34:28.688835 gidapptools-0.5.0/gidapptools/gid_config/parser/tokens.py
+-rw-r--r--   0        0        0        0 2022-09-23 03:58:23.085387 gidapptools-0.5.0/gidapptools/gid_database/__init__.py
+-rw-r--r--   0        0        0      145 2022-09-23 04:02:35.172766 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/__init__.py
+-rw-r--r--   0        0        0      153 2022-09-23 03:59:53.337430 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/__init__.py
+-rw-r--r--   0        0        0    14297 2023-02-15 16:01:15.473463 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/apsw_database.py
+-rw-r--r--   0        0        0     1520 2023-01-07 14:13:34.168833 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/constants.py
+-rw-r--r--   0        0        0        0 2022-09-23 10:53:55.853779 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/custom_base_models/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-23 11:29:26.257182 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/custom_fields/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-08 05:05:38.373765 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/__init__.py
+-rw-r--r--   0        0        0      670 2023-01-07 14:13:40.530819 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/commit_hook_functions.py
+-rw-r--r--   0        0        0     1071 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/profile_hook_functions.py
+-rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/rollback_hook_functions.py
+-rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/update_hook_functions.py
+-rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/wal_hook_functions.py
+-rw-r--r--   0        0        0     7754 2023-02-15 16:09:50.560537 gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/pragma_info.py
+-rw-r--r--   0        0        0      139 2023-01-03 18:51:48.004792 gidapptools-0.5.0/gidapptools/gid_image/__init__.py
+-rw-r--r--   0        0        0     3247 2023-01-07 14:13:32.626957 gidapptools-0.5.0/gidapptools/gid_image/size_manipulation.py
+-rw-r--r--   0        0        0        0 2021-11-04 00:01:05.741311 gidapptools-0.5.0/gidapptools/gid_logger/__init__.py
+-rw-r--r--   0        0        0     5368 2023-02-15 17:01:23.731015 gidapptools-0.5.0/gidapptools/gid_logger/enums.py
+-rw-r--r--   0        0        0    10633 2023-01-07 14:13:33.733996 gidapptools-0.5.0/gidapptools/gid_logger/fake_logger.py
+-rw-r--r--   0        0        0    17749 2023-07-20 21:33:22.892575 gidapptools-0.5.0/gidapptools/gid_logger/formatter.py
+-rw-r--r--   0        0        0     8175 2023-02-26 14:34:28.767869 gidapptools-0.5.0/gidapptools/gid_logger/handler.py
+-rw-r--r--   0        0        0    16292 2023-07-16 19:55:21.898252 gidapptools-0.5.0/gidapptools/gid_logger/logger.py
+-rw-r--r--   0        0        0     4177 2023-03-13 09:56:15.401301 gidapptools-0.5.0/gidapptools/gid_logger/misc.py
+-rw-r--r--   0        0        0     3697 2023-03-13 09:56:48.681021 gidapptools-0.5.0/gidapptools/gid_logger/records.py
+-rw-r--r--   0        0        0      149 2022-08-06 19:27:51.411743 gidapptools-0.5.0/gidapptools/gid_parsing/__init__.py
+-rw-r--r--   0        0        0     4219 2023-05-25 22:29:50.274352 gidapptools-0.5.0/gidapptools/gid_parsing/py_log_parsing.py
+-rw-r--r--   0        0        0        0 2022-01-15 19:38:52.874584 gidapptools-0.5.0/gidapptools/gid_parsing/tokens/__init__.py
+-rw-r--r--   0        0        0     1171 2023-01-07 14:13:32.664855 gidapptools-0.5.0/gidapptools/gid_parsing/tokens/base_tokens.py
+-rw-r--r--   0        0        0        0 2022-01-15 19:38:52.874584 gidapptools-0.5.0/gidapptools/gid_parsing/universal/__init__.py
+-rw-r--r--   0        0        0     2971 2023-01-07 14:13:32.626957 gidapptools-0.5.0/gidapptools/gid_parsing/universal/character_elements.py
+-rw-r--r--   0        0        0     4576 2023-01-07 14:13:32.741650 gidapptools-0.5.0/gidapptools/gid_parsing/universal/datetime_elements.py
+-rw-r--r--   0        0        0        0 2022-08-06 19:27:51.547380 gidapptools-0.5.0/gidapptools/gid_pytest/__init__.py
+-rw-r--r--   0        0        0      492 2023-01-07 14:13:32.665853 gidapptools-0.5.0/gidapptools/gid_pytest/parameter.py
+-rw-r--r--   0        0        0        0 2021-09-29 21:44:28.330981 gidapptools-0.5.0/gidapptools/gid_signal/__init__.py
+-rw-r--r--   0        0        0     1418 2023-01-07 14:13:33.733996 gidapptools-0.5.0/gidapptools/gid_signal/interface.py
+-rw-r--r--   0        0        0     1679 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/gid_signal/signal_registry.py
+-rw-r--r--   0        0        0        0 2021-09-29 21:44:28.330981 gidapptools-0.5.0/gidapptools/gid_signal/signals/__init__.py
+-rw-r--r--   0        0        0     3451 2023-01-07 14:13:32.626957 gidapptools-0.5.0/gidapptools/gid_signal/signals/abstract_signal.py
+-rw-r--r--   0        0        0     2345 2023-01-07 14:13:32.655879 gidapptools-0.5.0/gidapptools/gid_signal/signals/basic_signal.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:32.652887 gidapptools-0.5.0/gidapptools/gid_signal/signals/qt_signal.py
+-rw-r--r--   0        0        0       29 2022-03-11 23:29:54.398628 gidapptools-0.5.0/gidapptools/gid_utility/__init__.py
+-rw-r--r--   0        0        0     3773 2023-01-07 14:13:32.627954 gidapptools-0.5.0/gidapptools/gid_utility/version_item.py
+-rw-r--r--   0        0        0        0 2022-03-21 03:01:51.190903 gidapptools-0.5.0/gidapptools/gid_warning/__init__.py
+-rw-r--r--   0        0        0     3378 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/gid_warning/deprecation.py
+-rw-r--r--   0        0        0     1300 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/gid_warning/experimental.py
+-rw-r--r--   0        0        0      229 2022-04-18 18:34:33.321765 gidapptools-0.5.0/gidapptools/gidapptools_qt/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-18 20:52:02.729934 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/__init__.py
+-rw-r--r--   0        0        0     1249 2023-01-16 14:23:56.282011 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/images/__init__.py
+-rw-r--r--   0        0        0    32565 2023-01-16 14:18:24.219793 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/images/debugging_icon.png
+-rw-r--r--   0        0        0    12608 2022-08-18 05:21:13.655846 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/images/default_app_icon.png
+-rw-r--r--   0        0        0   134024 2021-12-11 23:04:26.441608 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/images/placeholder.png
+-rw-r--r--   0        0        0      421 2022-08-24 18:17:31.865700 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/templates/__init__.py
+-rw-r--r--   0        0        0      220 2022-08-24 18:35:31.118550 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/templates/about_stylesheet.css
+-rw-r--r--   0        0        0      598 2022-08-24 18:40:47.966025 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/templates/about_template.jinja_html
+-rw-r--r--   0        0        0      826 2022-08-24 18:14:01.808478 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/templates/arg_doc_html_template.jinja_html
+-rw-r--r--   0        0        0      218 2022-08-24 18:15:48.522228 gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/templates/arg_doc_markdown_template.jinja_md
+-rw-r--r--   0        0        0        0 2023-01-16 14:30:23.631080 gidapptools-0.5.0/gidapptools/gidapptools_qt/abc/__init__.py
+-rw-r--r--   0        0        0     5923 2023-01-16 14:32:05.111343 gidapptools-0.5.0/gidapptools/gidapptools_qt/abc/abstract_syntax_highlighting_rule.py
+-rw-r--r--   0        0        0        0 2021-11-25 19:55:33.355786 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/__init__.py
+-rw-r--r--   0        0        0    27397 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/application.py
+-rw-r--r--   0        0        0     1068 2023-01-07 14:13:34.168833 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/application_info.py
+-rw-r--r--   0        0        0     2054 2023-02-13 22:15:48.019581 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/application_new.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/command_line_parser.py
+-rw-r--r--   0        0        0     2830 2023-01-07 14:13:40.480953 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/main_window.py
+-rw-r--r--   0        0        0     5829 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/menu_bar.py
+-rw-r--r--   0        0        0     1452 2023-01-07 14:13:34.162849 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/status_bar.py
+-rw-r--r--   0        0        0     6475 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/sys_tray.py
+-rw-r--r--   0        0        0        0 2022-01-06 22:29:45.436190 gidapptools-0.5.0/gidapptools/gidapptools_qt/debug/__init__.py
+-rw-r--r--   0        0        0      723 2023-01-25 04:12:40.770472 gidapptools-0.5.0/gidapptools/gidapptools_qt/debug/debug_value_widgets/__init__.py
+-rw-r--r--   0        0        0     5143 2023-01-25 02:03:04.006135 gidapptools-0.5.0/gidapptools/gidapptools_qt/debug/debug_value_widgets/_checks.py
+-rw-r--r--   0        0        0    10979 2023-01-25 05:15:16.953587 gidapptools-0.5.0/gidapptools/gidapptools_qt/debug/debug_value_widgets/standard_types.py
+-rw-r--r--   0        0        0    19716 2023-01-25 05:04:53.017369 gidapptools-0.5.0/gidapptools/gidapptools_qt/debug/debug_widget.py
+-rw-r--r--   0        0        0     7339 2023-02-15 16:01:08.996748 gidapptools-0.5.0/gidapptools/gidapptools_qt/debug/event_analyzer.py
+-rw-r--r--   0        0        0        0 2021-12-07 00:05:58.701876 gidapptools-0.5.0/gidapptools/gidapptools_qt/dialogs/__init__.py
+-rw-r--r--   0        0        0     1791 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/dialogs/app_info_dialog.py
+-rw-r--r--   0        0        0        0 2021-12-07 22:19:08.564742 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-07 22:19:08.564742 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/command_line_parser/__init__.py
+-rw-r--r--   0        0        0     1493 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/command_line_parser/parser.py
+-rw-r--r--   0        0        0     1831 2023-03-15 23:35:57.577116 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/misc.py
+-rw-r--r--   0        0        0      747 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/object_name.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/signal_bridge.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:32:52.231212 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/syntax_highlighting/__init__.py
+-rw-r--r--   0        0        0     8783 2023-01-18 12:53:20.806844 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/syntax_highlighting/rules.py
+-rw-r--r--   0        0        0     1354 2023-10-21 23:10:32.561981 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/window_geometry_helper.py
+-rw-r--r--   0        0        0     2519 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/window_reference_keeper.py
+-rw-r--r--   0        0        0        0 2022-02-27 16:36:21.918865 gidapptools-0.5.0/gidapptools/gidapptools_qt/layouts/__init__.py
+-rw-r--r--   0        0        0     7553 2023-02-15 10:01:30.255286 gidapptools-0.5.0/gidapptools/gidapptools_qt/layouts/sorted_layout.py
+-rw-r--r--   0        0        0      823 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/layouts/vertical_form_layout.py
+-rw-r--r--   0        0        0        0 2021-12-02 11:38:53.174893 gidapptools-0.5.0/gidapptools/gidapptools_qt/models/__init__.py
+-rw-r--r--   0        0        0     1798 2023-01-10 12:47:37.778095 gidapptools-0.5.0/gidapptools/gidapptools_qt/models/basic_model.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:27.983921 gidapptools-0.5.0/gidapptools/gidapptools_qt/protocols/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-06 22:01:16.199629 gidapptools-0.5.0/gidapptools/gidapptools_qt/resources/__init__.py
+-rw-r--r--   0        0        0     1628 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/resources/placeholder.py
+-rw-r--r--   0        0        0     5394 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/resources/resources_helper.py
+-rw-r--r--   0        0        0     5126 2023-07-15 17:32:48.110111 gidapptools-0.5.0/gidapptools/gidapptools_qt/sub_typing.py
+-rw-r--r--   0        0        0        0 2021-12-02 11:32:36.936086 gidapptools-0.5.0/gidapptools/gidapptools_qt/views/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/views/basic_view.py
+-rw-r--r--   0        0        0        0 2021-12-07 00:05:58.701876 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/__init__.py
+-rw-r--r--   0        0        0    12484 2024-05-28 00:54:33.315218 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/app_log_viewer.py
+-rw-r--r--   0        0        0    10939 2023-01-24 15:57:36.849714 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/category_select_widget.py
+-rw-r--r--   0        0        0     7519 2023-03-15 23:37:04.290567 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/collapsible_widget.py
+-rw-r--r--   0        0        0     2841 2023-03-16 00:11:13.454353 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/hyperlink_label.py
+-rw-r--r--   0        0        0     3579 2023-03-31 22:17:40.477649 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/icon_text_button.py
+-rw-r--r--   0        0        0     1066 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/json_editor.py
+-rw-r--r--   0        0        0     6239 2023-07-29 00:25:52.761350 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/scrollable_widget.py
+-rw-r--r--   0        0        0     6380 2023-01-13 19:24:03.785389 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/separator_lines.py
+-rw-r--r--   0        0        0     5507 2023-07-08 12:51:52.873532 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/spinner_widget.py
+-rw-r--r--   0        0        0     6645 2023-01-07 14:13:46.165750 gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/std_stream_widget.py
+-rw-r--r--   0        0        0        0 2021-10-04 15:25:35.923246 gidapptools-0.5.0/gidapptools/gidcolor/__init__.py
+-rw-r--r--   0        0        0    10859 2023-09-12 18:49:22.065364 gidapptools-0.5.0/gidapptools/gidcolor/color.py
+-rw-r--r--   0        0        0    13948 2023-09-12 18:43:16.982322 gidapptools-0.5.0/gidapptools/gidcolor/color_item.py
+-rw-r--r--   0        0        0     6746 2023-04-28 16:48:17.765325 gidapptools-0.5.0/gidapptools/gidcolor/color_string_formatter.py
+-rw-r--r--   0        0        0     3995 2023-08-15 22:43:07.163783 gidapptools-0.5.0/gidapptools/gidcolor/coversion.py
+-rw-r--r--   0        0        0     4284 2023-05-01 20:54:30.254114 gidapptools-0.5.0/gidapptools/gidcolor/misc_calculations.py
+-rw-r--r--   0        0        0     3737 2023-01-07 14:13:32.664855 gidapptools-0.5.0/gidapptools/gidcolor/palette.py
+-rw-r--r--   0        0        0        0 2021-12-14 11:01:49.256730 gidapptools-0.5.0/gidapptools/gidcolor/preset_colors/__init__.py
+-rw-r--r--   0        0        0     1660 2023-04-02 21:57:49.861549 gidapptools-0.5.0/gidapptools/gidcolor/preset_colors/web_colors.py
+-rw-r--r--   0        0        0       96 2021-09-14 19:29:19.689941 gidapptools-0.5.0/gidapptools/meta_data/__init__.py
+-rw-r--r--   0        0        0     2816 2023-01-07 14:13:33.733996 gidapptools-0.5.0/gidapptools/meta_data/config_kwargs.py
+-rw-r--r--   0        0        0     7502 2023-01-07 14:13:32.665853 gidapptools-0.5.0/gidapptools/meta_data/interface.py
+-rw-r--r--   0        0        0       65 2021-09-19 15:57:06.694208 gidapptools-0.5.0/gidapptools/meta_data/meta_info/__init__.py
+-rw-r--r--   0        0        0     6335 2023-01-07 14:13:32.664855 gidapptools-0.5.0/gidapptools/meta_data/meta_info/meta_info_factory.py
+-rw-r--r--   0        0        0     6027 2023-06-04 19:32:02.729405 gidapptools-0.5.0/gidapptools/meta_data/meta_info/meta_info_item.py
+-rw-r--r--   0        0        0       67 2021-09-19 15:57:36.351976 gidapptools-0.5.0/gidapptools/meta_data/meta_paths/__init__.py
+-rw-r--r--   0        0        0     2420 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/meta_data/meta_paths/appdirs_implementations.py
+-rw-r--r--   0        0        0     2955 2023-01-07 14:13:32.664855 gidapptools-0.5.0/gidapptools/meta_data/meta_paths/meta_paths_factory.py
+-rw-r--r--   0        0        0     6482 2023-01-09 20:46:11.912758 gidapptools-0.5.0/gidapptools/meta_data/meta_paths/meta_paths_item.py
+-rw-r--r--   0        0        0        0 2021-09-22 03:09:38.138175 gidapptools-0.5.0/gidapptools/utility/__init__.py
+-rw-r--r--   0        0        0     3029 2023-01-07 14:13:32.664855 gidapptools-0.5.0/gidapptools/utility/enums.py
+-rw-r--r--   0        0        0     8794 2023-05-03 05:48:40.390181 gidapptools-0.5.0/gidapptools/utility/helper.py
+-rw-r--r--   0        0        0     2529 2023-01-07 14:13:33.732999 gidapptools-0.5.0/gidapptools/utility/kwarg_dict.py
+-rw-r--r--   0        0        0        0 2022-08-06 21:26:08.033946 gidapptools-0.5.0/gidapptools/vendored/__init__.py
+-rw-r--r--   0        0        0     7128 2022-11-02 13:03:50.593217 gidapptools-0.5.0/gidapptools/vendored/atomic_writes.py
+-rw-r--r--   0        0        0     1069 2022-06-30 02:44:23.800813 gidapptools-0.5.0/gidapptools/vendored/atomic_writes_LICENSE
+-rw-r--r--   0        0        0     3424 2024-05-26 17:04:20.571571 gidapptools-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 gidapptools-0.5.0/PKG-INFO
```

### Comparing `gidapptools-0.4.4/LICENSE` & `gidapptools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/__main__.py` & `gidapptools-0.5.0/gidapptools/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.cli_info import cli_show_info
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     cli_show_info()
 
-# endregion[Main_Exec]
+
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/abstract_classes/abstract_meta_factory.py` & `gidapptools-0.5.0/gidapptools/abstract_classes/abstract_meta_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 from typing import Any
 from pathlib import Path
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.meta_data.config_kwargs import ConfigKwargs
 from gidapptools.abstract_classes.abstract_meta_item import AbstractMetaItem
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class AbstractMetaFactory(ABC):
     product_class: AbstractMetaItem = None
     default_configuration: dict[str, Any] = {}
 
     def __init__(self, config_kwargs: ConfigKwargs) -> None:
@@ -69,12 +69,12 @@
         factory_instance = cls(config_kwargs=config_kwargs)
         instance = factory_instance._build()
         instance.to_storager(factory_instance.config_kwargs.get('storager'))
         factory_instance.config_kwargs.created_meta_items[factory_instance.product_name] = instance
         return instance
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/abstract_classes/abstract_meta_item.py` & `gidapptools-0.5.0/gidapptools/abstract_classes/abstract_meta_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable
 from pathlib import Path
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.string_helper import StringCaseConverter
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class AbstractMetaItem(ABC):
 
     @classmethod
     @property
     def __default_configuration__(cls) -> dict[str, Any]:
@@ -54,12 +54,12 @@
         ...
 
     @abstractmethod
     def clean_up(self, **kwargs) -> None:
         ...
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/cli_info.py` & `gidapptools-0.5.0/gidapptools/cli_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import sys
 from pathlib import Path
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def cli_show_info(argv=None):
     argv = argv or sys.argv[1:]
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     cli_show_info()
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/custom_types.py` & `gidapptools-0.5.0/gidapptools/custom_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,36 +8,37 @@
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import os
 import threading
 from typing import Union, TypeAlias
 from pathlib import Path
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 PATH_TYPE: TypeAlias = Union[str, os.PathLike[str], Path]
 
-LOCK_TYPE: TypeAlias = Union[type[threading.Lock], type[threading.RLock]]
+LOCK_TYPE: TypeAlias = Union[threading.Lock, threading.RLock]
+LOCK_CLASS_TYPE: TypeAlias = Union[type[threading.Lock], type[threading.RLock]]
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/__init__.py` & `gidapptools-0.5.0/gidapptools/data/gifs/__init__.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_1.gif` & `gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_1.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_2.gif` & `gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_2.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_3.gif` & `gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_3.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_4.gif` & `gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_4.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_5.gif` & `gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_5.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_6.gif` & `gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_6.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_7.gif` & `gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_7.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/data/gifs/busy_spinner_cat.gif` & `gidapptools-0.5.0/gidapptools/data/gifs/busy_spinner_cat.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/errors.py` & `gidapptools-0.5.0/gidapptools/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,43 +16,52 @@
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.general_helper.date_time import DateTimeFrame
     from gidapptools.gid_config.parser.config_data import ConfigData
     from gidapptools.gid_config.conversion.spec_item import SpecEntry
     from gidapptools.meta_data.meta_paths.meta_paths_item import NamedMetaPath
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
+
+
+def show_basic_error_pop_up(message: str, title: str = None) -> None:
+    from tkinter import messagebox
+    messagebox.showerror(title=title or "Error", message=message)
 
 
 class GidAppToolsBaseError(Exception):
     """
     Base Exception For GidAppTools.
     """
 
 
 class GidAppToolsFatalError(RuntimeError):
     ...
 
 
+class ConversionError(GidAppToolsBaseError):
+    ...
+
+
 class ApplicationInstanceAlreadyRunningError(GidAppToolsFatalError):
     def __init__(self, app_name: str, running_pid: int) -> None:
         self.app_name = app_name
         self.running_pid = running_pid
         os.environ["FATAL_ERROR_RAISED"] = "1"
         super().__init__(f"There is already an instance of {self.app_name!r} running with the pid of {self.running_pid!r}.")
 
@@ -214,14 +223,27 @@
     ...
 
 
 class TrailingCommentError(IniParsingError):
     ...
 
 
+class NotLoggingLevelError(GidConfigError):
+
+    def __init__(self, value, converter, section_name: str = None, entry_name: str = None, config=None) -> None:
+        self.value = value
+
+        self.converter = converter
+        self.section_name = section_name
+        self.entry_name = entry_name
+        self.config = config
+        self.msg = f"Entry {self.entry_name!r} of section {self.section_name}, of config {self.config!r} has a value ({self.value!r}) that is not a valid value of converter {self.converter!r}."
+        super().__init__(self.msg)
+
+
 class MinError(GidConfigError):
 
     def __init__(self, value, min_value, converter, section_name: str = None, entry_name: str = None, config=None) -> None:
         self.value = value
         self.min_value = min_value
         self.converter = converter
         self.section_name = section_name
@@ -355,13 +377,21 @@
 class AppNameMissingError(BaseMetaPathsError):
 
     def __init__(self) -> None:
         self.message = "The name of the App was not found in the 'kwargs_holder' or in the env ('APP_NAME')."
         super().__init__(self.message)
 
 
-# region[Main_Exec]
+class UnparsableHumanTimedelta(ConversionError):
+
+    def __init__(self, human_text: str) -> None:
+        self.human_text = human_text
+        self.message = f"Unable to parse the text {self.human_text!r} to a valid timedelta."
+        super().__init__(self.message)
+
+
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/checker.py` & `gidapptools-0.5.0/gidapptools/general_helper/checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 00000030: 6f72 7473 202d 2d2d 2d2d 2d2d 2d2d 2d2d  orts -----------
 00000040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000080: 2d3e 0d0a 6672 6f6d 2070 6174 686c 6962  ->..from pathlib
 00000090: 2069 6d70 6f72 7420 5061 7468 0d0a 0d0a   import Path....
-000000a0: 2320 656e 6472 6567 696f 6e5b 496d 706f  # endregion[Impo
-000000b0: 7274 735d 0d0a 0d0a 2320 7265 6769 6f6e  rts]....# region
-000000c0: 205b 544f 444f 5d0d 0a0d 0a0d 0a23 2065   [TODO]......# e
-000000d0: 6e64 7265 6769 6f6e 205b 544f 444f 5d0d  ndregion [TODO].
-000000e0: 0a0d 0a23 2072 6567 696f 6e20 5b4c 6f67  ...# region [Log
-000000f0: 6769 6e67 5d0d 0a0d 0a0d 0a23 2065 6e64  ging]......# end
-00000100: 7265 6769 6f6e 5b4c 6f67 6769 6e67 5d0d  region[Logging].
-00000110: 0a0d 0a23 2072 6567 696f 6e20 5b43 6f6e  ...# region [Con
-00000120: 7374 616e 7473 5d0d 0a0d 0a54 4849 535f  stants]....THIS_
-00000130: 4649 4c45 5f44 4952 203d 2050 6174 6828  FILE_DIR = Path(
-00000140: 5f5f 6669 6c65 5f5f 292e 7061 7265 6e74  __file__).parent
-00000150: 2e61 6273 6f6c 7574 6528 290d 0a0d 0a23  .absolute()....#
-00000160: 2065 6e64 7265 6769 6f6e 5b43 6f6e 7374   endregion[Const
-00000170: 616e 7473 5d0d 0a0d 0a0d 0a64 6566 2069  ants]......def i
-00000180: 735f 6861 7368 6162 6c65 286f 626a 3a20  s_hashable(obj: 
-00000190: 6f62 6a65 6374 2920 2d3e 2062 6f6f 6c3a  object) -> bool:
-000001a0: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
-000001b0: 2020 2020 6861 7368 286f 626a 290d 0a20      hash(obj).. 
-000001c0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000001d0: 7565 0d0a 2020 2020 6578 6365 7074 2054  ue..    except T
-000001e0: 7970 6545 7272 6f72 2061 7320 6572 726f  ypeError as erro
-000001f0: 723a 0d0a 2020 2020 2020 2020 6966 2027  r:..        if '
-00000200: 756e 6861 7368 6162 6c65 2720 696e 2073  unhashable' in s
-00000210: 7472 2865 7272 6f72 292e 6361 7365 666f  tr(error).casefo
-00000220: 6c64 2829 3a0d 0a20 2020 2020 2020 2020  ld():..         
-00000230: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00000240: 0a20 2020 2020 2020 2072 6169 7365 0d0a  .        raise..
-00000250: 0d0a 0d0a 2320 7265 6769 6f6e 5b4d 6169  ....# region[Mai
-00000260: 6e5f 4578 6563 5d0d 0a69 6620 5f5f 6e61  n_Exec]..if __na
-00000270: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
-00000280: 5f27 3a0d 0a20 2020 2070 6173 730d 0a0d  _':..    pass...
-00000290: 0a23 2065 6e64 7265 6769 6f6e 5b4d 6169  .# endregion[Mai
-000002a0: 6e5f 4578 6563 5d0d 0a                   n_Exec]..
+000000a0: 2320 656e 6472 6567 696f 6e20 5b49 6d70  # endregion [Imp
+000000b0: 6f72 7473 5d0d 0a0d 0a23 2072 6567 696f  orts]....# regio
+000000c0: 6e20 5b54 4f44 4f5d 0d0a 0d0a 0d0a 2320  n [TODO]......# 
+000000d0: 656e 6472 6567 696f 6e20 5b54 4f44 4f5d  endregion [TODO]
+000000e0: 0d0a 0d0a 2320 7265 6769 6f6e 205b 4c6f  ....# region [Lo
+000000f0: 6767 696e 675d 0d0a 0d0a 0d0a 2320 656e  gging]......# en
+00000100: 6472 6567 696f 6e20 5b4c 6f67 6769 6e67  dregion [Logging
+00000110: 5d0d 0a0d 0a23 2072 6567 696f 6e20 5b43  ]....# region [C
+00000120: 6f6e 7374 616e 7473 5d0d 0a0d 0a54 4849  onstants]....THI
+00000130: 535f 4649 4c45 5f44 4952 203d 2050 6174  S_FILE_DIR = Pat
+00000140: 6828 5f5f 6669 6c65 5f5f 292e 7061 7265  h(__file__).pare
+00000150: 6e74 2e61 6273 6f6c 7574 6528 290d 0a0d  nt.absolute()...
+00000160: 0a23 2065 6e64 7265 6769 6f6e 205b 436f  .# endregion [Co
+00000170: 6e73 7461 6e74 735d 0d0a 0d0a 0d0a 6465  nstants]......de
+00000180: 6620 6973 5f68 6173 6861 626c 6528 6f62  f is_hashable(ob
+00000190: 6a3a 206f 626a 6563 7429 202d 3e20 626f  j: object) -> bo
+000001a0: 6f6c 3a0d 0a20 2020 2074 7279 3a0d 0a20  ol:..    try:.. 
+000001b0: 2020 2020 2020 2068 6173 6828 6f62 6a29         hash(obj)
+000001c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000001d0: 2054 7275 650d 0a20 2020 2065 7863 6570   True..    excep
+000001e0: 7420 5479 7065 4572 726f 7220 6173 2065  t TypeError as e
+000001f0: 7272 6f72 3a0d 0a20 2020 2020 2020 2069  rror:..        i
+00000200: 6620 2775 6e68 6173 6861 626c 6527 2069  f 'unhashable' i
+00000210: 6e20 7374 7228 6572 726f 7229 2e63 6173  n str(error).cas
+00000220: 6566 6f6c 6428 293a 0d0a 2020 2020 2020  efold():..      
+00000230: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00000240: 7365 0d0a 2020 2020 2020 2020 7261 6973  se..        rais
+00000250: 650d 0a0d 0a0d 0a23 2072 6567 696f 6e20  e......# region 
+00000260: 5b4d 6169 6e5f 4578 6563 5d0d 0a69 6620  [Main_Exec]..if 
+00000270: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00000280: 6169 6e5f 5f27 3a0d 0a20 2020 2070 6173  ain__':..    pas
+00000290: 730d 0a0d 0a23 2065 6e64 7265 6769 6f6e  s....# endregion
+000002a0: 205b 4d61 696e 5f45 7865 635d 0d0a        [Main_Exec]..
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/class_helper.py` & `gidapptools-0.5.0/gidapptools/general_helper/class_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 from pathlib import Path
 from weakref import WeakSet, WeakMethod, ref
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from weakref import ReferenceType
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def ref_or_weakmethod(item, callback: Callable[["ReferenceType"], Any]) -> "ReferenceType":
     if inspect.ismethod(item):
         return WeakMethod(item, callback)
     return ref(item, callback)
 
@@ -89,12 +89,12 @@
         if obj is None:
             return self
         if self.fget is None:
             raise AttributeError(f'unreadable attribute {self._name}')
         return self.fget(obj)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/color/color.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/hyperlink_label.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,91 +3,108 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-from typing import Iterable
 from pathlib import Path
 
-# endregion[Imports]
+# * Qt Imports --------------------------------------------------------------------------------------->
+from PySide6.QtGui import QPalette, QMouseEvent, QDesktopServices
+from PySide6.QtCore import Qt, QUrl
+from PySide6.QtWidgets import QLabel, QApplication, QMainWindow, QWidget, QGridLayout, QHBoxLayout, QVBoxLayout
+from validators import url as validate_url
+import requests
+from time import perf_counter
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-class Color:
+class HyperlinkLabel(QLabel):
 
-    def __init__(self, values: Iterable[float], name: str = None) -> None:
-        self._values = tuple(values)
-        self._name = name
-        self._red: float = self._values[0]
-        self._green: float = self._values[1]
-        self._blue: float = self._values[2]
-        self._alpha: float = self._values[3]
+    def __init__(self, link: str = None, validate: bool = False, parent=None):
+        super().__init__(parent=parent)
+        self.validate = validate
+        self._link: str = None
+        if link:
+            self.set_link(link)
+        self._set_link_color()
+
+    @property
+    def link(self) -> str:
+        return self._link
+
+    def get_link(self) -> str:
+        return self._link
+
+    def get_link_as_QUrl(self) -> QUrl:
+        return QUrl(self._link)
+
+    def _validate_link(self, link: str):
+        result = validate_url(link)
+        if not result:
+            raise result
+
+    def _modify_link(self, link: str) -> str:
+        return link
+
+    def set_link(self, link: str):
+        link = self._modify_link(link)
+        if self.validate is True:
+            self._validate_link(link)
+        self._link = link
+        self.setText(link)
+        self.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+    def _set_link_color(self):
+        link_color = QApplication.instance().palette().color(QPalette.Button.Link)
+        r = link_color.red()
+        g = link_color.green()
+        b = link_color.blue()
+        self.setStyleSheet(f"color: rgb({', '.join(str(i) for i in [r,g,b])})")
+        self.setCursor(Qt.PointingHandCursor)
+
+    def _open_link(self):
+        QDesktopServices.openUrl(self._link)
+
+    def mousePressEvent(self, ev: QMouseEvent) -> None:
+        if ev.button() == Qt.LeftButton:
+            self._open_link()
+        else:
+            super().mousePressEvent(ev)
+# region [Main_Exec]
 
-    @property
-    def values(self) -> tuple[float]:
-        return self._values
-
-    @property
-    def name(self) -> str:
-        return self._name
 
-    @property
-    def red(self) -> float:
-        return self._red
-
-    @property
-    def green(self) -> float:
-        return self._green
+if __name__ == '__main__':
+    x = QApplication()
+    w = QMainWindow()
+    cont_wid = HyperlinkLabel("https://example.com/", validate=True)
 
-    @property
-    def blue(self) -> float:
-        return self._blue
+    cent_wid = QWidget()
+    cent_wid.setLayout(QVBoxLayout())
+    lab = QLabel("blah")
 
-    @property
-    def alpha(self) -> float:
-        return self._alpha
+    cent_wid.layout().addWidget(cont_wid)
 
-    def with_alpha(self, new_alpha: float, new_name: str = None) -> "Color":
-        new_values = (self.red, self.green, self.blue, new_alpha)
-        return self.__class__(new_values, name=new_name)
-
-    def with_red(self, new_red: float, new_name: str = None) -> "Color":
-        new_values = (new_red, self.green, self.blue, self.alpha)
-        return self.__class__(new_values, name=new_name)
-
-    def with_green(self, new_green: float, new_name: str = None) -> "Color":
-        new_values = (self.red, new_green, self.blue, self.alpha)
-        return self.__class__(new_values, name=new_name)
-
-    def with_blue(self, new_blue: float, new_name: str = None) -> "Color":
-        new_values = (self.red, self.green, new_blue, self.alpha)
-        return self.__class__(new_values, name=new_name)
-
-    def to_int_rgba(self) -> tuple[int]:
-        ...
-
-    def __repr__(self) -> str:
-        return f'{self.__class__.__name__}(values={self.values!r}, name={self.name!r})'
-# region[Main_Exec]
+    w.setCentralWidget(cent_wid)
+    url = cont_wid.get_link_as_QUrl()
 
+    w.show()
+    x.exec()
 
-if __name__ == '__main__':
-    pass
-
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/color/color_item.py` & `gidapptools-0.5.0/gidapptools/gidcolor/color_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,39 +14,49 @@
 from colorsys import hls_to_rgb, hsv_to_rgb, rgb_to_hls, rgb_to_hsv
 from functools import cached_property
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 import attr
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.general_helper.color.preset_colors.web_colors import get_webcolors_data
-
+from gidapptools.gidcolor.preset_colors.web_colors import _load_webcolors_data
+import numpy as np
 try:
     from PySide6.QtGui import QColor
     PYSIDE6_AVAILABLE = True
 except ImportError:
     PYSIDE6_AVAILABLE = False
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+
+from warnings import warn_explicit, warn
+from . import color
+
+warn(message=f"Submodule {__name__!r} is deprecated, please use submodule {color.__name__!r}.",
+     category=DeprecationWarning,
+     stacklevel=2)
+
+
+# endregion [Constants]
+
 
 INT_OR_FLOAT = Union[int, float]
 
 COLOR_FLOAT_TYPE = Union[tuple[float, float, float], tuple[float, float, float, float]]
 
 COLOR_INT_TYPE = Union[tuple[int, int, int], tuple[int, int, int, float]]
 
@@ -61,14 +71,27 @@
 def _alpha_converter(alpha: Union[int, float] = None) -> float:
     if alpha is None:
         return 1.0
 
     return float(alpha)
 
 
+def rgb_to_hex(r, g, b):
+    parts = []
+    for part in [r, g, b]:
+        if isinstance(part, float):
+            part = int(255 * part)
+        parts.append(part)
+    return '#' + ''.join(f"{p:X}"for p in parts)
+
+
+def rgb_float_to_rgb_int(in_rgb_float: tuple[float, float, float]) -> tuple[int, int, int]:
+    return tuple(int(255 * i) for i in in_rgb_float)
+
+
 class ColorTypus(Enum):
     RGB = auto()
     HLS = auto()
     HSV = auto()
 
 
 class BaseColor(ABC):
@@ -89,14 +112,22 @@
     def as_hls(self, include_alpha: bool = True, alpha_as_int: bool = False) -> COLOR_FLOAT_TYPE:
         ...
 
     @abstractmethod
     def as_hsv(self, include_alpha: bool = True, alpha_as_int: bool = False) -> COLOR_FLOAT_TYPE:
         ...
 
+    def as_hex(self, include_alpha: bool = True) -> str:
+        _rgb = self.as_rgb_int(include_alpha=include_alpha, alpha_as_int=True)
+        _hex = rgb_to_hex(*_rgb[:3])
+        if include_alpha is True and len(_rgb) == 4:
+            _hex += f"{_rgb[-1]:X}"
+
+        return _hex
+
     @cached_property
     def qcolor(self) -> Optional["QColor"]:
         if PYSIDE6_AVAILABLE:
             return QColor(*self.as_rgb_int(True, True))
 
     def to_q_style_rgba_string(self,) -> str:
         values = (str(i) for i in self.as_rgb_int(alpha_as_int=True))
@@ -125,14 +156,20 @@
     blue: float = attr.ib(validator=_validate_color_float, metadata={'is_core_color': True})
 
     alpha: float = attr.ib(default=1.0, converter=_alpha_converter, validator=_validate_color_float, metadata={'is_core_color': True})
 
     name: str = attr.ib(default=None)
     aliases: Iterable[str] = attr.ib(factory=set, converter=attr.converters.default_if_none(factory=set))
 
+    np_value: "np.ndarray" = attr.ib()
+
+    @np_value.default
+    def _np_value_default(self):
+        return np.asfarray(self.as_rgb_float(True, False), dtype=np.float32)
+
     def as_rgb_float(self, include_alpha: bool = True, alpha_as_int: bool = False) -> COLOR_FLOAT_TYPE:
         _out = list(self)[:-1]
         if include_alpha is True:
             if alpha_as_int is True:
                 _out.append(int(self.alpha * 255))
             else:
                 _out.append(self.alpha)
@@ -173,14 +210,20 @@
     lightness: float = attr.ib(validator=_validate_color_float, metadata={'is_core_color': True})
 
     alpha: float = attr.ib(default=1.0, converter=_alpha_converter, validator=_validate_color_float, metadata={'is_core_color': True})
 
     name: str = attr.ib(default=None)
     aliases: Iterable[str] = attr.ib(factory=set, converter=attr.converters.default_if_none(factory=set))
 
+    np_value: np.ndarray = attr.ib()
+
+    @np_value.default
+    def _np_value_default(self):
+        return np.asfarray(self.as_rgb_float(True, False), dtype=np.float32)
+
     def as_hls(self, include_alpha: bool = True, alpha_as_int: bool = False) -> COLOR_FLOAT_TYPE:
         _out = list(self)[:-1]
         if include_alpha is True:
             if alpha_as_int is True:
                 _out.append(int(self.alpha * 255))
             else:
                 _out.append(self.alpha)
@@ -220,14 +263,19 @@
     saturation: float = attr.ib(validator=_validate_color_float, metadata={'is_core_color': True})
     value: float = attr.ib(validator=_validate_color_float, metadata={'is_core_color': True})
 
     alpha: float = attr.ib(default=1.0, converter=_alpha_converter, validator=attr, metadata={'is_core_color': True})
 
     name: str = attr.ib(default=None)
     aliases: Iterable[str] = attr.ib(factory=set, converter=attr.converters.default_if_none(factory=set))
+    np_value: np.ndarray = attr.ib()
+
+    @np_value.default
+    def _np_value_default(self):
+        return np.asfarray(self.as_rgb_float(True, False), dtype=np.float32)
 
     def as_hsv(self, include_alpha: bool = True, alpha_as_int: bool = False) -> COLOR_FLOAT_TYPE:
         _out = list(self)[:-1]
         if include_alpha is True:
             if alpha_as_int is True:
                 _out.append(int(self.alpha * 255))
             else:
@@ -301,18 +349,32 @@
         self._add_color(color)
         return color
 
     def __call__(self, value: tuple, typus: ColorTypus, name: str = None, aliases: Iterable[str] = None) -> Any:
         return self.color_factory(value=value, typus=typus, name=name, aliases=aliases)
 
     def get_color_by_name(self, name: str) -> "RGBColor":
+        if len(self.colors_by_name) == 0:
+            for _p_color in _load_webcolors_data():
+                Color(**_p_color, typus=Color.color_typus.RGB)
+
         return self.colors_by_name[name.casefold()]
 
 
+xyx = []
 Color = ColorRegistry()
-for p_color in get_webcolors_data():
-    Color(**p_color, typus=Color.color_typus.RGB)
+for p_color in _load_webcolors_data():
+    xyx.append(Color.color_factory(**p_color, typus=Color.color_typus.RGB))
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
-    pass
-# endregion[Main_Exec]
+    from pympler.asizeof import asizeof
+    from gidapptools.general_helper.conversion import bytes2human
+    import inspect
+    print(f"{bytes2human(asizeof(xyx[0]))=}")
+    print(f"{bytes2human(asizeof(xyx[0].np_value))=}")
+    print(f"{xyx[0].np_value=}")
+
+    print(f"{RGBColor.f_code}")
+
+
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/color/preset_colors/web_colors.py` & `gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/profile_hook_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,50 +3,48 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-import json
-from typing import Any
+from typing import TYPE_CHECKING
 from pathlib import Path
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.data.json import THIS_FILE_DIR as JSON_DATA_DIR
+from gidapptools.general_helper.conversion import ns_to_s, number_to_pretty
 
-# endregion[Imports]
+# * Type-Checking Imports --------------------------------------------------------------------------------->
+if TYPE_CHECKING:
+    ...
+
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
-WEBCOLORS_JSON = JSON_DATA_DIR.joinpath("webcolors.json")
-# endregion[Constants]
 
+# endregion [Constants]
+
+
+def print_profile_hook(db, stmt: str, time_taken: int):
 
-def get_webcolors_data() -> list[dict[str:Any]]:
-    with WEBCOLORS_JSON.open('r', encoding='utf-8', errors='ignore') as f:
-        data = json.load(f)
-    _out = []
-    for item_data in data:
-        new_item_data = {}
-        new_item_data["name"] = item_data.get("name").casefold()
-        new_item_data["value"] = (item_data.get("rgb").get('r'), item_data.get("rgb").get('g'), item_data.get("rgb").get('b'), 1.0)
-        _out.append(new_item_data)
-    return _out
-# region[Main_Exec]
+    time_taken = ns_to_s(time_taken)
+    time_taken = number_to_pretty(time_taken) + " s"
+    print(f"Executed {stmt!r} in {time_taken}", flush=True)
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/compress.py` & `gidapptools-0.5.0/gidapptools/general_helper/compress.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,46 +12,46 @@
 from zipfile import ZIP_LZMA, ZipFile
 from multiprocessing import Process
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def compress_file(source: "PATH_TYPE", target: "PATH_TYPE", suffix: str = '.zip'):
     source = Path(source)
 
     target = Path(target)
     zip_target = target.with_suffix(suffix)
     with ZipFile(zip_target, "w", ZIP_LZMA) as zippy:
         zippy.write(source, source.name)
 
 
-def compress_in_process(source: "PATH_TYPE", target: "PATH_TYPE", suffix: str = '.zip'):
-    process = Process(daemon=False, target=compress_file, kwargs={"source": source, "target": target})
+def compress_in_process(source: "PATH_TYPE", target: "PATH_TYPE", suffix: str = '.zip') -> Process:
+    process = Process(daemon=False, target=compress_file, kwargs={"source": source, "target": target, "suffix": suffix})
     process.start()
     return process
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/concurrency/events.py` & `gidapptools-0.5.0/gidapptools/general_helper/concurrency/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,50 +7,56 @@
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from typing import Any
 from pathlib import Path
 from threading import Event
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class BlockingEvent(Event):
 
     def __init__(self) -> None:
         super().__init__()
         self.set()
 
+    def activate_blocking(self) -> None:
+        self.clear()
+
+    def clear_blocking(self) -> None:
+        self.set()
+
     def __enter__(self) -> None:
         self.clear()
 
     def __exit__(self, exception_type: type = None, exception_value: BaseException = None, traceback: Any = None) -> None:
         self.set()
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(state={self.is_set()!r})'
 
     def wait(self, timeout: float | None = None) -> bool:
         return super().wait(timeout)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/concurrency/locks.py` & `gidapptools-0.5.0/gidapptools/general_helper/concurrency/locks.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,96 +5,76 @@
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
 from threading import Lock, RLock
-
+from weakref import WeakValueDictionary
+from filelock import FileLock
 # * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.custom_types import LOCK_TYPE, PATH_TYPE
+from gidapptools.custom_types import LOCK_CLASS_TYPE, PATH_TYPE, LOCK_TYPE
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class FileLocksManager:
+    __slots__ = ("_lock_type",
+                 "_interaction_lock",
+                 "_file_locks")
 
-    def __init__(self, lock_type: LOCK_TYPE):
+    def __init__(self, lock_type: LOCK_CLASS_TYPE):
         self._lock_type = lock_type
         self._interaction_lock: Lock = Lock()
-        self._file_locks: dict[Path, LOCK_TYPE] = {}
+        self._file_locks: WeakValueDictionary[Path, LOCK_TYPE] = WeakValueDictionary()
 
     def _handle_file_path(self, file_path: PATH_TYPE) -> Path:
         return Path(file_path).resolve()
 
-    def _get_or_create(self, file_path: PATH_TYPE) -> LOCK_TYPE:
+    def _get_or_create(self, file_path: PATH_TYPE) -> LOCK_CLASS_TYPE:
         file_path = self._handle_file_path(file_path=file_path)
         with self._interaction_lock:
             try:
                 return self._file_locks[file_path]
             except KeyError:
                 file_lock = self._lock_type()
                 self._file_locks[file_path] = file_lock
                 return file_lock
 
-    def get_file_lock(self, file_path: PATH_TYPE) -> LOCK_TYPE:
+    def get_file_lock(self, file_path: PATH_TYPE) -> LOCK_CLASS_TYPE:
         return self._get_or_create(file_path=file_path)
 
-    def __getitem__(self, file_path: PATH_TYPE) -> LOCK_TYPE:
+    def __getitem__(self, file_path: PATH_TYPE) -> LOCK_CLASS_TYPE:
         return self.get_file_lock(file_path=file_path)
 
     def __len__(self) -> int:
         with self._interaction_lock:
             return len(self._file_locks)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(lock_type={self._lock_type!r})"
 
 
 GLOBAL_LOCK_MANAGER = FileLocksManager(Lock)
 GLOBAL_RLOCK_MANAGER = FileLocksManager(RLock)
 
 
-class PathSpecificLock:
-    _selection_lock = Lock()
-    _lock_registry: dict[Path, "PathSpecificLock"] = {}
-
-    def __new__(cls, path: Path) -> Lock:
-        with cls._selection_lock:
-            if path not in cls._lock_registry:
-                cls._lock_registry[path] = Lock()
-
-            return cls._lock_registry[path]
-
-
-class PathSpecificRLock:
-    _selection_lock = Lock()
-    _lock_registry: dict[Path, "PathSpecificLock"] = {}
-
-    def __new__(cls, path: Path) -> RLock:
-        with cls._selection_lock:
-            if path not in cls._lock_registry:
-                cls._lock_registry[path] = RLock()
-
-            return cls._lock_registry[path]
-
-
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/concurrency/switch.py` & `gidapptools-0.5.0/gidapptools/general_helper/concurrency/switch.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,31 +16,31 @@
     pass
 else:
     pass
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     ...
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class Switch:
     __slots__ = ("_lock", "_state")
 
     def __init__(self, initial_state: bool = False) -> None:
         self._lock = RLock()
@@ -72,15 +72,15 @@
 
     def __bool__(self) -> bool:
         return self.state
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(value={self.state!r})"
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/conversion.py` & `gidapptools-0.5.0/gidapptools/general_helper/conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,47 +5,46 @@
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import re
 from enum import Flag, auto
-from typing import Any, Union, Iterable
+from typing import Any, Union, Iterable, Literal, TypeVar
 from pathlib import Path
 from datetime import timedelta
 from operator import neg, or_, pos
 from functools import reduce, total_ordering, cached_property
 from collections import defaultdict
-
+from pprint import pprint
 # * Third Party Imports --------------------------------------------------------------------------------->
-import attr
 import pyparsing as pp
 import pyparsing.common as ppc
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.errors import FlagConflictError
-from gidapptools.data.conversion_data import RAW_TIMEUNITS, STRING_TRUE_VALUES, STRING_FALSE_VALUES, FILE_SIZE_SYMBOL_DATA, NANOSECONDS_IN_SECOND
+from gidapptools.errors import FlagConflictError, UnparsableHumanTimedelta
+from gidapptools.data.conversion_data import TimeUnit, TIMEUNITS, TIMEUNIT_NAME_MAP, STRING_TRUE_VALUES, STRING_FALSE_VALUES, FILE_SIZE_SYMBOL_DATA, NANOSECONDS_IN_SECOND, MICROSECONDS_IN_SECOND
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 @total_ordering
 class FileSizeUnit:
     __slots__ = ("_short_name", "_long_name", "factor", "aliases", "all_names", "all_names_casefolded")
 
     def __init__(self, short_name: str, long_name: str, factor: int, aliases: Iterable[str] = None) -> None:
@@ -173,40 +172,39 @@
 
 
 FILE_SIZE_REFERENCE = FileSizeReference()
 
 
 def bytes2human(n: int) -> str:
     # http://code.activestate.com/recipes/578019
-    # >>> bytes2human(10000)
-    # '9.8K'
-    # >>> bytes2human(100001221)
-    # '95.4M'
-    # if annotate is not None:
-
-    # symbols = ('Kb', 'Mb', 'Gb', 'Tb', 'Pb', 'Eb', 'Zb', 'Yb')
-    # prefix = {s: 1 << (i + 1) * 10 for i, s in enumerate(symbols)}
 
+    is_negative = n < 0
+    sign_prefix = ""
+    if is_negative:
+        n = n * (-1)
+        sign_prefix = "-"
     for unit in reversed(FILE_SIZE_REFERENCE.units):
         if n >= unit:
             _out = float(n) / unit
 
-            _out = f'{_out:.1f} {unit}'
+            _out = f'{sign_prefix}{_out:.2f} {unit}'
             return _out
     _out = n
 
-    return f"{_out} b"
+    return f"{sign_prefix}{_out} b"
 
 
 def human2bytes(in_text: str, strict: bool = False) -> int:
+
     def _clean_name(name: str) -> str:
         name = name.strip()
         name = name.casefold()
         name = white_space_regex.sub(' ', name)
         return name
+
     if in_text.strip() == "0" and strict is False:
         return ""
     white_space_regex = re.compile(r"\s{2,}")
     number_regex_pattern = r"(?P<number>[\d\.\,]+)"
     name_regex_pattern = r"(?P<name>\w([\w\s]+)?)"
     parse_regex = re.compile(number_regex_pattern + r'\s*' + name_regex_pattern)
 
@@ -216,97 +214,99 @@
         name = _clean_name(match.group('name'))
         unit = FILE_SIZE_REFERENCE.get_unit_by_name(name)
         return int(number * unit.factor)
     else:
         raise ValueError(f"Unable to parse input string {in_text!r}.")
 
 
-def ns_to_s(nano_seconds: int, decimal_places: int = None) -> Union[int, float]:
+def ns_to_s(nano_seconds: Union[int, float], decimal_places: int = None) -> Union[int, float]:
     seconds = nano_seconds / NANOSECONDS_IN_SECOND
     if decimal_places is None:
         return seconds
     return round(seconds, decimal_places)
 
 
-@attr.s(auto_attribs=True, auto_detect=True, frozen=True, slots=True, weakref_slot=True)
-class TimeUnit:
-    name: str = attr.ib()
-    symbol: str = attr.ib()
-    factor: int = attr.ib()
-    aliases: tuple[str] = attr.ib(converter=tuple)
-    plural: str = attr.ib()
-
-    @plural.default
-    def default_plural(self):
-        return self.name + "s"
-
-    def convert_seconds(self, in_seconds: int) -> int:
-        return in_seconds / self.factor
-
-    def convert_with_rest(self, in_seconds: int) -> tuple[int, int]:
-        _amount, _rest = divmod(in_seconds, self.factor)
-
-        return int(_amount), _rest
-
-    def value_to_string(self, in_value: int, use_symbols: bool = False) -> str:
-        if use_symbols is True:
-            return f"{in_value}{self.symbol}"
-        if in_value == 1:
-            return f"{in_value} {self.name}"
-        return f"{in_value} {self.plural}"
-
-
-TIMEUNITS = sorted([TimeUnit(*item) for item in RAW_TIMEUNITS], key=lambda x: x.factor, reverse=True)
+def ms_to_s(micro_seconds: Union[int, float], decimal_places: int = None) -> Union[int, float]:
+    seconds = micro_seconds / MICROSECONDS_IN_SECOND
+    if decimal_places is None:
+        return seconds
+    return round(seconds, decimal_places)
 
 
 class TimeUnits:
+    __slots__ = ("_with_year",
+                 "units",
+                 "name_dict",
+                 "symbol_dict",
+                 "alias_dict",
+                 "full_dict")
 
     def __init__(self, with_year: bool = True) -> None:
-        self._units = sorted(TIMEUNITS.copy(), key=lambda x: -x.factor)
         self._with_year = with_year
         self.units = self._get_units()
         self.name_dict: dict[str, TimeUnit] = {item.name.casefold(): item for item in self.units} | {item.plural.casefold(): item for item in self.units}
         self.symbol_dict: dict[str, TimeUnit] = {item.symbol.casefold(): item for item in self.units}
         self.alias_dict: dict[str, TimeUnit] = self._get_alias_dict()
         self.full_dict: dict[str, TimeUnit] = self.name_dict | self.symbol_dict | self.alias_dict
 
-    @cached_property
+    @property
     def smallest_unit(self) -> TimeUnit:
         return self.units[-1]
 
     def _get_units(self):
+        _all_units = sorted(TIMEUNITS.copy(), key=lambda x: -x.factor)
         if self._with_year is False:
-            return [u for u in self._units.copy() if u.name != 'year']
-        return self._units.copy()
+            return [u for u in _all_units if u.name != 'year']
+        return _all_units
 
     def _get_alias_dict(self) -> dict[str, TimeUnit]:
         _out = {}
         for item in self.units:
             for alias in item.aliases:
                 _out[alias] = item
                 _out[alias.casefold()] = item
         return _out
 
     def __getitem__(self, key: Union[int, str]) -> TimeUnit:
         if isinstance(key, int):
             return self.units[key]
 
+        if isinstance(key, str):
+            return self.full_dict[key.casefold()]
+
         return self.full_dict[key]
 
     def __iter__(self):
         return iter(self.units)
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(with_year={self._with_year!r})'
 
 
 _time_units_without_year = TimeUnits(False)
 _time_units_with_year = TimeUnits(True)
 
 
+def timedelta_to_stopwatch_format(t: Union[float, timedelta]) -> str:
+    """
+    Get a friendly timestamp represented as a string.
+    """
+    try:
+        all_seconds = t.total_seconds()
+    except AttributeError:
+        all_seconds = t
+
+    hour_unit = TIMEUNIT_NAME_MAP["hour"]
+    minute_unit = TIMEUNIT_NAME_MAP["minute"]
+    second_unit = TIMEUNIT_NAME_MAP["second"]
+
+    hours, minutes, seconds = hour_unit.convert_seconds(all_seconds), minute_unit.convert_seconds(all_seconds) % int(hour_unit.factor / minute_unit.factor), all_seconds % int(minute_unit.factor / second_unit.factor)
+    return f"{hours:02d}:{minutes:02d}:{seconds:05.2f}"
+
+
 def seconds2human(in_seconds: Union[int, float, timedelta],
                   as_list_result: bool = False,
                   as_dict_result: bool = False,
                   as_symbols: bool = False,
                   with_year: bool = True,
                   min_unit: str = None) -> Union[dict[TimeUnit, int], str]:
     if as_list_result is True and as_dict_result is True:
@@ -331,15 +331,15 @@
         if amount:
             result[unit] = int(amount)
 
     results = [k.value_to_string(v, as_symbols) for k, v in result.items() if k not in sub_min_units]
     if as_list_result is True:
         return results
     if as_dict_result is True:
-        return{k: v for k, v in result.items() if k not in sub_min_units}
+        return {k: v for k, v in result.items() if k not in sub_min_units}
 
     if not results:
         _unit = _time_units.smallest_unit if min_unit is None else min_unit
         _name = f" {_unit.plural}" if as_symbols is False else _unit.symbol
         return f"0{_name}"
     if len(results) > 1:
         return sign + ' '.join(results[:-1]) + ' and ' + results[-1]
@@ -399,30 +399,35 @@
 
     return pp.ZeroOrMore(prefixes)("prefix") + pp.OneOrMore(time_item + pp.Optional(combine_words))('time_data').set_parse_action(_time_data_action) + pp.ZeroOrMore(postfixes)("postfix")
 
 
 TIMEDELTA_PARSING_GRAMMAR = get_timedelta_parsing_grammar()
 
 
-def human2timedelta(in_text: str, default: Any = timedelta()) -> timedelta:
+def human2timedelta(in_text: str) -> timedelta:
+
     try:
         tokens = TIMEDELTA_PARSING_GRAMMAR.parse_string(in_text, parse_all=True).as_dict()
-    except pp.ParseBaseException:
-        return default
+    except pp.ParseBaseException as e:
+        raise UnparsableHumanTimedelta(in_text) from e
     _raw_modifier_data = tokens.get("prefix") + tokens.get('postfix')
     if _raw_modifier_data == []:
         _raw_modifier_data = [TimedeltaConversionModifiers.POSITIVE]
     modifiers = reduce(or_, {i for i in _raw_modifier_data if i})
 
     raw_timedelta_kwargs = {k.plural: v for k, v in tokens.get('time_data').items() if v}
 
     raw_timedelta = timedelta(**raw_timedelta_kwargs)
     return modifiers.sign(raw_timedelta)
 
 
+def human2seconds(in_text: str) -> float:
+    return human2timedelta(in_text=in_text).total_seconds()
+
+
 def str_to_bool(in_string: str, strict: bool = False) -> bool:
     if isinstance(in_string, bool):
         return in_string
     mod_string = in_string.casefold().strip()
     if strict is False:
         return mod_string in STRING_TRUE_VALUES
 
@@ -431,16 +436,18 @@
     if mod_string in STRING_FALSE_VALUES:
         return False
 
     raise TypeError(f'Unable to convert string {in_string!r} to a Boolean value.')
 
 
 def number_to_pretty(in_num: Union[int, float]) -> str:
+
     return f"{in_num:,}"
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
-    pass
+    import shutil
 
-# endregion[Main_Exec]
+    print(shutil.which("firefox"))
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/date_time.py` & `gidapptools-0.5.0/gidapptools/gid_parsing/py_log_parsing.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,145 +3,117 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-from enum import Enum
 from pathlib import Path
-from datetime import datetime, timezone, timedelta
-from functools import total_ordering
 
 # * Third Party Imports --------------------------------------------------------------------------------->
-import attr
+import pyparsing as ppa
+import pyparsing.common as ppc
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.errors import DateTimeFrameTimezoneError, NotUtcDatetimeError
+from gidapptools.gid_parsing.tokens.base_tokens import BaseTokenWithPos
+from gidapptools.gid_parsing.universal.datetime_elements import get_grammar_from_dt_format
+from gidapptools.gid_parsing.universal.character_elements import Ligatures, BaseElements
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-# def seconds2human()
+class LineNumberToken(BaseTokenWithPos):
 
+    def __init__(self, start: int, end: int, value: int) -> None:
+        super().__init__(start, end)
+        self.line_number = value
 
-class DatetimeFmt(str, Enum):
-    STANDARD = "%Y-%m-%d %H:%M:%S"
-    FILE = "%Y-%m-%d_%H-%M-%S"
-    LOCAL = "%x %X"
 
-    STANDARD_TZ = "%Y-%m-%d %H:%M:%S %Z"
-    FILE_TZ = "%Y-%m-%d_%H-%M-%S_%Z"
-    LOCAL_TZ = "%x %X %Z"
+class LogLevelToken(BaseTokenWithPos):
 
-    def strf(self, date_time: datetime) -> str:
-        non_tz_fmt = self if not self.name.endswith('_TZ') else getattr(self, self.name.removesuffix('_TZ'))
-        tz_fmt = self if self.name.endswith('_TZ') else getattr(self, self.name + '_TZ')
-        if date_time.tzinfo is None:
-            return date_time.strftime(non_tz_fmt)
-        return date_time.strftime(tz_fmt)
+    def __init__(self, start: int, end: int, value: str) -> None:
+        super().__init__(start, end)
+        self.log_level = value
 
 
-def get_aware_now(tz: timezone) -> datetime:
-    return datetime.now(tz=tz)
+class ThreadNameToken(BaseTokenWithPos):
 
+    def __init__(self, start: int, end: int, value: str) -> None:
+        super().__init__(start, end)
+        self.thread_name = value
 
-def get_utc_now() -> datetime:
-    return get_aware_now(tz=timezone.utc)
 
+class ModuleNameToken(BaseTokenWithPos):
 
-def _validate_date_time_frame_tzinfo(instance: "DateTimeFrame", attribute: attr.Attribute, value: datetime):
-    if instance.start.tzinfo is None or instance.end.tzinfo is None:
-        raise DateTimeFrameTimezoneError(instance, instance.start.tzinfo, instance.end.tzinfo, 'start time and end time need to be timezone aware')
-    if instance.start.tzinfo != instance.end.tzinfo:
-        raise DateTimeFrameTimezoneError(instance, instance.start.tzinfo, instance.end.tzinfo, 'start time and end time do not have the same timezone')
+    def __init__(self, start: int, end: int, value: str) -> None:
+        super().__init__(start, end)
+        self.module_name = value
+        self.module_name_parts = tuple(self.module_name.split('.'))
 
+    @property
+    def parent_module_name(self) -> str:
+        try:
+            return self.module_name_parts[-2]
+        except IndexError:
+            return "__main__"
 
-@attr.s(auto_attribs=True, auto_detect=True, frozen=True, slots=True)
-@total_ordering
-class DateTimeFrame:
-    start: datetime = attr.ib(validator=_validate_date_time_frame_tzinfo)
-    end: datetime = attr.ib(validator=_validate_date_time_frame_tzinfo)
 
-    @property
-    def delta(self) -> timedelta:
-        return self.end - self.start
+class FunctionNameToken(BaseTokenWithPos):
 
-    @property
-    def tzinfo(self) -> timezone:
-        return self.start.tzinfo
+    def __init__(self, start: int, end: int, value: str) -> None:
+        super().__init__(start, end)
+        self.function_name = value
 
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, datetime):
-            return self.start <= other <= self.end
-        if isinstance(other, self.__class__):
-            return self.start == other.start and self.end == other.end
-        if isinstance(other, timedelta):
-            return self.delta == other
-        return NotImplemented
-
-    def __lt__(self, other: object) -> bool:
-        if isinstance(other, datetime):
-            return self.start < other
-        if isinstance(other, self.__class__):
-            return self.end < other.start
-        if isinstance(other, timedelta):
-            return self.delta < other
-        return NotImplemented
-
-    def __contains__(self, other: object) -> bool:
-        if isinstance(other, datetime):
-            return self.start <= other <= self.end
-        return NotImplemented
-
-    def __str__(self) -> str:
-        return f"{self.start.isoformat(sep=' ')} until {self.end.isoformat(sep=' ')}"
-
-    def __hash__(self) -> int:
-        return hash(self.start) + hash(self.end) + hash(self.delta)
-
-
-ZERO_TIMEDELTA = timedelta()
-
-
-def calculate_utc_offset(utc_datetime: datetime, local_datetime: datetime, offset_class: type[timezone] = timezone):
-    if utc_datetime.tzinfo.tzname(None) != "UTC" and utc_datetime.tzinfo != timezone.utc and utc_datetime.tzinfo.utcoffset(None) != ZERO_TIMEDELTA:
-        raise NotUtcDatetimeError(utc_datetime)
-    difference_seconds = (local_datetime.replace(tzinfo=timezone.utc) - utc_datetime)
-
-    difference_seconds = difference_seconds.total_seconds()
-    offset_timedelta = timedelta(seconds=int(difference_seconds))
-    offset_hours = offset_timedelta.total_seconds() / (60 * 60)
 
-    offset_hours = int(offset_hours)
-    prefix = "" if offset_hours < 0 else "+"
+class MessageToken(BaseTokenWithPos):
 
-    name = prefix + str(offset_hours)
-    return offset_class(offset=offset_timedelta, name=name)
+    def __init__(self, start: int, end: int, value: str) -> None:
+        super().__init__(start, end)
+        self.message = value
 
-# region[Main_Exec]
 
+class GeneralGrammar:
+    _cached_grammar: ppa.ParserElement = None
 
-if __name__ == '__main__':
-    from tzlocal import get_localzone
-    from dateutil.tz import UTC
-    x = calculate_utc_offset(datetime.now(tz=UTC), datetime.now())
-    print(x)
+    @property
+    def ___grammar___(self) -> ppa.ParserElement:
+        if self._cached_grammar is None:
+            self.__class__._cached_grammar = self._construct_grammar()
+        return self._cached_grammar
+
+    def _construct_grammar(self):
+        non_pipe_printables = ppa.printables.replace("|", "")
+        time_stamp_part = get_grammar_from_dt_format("%Y-%m-%d %H:%M:%S.%f %Z")("time_stamp")
+        line_number_part = ppa.locatedExpr(ppa.Word(ppa.nums).set_parse_action(ppc.convert_to_integer)).set_parse_action(LineNumberToken.from_parse_action)("line_number")
+        level_part = ppa.locatedExpr(ppa.Keyword("DEBUG") | ppa.Keyword("INFO") | ppa.Keyword("CRITICAL") | ppa.Keyword("ERROR")).set_parse_action(LogLevelToken.from_parse_action)("level")
+        thread_name_part = ppa.locatedExpr(ppa.Word(non_pipe_printables)("thread")).set_parse_action(ThreadNameToken.from_parse_action)("thread")
+        module_name_part = ppa.locatedExpr(ppa.Word(non_pipe_printables)).set_parse_action(ModuleNameToken.from_parse_action)("module")
+        function_name_part = ppa.locatedExpr(ppa.Word(non_pipe_printables)).set_parse_action(FunctionNameToken.from_parse_action)("function")
+        return time_stamp_part + BaseElements.pipe + line_number_part + BaseElements.pipe + level_part + BaseElements.pipe + thread_name_part + BaseElements.pipe + \
+            module_name_part + BaseElements.pipe + function_name_part + BaseElements.pipe + BaseElements.pipe + Ligatures.big_arrow_right + ppa.locatedExpr(ppa.rest_of_line).set_parse_action(MessageToken.from_parse_action)("message")
 
+    def __call__(self, text: str) -> dict[str, BaseTokenWithPos]:
+        return self.___grammar___.parse_string(text, parse_all=True).as_dict()
 
-# endregion[Main_Exec]
+
+# region [Main_Exec]
+
+
+if __name__ == '__main__':
+    pass
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/development/inspect_helpers.py` & `gidapptools-0.5.0/gidapptools/general_helper/development/inspect_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,31 +28,31 @@
     import isort
 try:
     from rich.console import Console as RichConsole
     RICH_IMPORTABLE = True
 except ImportError:
     RICH_IMPORTABLE = False
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class ClassNameFinder(ast.NodeVisitor):
 
     def __init__(self) -> None:
         super().__init__()
         self.class_names: list[str] = []
@@ -128,16 +128,20 @@
     def import_string(self) -> str:
         import_path = self.qualname.rsplit('.', 1)[0]
         return f"from {import_path} import {self.name}"
 
     @property
     def all_members_import_string(self) -> str:
         text = f"from {self.qualname} import ({', '.join(self.member_names)})"
+        try:
+            return isort.code(text, line_length=200).strip()
+        except Exception as e:
+            print(f"Encountered exception {e!r}")
 
-        return isort.code(text, line_length=200).strip()
+            return text.strip()
 
     @property
     def member_names(self) -> tuple[str]:
 
         def _check(_name: str, _obj: object) -> bool:
             return not any([
                 getattr(_obj, "__module__", None) != self.module.__name__,
@@ -335,16 +339,17 @@
 
     if no_rich is True or RICH_IMPORTABLE is False:
         from pprint import pprint
         pprint(get_all_sub_module_data(in_module=in_module))
         return
 
     console = RichConsole(soft_wrap=True)
-    console.print(get_all_sub_module_data(in_module))
+    console.print_json(data=get_all_sub_module_data(in_module), default=str)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     from PySide6 import QtWidgets
-    print_all_sub_module_data(QtWidgets)
+    import importlib.resources
+    print_all_sub_module_data(importlib.resources)
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/development/misc.py` & `gidapptools-0.5.0/gidapptools/general_helper/development/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 from gidapptools.errors import MissingOptionalDependencyError
 
 with MissingOptionalDependencyError.try_import("gidapptools"):
     from rich import inspect as rinspect
     from rich import terminal_theme
     from rich.console import Console as RichConsole
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def make_dprint(**console_kwargs) -> Callable:
     use_seperator: bool = console_kwargs.pop('use_seperator', True)
     seperator_char: str = console_kwargs.pop('seperator_char', '-')
     use_print_count: bool = console_kwargs.pop('use_print_count', True)
 
@@ -99,13 +99,13 @@
         console.save_text(out_file)
 
 
 def is_dunder_name(in_name: str) -> bool:
     return in_name.startswith("__") and in_name.endswith("__")
 
 
-    # region[Main_Exec]
+    # region [Main_Exec]
 if __name__ == '__main__':
     from PySide6.QtWidgets import QMenu
     obj_inspection(QMenu)
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/dict_helper.py` & `gidapptools-0.5.0/gidapptools/general_helper/dict_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 from collections import UserDict, namedtuple
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import KeyPathError, NotMappingError, AdvancedDictError, DictMergeConflict
 from gidapptools.general_helper.enums import MiscEnum
 from gidapptools.general_helper.checker import is_hashable
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def replace_dict_keys(in_dict: dict, *replacement_pairs: tuple[Hashable, Hashable]) -> dict:
     # replacement_table = {item[0]: item[1] for item in replacement_pairs}
     # return in_dict.__class__(**{replacement_table.get(k, k): v for k, v in in_dict.items()})
 
     for old_key, new_key in replacement_pairs:
@@ -390,11 +390,11 @@
         if isinstance(other, UserDict):
             self.data = self.safe_merge(self.data, other.data)
         else:
             self.data = self.safe_merge(self.data, other)
         return self
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/dispatch_table.py` & `gidapptools-0.5.0/gidapptools/general_helper/dispatch_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 import inspect
 from typing import Union, Mapping, Callable, Hashable, Iterable
 from pathlib import Path
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.enums import MiscEnum
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class dispatch_mark:
     """
     Marks a method as a dispatch function for an instance `BaseDispatchTable`.
     """
     key_attribute_name: str = '_dispatch_key'
@@ -135,13 +135,13 @@
     def get(self, key: Hashable, default=MiscEnum.NOTHING) -> Callable:
         try:
             return self[key]
         except KeyError:
             return self.default_dispatch if default is MiscEnum.NOTHING else default
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/enums.py` & `gidapptools-0.5.0/gidapptools/general_helper/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from enum import Enum, auto, unique
 from pathlib import Path
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.utility.enums import BaseGidEnum
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 @unique
 class MiscEnum(Enum):
     NOTHING = auto()
     ALL = auto()
     DEFAULT = auto()
@@ -104,11 +104,11 @@
 
     # aliases
     CMD = BAT
     YML = YAML
     JPG = JPEG
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/general.py` & `gidapptools-0.5.0/gidapptools/general_helper/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 import sys
 import random
 from typing import Any, Union, TypeVar, Callable, Hashable, Iterable, Optional, Generator
 from logging import Logger
 from pathlib import Path
 from itertools import tee, filterfalse
 
+
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.enums import MiscEnum
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 T = TypeVar("T")
 _DEFAULT_TYPE = TypeVar("_DEFAULT_TYPE", object, None)
 
 
 def defaultable_list_pop(in_list: Optional[list[T]], idx: int, default: _DEFAULT_TYPE = None) -> Union[T, _DEFAULT_TYPE]:
     if in_list is None:
@@ -120,16 +121,16 @@
     return default
 
 
 def is_frozen() -> bool:
     return getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS')
 
 
-def get_all_available_loggers(logger: Logger) -> tuple[str]:
-    manager = logger.manager
+def get_all_available_loggers(logger: Logger = None) -> tuple[str]:
+    manager = logger.manager if logger is not None else Logger.manager
     names = set(manager.loggerDict)
     return tuple(sorted(names, key=len))
 
 
 T = TypeVar("T")
 
 
@@ -146,25 +147,26 @@
         if len(collected) == group_size:
             yield tuple(collected)
             collected.clear()
 
     if len(collected) != 0:
         yield tuple(collected)
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
-    from gidapptools.general_helper.timing import time_execution
-
-    def checker(in_num: int) -> bool:
-        return len(in_num) == 2
+    # from gidapptools.general_helper.timing import time_execution
 
-    t = [str(random.randint(0, 1_000)) for _ in range(10_000)]
+    # def checker(in_num: int) -> bool:
+    #     return len(in_num) == 2
 
-    with time_execution(also_pretty=True):
-        a, b = split_iter(t, checker, Generator)
-        for xx in a:
-            print(xx)
+    # t = [str(random.randint(0, 1_000)) for _ in range(10_000)]
 
+    # with time_execution(also_pretty=True):
+    #     a, b = split_iter(t, checker, Generator)
+    #     for xx in a:
+    #         print(xx)
+    for l in get_all_available_loggers():
+        print(l)
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/general_classes.py` & `gidapptools-0.5.0/gidapptools/general_helper/general_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Type, TypeVar, Callable
 from pathlib import Path
 from threading import Lock
 from contextlib import contextmanager
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 log = logging.getLogger(__name__)
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class AbstractThreadsafePool(ABC):
     __slots__ = ("_lock", "_max_size", "_prefill", "_objects", "_queue")
 
     def __init__(self, max_size: int = None, prefill: bool = False) -> None:
         self._lock = Lock()
@@ -111,12 +111,12 @@
 class DecorateAbleList(list[T]):
 
     def __call__(self, item: T) -> T:
         super().append(item)
         return item
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/hashing.py` & `gidapptools-0.5.0/gidapptools/general_helper/hashing.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,58 +10,59 @@
 from typing import TYPE_CHECKING, Callable
 from hashlib import sha1, blake2b
 from pathlib import Path
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
+    from hashlib import _Hash
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 # FILE_HASH_INCREMENTAL_THRESHOLD: int = 104857600  # 100mb
 FILE_HASH_INCREMENTAL_THRESHOLD: int = 52428800  # 50mb
 
 
-def file_hash(in_file: "PATH_TYPE", hash_algo: Callable = blake2b) -> str:
-    in_file = Path(in_file)
-    if not in_file.is_file():
-        raise OSError(f"The path {in_file.as_posix()!r} either does not exist or is a Folder.")
+def _actual_hash_file(in_file: Path, hash_algo: Callable = blake2b) -> "_Hash":
     if in_file.stat().st_size > FILE_HASH_INCREMENTAL_THRESHOLD:
         _hash = hash_algo(usedforsecurity=False)
         with in_file.open("rb", buffering=FILE_HASH_INCREMENTAL_THRESHOLD // 4) as f:
             for chunk in f:
                 _hash.update(chunk)
-        return _hash.hexdigest()
+        return _hash
 
-    return hash_algo(in_file.read_bytes(), usedforsecurity=False).hexdigest()
+    return hash_algo(in_file.read_bytes(), usedforsecurity=False)
+
+
+def file_hash(in_file: "PATH_TYPE", hash_algo: Callable = blake2b) -> str:
+    in_file = Path(in_file)
+    if not in_file.is_file():
+        raise OSError(f"The path {in_file.as_posix()!r} either does not exist or is a Folder.")
+    return _actual_hash_file(in_file=in_file, hash_algo=hash_algo).hexdigest()
 
 
 def hash_to_int(in_hash: str) -> int:
     return int(in_hash, base=16)
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
-    x = b"aaaaaaaaakdkdkdkdkkd"
-    y = sha1(x).hexdigest()
-    z = hash_to_int(y)
-    print(z)
-
-# endregion[Main_Exec]
+    pass
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/import_helper.py` & `gidapptools-0.5.0/gidapptools/general_helper/import_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,39 +6,47 @@
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import sys
 import pkgutil
 import importlib
+import os
 import importlib.util
 import importlib.metadata
 from types import ModuleType
 from pathlib import Path
+from typing import Union, Iterable, Mapping
+
+
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.utility.helper import PackageMetadataDict
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def is_importable(package_name: str) -> bool:
     """
     Checks if the package is importable, without actually trying to import it.
 
     :param package_name: Name of the Package to check, is case-sensitive
@@ -55,26 +63,43 @@
 
 
 def import_from_name(name: str) -> ModuleType:
     module = importlib.import_module(name)
     return module
 
 
+def import_from_file_path(file_path: Union[str, os.PathLike, Path],
+                          add_to_global_modules: bool = False) -> ModuleType:
+    file_path = Path(file_path).resolve()
+    _name = file_path.stem
+    spec = importlib.util.spec_from_file_location(_name, file_path)
+    _module = importlib.util.module_from_spec(spec)
+
+    if add_to_global_modules is True:
+        sys.modules[_name] = _module
+
+    spec.loader.exec_module(_module)
+
+    return _module
+
+
 def all_importable_package_names(exclude_underscored: bool = True, exclude_std_lib: bool = False, exclude_main: bool = True) -> tuple[str]:
 
     def _check_exclude(in_name: str) -> bool:
         if exclude_underscored is True and in_name.startswith("_"):
             return False
         if exclude_std_lib is True and in_name in sys.stdlib_module_names:
             return False
         if exclude_main is True and in_name == "__main__":
             return False
         return True
 
     return tuple(sorted([i.name for i in pkgutil.iter_modules() if _check_exclude(i.name)], key=lambda x: x.casefold()))
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
-    pass
-# endregion[Main_Exec]
+    for x in all_importable_package_names():
+        if "css" in x.casefold():
+            print(x)
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/io_helper.py` & `gidapptools-0.5.0/gidapptools/general_helper/io_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 import os
 from typing import Union
 from pathlib import Path
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.custom_types import PATH_TYPE
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def amount_lines_in_file(in_file: PATH_TYPE):
     in_file = Path(in_file)
     if in_file.is_file() is False:
         raise FileNotFoundError(f"The path {in_file.as_posix()!r} is not a file.")
     with in_file.open("r", encoding='utf-8', errors='ignore') as f:
@@ -85,12 +85,12 @@
 
     if len(directory.parts) <= 1:
         raise FileNotFoundError(f"Unable to find the file with the name {file_name!r}.")
 
     return escalating_find_file(file_name=file_name, directory=directory.parent, case_sensitive=case_sensitive)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/meta_helper/single_running_instance.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/icon_text_button.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,110 +3,118 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-import os
-from typing import ClassVar
+import sys
+from typing import Union, Optional
 from pathlib import Path
 
-# * Third Party Imports --------------------------------------------------------------------------------->
-import attrs
-import psutil
-
-# * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.errors import ApplicationInstanceAlreadyRunningError
-from gidapptools.custom_types import PATH_TYPE
+# * Qt Imports --------------------------------------------------------------------------------------->
+import PySide6
+from PySide6.QtGui import QIcon, QPixmap
+from PySide6.QtCore import Qt, QSize
+from PySide6.QtWidgets import QLabel, QBoxLayout, QHBoxLayout, QPushButton, QVBoxLayout, QApplication
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-@attrs.define(frozen=True, slots=True)
-class LockFileData:
-    text_separator: ClassVar[str] = "|:|"
-    app_name: str = attrs.field()
-    pid: int = attrs.field()
+class ImageTextButton(QPushButton):
 
-    @property
-    def is_running(self) -> bool:
-        return psutil.pid_exists(self.pid)
-
-    @classmethod
-    def from_file(cls, file_path: PATH_TYPE) -> "LockFileData":
-        content = Path(file_path).resolve().read_text(encoding='utf-8', errors='ignore').strip()
-        app_name, raw_pid = (p.strip() for p in content.split(cls.text_separator))
-        pid = int(raw_pid)
-        return cls(app_name=app_name, pid=pid)
-
-    def to_text(self) -> str:
-        return f"{self.app_name}{self.text_separator}{self.pid}"
-
-
-class SingleRunningInstanceRestrictor:
-    _lock_file_name: str = ".running_instance"
-
-    def __init__(self, storage_folder: PATH_TYPE, app_name: str) -> None:
-        self._storage_folder = Path(storage_folder).resolve()
-        self._app_name = app_name
-        self._pid = os.getpid()
-        self._current_process_lock_file_data = LockFileData(app_name=self._app_name, pid=self._pid)
+    def __init__(self, icon: QPixmap = None, text: str = None, direction: Union[type[Qt.Vertical], type[Qt.Horizontal]] = Qt.Vertical, parent=None):
+        super().__init__(parent=parent)
+        layout = QVBoxLayout() if direction == Qt.Vertical else QHBoxLayout()
+        self.setLayout(layout)
+        self.text_label = QLabel()
+        self.text_label.setAlignment(Qt.AlignCenter)
+        self.set_text(text)
+        self.layout.addWidget(self.text_label)
+
+        self.icon_label = QLabel()
+        self.icon_label.setAlignment(Qt.AlignCenter)
+        self.set_icon(icon)
+        self.layout.addWidget(self.icon_label)
 
     @property
-    def lock_file_path(self) -> Path:
-        return self._storage_folder / self._lock_file_name
+    def direction(self):
+        if isinstance(self.layout, QVBoxLayout):
+            return Qt.Vertical
+        return Qt.Horizontal
 
     @property
-    def lock_file_exists(self) -> bool:
-        return self.lock_file_path.is_file()
-
-    def get_existing_lock_file_data(self) -> LockFileData:
-        return LockFileData.from_file(self.lock_file_path)
+    def label_text(self) -> Optional[str]:
+        return self.text_label.text()
 
-    def store_in_lock_file(self) -> None:
-        self.lock_file_path.parent.mkdir(exist_ok=True, parents=True)
-        self.lock_file_path.write_text(self._current_process_lock_file_data.to_text())
+    @property
+    def icon(self) -> Optional[QIcon]:
+        return QIcon(self.icon_label.pixmap())
 
-    def on_other_instance_running(self):
-        other_instance_data = self.get_existing_lock_file_data()
-        raise ApplicationInstanceAlreadyRunningError(app_name=other_instance_data.app_name, running_pid=other_instance_data.pid)
+    def _get_correct_image_size(self) -> QSize:
+        if not self.label_text:
 
-    def aquire(self):
-        if self.lock_file_exists is True:
-            existing_instance_data = self.get_existing_lock_file_data()
-            if existing_instance_data.is_running is True and existing_instance_data.app_name == self._app_name:
-                self.on_other_instance_running()
-        else:
-            self.store_in_lock_file()
+            return self.sizeHint()
 
-    def release(self):
-        self.lock_file_path.unlink(missing_ok=True)
+        fm = self.text_label.fontMetrics()
+        widths = []
+        heights = []
+        for line in self.label_text.splitlines():
+            br = fm.boundingRect(line)
+            widths.append(br.width())
+            heights.append(br.height())
+        # if self.direction == Qt.Vertical:
+        #     return QSize(max(widths), max(heights))
+        # else:
+        #     return QSize(max(widths), sum(heights))
+        return QSize(max(widths), sum(heights))
+
+    def set_text(self, text: str):
+        if text is None:
+            self.text_label.clear()
+            return
+
+        self.text_label.setText(text)
+
+    def set_icon(self, icon: Union[QIcon, QPixmap]):
+        if icon is None:
+            self.icon_label.clear()
+            return
+
+        if isinstance(icon, QIcon):
+            icon = icon.pixmap(self._get_correct_image_size(), QIcon.Normal, QIcon.On)
+        elif isinstance(icon, QPixmap):
+            icon = icon.scaled(self._get_correct_image_size(), Qt.KeepAspectRatioByExpanding, Qt.SmoothTransformation)
+        self.icon_label.setPixmap(icon)
 
-    def __enter__(self) -> None:
-        self.aquire()
+    def sizeHint(self) -> PySide6.QtCore.QSize:
+        return self.layout.sizeHint()
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.release()
+    @property
+    def layout(self) -> QBoxLayout:
+        return super().layout()
+# region [Main_Exec]
 
 
-# region[Main_Exec]
 if __name__ == '__main__':
-    pass
+    app = QApplication()
+    w = ImageTextButton(icon=QPixmap(r"D:\Dropbox\hobby\Modding\Programs\Github\My_Repos\GidAppTools\gidapptools\data\images\placeholder.png"), text="this is a test" + ('\n' + "this is a test") * 10, direction=Qt.Vertical)
+    w.show()
+    sys.exit(app.exec())
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/mixins/file_mixin.py` & `gidapptools-0.5.0/gidapptools/general_helper/mixins/file_mixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import os
 from enum import unique
-from typing import TYPE_CHECKING, Union, AnyStr, Literal, Iterable
+from typing import TYPE_CHECKING, Union, AnyStr, Literal, Iterable, Callable
 from hashlib import md5, sha256, blake2b, blake2s, sha3_512
 from pathlib import Path
 from threading import RLock
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.enums import BaseGidEnum
 from gidapptools.gid_signal.interface import get_signal
@@ -22,32 +22,32 @@
 from gidapptools.general_helper.conversion import human2bytes
 from gidapptools.general_helper.concurrency.locks import GLOBAL_RLOCK_MANAGER
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 get_dummy_profile_decorator_in_globals()
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 READ_TYPE = Union[Literal["r"], Literal["rb"]]
 WRITE_TYPE = Union[Literal["w"], Literal["wb"], Literal['a'], Literal['ab']]
 ON_ERRORS_TYPE = Union[Literal['replace'], Literal['ignore'], AnyStr]
 HASH_FUNC_TYPE = Union[blake2b, md5, sha256, sha3_512, blake2s]
 
@@ -59,28 +59,32 @@
     hash_func: HASH_FUNC_TYPE = md5
     file_hash_size_threshold: int = human2bytes("100 mb")
 
     @ unique
     class ChangeParameter(BaseGidEnum):
         SIZE = "size"
         FILE_HASH = "file_hash"
-        CHANGED_TIME = "changed_time"
+        MTIME = "mtime"
         ALWAYS = "always"
         NEVER = "never"
         ALL = "all"
 
+        def get_check_method(self, instance: "FileMixin") -> Callable[[], bool]:
+            return getattr(instance, f"_on_{self.value}_changed_check")
+
     def __init__(self, file_path: "PATH_TYPE", changed_parameter: str = None, missing_ok: bool = True, **kwargs) -> None:
         self.file_path = Path(file_path)
         self.changed_parameter = self.ChangeParameter.SIZE if changed_parameter is None else self.ChangeParameter(changed_parameter)
+        self.changed_check_func: Callable[[], bool] = self.changed_parameter.get_check_method(self)
         self.missing_ok = missing_ok
         self.read_mode: READ_TYPE = 'r'
         self.write_mode: WRITE_TYPE = 'w'
         self.last_size: int = None
         self.last_file_hash: str = None
-        self.last_changed_time: int = None
+        self.last_mtime: int = None
         self.changed_signal = get_signal(key=self.file_path)
         self.lock: RLock = GLOBAL_RLOCK_MANAGER.get_file_lock(self.file_path)
         self.file_was_created: bool = False
         self._check_handle_not_existing()
         super().__init__(**kwargs)
 
     @staticmethod
@@ -95,14 +99,16 @@
 
     def set_changed_parameter(self, changed_parameter: Union["ChangeParameter", str]) -> None:
         if isinstance(changed_parameter, self.ChangeParameter):
             self.changed_parameter = changed_parameter
         else:
             self.changed_parameter = self.ChangeParameter(changed_parameter)
 
+        self.changed_check_func = self.changed_parameter.get_check_method(self)
+
     def _check_handle_not_existing(self) -> None:
         with self.lock:
             if self.file_path.exists() is True:
                 return
             if self.missing_ok is True:
                 self.file_path.parent.mkdir(parents=True, exist_ok=True)
                 self.file_path.touch(exist_ok=True)
@@ -131,70 +137,64 @@
                 return self.hash_func(f.read()).hexdigest()
             _file_hash = self.hash_func()
             for chunk in f:
                 _file_hash.update(chunk)
             return _file_hash.hexdigest()
 
     @ property
-    def changed_time(self) -> int:
+    def mtime(self) -> int:
         self._check_handle_not_existing()
         return self.file_path.stat().st_mtime
 
-    @ property
-    def has_changed(self) -> bool:
+    def _on_size_changed_check(self) -> bool:
+        return self.last_size is None or self.last_size != self.size
 
-        def on_size() -> bool:
-            return self.last_size is None or self.last_size != self.size
+    def _on_file_hash_changed_check(self) -> bool:
+        return self.last_file_hash is None or self.last_file_hash != self.file_hash
 
-        def on_file_hash() -> bool:
-            return self.last_file_hash is None or self.last_file_hash != self.file_hash
+    def _on_mtime_changed_check(self) -> bool:
+        return self.last_mtime is None or self.last_mtime != self.mtime
 
-        def on_time() -> bool:
-            return self.last_changed_time is None or self.last_changed_time != self.changed_time
+    def _on_all_changed_check(self) -> bool:
+        return any([self._on_size_changed_check(), self._on_file_hash_changed_check(), self._on_mtime_changed_check()])
 
-        def on_all() -> bool:
-            return any([on_size(), on_file_hash(), on_time()])
-
-        def on_always() -> bool:
-            return True
-
-        def on_never() -> bool:
-            return False
-        checks = {self.ChangeParameter.SIZE: on_size,
-                  self.ChangeParameter.FILE_HASH: on_file_hash,
-                  self.ChangeParameter.CHANGED_TIME: on_time,
-                  self.ChangeParameter.ALL: on_all,
-                  self.ChangeParameter.ALWAYS: on_always,
-                  self.ChangeParameter.NEVER: on_never}
+    def _on_always_changed_check(self) -> bool:
+        return True
+
+    def _on_never_changed_check(self) -> bool:
+        return False
+
+    @ property
+    def has_changed(self) -> bool:
         with self.lock:
-            result = checks[self.changed_parameter]()
+            result = self.changed_check_func()
             if result is True:
                 self.changed_signal.delayed_fire_and_forget(1, self)
         return result
 
     def _update_changed_data(self) -> None:
 
         def _update_size():
             self.last_size = self.size
 
         def _update_file_hash():
             self.last_file_hash = self.file_hash
 
-        def _update_changed_time():
-            self.last_changed_time = self.changed_time
+        def _update_mtime():
+            self.last_mtime = self.mtime
 
         def _update_all():
             _update_size()
             _update_file_hash()
-            _update_changed_time()
+            _update_mtime()
         update_table = {self.ChangeParameter.NEVER: lambda: ...,
                         self.ChangeParameter.ALWAYS: lambda: ...,
                         self.ChangeParameter.SIZE: _update_size,
                         self.ChangeParameter.FILE_HASH: _update_file_hash,
-                        self.ChangeParameter.CHANGED_TIME: _update_changed_time,
+                        self.ChangeParameter.MTIME: _update_mtime,
                         self.ChangeParameter.ALL: _update_all}
         update_table[self.changed_parameter]()
 
     @ property
     def _read_kwargs(self) -> dict[str, str]:
         kwargs = {"mode": self.read_mode}
         if 'b' not in self.read_mode:
@@ -225,13 +225,13 @@
                 f.write(data)
 
     def __fspath__(self) -> str:
         return str(self.file_path)
 
     def __str__(self) -> str:
         return self.__fspath__()
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/output_helper/rich_helper.py` & `gidapptools-0.5.0/gidapptools/general_helper/output_helper/rich_helper/rich_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,39 +17,39 @@
 from string import ascii_letters
 from typing import Any
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import MissingOptionalDependencyError
-
+from gidapptools.gid_logger.logger import get_logger
 with MissingOptionalDependencyError.try_import("gidapptools"):
     from rich import inspect as rinspect
     from rich.tree import Tree
     from rich.panel import Panel
     from rich.console import Console as RichConsole
     from rich.terminal_theme import TerminalTheme
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
-
-# endregion[Constants]
+log = get_logger(__name__)
+# endregion [Constants]
 
 MY_TERMINAL_THEME = TerminalTheme(
     (40, 40, 40),
     (102, 255, 50),
     [
         (0, 0, 0),
         (15, 140, 220),
@@ -127,15 +127,15 @@
 
     with StringIO() as throw_away_file:
         console = RichConsole(soft_wrap=True, record=True, file=throw_away_file)
         title = None
         try:
             title = _make_title(obj)
         except Exception as e:
-            print(e)
+            log.error(e, exc_info=True)
             title = None
         rinspect(obj=obj,
                  title=title,
                  help=show_help,
                  methods=show_methods,
                  docs=show_docs,
                  private=show_private,
@@ -149,13 +149,13 @@
             firefox = shutil.which("firefox.exe")
             cmd = f'"{firefox}" -new-window "{str(out_file)}"'
 
             _cmd = subprocess.run(cmd, check=True, text=True)
             sleep(0.5)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
 
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/path_helper.py` & `gidapptools-0.5.0/gidapptools/general_helper/path_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.utility.enums import OperatingSystem
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def get_all_drives(also_non_physical: bool = False) -> tuple[Path]:
     return tuple(Path(drive.mountpoint) for drive in disk_partitions(all=also_non_physical))
 
 
 def get_all_drives_non_psutil(*args):
@@ -129,11 +129,32 @@
         case OperatingSystem.MAC_OS:
             subprocess.run(['open', in_folder], check=False)
 
         case _:
             raise RuntimeError(f"Not able to open folder {in_folder.as_posix()!r}, because no known procedure for Operating System {operating_system!s}.")
 
 
-# region[Main_Exec]
+ILLEGAL_FILE_NAME_CHARS: set[str] = set("\"|%:/,.\\[]<>*?")
+
+EXTENDED_ILLEGAL_FILE_NAME_CHARS: set[str] = ILLEGAL_FILE_NAME_CHARS.union("'&§\{\};#=")
+
+
+def ensure_valid_file_stem(file_stem: str,
+                           strict: bool = False,
+                           replace_all_spaces: bool = False) -> str:
+    illegal_chars = ILLEGAL_FILE_NAME_CHARS
+    file_stem = file_stem.rstrip()
+
+    if strict is True:
+        illegal_chars = EXTENDED_ILLEGAL_FILE_NAME_CHARS
+        file_stem = file_stem.lstrip()
+
+    if replace_all_spaces is True:
+        file_stem = file_stem.replace(" ", "_")
+
+    return "".join(c for c in file_stem if c not in illegal_chars)
+
+
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/regex/datetime_regex.py` & `gidapptools-0.5.0/gidapptools/general_helper/regex/datetime_regex.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import re
 from pathlib import Path
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 from frozendict import frozendict
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 DATETIME_FORMAT_REGEX_MAPPING: frozendict[str, str] = frozendict(**{r"%Y": r"(?P<year>\d{4})",
                                                                     r"%m": r"(?P<month>[01]?\d)",
                                                                     r"%d": r"(?P<day>[0123]?\d)",
                                                                     r"%H": r"(?P<hour>[012]?\d)",
                                                                     r"%M": r"(?P<minute>[0-5]?\d)",
                                                                     r"%S": r"(?P<second>[0-5]?\d)",
@@ -43,14 +43,14 @@
 
 def datetime_format_to_regex(in_format: str, flags: re.RegexFlag) -> re.Pattern:
     pattern_string = in_format
     for k, v in DATETIME_FORMAT_REGEX_MAPPING.items():
         pattern_string = pattern_string.replace(k, v)
     return re.compile(pattern_string, flags)
 
-    # region[Main_Exec]
+    # region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/string_helper.py` & `gidapptools-0.5.0/gidapptools/general_helper/string_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,96 +17,105 @@
 # * Third Party Imports --------------------------------------------------------------------------------->
 import pyparsing as ppa
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.enums import StringCase
 from gidapptools.gid_warning.experimental import mark_experimental
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
 
-# endregion[Constants]
+# endregion [Constants]
 
 STRING_CASE_FUNC_TYPE = Callable[[Iterable[str]], str]
 
 
 # TODO: Rewrite as normal class/Module-Singleton
-class StringCaseConverter:
-    """ """
+class _StringCaseConverter:
     SNAKE = StringCase.SNAKE
     SCREAMING_SNAKE = StringCase.SCREAMING_SNAKE
     CAMEL = StringCase.CAMEL
     PASCAL = StringCase.PASCAL
     KEBAP = StringCase.KEBAP
     SPLIT = StringCase.SPLIT
     CLASS = StringCase.CLASS
     TITLE = StringCase.TITLE
     BLOCK_UPPER = StringCase.BLOCK_UPPER
 
-    _split_grammar: Optional[ppa.ParserElement] = None
     split_pascal_case_regex = re.compile(r"(?<!\_)(\B[A-Z])")
     snake_case_to_pascal_case_regex = re.compile(r"(_|^)(\w)")
-    _word_list_split_chars = {'-', '_', ' '}
-    _word_list_split_regex = re.compile(r'|'.join(list(_word_list_split_chars) + [r"(?=[A-Z])"]))
+    _word_list_split_chars = frozenset({'-', '_', ' '})
 
-    _dispatch_table: Optional[dict[str, STRING_CASE_FUNC_TYPE]] = None
-    _bad_chars: Optional[set[str]] = None
+    __slots__ = ("_split_grammar",
+                 "_word_list_split_regex",
+                 "_dispatch_table",
+                 "_bad_chars")
+
+    def __init__(self) -> None:
+        self._split_grammar: Optional[ppa.ParserElement] = None
+
+        self._word_list_split_regex = None
+
+        self._dispatch_table: Optional[dict[str, STRING_CASE_FUNC_TYPE]] = None
+        self._bad_chars: Optional[frozenset[str]] = None
+
+    @property
+    def bad_chars(self) -> set[str]:
+        if self._bad_chars is None:
+            self._bad_chars = frozenset({c for c in punctuation if c not in self._word_list_split_chars})
+        return self._bad_chars
 
-    @classmethod
     @property
-    def bad_chars(cls) -> set[str]:
-        if cls._bad_chars is None:
-            cls._bad_chars = {c for c in punctuation if c not in cls._word_list_split_chars}
-        return cls._bad_chars
+    def word_list_split_regex(self) -> re.Pattern:
+        if self._word_list_split_regex is None:
+            self._word_list_split_regex = re.compile(r'|'.join(list(self._word_list_split_chars) + [r"(?=[A-Z])"]))
+        return self._word_list_split_regex
 
-    @classmethod
     @property
-    def dispatch_table(cls) -> dict[StringCase, STRING_CASE_FUNC_TYPE]:
-        if cls._dispatch_table is None:
-            cls._dispatch_table = {}
-            for meth_name, meth_obj in inspect.getmembers(cls):
+    def dispatch_table(self) -> dict[StringCase, STRING_CASE_FUNC_TYPE]:
+        if self._dispatch_table is None:
+            self._dispatch_table = {}
+            for meth_name, meth_obj in inspect.getmembers(self):
                 if meth_name.startswith('_to_') and meth_name.endswith('_case'):
                     key_name = meth_name.removeprefix('_to_').removesuffix('_case')
-                    cls._dispatch_table[StringCase(key_name)] = meth_obj
-        return cls._dispatch_table
+                    self._dispatch_table[StringCase(key_name)] = meth_obj
+        return self._dispatch_table
 
-    @classmethod
     @property
-    def split_grammar(cls) -> ppa.ParserElement:
-        if cls._split_grammar is None:
+    def split_grammar(self) -> ppa.ParserElement:
+        if self._split_grammar is None:
             underscore = ppa.Literal('_').suppress()
             dash = ppa.Literal("-").suppress()
             all_upper_word = ppa.Regex(r"[A-Z]+(?![a-z])")
             all_lower_word = ppa.Word(ascii_lowercase, ascii_lowercase)
             title_word = ppa.Regex(r"[A-Z][a-z]+")
             number = ppa.Word(ppa.nums)
             words = (title_word | all_upper_word | all_lower_word | number).set_parse_action(lambda x: x[0].casefold())
             grammar = words | underscore | dash
-            cls._split_grammar = ppa.OneOrMore(grammar)
-        return cls._split_grammar
+            self._split_grammar = ppa.OneOrMore(grammar)
+        return self._split_grammar
 
-    @classmethod
-    def _to_word_list(cls, in_string: str) -> list[str]:
+    def _to_word_list(self, in_string: str) -> list[str]:
         """
         :param in_string: str:
         """
-        parts: ppa.ParseResults = cls.split_grammar.parse_string(in_string, parse_all=True)
+        parts: ppa.ParseResults = self.split_grammar.parse_string(in_string, parse_all=True)
 
         return [word for word in parts if word]
 
     @staticmethod
     def _to_block_upper_case(word_list: Iterable[str]) -> str:
         """
         :param word_list: Iterable[str]:
@@ -175,39 +184,38 @@
         """
 
         :param word_list: Iterable[str]:
 
         """
         return ' '.join(word.upper() for word in word_list)
 
-    @classmethod
-    def remove_bad_chars(cls, in_string: str) -> str:
+    def remove_bad_chars(self, in_string: str) -> str:
         new_string = str(in_string)
-        for char in cls.bad_chars:
+        for char in self.bad_chars:
             new_string: str = new_string.replace(char, "")
 
         return new_string
 
-    @classmethod
-    def convert_to(cls, in_string: str, target_case: Union[str, StringCase], clean_in_string: bool = False) -> str:
+    def convert_to(self, in_string: str, target_case: Union[str, StringCase], clean_in_string: bool = False) -> str:
         """
 
         :param in_string: str:
         :param target_case: Union[str, StringCase]:
 
         """
         if clean_in_string is True:
-            in_string = cls.remove_bad_chars(in_string)
+            in_string = self.remove_bad_chars(in_string)
         target_case = StringCase(target_case) if isinstance(target_case, str) else target_case
-        word_list = cls._to_word_list(in_string)
-        return cls.dispatch_table.get(target_case)(word_list)
+        word_list = self._to_word_list(in_string)
+        return self.dispatch_table.get(target_case)(word_list)
 
 
-_ = StringCaseConverter.dispatch_table
-_ = StringCaseConverter.split_grammar
+StringCaseConverter = _StringCaseConverter()
+# _ = StringCaseConverter.dispatch_table
+# _ = StringCaseConverter.split_grammar
 
 
 def replace_by_dict(in_string: str, in_dict: dict[str, str]) -> str:
     """
 
     :param in_string: str:
     :param in_dict: dict[str, str]:
@@ -249,15 +257,21 @@
     """
     cleaned_text = SPACE_CLEANING_REGEX.sub(' ', in_text)
     if replace_newline is True:
         cleaned_text = NEWLINE_CLEANING_REGEX.sub(' ', cleaned_text)
     return cleaned_text
 
 
-def shorten_string(in_text: str, max_length: int, shorten_side: Literal["right", "left"] = "right", placeholder: str = '...', clean_before: bool = True, ensure_space_around_placeholder: bool = False, split_on: str = r'\s|\n') -> str:
+def shorten_string(in_text: str,
+                   max_length: int,
+                   shorten_side: Literal["right", "left"] = "right",
+                   placeholder: str = '...',
+                   clean_before: bool = True,
+                   ensure_space_around_placeholder: bool = False,
+                   split_on: str = r'\s|\n') -> str:
     """
 
     :param in_text: str:
     :param max_length: int:
     :param shorten_side: Literal["right", "left"]:  (Default value = "right")
     :param placeholder: str:  (Default value = "...")
     :param clean_before: bool:  (Default value = True)
@@ -285,29 +299,29 @@
         split_on = r"."
     find_regex = re.compile(split_on)
     last_space_position = list(find_regex.finditer(new_text))
 
     return new_text[:last_space_position[-1].span()[0]].strip() + placeholder if shorten_side == 'right' else placeholder + new_text[last_space_position[0].span()[0]:].strip()
 
 
-def split_quotes_aware(text: str, split_chars: Iterable[str] = None, quote_chars: Iterable[str] = None, strip_parts: bool = True) -> list[str]:
+def split_quotes_aware(text: str,
+                       split_chars: Iterable[str] = None,
+                       quote_chars: Iterable[str] = None,
+                       strip_parts: bool = True) -> list[str]:
     """Splits a string on but not if the separator char is inside of quotes.
 
     :param text: The string to split.
     :type text: str
     :param split_chars: The characters to split on. Defaults to `,`.
     :type split_chars: Iterable[str]
     :param quote_chars: The quote chars that should be considered real quotes. Defaults to `"` and `'`.
     :type quote_chars: Iterable[str]
     :param strip_parts: If each found substrin should be striped of preceding and trailing whitespace in the result. Defaults to True.
     :type strip_parts: bool
     :param text: str:
-    :param split_chars: Iterable[str]:  (Default value = None)
-    :param quote_chars: Iterable[str]:  (Default value = None)
-    :param strip_parts: bool:  (Default value = True)
     :returns: The found sub-parts.
     :rtype: list[str]
 
     """
     split_chars = {','} if split_chars is None else set(split_chars)
     quote_chars = {"'", '"'} if quote_chars is None else set(quote_chars)
     parts = []
@@ -357,37 +371,29 @@
     in_string = re.sub('[^0-9a-zA-Z_]', '', in_string)
 
     # Remove leading characters until we find a letter or underscore
     in_string = re.sub('^[^a-zA-Z_]+', '', in_string)
 
     return in_string.casefold()
 
+# [2,"""",""__SERVER__"",false,2,""2""]
 
-def fix_multiple_quotes(_text: str, max_consecutive_quotes: int = None) -> str:
+
+FIX_MULTIPLE_QUOTES_PATTERN = re.compile(r"""(\"|\')(\"{1,1}|\'{1,1})""")
+
+
+def fix_multiple_quotes(_text: str) -> str:
     """
 
     :param _text: str:
     :param max_consecutive_quotes: int:  (Default value = None)
 
     """
 
-    def _replace_function(match: re.Match):
-        """
-
-        :param match: re.Match:
-
-        """
-        return match.group()[0]
-    if max_consecutive_quotes is None:
-        pattern = r"""(\"+)|(\'+)"""
-    elif max_consecutive_quotes <= 1:
-        raise ValueError("'max_consecutive_quotes' cannot be less than 2.")
-    else:
-        pattern = rf"""(\"{{2,{max_consecutive_quotes}}})|(\'{{2,{max_consecutive_quotes}}})"""
-    return re.sub(pattern, _replace_function, _text)
+    return FIX_MULTIPLE_QUOTES_PATTERN.sub("\\g<1>", _text)
 
 
 def escape_doubled_quotes(text: str) -> str:
     """
 
     :param text: str:
 
@@ -495,15 +501,17 @@
     for k, v in replacement_map.items():
         new_string = new_string.replace(k, v)
 
     return new_string
 
 
 class RegexMapReplacer:
-    # 3x slower than just replace loop
+    """
+    3x slower than just replace loop
+    """
     __slots__ = ("_replacement_map", "_pattern")
 
     @mark_experimental()
     def __init__(self, replacement_map: Mapping[str, str]) -> None:
         self._replacement_map = replacement_map
         self._pattern: re.Pattern = re.compile(r"|".join(rf"{k}" for k in self._replacement_map))
 
@@ -512,13 +520,14 @@
         return self._replacement_map[orig_text_part]
 
     def apply(self, text: str) -> str:
         return self._pattern.sub(self._replacement_lookup, text)
 
     def __call__(self, text: str) -> Any:
         return self.apply(text=text)
-# region[Main_Exec]
+
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/timing.py` & `gidapptools-0.5.0/gidapptools/general_helper/timing.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import os
 from time import perf_counter_ns
 from typing import Union, Callable
 from pathlib import Path
-from functools import wraps
+from functools import wraps, partial
 from threading import RLock
 from contextlib import contextmanager
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.conversion import seconds2human
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 TIME_NS_FUNC_TYPE = Callable[[], float]
 
 
 time_execution_path_locks: dict[Path, RLock] = {}
 
@@ -50,15 +50,15 @@
         time_execution_path_locks[path] = lock
     return lock
 
 
 @contextmanager
 def time_execution(identifier: str = None,
                    time_ns_func: TIME_NS_FUNC_TYPE = perf_counter_ns,
-                   output: Union[Callable, Path] = print,
+                   output: Union[Callable, Path] = partial(print, flush=True),
                    output_kwargs: dict[str, object] = None,
                    condition: Union[bool, Callable[[], bool]] = True,
                    as_seconds: bool = True,
                    decimal_places: Union[int, None] = None,
                    also_pretty: bool = False) -> None:
     if callable(condition):
         condition = condition()
@@ -85,15 +85,15 @@
             output_kwargs = output_kwargs or {}
             output(f"{identifier} took {full_time:f} {unit}{pretty}", **output_kwargs)
     else:
         yield
 
 
 def time_func(time_ns_func: TIME_NS_FUNC_TYPE = perf_counter_ns,
-              output: Callable = print,
+              output: Callable = partial(print, flush=True),
               output_kwargs: dict[str, object] = None,
               use_qualname: bool = True,
               condition: Union[bool, Callable[[], bool]] = True,
               as_seconds: bool = True,
               decimal_places: int = None,
               also_pretty: bool = False):
 
@@ -150,12 +150,12 @@
         __builtins__["profile"] = profile
     # stk = inspect.stack()[1]
     # mod = inspect.getmodule(stk[0])
     # if mod is not None:
     #     setattr(mod, "profile", profile)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/typing_helper.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/object_name.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,51 +3,42 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-from typing import Type
 from pathlib import Path
 
-# endregion[Imports]
+# * Qt Imports --------------------------------------------------------------------------------------->
+from PySide6.QtCore import QObject
+
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-def implements_protocol(proto: Type):
-    """
-    Creates a decorator for classes that checks that the decorated class implements the runtime protocol `proto`.
-
-        from https://stackoverflow.com/a/62923698/13989012
-    """
-    def _deco(cls_def):
-        try:
-            assert issubclass(cls_def, proto)
-        except AssertionError as error:
-            error.args = (f"{cls_def} does not implement protocol {proto}",)
-            raise
-        return cls_def
-    return _deco
+def set_std_object_name(obj: QObject):
+    name = obj.__class__.__name__
+    obj.setObjectName(name)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/general_helper/web_helper.py` & `gidapptools-0.5.0/gidapptools/gid_config/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,47 +3,40 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-from time import sleep, process_time_ns
+from enum import Enum, auto
 from pathlib import Path
-from contextlib import contextmanager
 
-# * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.gid_warning.experimental import mark_experimental
-
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-@mark_experimental
-@contextmanager
-def download_limit():
-    start = process_time_ns()
-    yield
-    if (duration := (process_time_ns() - start) / 1_000_000_000) < 1:
-        sleep(1 - duration)
+class SpecialTypus(Enum):
+    AUTO = auto()
+    RAW = auto()
+    DELAYED = auto()
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_argparse/custom_parser.py` & `gidapptools-0.5.0/gidapptools/gid_argparse/custom_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.import_helper import import_from_name, meta_data_from_module
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     ...
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def url_sorter(in_name_and_url: tuple[str, str]):
     order = ("homepage",
              "home-page",
              "documentation",
              "wiki",
@@ -160,16 +160,16 @@
         init_kwargs["version"] = getattr(package_module, "__version__", meta_data["version"])
         init_kwargs["prog"] = pretty_name or meta_data["name"]
         init_kwargs["description"] = meta_data.get("summary") or (inspect.getdoc(package_module) or "")
         init_kwargs["urls"] = meta_data.all_urls
 
         init_kwargs = init_kwargs | kwargs
         return cls(**init_kwargs)
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     x = import_from_name("gidapptools")
     y = meta_data_from_module(x)
     pprint(y)
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/__init__.py` & `gidapptools-0.5.0/gidapptools/gid_config/__init__.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/conversion/base_converters.py` & `gidapptools-0.5.0/gidapptools/gid_config/conversion/base_converters.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,52 +6,54 @@
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Union, Literal, TypeVar, Optional
 from pathlib import Path
+import logging
 from datetime import datetime, timedelta
-
+import os
 # * Third Party Imports --------------------------------------------------------------------------------->
 from frozendict import frozendict
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.errors import MaxError, MinError
+from gidapptools.errors import MaxError, MinError, ValueValidationError, NotLoggingLevelError
 from gidapptools.general_helper.enums import MiscEnum
 from gidapptools.general_helper.conversion import bytes2human, human2bytes, str_to_bool, seconds2human, human2timedelta
 from gidapptools.general_helper.import_helper import is_importable
+from gidapptools.general_helper.timing import get_dummy_profile_decorator_in_globals
 
 try:
     RICH_AVAILABLE = True
 except ImportError:
     RICH_AVAILABLE = False
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gid_config.conversion.conversion_table import ConversionTable
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 PYSIDE6_AVAILABLE = is_importable("PySide6")
 YARL_AVAILABLE = is_importable("yarl")
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-
-# endregion[Constants]
+get_dummy_profile_decorator_in_globals()
+# endregion [Constants]
 
 
 class ConfigValueConverter(ABC):
     __slots__ = ("conversion_table",)
     is_standard_converter: bool = False
     value_typus: str = None
     value_typus_aliases: tuple[str] = tuple()
@@ -104,21 +106,21 @@
 
     def to_config_value(self, value: int) -> str:
         try:
             self.validate_value(value, None, None, None)
         except MinError:
             if self.on_min_error == "raise":
                 raise
-            elif self.on_min_error == "set_minimum":
+            if self.on_min_error == "set_minimum":
                 value = self.minimum
 
         except MaxError:
             if self.on_max_error == "raise":
                 raise
-            elif self.on_max_error == "set_maximum":
+            if self.on_max_error == "set_maximum":
                 value = self.maximum
 
         if value is None:
             return ""
 
         return str(value)
 
@@ -235,32 +237,33 @@
 
 class PathConfigValueConverter(ConfigValueConverter):
     __slots__ = ("resolve",)
     is_standard_converter: bool = True
     value_typus = "path"
     value_typus_aliases = ("fs_path",)
 
-    def __init__(self, conversion_table: "ConversionTable", resolve: bool = False) -> None:
+    def __init__(self, conversion_table: "ConversionTable", resolve: bool = True) -> None:
         super().__init__(conversion_table)
         self.resolve = resolve
 
     def to_config_value(self, value: Path) -> str:
         if value is None:
             return ""
         path = Path(value)
         if self.resolve is True:
             path = path.resolve()
         return path.as_posix()
 
     def to_python_value(self, value: str) -> Union[Path, None]:
         if value is None:
             return None
-        path = Path(value)
+        path = Path(value.strip())
         if self.resolve is True:
-            path = path.resolve()
+            path = Path(os.path.expandvars(path)).resolve()
+
         return path
 
 
 class FileSizeConfigValueConverter(ConfigValueConverter):
     __slots__ = ()
     is_standard_converter: bool = True
     value_typus: str = "file_size"
@@ -299,14 +302,53 @@
     def to_python_value(self, value: str) -> Union[list[SUB_TYPUS_TYPE], None]:
         if value is None:
             return None
         sub_converter: "ConfigValueConverter" = self.conversion_table.converters[self.sub_typus](self.conversion_table)
         return [sub_converter.to_python_value(item) for item in value.split(self.split_char) if item.strip()]
 
 
+class LoggingLevelValueConverter(ConfigValueConverter):
+    __slots__ = tuple()
+    is_standard_converter: bool = True
+    value_typus = "logging_level"
+
+    def validate_value(self, value, entry_name: str, section_name: str, config) -> None:
+        if not isinstance(value, (str, int)):
+            raise NotLoggingLevelError(value=value, converter=self, entry_name=entry_name, section_name=section_name, config=config)
+
+        if isinstance(value, int) and value not in logging._levelToName:
+            raise NotLoggingLevelError(value=value, converter=self, entry_name=entry_name, section_name=section_name, config=config)
+
+        if isinstance(value, str) and value not in logging._nameToLevel:
+            raise NotLoggingLevelError(value=value, converter=self, entry_name=entry_name, section_name=section_name, config=config)
+
+    def to_config_value(self, value: Any, **named_arguments) -> str:
+        if value is None:
+            return ""
+
+        if isinstance(value, int):
+
+            value = logging._levelToName[value]
+
+        if isinstance(value, str):
+            value = value.upper()
+
+        self.validate_value(value, None, None, None)
+
+        return value
+
+    def to_python_value(self, value: str, **named_arguments) -> Union[int, None]:
+
+        value = value.upper()
+
+        self.validate_value(value, None, None, None)
+
+        return logging._nameToLevel[value]
+
+
 if PYSIDE6_AVAILABLE is True:
     from PySide6.QtGui import QColor
 
     class QColorValueConverter(ConfigValueConverter):
         __slots__ = tuple()
         is_standard_converter: bool = True
         value_typus = "qcolor"
@@ -344,12 +386,12 @@
             return URL(value)
 
 
 def get_standard_converter() -> tuple[type["ConfigValueConverter"]]:
     return tuple(sc for sc in ConfigValueConverter.__subclasses__() if sc.is_standard_converter is True)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/conversion/conversion_table.py` & `gidapptools-0.5.0/gidapptools/gid_config/conversion/conversion_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import UnconvertableTypusError
 from gidapptools.general_helper.enums import MiscEnum
 from gidapptools.general_helper.timing import get_dummy_profile_decorator_in_globals
 from gidapptools.gid_config.conversion.base_converters import ConfigValueConverter, get_standard_converter
 from gidapptools.gid_config.conversion.converter_grammar import ConverterSpecData
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 get_dummy_profile_decorator_in_globals()
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class ConversionTable:
     __slots__ = ("_standard_converters", "_extra_converters", "_resolved_converters")
 
     def __init__(self,
                  extra_converter: Iterable[type[ConfigValueConverter]] = None) -> None:
@@ -77,12 +77,12 @@
         return converter(self, **converter_data["kw_arguments"])
 
     def add_extra_converter(self, converter: type[ConfigValueConverter]) -> None:
         self._extra_converters = tuple(self._extra_converters + (converter,))
         self._resolved_converters = None
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/conversion/converter_grammar.py` & `gidapptools-0.5.0/gidapptools/gid_config/conversion/converter_grammar.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 import pyparsing as ppa
 from pyparsing import common as ppc
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import InvalidConverterValue
 from gidapptools.general_helper.timing import get_dummy_profile_decorator_in_globals
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 get_dummy_profile_decorator_in_globals()
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 REPLACE_WORDS = {"$comma$": ",",
                  "$equals$": "="}
 
 
 def replace_value_words(in_tok: ppa.ParseResults) -> str:
@@ -92,11 +92,11 @@
     try:
         result = CONVERTER_SPECIFICATION_GRAMMAR.parse_string(raw_specification, parse_all=True).as_dict()
         return ConverterSpecData(typus=result["typus"], kw_arguments=result.get("kw_arguments", dict()))
     except ppa.ParseException as error:
         raise InvalidConverterValue(f"{raw_specification!r} is not a valid converter specification") from error
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/conversion/extra_base_typus.py` & `gidapptools-0.5.0/gidapptools/gid_config/conversion/extra_base_typus.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from enum import Enum, auto
 from pathlib import Path
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 SPEC_BASE_DATA = {
     "__env__": {
         "__default__": {"converter": "string"},
         "PATH": {"converter": "list(sub_typus=path, split_char=;)"},
         "APPDATA": {"converter": "path"},
         "LOCALAPPDATA": {"converter": "path"},
         "PROGRAMFILES(X86)": {"converter": "path"},
@@ -49,12 +49,12 @@
 
 class NonTypeBaseTypus(Enum):
     DEFAULT = auto()
     FILE_SIZE = auto()
     STRING_CHOICE = auto()
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/conversion/spec_data.py` & `gidapptools-0.5.0/gidapptools/gid_config/conversion/spec_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,47 +5,51 @@
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import json
 from typing import TYPE_CHECKING, Union, Literal, Callable, Optional
+from types import ModuleType
 from pathlib import Path
 from threading import RLock
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import SpecDataMissingError
 from gidapptools.custom_types import PATH_TYPE
 from gidapptools.general_helper.timing import get_dummy_profile_decorator_in_globals
 from gidapptools.general_helper.class_helper import MethodEnabledWeakSet
 from gidapptools.gid_config.conversion.spec_item import SpecEntry, SpecSection
 from gidapptools.general_helper.mixins.file_mixin import FileMixin
 from gidapptools.gid_config.conversion.converter_grammar import ConverterSpecData, parse_specification
 
+import orjson
+
+
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     pass
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 get_dummy_profile_decorator_in_globals()
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class SpecLoader:
     __slots__ = ("spec_section_class",
                  "spec_entry_class",
                  "parse_func",
                  "loaded_data")
@@ -150,14 +154,16 @@
         """
         return f'{self.__class__.__name__}(name={self.name!r}, loader={self.loader!r})'
 
 
 class SpecFile(FileMixin, SpecData):
     _name_suffixes_to_remove: tuple[str] = ("_configspec", "_spec", "_config", "_config_spec", "_spec_config", "_specconfig")
 
+    json_load_func: Callable[[str], dict[str, object]] = orjson.loads
+
     def __init__(self,
                  file_path: PATH_TYPE,
                  loader: SpecLoader = None,
                  changed_parameter: Union[Literal['size'], Literal['file_hash']] = 'size') -> None:
         super().__init__(name=self._generate_name_from_path(file_path, suffixes_to_remove=self._name_suffixes_to_remove),
                          loader=loader or SpecLoader(),
                          file_path=file_path,
@@ -191,27 +197,28 @@
         self.load()
         for target in self._on_reload_targets:
             target()
         return self
 
     def load(self) -> "SpecFile":
         with self.lock:
-            self.load_data(json.loads(self.read()))
+
+            self.load_data(self.json_load_func(self.read()))
 
         return self
 
     def save(self) -> None:
         with self.lock:
             data = self.original_data
             json_data = json.dumps(data, indent=4, sort_keys=False)
             self.write(json_data)
 
     def __repr__(self) -> str:
 
         return f'{self.__class__.__name__}(name={self.name!r}, file_path={self.file_path.as_posix()!r})'
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/conversion/spec_item.py` & `gidapptools-0.5.0/gidapptools/gid_config/conversion/spec_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 from gidapptools.general_helper.enums import MiscEnum
 from gidapptools.gid_config.conversion.converter_grammar import ConverterSpecData, reverse_replace_value_words
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     pass
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class SpecSection:
     __slots__ = ("name",
                  "default_converter",
                  "description",
                  "dynamic_entries_allowed",
@@ -142,12 +142,12 @@
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(name={self.name!r})'
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/enums.py` & `gidapptools-0.5.0/gidapptools/general_helper/web_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,40 +3,38 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-from enum import Enum, auto
+from time import sleep, process_time_ns
 from pathlib import Path
+from contextlib import contextmanager
 
-# endregion[Imports]
+# * Gid Imports ----------------------------------------------------------------------------------------->
+from gidapptools.gid_warning.experimental import mark_experimental
+
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
-
-
-class SpecialTypus(Enum):
-    AUTO = auto()
-    RAW = auto()
-    DELAYED = auto()
+# endregion [Constants]
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/interface.py` & `gidapptools-0.5.0/gidapptools/gid_config/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,31 +24,31 @@
 from gidapptools.gid_config.conversion.conversion_table import ConversionTable, ConfigValueConverter
 from gidapptools.gid_config.conversion.converter_grammar import ConverterSpecData
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 get_dummy_profile_decorator_in_globals()
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class SectionAccessor:
 
     def __init__(self, config: "GidIniConfig", section_name: str) -> None:
         self.config = config
         self.section_name = section_name
@@ -243,14 +243,15 @@
                 return default
             raise
 
     def set(self, section_name: str, entry_name: str, value: Any) -> None:
         spec_item = self.get_spec_item(section_name=section_name, entry_name=entry_name)
         converter = self.get_converter(spec_item.converter)
         self.config.set_value(section_name=section_name, entry_key=entry_name, entry_value=converter.to_config_value(value))
+        self.clear_cache()
         self.reload_if_changed()
 
     def ensure_section(self, section_name: str) -> None:
         section = Section(section_name)
         self.config.add_section(section)
 
     def set_if_not_exists(self, section_name: str, entry_name: str, value: Any) -> None:
@@ -295,26 +296,26 @@
 
 
 def get_config(spec_path: "PATH_TYPE",
                config_path: "PATH_TYPE",
                spec_loader: SpecLoader = None,
                config_parser: BaseIniParser = None,
                config_auto_write: bool = True,
-               changed_parameter: Union[Literal['size'], Literal['file_hash'], Literal["changed_time"]] = 'changed_time',
+               changed_parameter: Union[Literal['size'], Literal['file_hash'], Literal["mtime"], Literal["never"], Literal["always"], Literal["all"]] = 'mtime',
                extra_converter: Iterable[ConfigValueConverter] = None,
                empty_is_missing: bool = True,
                preload_ini_file: bool = False) -> GidIniConfig:
 
     conversion_table = ConversionTable(extra_converter=extra_converter)
     spec = SpecFile(spec_path, loader=spec_loader or SpecLoader(), changed_parameter=changed_parameter)
     config = ConfigFile(config_path, parser=config_parser or BaseIniParser(), changed_parameter=changed_parameter, auto_write=config_auto_write)
     config_item = GidIniConfig(spec, config, conversion_table=conversion_table, empty_is_missing=empty_is_missing)
 
     if preload_ini_file is True:
         preload_config(config_item)
     return config_item
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/parser/config_data.py` & `gidapptools-0.5.0/gidapptools/gid_config/parser/config_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 from gidapptools.gid_config.parser.ini_parser import BaseIniParser
 from gidapptools.general_helper.mixins.file_mixin import FileMixin
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 get_dummy_profile_decorator_in_globals()
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class ConfigData:
 
     def __init__(self, name: str) -> None:
         self.name = name
         self._sections: dict[str, Section] = None
@@ -249,14 +249,14 @@
 
             self.write(data)
 
     def load(self) -> None:
         with self.lock:
             content = self.read()
             self._sections = {section.name: section for section in self.parser.parse(content)}
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/parser/grammar.py` & `gidapptools-0.5.0/gidapptools/gid_config/parser/grammar.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 import pyparsing as pp
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gid_config.parser.tokens import TokenFactory
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class BaseIniGrammar:
     """
     Builds the pyparsing Grammar for the Parser.
 
     Args:
@@ -106,12 +106,12 @@
 
     def get_grammar(self, **kwargs) -> pp.ParserElement:
         all_elements = pp.MatchFirst([self.section_name, self.entry, self.comment])
         # all_elements = self.section_name | self.entry | self.comment
         return all_elements.set_parse_action(self.token_factory.parse_action)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/parser/ini_parser.py` & `gidapptools-0.5.0/gidapptools/gid_config/parser/ini_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 # * Third Party Imports --------------------------------------------------------------------------------->
 import pyparsing as pp
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import TrailingCommentError
 from gidapptools.gid_config.parser.tokens import Entry, Token, Comment, Section, TokenFactory
 from gidapptools.gid_config.parser.grammar import BaseIniGrammar
-
-# endregion[Imports]
+from gidapptools.general_helper.timing import get_dummy_profile_decorator_in_globals
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
-
+get_dummy_profile_decorator_in_globals()
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class BaseIniParser:
     """
     Parser for text in `ini` format.
 
     Keeps normal comments, but strips inline comments. Can handle multiline values as long as they are indented. Orphaned Entries (Entries under no section) are not allowed.
@@ -146,13 +146,13 @@
             self.grammar = self.grammar_item.get_grammar(**kwargs)
         text = self._pre_process(text)
 
         return self._parse(text)
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}'
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_config/parser/tokens.py` & `gidapptools-0.5.0/gidapptools/gid_config/parser/tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 from typing import Any
 from pathlib import Path
 from weakref import ProxyType, proxy
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 import pyparsing as pp
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class Token:
     __slots__ = tuple()
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(" + ', '.join(f"{n}={getattr(self, n)!r}" for n in self.__slots__) + ')'
@@ -159,12 +159,12 @@
 
     def parse_action(self, tokens: pp.ParseResults) -> Token:
         name = tokens.get_name()
         token_class = self.token_map[name]
         return token_class(*tokens)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/apsw_database.py` & `gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/apsw_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,37 +29,38 @@
 import peewee
 from frozendict import frozendict
 from playhouse.apsw_ext import APSWDatabase
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gid_database.orm_peewee.sqlite.constants import MEMORY_DB_PATH, STD_DEFAULT_PRAGMAS, STD_DEFAULT_EXTENSIONS
 from gidapptools.gid_database.orm_peewee.sqlite.pragma_info import PragmaInfo
+from gidapptools.gid_logger.logger import get_logger
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
+log = get_logger(__name__)
 
-
-# endregion[Constants]
+# endregion [Constants]
 
 # region [Types]
 
 WAL_HOOK_TYPE: TypeAlias = Optional[Callable[["GidAPSWDatabase", apsw.Connection, str, int], int]]
 
 PROFILE_HOOK_TYPE: TypeAlias = Optional[Callable[["GidAPSWDatabase", str, int], None]]
 
@@ -325,15 +326,15 @@
     def _setup_db_path(self, overwrite: bool = False) -> None:
         if self.db_path is not None:
             self.db_path.parent.mkdir(exist_ok=True, parents=True)
             if overwrite is True:
                 self.db_path.unlink(missing_ok=True)
 
     def _set_page_size(self):
-        print("setting page size")
+        log.debug("setting page size")
         wal_mode = False
         conn: apsw.Connection = self.connection()
         journal_mode = conn.execute("PRAGMA journal_mode;").fetchone()[0]
         if journal_mode.casefold() == "wal":
             wal_mode = True
         page_size = next((i[1] for i in self._pragmas if i[0] == "page_size"), None)
 
@@ -383,22 +384,22 @@
     def _post_setup(self) -> None:
         self.pragma_info = PragmaInfo(self).fill_with_data()
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(database_name={self.db_file_name!r}, setup_status={self.setup_status.name!r})"
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
 
     def run_setup(db):
         script_path = Path(r"D:\Dropbox\hobby\Modding\Programs\Github\My_Repos\GidAppTools\tests\gid_database\sqlite\data\simple_db_setup.sql")
         script = script_path.read_text(encoding='utf-8', errors='ignore')
         db.execute(peewee.SQL(script))
     x = GidAPSWDatabase(MEMORY_DB_PATH)
     x.setup(data_setup=run_setup)
     with x:
         print(x.execute(peewee.SQL('SELECT "Person"."name", "Country"."name" FROM "Person"  INNER JOIN "Country"  ON "Country"."id"=="Person"."country"')).fetchall())
     pp(x.pragma_info.pragma_data)
 
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/constants.py` & `gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 from frozendict import frozendict
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 STD_DEFAULT_PRAGMAS = frozendict({
     "wal_autocheckpoint": 1_000,
     "auto_vacuum": 2,
     "cache_size": -1 * 256_000,  # 128mb
     "journal_mode": 'WAL',
     "synchronous": 0,
@@ -53,13 +53,13 @@
                                      "json_contains": True,
                                      "bloomfilter": False,
                                      "regexp_function": True})
 
 
 MEMORY_DB_PATH = ":memory:"
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/commit_hook_functions.py` & `gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/commit_hook_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 from typing import TYPE_CHECKING
 from pathlib import Path
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     ...
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/profile_hook_functions.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/application_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,48 +3,48 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 from pathlib import Path
 
-# * Gid Imports ----------------------------------------------------------------------------------------->
-from gidapptools.general_helper.conversion import ns_to_s, number_to_pretty
+# * Qt Imports --------------------------------------------------------------------------------------->
+import PySide6
+from PySide6.QtWidgets import QWidget, QApplication
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
-    ...
+    pass
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
-
+# endregion [Constants]
 
-def print_profile_hook(db, stmt: str, time_taken: int):
 
-    time_taken = ns_to_s(time_taken)
-    time_taken = number_to_pretty(time_taken) + " s"
-    print(f"Executed {stmt!r} in {time_taken}", flush=True)
-# region[Main_Exec]
+class ApplicationInfoWidget(QWidget):
 
+    def __init__(self, app: QApplication, parent: Optional[PySide6.QtWidgets.QWidget] = None) -> None:
+        self.app = app
+        super().__init__(parent)
 
+        # region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/rollback_hook_functions.py` & `gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/rollback_hook_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 from typing import TYPE_CHECKING
 from pathlib import Path
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     ...
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/update_hook_functions.py` & `gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/update_hook_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 from typing import TYPE_CHECKING
 from pathlib import Path
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     ...
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/wal_hook_functions.py` & `gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/wal_hook_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 from typing import TYPE_CHECKING
 from pathlib import Path
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     ...
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_database/orm_peewee/sqlite/pragma_info.py` & `gidapptools-0.5.0/gidapptools/gid_database/orm_peewee/sqlite/pragma_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,40 +9,42 @@
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import sys
 from typing import TYPE_CHECKING, Union, TypeVar
 from pathlib import Path
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 from frozendict import frozendict
+from gidapptools.gid_logger.logger import get_logger
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gid_database.orm_peewee.sqlite.apsw_database import GidAPSWDatabase
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
+log = get_logger(__name__)
 
-# endregion[Constants]
+# endregion [Constants]
 
 x = {'analysis_limit': 100000,
      'application_id': 0,
      'auto_vacuum': 2,
      'automatic_index': 1,
      'busy_timeout': 0,
      'cache_size': -128000,
@@ -180,22 +182,23 @@
         return tuple(i[0].strip() for i in self.database.connection().execute("PRAGMA module_list"))
 
     def fill_with_data(self) -> Self:
         self._all_pragma_names = self._get_all_pragma_names()
         self._pragma_data = self._get_pragma_data()
         self._compile_options = self._get_compile_options()
         self._module_list = self._get_module_list()
+        log.info("finished filling %r with data", self)
         return self
 
     def reset(self) -> Self:
         self._all_pragma_names = None
         self._pragma_data = None
         self._compile_options = None
         self._module_list = None
-
+        log.info("reset %r", self)
         return self
 
     def __getitem__(self, key: str) -> Union[str, int]:
         return self.pragma_data[key]
 
     def get(self, key: str, default: _GET_DEFAULT_TYPE = None) -> Union[_GET_DEFAULT_TYPE, int, str]:
         try:
@@ -203,12 +206,15 @@
         except KeyError:
             return default
 
     def on_pragma_set(self, pragma_name: str, value: Union[str, int, None]) -> None:
         if pragma_name in self.pragma_data:
             self._pragma_data[pragma_name] = value
 
+    def __repr__(self) -> str:
+        return f'{self.__class__.__name__}(database={self.database!r})'
+
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_logger/enums.py` & `gidapptools-0.5.0/gidapptools/gid_logger/enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,34 +7,35 @@
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import inspect
 import logging
 import warnings
 from enum import Enum
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, Iterable
 from pathlib import Path
+from functools import partial
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def _add_new_logging_level(name: str, value: int) -> None:
     if (name in logging._nameToLevel and value in logging._levelToName) and (logging._nameToLevel.get(name) == value and logging._levelToName.get(value) == name):
         return
     if name not in logging._nameToLevel:
         if logging._levelToName.get(value) is not None:
@@ -66,22 +67,37 @@
     return text.center(width)
 
 
 def _align_right(text: str, width: int = 0) -> str:
     return text.rjust(width)
 
 
+def _align_left_extra_padded(text: str, width: int = 0, amount_extra_padding: int = 1) -> str:
+    extra_padding = " " * amount_extra_padding
+    return (extra_padding + text).ljust(width)
+
+
+def _align_none(text: str, width: int = 0) -> str:
+    return text
+
+
 class LoggingSectionAlignment(Enum):
-    LEFT = (_align_left, "<")
-    CENTER = (_align_center, "^")
-    RIGHT = (_align_right, ">")
+    NONE = (_align_none, ("none",))
+
+    LEFT = (_align_left, ("<",))
+    CENTER = (_align_center, ("^",))
+    RIGHT = (_align_right, (">",))
+
+    LEFT_EXTRA_PADDED_ONCE = (partial(_align_left_extra_padded, amount_extra_padding=1), ("<+1", "l_pad_1"))
+    LEFT_EXTRA_PADDED_TWICE = (partial(_align_left_extra_padded, amount_extra_padding=2), ("<+2", "l_pad_2"))
+    LEFT_EXTRA_PADDED_THRICE = (partial(_align_left_extra_padded, amount_extra_padding=3), ("<+3", "l_pad_3"))
 
-    def __init__(self, align_func: Callable[[str, Optional[int]], str], aliases: str = "") -> None:
+    def __init__(self, align_func: Callable[[str, Optional[int]], str], aliases: Iterable = None) -> None:
         self.align_func = align_func
-        self.aliases = set(aliases)
+        self.aliases = set(aliases) if aliases else set()
 
     def align(self, text: str, width: int = 0) -> str:
         return self.align_func(text, width)
 
     @classmethod
     def _missing_(cls, value: object) -> Any:
         if isinstance(value, str):
@@ -131,11 +147,11 @@
     def __str__(self) -> str:
         return self.name
 
 
 _check_if_all_levels_are_in_LoggingLevel()
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_logger/fake_logger.py` & `gidapptools-0.5.0/gidapptools/gid_logger/fake_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 from rich.console import Console as RichConsole
 from rich.console import JustifyMethod
 from rich.logging import LogRender
 from rich.measure import measure_renderables
 from rich.protocol import is_renderable
 from rich.containers import Renderables
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 CONSOLE = RichConsole(soft_wrap=True)
 
 
 def dprint(*args, **kwargs):
     CONSOLE.print(*args, **kwargs)
     CONSOLE.rule()
@@ -221,12 +221,12 @@
         if is_renderable(in_obj):
             return in_obj
         return str(in_obj)
 
 
 fake_logger = FakeLogger(as_panel=False, dynamic_panel_title="all", default_justify=None)
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_logger/formatter.py` & `gidapptools-0.5.0/gidapptools/gid_logger/formatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,31 +22,31 @@
 from gidapptools.gid_logger.enums import LoggingLevel, LoggingSectionAlignment
 from gidapptools.general_helper.string_helper import StringCase, StringCaseConverter
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gid_logger.records import LOG_RECORD_TYPES
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def get_all_func_names(file: Path, recursive: bool = True):
     import ast
 
     def _get_names(source_file: Path) -> list[str]:
         root = ast.parse(source_file.read_text(encoding='utf-8', errors='ignore'))
@@ -88,20 +88,25 @@
 
 
 class AbstractLoggingStyleSection:
     default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.LEFT
     default_width: int = 0
     default_text: str = str(None)
 
+    __slots__ = ("position",
+                 "width",
+                 "alignment")
+
     def __init__(self,
                  position: int = None,
                  width: int = None,
                  alignment: Union[LoggingSectionAlignment, str] = None) -> None:
         self.position = position
         self.width = width or self.default_width
+
         if alignment is None:
             self.alignment = self.default_alignment
         elif isinstance(alignment, str):
             self.alignment = LoggingSectionAlignment(alignment)
         else:
             self.alignment = alignment
 
@@ -133,14 +138,18 @@
 class TimeSection(AbstractLoggingStyleSection):
 
     local_timezone: timezone = get_localzone()
     default_time_format = '%Y-%m-%d %H:%M:%S'
     default_msec_format = '.{msec:03.0f}'
     default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.LEFT
 
+    __slots__ = ("time_zone",
+                 "time_format",
+                 "msec_format")
+
     def __init__(self,
                  position: int = None,
                  time_zone: timezone = None,
                  time_format: str = None,
                  msec_format: str = None,
                  width: int = None,
                  alignment: Union[LoggingSectionAlignment, str] = None) -> None:
@@ -173,58 +182,77 @@
         if self.time_format.casefold() == "isoformat":
             return time_value.isoformat(timespec='seconds') + self.msec_format.format(msec=msec_value)
         return (time_value.strftime(self.time_format) + msec_string + time_value.strftime(" %Z")).strip()
 
 
 class LevelSection(AbstractLoggingStyleSection):
     default_case: StringCase = StringCase.UPPER
-    default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.CENTER
-    default_width: int = max(len(i) for i in LoggingLevel._member_names_) + 4
+    default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.LEFT_EXTRA_PADDED_ONCE
+    default_width: int = max(len(i) for i in LoggingLevel._member_names_) + 2
+    __slots__ = ("case",
+                 "_formated_value_cache")
 
     def __init__(self,
                  position: int = None,
                  case: StringCase = None,
                  width: int = None,
                  alignment: Union[LoggingSectionAlignment, str] = None) -> None:
         super().__init__(position=position, alignment=alignment, width=width)
         if case is None:
             self.case = self.default_case
         elif isinstance(case, str):
             self.case = StringCase(case)
         else:
             self.case = case
 
+        self._formated_value_cache: dict[str, str] = {}
+
     def get_formated_value(self, record: "LOG_RECORD_TYPES") -> str:
-        level_name = StringCaseConverter.convert_to(record.levelname, self.case)
         try:
-            if record.extras.get("is_qt", False) is True:
-                level_name = StringCaseConverter.convert_to("Qt", self.case) + level_name
-        except AttributeError:
-            pass
-        return level_name
+            is_qt = record.extras["is_qt"]
+
+        except (AttributeError, KeyError):
+            is_qt = False
+
+        raw_level_name = record.levelname
+
+        if is_qt is True:
+            raw_level_name = "Qt_" + raw_level_name
+
+        try:
+            return self._formated_value_cache[raw_level_name]
+        except KeyError:
+            formated_level_name = StringCaseConverter.convert_to(raw_level_name, self.case)
+            self._formated_value_cache[raw_level_name] = formated_level_name
+
+            return formated_level_name
 
 
 class ThreadSection(AbstractLoggingStyleSection):
     default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.CENTER
     default_width: int = 20
+    __slots__ = tuple()
 
     def get_formated_value(self, record: "LOG_RECORD_TYPES") -> str:
         return record.threadName
 
 
 class LineNumberSection(AbstractLoggingStyleSection):
     default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.CENTER
     default_width: int = 5
+    __slots__ = tuple()
 
     def get_formated_value(self, record: "LOG_RECORD_TYPES") -> str:
         return record.lineno
 
 
 class PathSection(AbstractLoggingStyleSection):
     default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.LEFT
+    __slots__ = ("with_extension",
+                 "_width_cache")
 
     def __init__(self,
                  position: int = None,
                  with_extension: bool = True,
                  width: int = None,
                  alignment: Union[LoggingSectionAlignment, str] = None) -> None:
         super().__init__(position=position, width=self.width_from_env, alignment=alignment)
@@ -247,76 +275,69 @@
             path = path.with_suffix('')
 
         return './' + path.as_posix()
 
 
 class LoggerNameSection(AbstractLoggingStyleSection):
     default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.LEFT
+    default_width: int = 20
+    __slots__ = tuple()
 
     def __init__(self,
                  position: int = None,
                  width: int = None,
                  alignment: Union[LoggingSectionAlignment, str] = None) -> None:
-        super().__init__(position=position, width=self.width_from_env, alignment=alignment)
-        self._width_cache: int = width or None
-
-    def width_from_env(self) -> int:
-        if self._width_cache is None:
-            self._width_cache = int(os.getenv("MAX_MODULE_NAME_LEN", "20"))
-        return self._width_cache
+        super().__init__(position=position, width=width, alignment=alignment)
 
     def get_formated_value(self, record: "LOG_RECORD_TYPES") -> str:
         if record.extras.get("module", None) is not None:
             return record.extras["module"]
         return record.name
 
 
 class FunctionNameSection(AbstractLoggingStyleSection):
     default_alignment: LoggingSectionAlignment = LoggingSectionAlignment.LEFT
-    default_width: int = int(os.getenv("MAX_FUNC_NAME_LEN", "10"))
+    default_width: int = 20
     default_text: str = "-"
+    __slots__ = tuple()
 
-    def __init__(self) -> None:
-        super().__init__(width=self.width_from_env)
-        self._width_cache: int = None
-
-    def width_from_env(self) -> int:
-        if self._width_cache is None:
-            self._width_cache = int(os.getenv("MAX_FUNC_NAME_LEN", "10"))
-        return self._width_cache
+    def __init__(self, width: int = None) -> None:
+        super().__init__(width=width)
 
     def get_formated_value(self, record: "LOG_RECORD_TYPES") -> str:
         if record.funcName == "<module>":
             return self.default_text
         if record.extras.get("function_name", None) is not None:
             return record.extras["function_name"]
         return record.funcName
 
 
 class ExtrasSection(AbstractLoggingStyleSection):
+    __slots__ = tuple()
 
     def __init__(self) -> None:
         super().__init__(width=100)
 
     def get_formated_value(self, record: "LOG_RECORD_TYPES") -> str:
         try:
             extras = record.extras
         except AttributeError:
             return ""
 
         return ' + '.join(f"{k}={v!r}" for k, v in extras.items())
 
 
 class PackageNameSection(AbstractLoggingStyleSection):
+    __slots__ = tuple()
 
     def __init__(self,
                  position: int = None,
                  width: int = None,
                  alignment: Union[LoggingSectionAlignment, str] = None) -> None:
-        super().__init__(position, width or 10, alignment)
+        super().__init__(position, width or 12, alignment)
 
     def get_formated_value(self, record: "LOG_RECORD_TYPES") -> str:
 
         name_parts = record.name.split('.')
 
         package_name = name_parts[0]
 
@@ -327,14 +348,19 @@
             pass
         return package_name
 
 
 class AbstractSectionLoggingStyle(ABC):
     default_separator: str = " | "
     default_message_start_indicator: str = ' ||--> '
+    __slots__ = ("sections",
+                 "sorted_sections",
+                 "separator",
+                 "message_start_indicator",
+                 "message_section")
 
     def __init__(self, sections: Iterable[Union[str, AbstractLoggingStyleSection]], separator: str = None, message_start_indicator: str = None, message_section: AbstractLoggingStyleSection = None):
         self.sections = self._handle_sections(sections)
         self.sorted_sections: tuple[AbstractLoggingStyleSection] = self.sort_sections()
         self.separator = separator or self.default_separator
         self.message_start_indicator = message_start_indicator or self.default_message_start_indicator
         self.message_section = message_section
@@ -375,14 +401,15 @@
         _out = {}
         for klass in AbstractLoggingStyleSection.__subclasses__():
             _out[klass.___section_name___] = klass
         return _out
 
 
 class GidSectionLoggingStyle(AbstractSectionLoggingStyle):
+    __slots__ = tuple()
 
     def validate(self) -> None:
         if any(isinstance(i, AbstractLoggingStyleSection) is False for i in self.sections):
             raise ValueError("invalid format")
 
     def _format(self, record: "LOG_RECORD_TYPES") -> str:
 
@@ -422,28 +449,43 @@
 
     def format_exception(self, record: "LOG_RECORD_TYPES") -> "LOG_RECORD_TYPES":
         if record.exc_info:
             if not record.exc_text:
                 record.exc_text = self.formatException(ei=record.exc_info)
         return record
 
+    def modify_meta_record(self, record: "LOG_RECORD_TYPES") -> "LOG_RECORD_TYPES":
+
+        if getattr(record, "is_meta", False) is False:
+            return record
+
+        record.name = "__META__"
+        record.module = "-"
+        record.funcName = "-"
+        record.lineno = "-"
+        extras = getattr(record, "extras", {})
+        extras["module"] = "-"
+        record.extras = extras
+        return record
+
     def format(self, record: "LOG_RECORD_TYPES") -> str:
         record = self.set_time(record=record)
+        record = self.modify_meta_record(record)
         text = self.format_message(record=record)
         record = self.format_exception(record=record)
         if record.exc_text:
             if text[-1:] != "\n":
                 text = text + "\n"
             text = text + record.exc_text
         if record.stack_info:
             if text[-1:] != "\n":
                 text = text + "\n"
             text = text + self.format_stack(record.stack_info)
         return text
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_logger/handler.py` & `gidapptools-0.5.0/gidapptools/gid_logger/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 from gidapptools.general_helper.regex.datetime_regex import datetime_format_to_regex
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
     from gidapptools.gid_logger.records import LOG_RECORD_TYPES
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 DEFAULT_MAX_BYTES = human2bytes("5 mb")
 
 
 class BaseFileNameTemplate(ABC):
 
@@ -229,13 +229,13 @@
         return _out
 
     def __len__(self) -> int:
         _out = 0
         for store in self.table.values():
             _out += len(store)
         return _out
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_logger/misc.py` & `gidapptools-0.5.0/gidapptools/gid_logger/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,45 +16,48 @@
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gid_logger.logger import get_logger, get_meta_logger
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gid_logger.records import LOG_RECORD_TYPES
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class ProhibitiveSingletonMeta(type):
     _instance = None
 
     def __call__(cls, *args, **kwargs):
         if cls._instance is not None:
             raise RuntimeError(f"There can only be one instance of {cls.__name__}")
         cls._instance = super(ProhibitiveSingletonMeta, cls).__call__(*args, **kwargs)
         return cls._instance
 
 
 class QtMessageHandler(metaclass=ProhibitiveSingletonMeta):
     received_records: list["LOG_RECORD_TYPES"] = []
+    __slots__ = ("msg_split_regex",
+                 "is_installed",
+                 "_old_messagehandler")
 
     def __init__(self) -> None:
         self.msg_split_regex = re.compile(r"(?P<q_class>.*)\:\:(?P<q_method>.*)\:(?P<actual_message>.*)")
         self.is_installed: bool = False
         self._old_messagehandler = None
 
     def install(self, overwrite_install: bool = False) -> "QtMessageHandler":
@@ -111,12 +114,12 @@
         log_level = self.mode_to_log_level(mode)
         msg, extras = self.modify_message(message)
         record = logger.makeRecord(logger.name, log_level, msg=msg, extra=extras, exc_info=None, args=None, ** context_data)
         logger.handle(record)
         self.received_records.append(record)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_logger/records.py` & `gidapptools-0.5.0/gidapptools/gid_logger/records.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,38 +14,40 @@
 from enum import Enum
 from typing import Any, Union, Callable
 from pathlib import Path
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gid_logger.enums import LoggingLevel
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 logging.basicConfig()
 log = logging.getLogger(__name__)
 
 log.setLevel(LoggingLevel.DEBUG)
-# endregion[Constants]
+# endregion [Constants]
 
 
 class GidLogRecordFactory:
     activation_lock = threading.RLock()
+    __slots__ = ("special_records_registry",
+                 "original_factory")
 
     def __init__(self) -> None:
         self.special_records_registry: dict[str, logging.LogRecord] = {}
         self.original_factory: Callable = None
 
     def is_active(self) -> bool:
         return logging.getLogRecordFactory() is self
@@ -115,12 +117,12 @@
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.extras = {}
 
 
 LOG_RECORD_TYPES = Union[logging.LogRecord, GidBaseLogRecord]
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_parsing/py_log_parsing.py` & `gidapptools-0.5.0/gidapptools/gid_parsing/universal/datetime_elements.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,117 +4,122 @@
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
+from datetime import datetime, timezone, timedelta
+from operator import add
+from functools import reduce, cached_property
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 import pyparsing as ppa
 import pyparsing.common as ppc
+from dateutil.tz import gettz
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gid_parsing.tokens.base_tokens import BaseTokenWithPos
-from gidapptools.gid_parsing.universal.datetime_elements import get_grammar_from_dt_format
-from gidapptools.gid_parsing.universal.character_elements import Ligatures, BaseElements
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-class LineNumberToken(BaseTokenWithPos):
-
-    def __init__(self, start: int, end: int, value: int) -> None:
-        super().__init__(start, end)
-        self.line_number = value
-
-
-class LogLevelToken(BaseTokenWithPos):
-
-    def __init__(self, start: int, end: int, value: str) -> None:
-        super().__init__(start, end)
-        self.log_level = value
-
-
-class ThreadNameToken(BaseTokenWithPos):
-
-    def __init__(self, start: int, end: int, value: str) -> None:
-        super().__init__(start, end)
-        self.thread_name = value
-
-
-class ModuleNameToken(BaseTokenWithPos):
-
-    def __init__(self, start: int, end: int, value: str) -> None:
-        super().__init__(start, end)
-        self.module_name = value
-        self.module_name_parts = tuple(self.module_name.split('.'))
-
-    @property
-    def parent_module_name(self) -> str:
-        try:
-            return self.module_name_parts[-2]
-        except IndexError:
-            return "__main__"
-
-
-class FunctionNameToken(BaseTokenWithPos):
-
-    def __init__(self, start: int, end: int, value: str) -> None:
-        super().__init__(start, end)
-        self.function_name = value
-
-
-class MessageToken(BaseTokenWithPos):
-
-    def __init__(self, start: int, end: int, value: str) -> None:
-        super().__init__(start, end)
-        self.message = value
-
-
-class GeneralGrammar:
-    _cached_grammar: ppa.ParserElement = None
-
-    @property
-    def ___grammar___(self) -> ppa.ParserElement:
-        if self._cached_grammar is None:
-            self.__class__._cached_grammar = self._construct_grammar()
-        return self._cached_grammar
-
-    def _construct_grammar(self):
-        non_pipe_printables = ppa.printables.replace("|", "")
-        time_stamp_part = get_grammar_from_dt_format("%Y-%m-%d %H:%M:%S.%f %Z")("time_stamp")
-        line_number_part = ppa.locatedExpr(ppa.Word(ppa.nums).set_parse_action(ppc.convert_to_integer)).set_parse_action(LineNumberToken.from_parse_action)("line_number")
-        level_part = ppa.locatedExpr(ppa.Keyword("DEBUG") | ppa.Keyword("INFO") | ppa.Keyword("CRITICAL") | ppa.Keyword("ERROR")).set_parse_action(LogLevelToken.from_parse_action)("level")
-        thread_name_part = ppa.locatedExpr(ppa.Word(non_pipe_printables)("thread")).set_parse_action(ThreadNameToken.from_parse_action)("thread")
-        module_name_part = ppa.locatedExpr(ppa.Word(non_pipe_printables)).set_parse_action(ModuleNameToken.from_parse_action)("module")
-        function_name_part = ppa.locatedExpr(ppa.Word(non_pipe_printables)).set_parse_action(FunctionNameToken.from_parse_action)("function")
-        return time_stamp_part + BaseElements.pipe + line_number_part + BaseElements.pipe + level_part + BaseElements.pipe + thread_name_part + BaseElements.pipe + \
-            module_name_part + BaseElements.pipe + function_name_part + BaseElements.pipe + BaseElements.pipe + Ligatures.big_arrow_right + ppa.locatedExpr(ppa.rest_of_line).set_parse_action(MessageToken.from_parse_action)("message")
-
-    def __call__(self, text: str) -> dict[str, BaseTokenWithPos]:
-        return self.___grammar___.parse_string(text, parse_all=True).as_dict()
-
-
-# region[Main_Exec]
+def microsecond_parse_action(tokens):
+    miliseconds_string = tokens[0]
+    while len(miliseconds_string) < 6:
+        miliseconds_string += "0"
+    return int(miliseconds_string)
+
+
+datetime_format_mapping: dict[str, ppa.ParserElement] = {"%Y": ppa.Regex(r"\d{4}").set_parse_action(ppc.convert_to_integer)("year"),
+                                                         "%m": ppa.Regex(r"[01]?\d").set_parse_action(ppc.convert_to_integer)("month"),
+                                                         "%d": ppa.Regex(r"[0123]?\d").set_parse_action(ppc.convert_to_integer)("day"),
+                                                         "%H": ppa.Regex(r"[012]?\d").set_parse_action(ppc.convert_to_integer)("hour"),
+                                                         "%M": ppa.Regex(r"[0-5]?\d").set_parse_action(ppc.convert_to_integer)("minute"),
+                                                         "%S": ppa.Regex(r"[0-5]?\d").set_parse_action(ppc.convert_to_integer)("second"),
+                                                         "%f": ppa.Regex(r"\d+").set_parse_action(microsecond_parse_action)("microsecond"),
+                                                         "%Z": ppa.Combine(ppa.Word(ppa.alphas) + ppa.Optional(ppa.one_of(["+", "-"]) + ppa.Word(ppa.nums) + ppa.Literal(":") + ppa.Word(ppa.nums)))("tzinfo")}
+
+
+class DateTimeToken(BaseTokenWithPos):
+
+    def __init__(self,
+                 start: int,
+                 end: int,
+                 year: int,
+                 month: int,
+                 day: int,
+                 hour: int,
+                 minute: int,
+                 second: int,
+                 microsecond: int = 0,
+                 tzinfo: str = None) -> None:
+        super().__init__(start=start, end=end)
+        self.year = year
+        self.month = month
+        self.day = day
+        self.hour = hour
+        self.minute = minute
+        self.second = second
+        self.microsecond = microsecond
+        self.raw_tzinfo = tzinfo
+
+    @classmethod
+    def from_parse_action(cls, s, l, t) -> "BaseTokenWithPos":
+        data_dict = t[0].as_dict()
+        data_dict["start"] = data_dict.pop("locn_start")
+        data_dict["end"] = data_dict.pop("locn_end")
+        data_dict.pop("value")
+        return cls(**data_dict)
+
+    @cached_property
+    def tzinfo(self) -> timezone:
+        if self.raw_tzinfo is None:
+            return None
+        if self.raw_tzinfo == "UTC":
+            return timezone.utc
+
+        if self.raw_tzinfo.startswith("UTC"):
+            offset_part = self.raw_tzinfo.removeprefix("UTC").split(":")[0]
+            amount = int(offset_part[1:].strip())
+            if offset_part[0] == "-":
+                amount = amount * (-1)
+            return timezone(timedelta(hours=amount))
+
+        return gettz(self.raw_tzinfo)
+
+    def as_datetime(self) -> datetime:
+        return datetime(year=self.year, month=self.month, day=self.day, hour=self.hour, minute=self.minute, second=self.second, microsecond=self.microsecond, tzinfo=self.tzinfo)
+
+
+def get_grammar_from_dt_format(dt_format: str) -> ppa.ParserElement:
+    parts = []
+    previous_char = ""
+    for char in dt_format:
+        if previous_char == "%":
+            parts.append(datetime_format_mapping[previous_char + char])
+        elif char not in {"%", " "}:
+            parts.append(ppa.Literal(char).suppress())
+        previous_char = char
+    return ppa.locatedExpr(reduce(add, parts)).set_parse_action(DateTimeToken.from_parse_action)
 
 
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_parsing/tokens/base_tokens.py` & `gidapptools-0.5.0/gidapptools/gid_parsing/tokens/base_tokens.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class BaseToken:
 
     def __repr__(self) -> str:
         var_parts = [f"{k}={v!r}" for k, v in vars(self).items()]
         return f"{self.__class__.__name__}({', '.join(var_parts)})"
@@ -48,13 +48,13 @@
     def from_parse_action(cls, s, l, t) -> "BaseTokenWithPos":
         data_dict = t[0].as_dict()
         data_dict["start"] = data_dict.pop("locn_start")
         data_dict["end"] = data_dict.pop("locn_end")
         return cls(**data_dict)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_parsing/universal/character_elements.py` & `gidapptools-0.5.0/gidapptools/gid_parsing/universal/character_elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 import pyparsing as pp
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class BaseElements:
     comma = pp.Literal(",").suppress()
     colon = pp.Literal(":").suppress()
     semi_colon = pp.Literal(";").suppress()
     period = pp.Literal(".").suppress()
@@ -100,12 +100,12 @@
 
 
 ARROW_RIGHT = Ligatures.arrow_right
 ARROW_LEFT = Ligatures.arrow_left
 BIG_ARROW_RIGHT = Ligatures.big_arrow_right
 BIG_ARROW_LEFT = Ligatures.big_arrow_left
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_signal/interface.py` & `gidapptools-0.5.0/gidapptools/gid_signal/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 from gidapptools.gid_signal.signal_registry import signal_registry
 from gidapptools.gid_signal.signals.basic_signal import GidSignal
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gid_signal.signals.abstract_signal import AbstractSignal
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 GET_SIGNAL_LOCK = Lock()
 
 
 def get_signal(key: Hashable, klass: Optional["AbstractSignal"] = None) -> "AbstractSignal":
     klass = GidSignal if klass is None else klass
     with GET_SIGNAL_LOCK:
@@ -47,13 +47,13 @@
         if signal is None:
             signal = klass(key=key)
             signal_registry.register(signal)
 
     return signal
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_signal/signal_registry.py` & `gidapptools-0.5.0/gidapptools/gid_signal/signal_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 from pathlib import Path
 from weakref import WeakValueDictionary
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gid_signal.signals.abstract_signal import AbstractSignal
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [AppUserData]
 
 
 # endregion [AppUserData]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(os.path.dirname(__file__)).absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class SignalRegistry(WeakValueDictionary):
 
     def register(self, signal: "AbstractSignal"):
         key = signal.key
         self[key] = signal
@@ -63,12 +63,12 @@
         for key in list(self):
             del self[key]
 
 
 signal_registry = SignalRegistry()
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_signal/signals/abstract_signal.py` & `gidapptools-0.5.0/gidapptools/gid_signal/signals/abstract_signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 from typing import Any, Union, Callable, Hashable
 from pathlib import Path
 from weakref import WeakSet, WeakMethod, ref
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.utility.helper import get_qualname_or_name
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class AdaptableWeakSet(WeakSet):
 
     def add(self, item) -> None:
         if self._pending_removals:
             self._commit_removals()
@@ -106,12 +106,12 @@
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(key={self.key!r})"
 
     def __str__(self):
         return f"{self.__class__.__name__}-{self.key}(targets={self.targets!r})"
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_signal/signals/basic_signal.py` & `gidapptools-0.5.0/gidapptools/gid_signal/signals/basic_signal.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 from concurrent.futures import ThreadPoolExecutor
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.utility.helper import get_qualname_or_name
 
 from .abstract_signal import AbstractSignal
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def run_delayed(delay: Union[int, float], emit_func: Callable):
     sleep(delay)
     emit_func()
 
 
@@ -78,11 +78,11 @@
             if info.get('is_coroutine') is False:
                 task = asyncio.to_thread(target, *args, **kwargs)
             else:
                 task = target(*args, **kwargs)
             asyncio.create_task(task, name=task_name)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_utility/version_item.py` & `gidapptools-0.5.0/gidapptools/gid_utility/version_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 from typing import Union, ClassVar, Optional
 from pathlib import Path
 from functools import total_ordering
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 import attr
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 __all__ = ["VersionItem"]
 
 
 def try_convert_int(data: Union[str, int, None]) -> Union[str, int, None]:
     if data is None:
@@ -108,14 +108,14 @@
                 return True
             return False
 
         if isinstance(other, str):
             return False
         return NotImplemented
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_warning/deprecation.py` & `gidapptools-0.5.0/gidapptools/gid_warning/deprecation.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 from pathlib import Path
 from warnings import warn_explicit
 from functools import wraps
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.enums import MiscEnum
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class DeprecationWarningTypus(Enum):
     ARGUMENT = auto()
 
 
 def _replace_default_argument_w_NOTHING(func, arg_name: str, *args, **kwargs) -> inspect.BoundArguments:
@@ -85,12 +85,12 @@
             return func(*args, **kwargs)
 
         return _wrapped
 
     return _wrapper
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gid_warning/experimental.py` & `gidapptools-0.5.0/gidapptools/gid_warning/experimental.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
 from warnings import warn, warn_explicit
 from functools import wraps
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def mark_experimental(extra_message: str = ""):
     def _wrapper(func):
         @wraps(func)
         def _wrapped(*args, **kwargs):
             func_name = func.__qualname__ or func.__name__
@@ -41,14 +41,14 @@
             except Exception:
                 warn(message=message, category=UserWarning, stacklevel=4)
             return func(*args, **kwargs)
 
         return _wrapped
     return _wrapper
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/images/__init__.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/images/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 PLACEHOLDER_IMAGE = StoredImage(IMAGES_DIR.joinpath("placeholder.png"))
 DEFAULT_APP_ICON_IMAGE = StoredImage(IMAGES_DIR.joinpath("default_app_icon.png"))
 
 
 @cache
 def get_image(name: str) -> StoredImage:
-    cleaned_name = name.rsplit(".", 1)
+    cleaned_name = name.rsplit(".", 1)[0]
     for dirname, folderlist, filelist in os.walk(IMAGES_DIR):
         for file in filelist:
             if file.rsplit(".", 1)[-1] in StoredImage.allowed_extensions and file.casefold().rsplit(".", 1)[0] == cleaned_name:
                 path = Path(dirname, file)
                 image = StoredImage(path)
 
                 return image
-    raise FileNotFoundError(f"No gif with name {name!r} found.")
+    raise FileNotFoundError(f"No image with name {name!r} found.")
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/images/default_app_icon.png` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/images/default_app_icon.png`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/images/placeholder.png` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/images/placeholder.png`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/templates/about_template.jinja_html` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/templates/about_template.jinja_html`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/_data/templates/arg_doc_html_template.jinja_html` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/_data/templates/arg_doc_html_template.jinja_html`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/application.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,31 +41,31 @@
 # * Local Imports --------------------------------------------------------------------------------------->
 from gidapptools import get_meta_info
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gidapptools_qt.resources.resources_helper import PixmapResourceItem
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]-uz1
+# endregion [Constants]-uz1
 
 
 class AppArgParserResult:
 
     def __init__(self) -> None:
         self.exec_file: Path = None
         self.main_window_flags = Qt.WindowFlags()
@@ -705,13 +705,13 @@
             main_window = self._build_main_window()
             application.main_window = main_window
         if self.style_sheet_file:
             application.setStyleSheet(self.style_sheet_file.read_text(encoding='utf-8', errors='ignore'))
         return application
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
 
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/application_info.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/json_editor.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,48 +3,50 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
-from typing import TYPE_CHECKING, Optional
+from typing import Optional
 from pathlib import Path
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 import PySide6
-from PySide6.QtWidgets import QWidget, QApplication
+from PySide6.QtCore import Qt
+from PySide6.QtWidgets import QWidget, QGridLayout
 
-# * Type-Checking Imports --------------------------------------------------------------------------------->
-if TYPE_CHECKING:
-    pass
-
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
+
+
+class JsonEditorWidget(QWidget):
+
+    def __init__(self, parent: Optional[PySide6.QtWidgets.QWidget] = None, f: PySide6.QtCore.Qt.WindowFlags = None) -> None:
+        super().__init__(parent, f or Qt.WindowFlags())
+        self.setLayout(QGridLayout())
 
+    def layout(self) -> QGridLayout:
+        return super().layout()
 
-class ApplicationInfoWidget(QWidget):
 
-    def __init__(self, app: QApplication, parent: Optional[PySide6.QtWidgets.QWidget] = None) -> None:
-        self.app = app
-        super().__init__(parent)
+# region [Main_Exec]
 
-        # region[Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/application_new.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/application_new.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,43 +4,50 @@
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import sys
-from typing import Union, Iterable, Optional, Protocol
+from typing import Union, Iterable, Optional, Protocol, TYPE_CHECKING
 from pathlib import Path
 
 # * Third Party Imports --------------------------------------------------------------------------------->
 from yarl import URL
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtWidgets import QApplication
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gid_utility.version_item import VersionItem
+import sys
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+if TYPE_CHECKING:
+    from gidapptools.meta_data.meta_info.meta_info_item import MetaInfo
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class ApplicationInfo(Protocol):
     app_name: str
     app_author: str
     version: Optional[Union[str, VersionItem]]
     url: Optional[Union[str, URL]]
@@ -52,17 +59,24 @@
         super().__init__(argv or sys.argv)
         self.is_setup: bool = False
 
     @classmethod
     def is_ready(cls) -> bool:
         return cls.startingUp() is False and cls.instance().is_setup is True
 
+    def setup_from_meta_info(self,
+                             meta_info: "MetaInfo") -> Self:
+        ...
+
     def setup(self,
-              application_core_info: "ApplicationCoreInfo") -> "GidBaseApplication":
+              app_name: str = None,
+              app_author: str = None,
+              version: Union[str, "VersionItem"] = None,
+              url: Union[URL, str] = None) -> Self:
         ...
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/main_window.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/main_window.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,31 +19,31 @@
 from gidapptools.gidapptools_qt.basics.menu_bar import BaseMenuBar
 from gidapptools.gidapptools_qt.basics.status_bar import GidBaseStatusBar
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gidapptools_qt.basics.application import GidQtApplication
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class GidBaseMainWindow(QMainWindow):
 
     def __init__(self, parent: Optional[PySide6.QtWidgets.QWidget] = None, flags: PySide6.QtCore.Qt.WindowFlags = None, menu_bar: BaseMenuBar = None, status_bar: GidBaseStatusBar = None) -> None:
         super().__init__(*(i for i in [parent, flags] if i))
         self.setObjectName("MainWindow")
@@ -86,14 +86,14 @@
     def status_bar(self, status_bar: QStatusBar):
         status_bar.setParent(self)
         try:
             status_bar.setup()
         except AttributeError:
             pass
         self.setStatusBar(status_bar)
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/menu_bar.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/menu_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import ApplicationNotExistingError
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gidapptools_qt.basics.application import GidQtApplication
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class BaseMenuBar(QMenuBar):
     general_disabled_action_names: frozenset[str] = frozenset()
 
     def __init__(self, parent: Optional[QWidget] = None, auto_connect_standard_actions: bool = True) -> None:
         super().__init__(parent=parent)
@@ -151,12 +151,12 @@
         menu.setEnabled(True)
         return action
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(auto_connect_standard_actions={self.auto_connect_standard_actions!r})"
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/status_bar.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/status_bar.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,44 +17,44 @@
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import ApplicationNotExistingError
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gidapptools_qt.basics.application import GidQtApplication
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class GidBaseStatusBar(QStatusBar):
 
     def __init__(self, parent: Optional[PySide6.QtWidgets.QWidget] = None) -> None:
         super().__init__(parent)
 
     @property
     def app(self) -> "GidQtApplication":
         app = QApplication.instance()
         if app is None:
             raise ApplicationNotExistingError()
         return app
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/basics/sys_tray.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/basics/sys_tray.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 from gidapptools.errors import ApplicationNotExistingError
 from gidapptools.general_helper.enums import MiscEnum
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.gidapptools_qt.basics.application import GidQtApplication
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class MenuTitle(QFrame):
 
     def __init__(self, text: str = None, icon: Union[QIcon, QPixmap] = None, parent=None):
         super().__init__(parent=parent)
         self.setup_styling()
@@ -191,13 +191,13 @@
         try:
             return self.actions[self._normalize_action_name(key)]
         except KeyError as error:
             raise KeyError(f"No action named {key!r}") from error
 
     def get(self, key: str, default: Any = None) -> Union[QAction, Any]:
         return self.actions.get(key, default)
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
-    # endregion[Main_Exec]
+    # endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/debug/event_analyzer.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/debug/event_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,36 +10,37 @@
 import json
 import shutil
 import inspect
 from typing import Any, Union, Callable, Iterable, Optional
 from pathlib import Path
 from datetime import datetime
 from collections import defaultdict
+from gidapptools.gid_logger.logger import get_logger
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtGui import QMouseEvent, QPaintEvent, QResizeEvent, QStatusTipEvent, QPlatformSurfaceEvent, QInputMethodQueryEvent
 from PySide6.QtCore import QEvent, QChildEvent, QDynamicPropertyChangeEvent
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
-
-# endregion[Constants]
+log = get_logger(__name__)
+# endregion [Constants]
 
 
 class JsonOutputter:
 
     def __init__(self, target_folder: Path, file_stem_suffix: str = None) -> None:
         self.target_folder = target_folder
         self.specific_folder = self.target_folder.joinpath("event_specific_data")
@@ -77,20 +78,20 @@
 
 
 def _data_getter_class_name(obj: object) -> str:
     try:
         if inspect.isclass(obj):
             return obj.__name__
     except Exception as e:
-        print(e)
+        log.error(e, exc_info=True)
 
     try:
         return obj.__class__.__name__
     except Exception as e:
-        print(e)
+        log.error(e, exc_info=True)
 
     return "Not able to determine class Name".upper()
 
 
 def _data_getter_all_subclasses(obj: object) -> tuple[type]:
 
     if inspect.isclass(obj):
@@ -184,12 +185,12 @@
 
     def __call__(self, event: QEvent) -> None:
         text_or_data = self.analyze(event)
         if text_or_data is not None:
             self.output(text_or_data)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/dialogs/app_info_dialog.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/dialogs/app_info_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 from pathlib import Path
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtGui import QFont
 from PySide6.QtCore import Qt, QSize
 from PySide6.QtWidgets import QLabel, QDialog, QLineEdit, QVBoxLayout
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class AppInfoDialog(QDialog):
 
     def __init__(self) -> None:
         super().__init__()
 
@@ -67,13 +67,13 @@
         self.verticalLayout = QVBoxLayout(self)
 
         for label, data in self.parts:
             self.verticalLayout.addWidget(label)
             self.verticalLayout.addWidget(data)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/command_line_parser/parser.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/command_line_parser/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 from typing import TYPE_CHECKING, Any
 from pathlib import Path
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     pass
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class GidBaseCommandLineParser(argparse.ArgumentParser):
 
     def __init__(self,
                  prog: str = None,
                  fromfile_prefix_chars: str = None,
@@ -49,13 +49,13 @@
                          argument_default=argument_default,
                          conflict_handler=conflict_handler,
                          add_help=add_help,
                          allow_abbrev=allow_abbrev,
                          exit_on_error=exit_on_error)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/misc.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,36 +4,37 @@
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
-
+from typing import TypeVar
+from collections.abc import Mapping, Iterable
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtGui import QScreen
 from PySide6.QtWidgets import QWidget, QApplication
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def center_window(window: QWidget, allow_window_resize: bool = True) -> QWidget:
     app = QApplication.instance()
     if allow_window_resize is True:
         window.resize(window.sizeHint())
 
@@ -42,14 +43,36 @@
     screen_center = screen_geo.center()
 
     window_geo = window.frameGeometry()
     window_geo.moveCenter(screen_center)
     window.move(window_geo.topLeft())
     return window
 
-# region[Main_Exec]
+
+T_WIDGET = TypeVar("T_WIDGET", bound=QWidget)
+
+
+def batch_modify_widget(widget: T_WIDGET, **kwargs) -> T_WIDGET:
+    for method_name, method_arguments in kwargs.items():
+        method = getattr(widget, method_name)
+
+        if isinstance(method_arguments, Mapping):
+            method(**method_arguments)
+
+        elif isinstance(method_arguments, Iterable) and not isinstance(method_arguments, str):
+            method(*method_arguments)
+
+        elif method_arguments is ...:
+            method()
+
+        else:
+            method(method_arguments)
+
+    return widget
+
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/object_name.py` & `gidapptools-0.5.0/gidapptools/general_helper/output_helper/rich_helper/rich_styles.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,41 +4,35 @@
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from pathlib import Path
-
-# * Qt Imports --------------------------------------------------------------------------------------->
-from PySide6.QtCore import QObject
-
-# endregion[Imports]
+from rich.console import Console as RichConsole
+from rich.style import Style
+from rich.default_styles import DEFAULT_STYLES
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
-
-
-def set_std_object_name(obj: QObject):
-    name = obj.__class__.__name__
-    obj.setObjectName(name)
+# endregion [Constants]
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/window_geometry_helper.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/window_geometry_helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,41 +19,45 @@
     pass
 else:
     pass
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     ...
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def move_to_center_of_screen(widget: QWidget, screen: QScreen = None) -> None:
     screen = screen or QApplication.instance().screenAt(widget.cursor().pos())
 
     screen_center = screen.availableGeometry().center()
-    widget_geometry = widget.geometry()
-    widget_geometry.moveCenter(screen_center)
-    widget.setGeometry(widget_geometry)
+    widget_frame_geometry = widget.frameGeometry()
 
+    widget_frame_geometry.moveCenter(screen_center)
 
-# region[Main_Exec]
+    # widget.setGeometry(widget_frame_geometry)
+
+    # widget.move(screen_center)
+
+
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/helper/window_reference_keeper.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/helper/window_reference_keeper.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 from threading import RLock
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtGui import Qt, QCloseEvent
 from PySide6.QtCore import Signal
 from PySide6.QtWidgets import QWidget, QApplication
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class SecondaryWindow(QWidget):
     close_signal = Signal(QWidget)
 
     def __init__(self, parent: QWidget = None, f: Qt.WindowFlags = None, name: str = None) -> None:
         super().__init__(*[i for i in [parent, f] if i is not None])
@@ -82,12 +82,12 @@
                 pass
 
     def remove_already_closed(self) -> None:
         with self.lock:
             self._open_windows = [w for w in self._open_windows if w.is_closed is False]
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/layouts/vertical_form_layout.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/layouts/vertical_form_layout.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from typing import Optional
 from pathlib import Path
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtWidgets import QLayout, QWidget
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class VerticalFormLayout(QLayout):
 
     def __init__(self, parent: Optional[QWidget] = None) -> None:
         super().__init__(parent)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/models/basic_model.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/models/basic_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from typing import Any, Union, Callable, Iterable, Optional
 from pathlib import Path
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 import PySide6
-from PySide6.QtCore import Qt, QAbstractTableModel
+from PySide6.QtCore import Qt, QAbstractTableModel, QModelIndex, QPersistentModelIndex, QObject
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
-PYSIDE_INDEX_TYPE = Union[PySide6.QtCore.QModelIndex, PySide6.QtCore.QPersistentModelIndex]
+PYSIDE_INDEX_TYPE = Union[QModelIndex, QPersistentModelIndex]
 
 
 class BasicTableModel(QAbstractTableModel):
 
-    def __init__(self, parent: Optional[PySide6.QtCore.QObject] = None) -> None:
+    def __init__(self, parent: Optional[QObject] = None) -> None:
         super().__init__(parent=parent)
         self.data_dispatch: dict[Qt.ItemDataRole:Callable[[PYSIDE_INDEX_TYPE], Any]] = {}
         self.header_dispatch: dict[Qt.ItemDataRole:Callable[[int, Qt.Orientation], Any]] = {}
         self.content: Iterable[object] = None
 
     def data(self, index: PYSIDE_INDEX_TYPE, role: int = ...) -> Any:
         try:
@@ -56,14 +56,14 @@
             pass
 
     def rowCount(self, parent: PYSIDE_INDEX_TYPE = None) -> int:
         if self.content is None:
             return 0
         return len(self.content)
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/resources/placeholder.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/resources/placeholder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtGui import QIcon, QPixmap
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gidapptools_qt._data.images import PLACEHOLDER_IMAGE, DEFAULT_APP_ICON_IMAGE, StoredImage
 from gidapptools.gidapptools_qt.resources.resources_helper import PixmapResourceItem
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class GidQtPlaceholderImage:
 
     def __init__(self, stored_image: StoredImage) -> None:
         self.stored_image = stored_image
         self._pixmap: QPixmap = None
@@ -53,13 +53,13 @@
         if self._icon is None:
             self._icon = QIcon(self.pixmap)
         return self._icon
 
 
 QT_PLACEHOLDER_IMAGE = PixmapResourceItem(PLACEHOLDER_IMAGE.path)
 QT_DEFAULT_APP_ICON_IMAGE = PixmapResourceItem(DEFAULT_APP_ICON_IMAGE.path)
-# region[Main_Exec]
+# region [Main_Exec]
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/resources/resources_helper.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/resources/resources_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 from pathlib import Path
 from threading import RLock
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtGui import QIcon, QImage, QMovie, QPixmap
 from PySide6.QtCore import Qt, QFile, QSize, QByteArray
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 def make_ressource_name(in_item_name: str, in_section_name: str = None) -> str:
     item_name = in_item_name.rsplit('.', 1)[0]
     if in_section_name:
         return f":/{in_section_name}/{item_name}"
     return f":/{item_name}"
@@ -162,14 +162,14 @@
     def __getattr__(cls, name: str) -> "ResourceItem":
         if any(name.casefold().endswith(f"_{cat}") for cat in cls.categories):
             cat_name = name.split('_')[-1].casefold()
             cls.missing_items[cat_name].add(name)
             return cls.placeholder_image
         raise AttributeError(f"{cls.__name__} has not attribute {name!r}")
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/app_log_viewer.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/app_log_viewer.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,52 +5,55 @@
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from typing import Optional
 from pathlib import Path
-
+import logging
+import re
 # * Third Party Imports --------------------------------------------------------------------------------->
 from pyparsing.exceptions import ParseBaseException
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 import PySide6
 from PySide6.QtGui import QFont, QColor, QTextCharFormat, QSyntaxHighlighter
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QLabel, QWidget, QGroupBox, QTextEdit, QFormLayout, QGridLayout
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gid_logger.logger import get_main_logger
 from gidapptools.general_helper.conversion import bytes2human
 from gidapptools.gid_parsing.py_log_parsing import GeneralGrammar
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class AppLogHighlighter(QSyntaxHighlighter):
     grammar = GeneralGrammar()
+    level_regex = re.compile(r"(?P<level>(DEBUG)|(INFO)|(WARN(ING)?)|(CRITICAL)|(ERROR))")
+    line_number_regex = re.compile(r"\| *(?P<line_number>\d+) *\|")
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.formats: dict[str, QTextCharFormat] = {}
         self.setup_formats()
 
     def setup_formats(self):
@@ -100,25 +103,31 @@
         self.formats["module"] = module_format
 
         function_format = QTextCharFormat()
         self.formats["function"] = function_format
 
     def highlightBlock(self, text: str) -> None:
 
-        try:
-            tokens = self.grammar(text)
-            background_fmt = self.formats[tokens["level"].log_level.casefold()]
-            self.setFormat(0, len(text), background_fmt)
-            for name, token in tokens.items():
-                fmt = self.formats.get(name, self.base_format)
-                fmt.setBackground(background_fmt.background())
-                self.setFormat(token.start, token.span, fmt)
+        # try:
+        #     tokens = self.grammar(text)
+        #     background_fmt = self.formats[tokens["level"].log_level.casefold()]
+        #     self.setFormat(0, len(text), background_fmt)
+        #     for name, token in tokens.items():
+        #         fmt = self.formats.get(name, self.base_format)
+        #         fmt.setBackground(background_fmt.background())
+        #         self.setFormat(token.start, token.span, fmt)
+
+        # except ParseBaseException as e:
+        # print(f"{e=} | {e.args=}", flush=True)
+
+        if match := self.level_regex.search(text):
+            self.setFormat(0, len(text), self.formats.get(match.group("level").casefold(), self.base_format))
 
-        except ParseBaseException:
-            pass
+        if match := self.line_number_regex.search(text):
+            self.setFormat(match.start("line_number"), match.end("line_number") - match.start("line_number"), self.formats["line_number"])
 
     # def highlightBlock(self, text: str) -> None:
     #     try:
     #         backgrounds = {"debug": QColor(0, 200, 0, 50),
     #                        "info": QColor(0, 0, 255, 50),
     #                        "critical": QColor(255, 200, 0, 50),
     #                        "error": QColor(255, 0, 0, 100)}
@@ -262,17 +271,17 @@
         if self.timer_id is not None:
             self.killTimer(self.timer_id)
         event.accept()
 
 
 class StoredAppLogViewer(QWidget):
 
-    def __init__(self, parent: Optional[PySide6.QtWidgets.QWidget] = None) -> None:
+    def __init__(self, parent: Optional[PySide6.QtWidgets.QWidget] = None, storage_handler: logging.Handler = None) -> None:
         super().__init__(parent)
-        self.storage_handler = get_main_logger().all_handlers["que_handlers"]["GidStoringHandler"]
+        self.storage_handler = storage_handler or get_main_logger().all_handlers["que_handlers"]["GidStoringHandler"]
         self.last_len = 0
         self.timer_id = None
 
     def setup(self) -> "StoredAppLogViewer":
         self.setLayout(QGridLayout())
         self.setWindowTitle("Application Log")
 
@@ -286,16 +295,18 @@
     def setup_widgets(self):
         self.text_widget = QTextEdit(self)
         self.text_widget.setReadOnly(True)
         self.text_widget.setLineWrapMode(QTextEdit.NoWrap)
         font: QFont = self.text_widget.font()
         font.setStyleHint(QFont.Monospace)
         font.setFamily("Consolas")
+        font.setPointSizeF(font.pointSizeF() * 1.25)
         self.text_widget.setFont(font)
-
+        self.highlighter = AppLogHighlighter()
+        self.highlighter.setDocument(self.text_widget.document())
         self.layout.addWidget(self.text_widget)
 
     @property
     def layout(self) -> QGridLayout:
         return super().layout()
 
     def gather_content(self):
@@ -319,14 +330,14 @@
         self.gather_content()
         return super().timerEvent(event)
 
     def closeEvent(self, event: PySide6.QtGui.QCloseEvent) -> None:
         if self.timer_id is not None:
             self.killTimer(self.timer_id)
         event.accept()
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/category_select_widget.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/category_select_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,31 +20,31 @@
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.string_helper import StringCase, StringCaseConverter
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     ...
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class SelectorPosition(Enum):
     TOP = auto()
     Bottom = auto()
     LEFT = auto()
     RIGHT = auto()
@@ -94,18 +94,19 @@
     def sizeHint(self) -> QSize:
         width = self.text.sizeHint().width() + self.picture.sizeHint().width()
         height = self.text.sizeHint().height() + self.picture.sizeHint().height()
         return QSize(w=width, h=height)
 
     def mousePressEvent(self, event: QtGui.QMouseEvent) -> None:
         self.setFrameStyle(QFrame.Sunken | QFrame.Panel)
-        self.clicked.emit(self.category_page_number)
+
 
     def mouseReleaseEvent(self, event: QtGui.QMouseEvent) -> None:
         self.setFrameStyle(self.base_style)
+        self.clicked.emit(self.category_page_number)
 
     @property
     def layout(self) -> QVBoxLayout:
         return super().layout()
 
     def __repr__(self) -> str:
         """
@@ -276,15 +277,15 @@
     def __repr__(self) -> str:
         """
         Basic Repr
         !REPLACE!
         """
         return f'{self.__class__.__name__}'
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     # app = QApplication()
 
     # select_widget = CategorySelectWidget(selector_position=SelectorPosition.LEFT).setup()
     # content = QTextEdit()
@@ -297,8 +298,8 @@
     # content2.category_picture = QPixmap(r"D:\Dropbox\hobby\Modding\Ressources\Icons\To_Sort_Icons\png_icons\document(1).png")
     # select_widget.add_category(content_widget=content)
     # select_widget.add_category(content_widget=content2)
     # select_widget.show()
     # app.exec()
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/hyperlink_label.py` & `gidapptools-0.5.0/gidapptools/utility/kwarg_dict.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,79 +3,81 @@
 
 Soon.
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
+import inspect
+from abc import ABCMeta
+from typing import Any, Union, Iterable, Optional
 from pathlib import Path
+from collections import UserDict
 
-# * Qt Imports --------------------------------------------------------------------------------------->
-from PySide6.QtGui import QPalette, QMouseEvent, QDesktopServices
-from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QLabel, QApplication
+# * Gid Imports ----------------------------------------------------------------------------------------->
+from gidapptools.general_helper.enums import MiscEnum
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
-class HyperlinkLabel(QLabel):
-
-    def __init__(self, link: str = None, validate: bool = False, parent=None):
-        super().__init__(parent=parent)
-        self.validate = validate
-        self.link: str = None
-        if link:
-            self.set_link(link)
-        self._set_link_color()
-
-    def _validate_link(self, link: str):
-        pass
-
-    def _modify_link(self, link: str) -> str:
-        return link
-
-    def set_link(self, link: str):
-        link = self._modify_link(link)
-        if self.validate is True:
-            self._validate_link(link)
-        self.link = link
-        self.setText(link)
-
-    def _set_link_color(self):
-        link_color = QApplication.instance().palette().color(QPalette.Button.Link)
-        r = link_color.red()
-        g = link_color.green()
-        b = link_color.blue()
-        self.setStyleSheet(f"color: rgb({', '.join(str(i) for i in [r,g,b])})")
-        self.setCursor(Qt.PointingHandCursor)
-
-    def _open_link(self):
-        QDesktopServices.openUrl(self.link)
-
-    def mousePressEvent(self, ev: QMouseEvent) -> None:
-        if ev.button() == Qt.LeftButton:
-            self._open_link()
-        else:
-            super().mousePressEvent(ev)
-# region[Main_Exec]
+class PostInitMeta(ABCMeta):
+    def __call__(cls, *args: Any, **kwargs: Any) -> Any:
+        instance = super(PostInitMeta, cls).__call__(*args, **kwargs)
+        if hasattr(instance, "_post_init"):
+            instance._post_init()
+        return instance
+
+
+class KwargDict(UserDict, metaclass=PostInitMeta):
+    # pylint: disable=useless-super-delegation
+    def __init__(self, base_defaults: dict = None, **kwargs) -> None:
+        super().__init__(base_defaults, **kwargs)
+
+    def get_kwargs_for(self, target_class: object, defaults: dict[str, Any] = None, exclude: Iterable[str] = None, overwrites: dict[str, Any] = None) -> Optional[dict[str, Any]]:
+        defaults = {} if defaults is None else defaults
+        overwrites = {} if overwrites is None else overwrites
+        exclude = set() if exclude is None else set(exclude)
+        kwarg_names = [name for name, obj in inspect.signature(target_class).parameters.items() if obj.kind is not obj.VAR_KEYWORD]
+
+        _kwargs = {}
+        for name in kwarg_names:
+            if name in exclude:
+                continue
+            if name in overwrites:
+                value = overwrites.get(name)
+            else:
+                value = self.get(name, defaults.get(name, MiscEnum.NOTHING))
+
+            if value is MiscEnum.NOTHING or value is MiscEnum.OPTIONAL:
+                continue
+            _kwargs[name] = value
+        return _kwargs
+
+    def get_many(self, keys: Union[list[str], dict[str, Any]]) -> dict[str, Any]:
+        keys = keys if isinstance(keys, dict) else {key: None for key in keys}
+        result = {}
+        for key in keys:
+            result[key] = self.get(key, keys.get(key, None))
+        return result
 
 
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/spinner_widget.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/spinner_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 # * Standard Library Imports ---------------------------------------------------------------------------->
 from typing import Union
 from pathlib import Path
 from concurrent.futures import Future
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 import PySide6
-from PySide6.QtGui import QMovie
+from PySide6.QtGui import QMovie, QColor
 from PySide6.QtCore import Qt, QSize, Signal
 from PySide6.QtWidgets import QLabel, QWidget, QPushButton, QSizePolicy, QVBoxLayout, QApplication
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.data.gifs import StoredGif, get_gif
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class BusySpinnerWidget(QLabel):
     default_gif_name: str = "busy_spinner_4.gif"
     default_spinner_size: tuple[int, int] = (75, 75)
     _stop_signal = Signal(Future)
 
@@ -67,14 +67,15 @@
             else:
                 spinner_gif = get_gif(spinner_gif)
         elif isinstance(spinner_gif, Path):
             spinner_gif = StoredGif(spinner_gif)
 
         spinner_gif_item = spinner_gif or get_gif(self.default_gif_name)
         spinner_gif = QMovie(str(spinner_gif_item.path))
+
         spinner_gif.setScaledSize(self.spinner_size)
         spinner_gif.setCacheMode(QMovie.CacheAll)
         self.setMovie(spinner_gif)
         return spinner_gif_item, spinner_gif
 
     def start(self):
         self.spinner_gif.start()
@@ -154,15 +155,15 @@
         future.add_done_callback(self.busy_spinner_widget._stop_signal.emit)
 
     def start_spinner_with_stop_signal(self, stop_signal: Signal):
         self.start_spinner()
         stop_signal.connect(self.stop_spinner)
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     app = QApplication()
     x = BusySpinnerWidget()
     x.show()
     app.exec()
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/gidapptools_qt/widgets/std_stream_widget.py` & `gidapptools-0.5.0/gidapptools/gidapptools_qt/widgets/std_stream_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 from collections import deque
 
 # * Qt Imports --------------------------------------------------------------------------------------->
 from PySide6.QtGui import QFont, QColor, QTextCharFormat, QSyntaxHighlighter
 from PySide6.QtCore import Signal, QObject
 from PySide6.QtWidgets import QWidget, QTextEdit, QGridLayout
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class StreamCaptureSignaler(QObject):
     flushed_text = Signal(str)
     flushed_items = Signal(tuple)
 
 
@@ -194,12 +194,12 @@
         return super().layout()
 
     def show(self) -> None:
         self.text_view.verticalScrollBar().setValue(self.text_view.verticalScrollBar().maximum())
         return super().show()
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/meta_data/config_kwargs.py` & `gidapptools-0.5.0/gidapptools/meta_data/config_kwargs.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.meta_data.meta_info.meta_info_item import MetaInfo
     from gidapptools.meta_data.meta_paths.meta_paths_item import MetaPaths
     meta_items_type = Union[MetaInfo, MetaPaths, object]
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class ConfigKwargs(KwargDict):
 
     def __init__(self, base_configuration: dict = None, **kwargs) -> None:
         self._path_overwrites: dict[NamedMetaPath, Path] = {}
         self.created_meta_items: dict[str, "meta_items_type"] = {}
@@ -76,13 +76,13 @@
 
     def __repr__(self) -> str:
         """
         Basic Repr
         !REPLACE!
         """
         return f'{self.__class__.__name__}'
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/meta_data/interface.py` & `gidapptools-0.5.0/gidapptools/meta_data/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 from gidapptools.general_helper.enums import MiscEnum
 from gidapptools.meta_data.meta_paths import MetaPaths, MetaPathsFactory
 from gidapptools.meta_data.config_kwargs import ConfigKwargs
 from gidapptools.general_helper.dict_helper import SafeMergeDict
 from gidapptools.abstract_classes.abstract_meta_item import AbstractMetaItem
 from gidapptools.abstract_classes.abstract_meta_factory import AbstractMetaFactory
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 META_ITEMS_TYPE = Any
 
 
 class AppMeta:
     factories: list[AbstractMetaFactory] = [MetaInfoFactory,
@@ -193,13 +193,13 @@
     return app_meta['meta_info']
 
 
 def get_meta_paths() -> MetaPaths:
     return app_meta['meta_paths']
 
 
-    # region[Main_Exec]
+    # region [Main_Exec]
 if __name__ == '__main__':
     from faked_pack_src import call_and_return
     call_and_return(setup_meta_data)
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/meta_data/meta_info/meta_info_factory.py` & `gidapptools-0.5.0/gidapptools/meta_data/meta_info/meta_info_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,31 +17,31 @@
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.utility.helper import meta_data_from_path
 from gidapptools.meta_data.config_kwargs import ConfigKwargs
 from gidapptools.general_helper.conversion import str_to_bool
 from gidapptools.meta_data.meta_info.meta_info_item import MetaInfo
 from gidapptools.abstract_classes.abstract_meta_factory import AbstractMetaFactory
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class License:
     special_licenses: dict[str, "License"] = {}
 
     def __init__(self, name: str, osi_approved: bool, description: str = None):
         self.name = name
@@ -165,14 +165,14 @@
             # TODO: maybe raise error instead
             self.setup()
         meta_info_kwargs = self._build_meta_info_args()
         instance = self.product_class(**meta_info_kwargs)
         return instance
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/meta_data/meta_info/meta_info_item.py` & `gidapptools-0.5.0/gidapptools/meta_data/meta_info/meta_info_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import os
 import sys
 import platform
 from typing import TYPE_CHECKING, Any, Union, Callable, Optional
 from pathlib import Path
 from datetime import datetime, timezone
-from functools import cached_property
-
+from functools import cached_property, partial
+import psutil
 # * Third Party Imports --------------------------------------------------------------------------------->
 import attr
 from yarl import URL
 from tzlocal import get_localzone
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.gid_utility import VersionItem
@@ -30,33 +30,33 @@
 from gidapptools.general_helper.string_helper import StringCase, StringCaseConverter
 from gidapptools.abstract_classes.abstract_meta_item import AbstractMetaItem
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.meta_data.meta_info.meta_info_factory import License
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 # - Make into a class
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
 
-# endregion[Constants]
+# endregion [Constants]
 
 def url_converter(in_url: Optional[str]) -> Optional[URL]:
     if in_url is None:
         return in_url
     return URL(in_url)
 
 
@@ -78,69 +78,68 @@
 class MetaInfo(AbstractMetaItem):
     app_name: str = attr.ib(default="python_script")
     app_author: str = attr.ib(default=None)
     version: VersionItem = attr.ib(default=None, converter=version_converter)
     url: URL = attr.ib(converter=url_converter, default=None)
     other_urls: dict[str, URL] = attr.ib(converter=many_url_converter, default=dict())
     pid: int = attr.ib(factory=os.getpid)
+    process: psutil.Process = attr.ib(factory=partial(psutil.Process, os.getpid()))
     os: OperatingSystem = attr.ib(factory=OperatingSystem.determine_operating_system)
     os_release: str = attr.ib(factory=platform.release)
     python_version: VersionItem = attr.ib(factory=platform.python_version, converter=version_converter)
-    started_at: datetime = attr.ib(factory=utc_now)
-    base_mem_use: int = attr.ib(default=memory_in_use())
     is_dev: bool = attr.ib(default=None, converter=attr.converters.default_if_none(False))
     is_gui: bool = attr.ib(default=None, converter=attr.converters.default_if_none(False))
     local_tz: timezone = attr.ib(default=get_localzone())
     summary: str = attr.ib(default=None)
     app_license: "License" = attr.ib(default=None)
     description: str = attr.ib(default=None)
 
-    @cached_property
+    @property
+    def started_at(self) -> datetime:
+        time_stamp = self.process.create_time()
+        return datetime.fromtimestamp(time_stamp, tz=timezone.utc)
+
+    @property
     def is_frozen_app(self) -> bool:
         return is_frozen()
 
-    @cached_property
+    @property
     def frozen_folder_path(self) -> Optional[Path]:
         if self.is_frozen_app is True:
             return Path(sys._MEIPASS)
 
-    @cached_property
+    @property
     def cli_name(self) -> str:
         return self.app_name.replace(" ", "-").replace("_", '-')
 
     @classmethod
     @property
     def __default_configuration__(cls) -> dict[str, Any]:
         default_configuration = {}
         return default_configuration
 
-    @cached_property
+    @property
     def pretty_is_dev(self) -> str:
         return "Yes" if self.is_dev else "No"
 
-    @cached_property
+    @property
     def pretty_app_name(self) -> str:
         if self.app_name:
             return StringCaseConverter.convert_to(self.app_name, StringCase.TITLE)
 
-    @cached_property
+    @property
     def pretty_app_author(self) -> str:
         if self.app_author:
             return StringCaseConverter.convert_to(self.app_author, StringCase.TITLE)
 
-    @cached_property
-    def pretty_base_mem_use(self) -> str:
-        return bytes2human(self.base_mem_use)
-
-    @cached_property
+    @property
     def pretty_started_at(self) -> str:
-        return DatetimeFmt.STANDARD.strf(self.started_at)
+        return self.started_at.strftime(DatetimeFmt.STANDARD)
 
     def as_dict(self, pretty: bool = False) -> dict[str, Any]:
-
         if pretty is True:
             return make_pretty(self)
         return attr.asdict(self)
 
     def to_storager(self, storager: Callable = None) -> None:
         if storager is None:
             return
@@ -156,17 +155,18 @@
                        url: Union[str, URL] = None,
                        other_urls: dict[str, Union[str, URL]] = None,
                        is_dev: bool = None,
                        is_gui: bool = None,
                        summary: str = None,
                        description: str = None) -> MetaInfo:
 
-    kwargs = dict(app_name=app_name, app_author=app_author, version=version, url=url, other_urls=other_urls, is_dev=is_dev or os.getenv("IS_DEV", "0") != "0", is_gui=is_gui, summary=summary, description=description)
+    is_dev = is_dev if is_dev is not None else os.getenv("IS_DEV", "0") != "0"
+    kwargs = dict(app_name=app_name, app_author=app_author, version=version, url=url, other_urls=other_urls, is_dev=is_dev, is_gui=is_gui, summary=summary, description=description)
     for k in list(kwargs):
         if kwargs[k] is None:
             kwargs.pop(k)
     return MetaInfo(**kwargs)
 
-    # region[Main_Exec]
+    # region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/meta_data/meta_paths/appdirs_implementations.py` & `gidapptools-0.5.0/gidapptools/meta_data/meta_paths/appdirs_implementations.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 from pathlib import Path
 from tempfile import gettempdir
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.utility.enums import NamedMetaPath
 from gidapptools.utility.helper import PathLibAppDirs
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class GidAppDirs(PathLibAppDirs):
 
     @PathLibAppDirs.mark_path
     def user_config_dir(self) -> Path:
         config_dir = super().user_config_dir().joinpath('config')
@@ -76,12 +76,12 @@
                              app_author: str = None,
                              roaming: bool = True,
                              multipath: bool = False) -> dict[NamedMetaPath, Optional[Path]]:
         inst = cls(appname=app_name, appauthor=app_author, roaming=roaming, multipath=multipath)
         return inst.as_path_dict()
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/meta_data/meta_paths/meta_paths_factory.py` & `gidapptools-0.5.0/gidapptools/meta_data/meta_paths/meta_paths_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,45 +16,45 @@
 from gidapptools.utility.enums import EnvName, NamedMetaPath
 from gidapptools.general_helper.enums import MiscEnum
 from gidapptools.meta_data.config_kwargs import ConfigKwargs
 from gidapptools.meta_data.meta_paths.meta_paths_item import MetaPaths
 from gidapptools.abstract_classes.abstract_meta_factory import AbstractMetaFactory
 from gidapptools.meta_data.meta_paths.appdirs_implementations import GidAppDirs
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class MetaPathsFactory(AbstractMetaFactory):
     appdirs_class = GidAppDirs
     product_class = MetaPaths
     default_configuration = {"roaming": MiscEnum.OPTIONAL, "multipath": MiscEnum.OPTIONAL}
 
     def __init__(self, config_kwargs: ConfigKwargs) -> None:
         super().__init__(config_kwargs=config_kwargs)
         self.code_base_dir = Path(self.config_kwargs.get('init_path')).parent
 
     def get_path_dict(self) -> dict[NamedMetaPath, Optional[Path]]:
-        defaults = {'app_name': os.getenv(EnvName.APP_NAME),
-                    'app_author': os.getenv(EnvName.APP_AUTHOR)}
+        defaults = {'app_name': os.getenv(EnvName.APP_NAME.value),
+                    'app_author': os.getenv(EnvName.APP_AUTHOR.value)}
         _kwargs = self.config_kwargs.get_kwargs_for(self.appdirs_class.get_path_dict_direct, defaults)
         if _kwargs.get('app_name') is None:
             raise AppNameMissingError()
 
         path_overwrites = self.config_kwargs.get('path_overwrites', {})
         if self.config_kwargs.created_meta_items["meta_info"].is_dev is True and NamedMetaPath.DEBUG_DUMP not in path_overwrites:
             path_overwrites[NamedMetaPath.DEBUG_DUMP] = self.code_base_dir.joinpath("debug_dump")
@@ -75,14 +75,14 @@
             self.setup()
         _kwargs = self.config_kwargs.get_kwargs_for(self.product_class, defaults={'code_base_dir': self.code_base_dir, 'paths': self.path_dict})
         instance = self.product_class(**_kwargs)
 
         return instance
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/meta_data/meta_paths/meta_paths_item.py` & `gidapptools-0.5.0/gidapptools/meta_data/meta_paths/meta_paths_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,51 +8,61 @@
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import shutil
 import logging
 from pprint import pformat
 from typing import Any, Union, TypeVar, Callable, Optional
 from pathlib import Path
+from threading import Lock, RLock
 from tempfile import mkdtemp
 from contextlib import contextmanager
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.errors import NotImplementedMetaPath, UnknownMetaPathIdentifier
 from gidapptools.utility.enums import NamedMetaPath
 from gidapptools.utility.helper import make_pretty
 from gidapptools.abstract_classes.abstract_meta_item import AbstractMetaItem
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 log = logging.getLogger(__name__)
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 _T = TypeVar("_T")
 
 
 class TempPathStorage(set):
 
+    @property
+    def discard_lock(self) -> RLock:
+        try:
+            return self._discard_lock
+        except AttributeError:
+            self._discard_lock = RLock()
+            return self._discard_lock
+
     def discard_non_existing(self) -> None:
-        to_discard = [i for i in self if i.exists() is False]
+        with self.discard_lock:
+            to_discard = [i for i in self if i.exists() is False]
 
-        for item in list(to_discard):
-            self.discard(item)
+            for item in list(to_discard):
+                self.discard(item)
 
     def add(self, item: _T) -> None:
         self.discard_non_existing()
         return super().add(item)
 
 
 class MetaPaths(AbstractMetaItem):
@@ -123,17 +133,18 @@
         full_name = f"{name}{_suffix}{_number}"
         return self.temp_dir.joinpath(full_name)
 
     def get_new_temp_dir(self, suffix: str = None, name: str = None, exists_ok: bool = False) -> Path:
         if name is not None:
             _number = 0
             temp_dir = self._generate_named_temp_dir_path(name, suffix=suffix, number=_number)
-            while exists_ok is False and temp_dir.exists():
-                _number += 1
-                temp_dir = self._generate_named_temp_dir_path(name, suffix=suffix, number=_number)
+            if exists_ok is False:
+                while temp_dir.exists():
+                    _number += 1
+                    temp_dir = self._generate_named_temp_dir_path(name, suffix=suffix, number=_number)
 
         else:
             temp_dir = Path(mkdtemp(dir=self.temp_dir, suffix=suffix))
 
         temp_dir.mkdir(parents=True, exist_ok=True)
         self._created_temp_dirs.add(temp_dir)
         return temp_dir
@@ -177,11 +188,11 @@
                         log.info("Deleting temp-folder %r and its contents.", path.as_posix())
                         shutil.rmtree(path)
 
         self.running_pid_storage_file.unlink(missing_ok=True)
         # TODO: find a way to clean shit up, but completely, also add optional kwarg that also removes the author folder
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/utility/enums.py` & `gidapptools-0.5.0/gidapptools/utility/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import platform
 from enum import Enum, auto
 from typing import Any
 from pathlib import Path
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.absolute()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class BaseGidEnum(Enum):
     @classmethod
     def _missing_(cls, value: object) -> Any:
         if isinstance(value, str):
             mod_value = value.casefold()
@@ -110,14 +110,14 @@
 
 class EnvName(str, Enum):
     APP_NAME = 'APP_NAME'
     APP_AUTHOR = 'APP_AUTHOR'
     LOG_DIR = 'APP_LOG_DIR'
 
 
-# region[Main_Exec]
+# region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/utility/helper.py` & `gidapptools-0.5.0/gidapptools/utility/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import sys
 import json
 import inspect
 from abc import abstractmethod
+import os
 from enum import Enum
 from typing import Any, Mapping, TypeVar, Callable, Optional
 from pathlib import Path
 from datetime import datetime, timezone
 from importlib.metadata import PackageMetadata, metadata
 
 # * Third Party Imports --------------------------------------------------------------------------------->
@@ -22,32 +23,33 @@
 from yarl import URL
 from platformdirs import PlatformDirs
 
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.custom_types import PATH_TYPE
 from gidapptools.utility.enums import NamedMetaPath
 from gidapptools.general_helper.date_time import DatetimeFmt
+from gidapptools.general_helper.conversion import str_to_bool
 
-# endregion[Imports]
+# endregion [Imports]
 
 # region [TODO]
 
 
 # endregion [TODO]
 
 # region [Logging]
 
 
-# endregion[Logging]
+# endregion [Logging]
 
 # region [Constants]
 
 THIS_FILE_DIR = Path(__file__).parent.resolve()
 
-# endregion[Constants]
+# endregion [Constants]
 
 
 class PackageMetadataDict(dict):
     list_fields: set[str] = {"dynamic",
                              "platform",
                              "supported-platform",
                              "classifier",
@@ -134,24 +136,33 @@
     _metadata = metadata(_init_module.__package__)
 
     _out = PackageMetadataDict.from_meta_importlib_meta_data(_metadata)
 
     return _out
 
 
+def meta_data_from_package_name(package_name: str) -> dict[str, Any]:
+
+    _metadata = metadata(package_name)
+
+    _out = PackageMetadataDict.from_meta_importlib_meta_data(_metadata)
+
+    return _out
+
+
 TCallable = TypeVar("TCallable", bound=Callable)
 
 
-def mark_appdir_path(func: TCallable) -> TCallable:
+def _mark_appdir_path(func: TCallable) -> TCallable:
     func._appdir_path_type = NamedMetaPath(func.__name__)
     return func
 
 
 class PathLibAppDirs:
-    mark_path = mark_appdir_path
+    mark_path = _mark_appdir_path
 
     def __init__(self,
                  appname: str,
                  appauthor: str = None,
                  version: str = None,
                  roaming: bool = True,
                  multipath: bool = False) -> None:
@@ -161,39 +172,39 @@
     def appname(self) -> str:
         return self.platform_dirs.appname
 
     @property
     def authorname(self) -> Optional[str]:
         return self.platform_dirs.appauthor
 
-    @mark_appdir_path
+    @mark_path
     def user_data_dir(self) -> Path:
         return Path(self.platform_dirs.user_data_path)
 
-    @mark_appdir_path
+    @mark_path
     def user_log_dir(self) -> Path:
         return Path(self.platform_dirs.user_log_path)
 
-    @mark_appdir_path
+    @mark_path
     def user_cache_dir(self) -> Path:
         return Path(self.platform_dirs.user_cache_path)
 
-    @mark_appdir_path
+    @mark_path
     def user_config_dir(self) -> Path:
         return Path(self.platform_dirs.user_config_path)
 
-    @mark_appdir_path
+    @mark_path
     def user_state_dir(self) -> Path:
         return Path(self.platform_dirs.user_state_path)
 
-    @mark_appdir_path
+    @mark_path
     def site_data_dir(self) -> Path:
         return Path(self.platform_dirs.user_data_path)
 
-    @mark_appdir_path
+    @mark_path
     def site_config_dir(self) -> Path:
 
         return Path(self.platform_dirs.site_config_path)
 
     def as_path_dict(self) -> dict[NamedMetaPath, Optional[Path]]:
         path_dict = {named_path_item: None for named_path_item in NamedMetaPath.__members__.values()}
         for meth_name, meth_object in inspect.getmembers(self, inspect.ismethod):
@@ -270,11 +281,16 @@
 
 def get_main_module_path() -> Path:
     main_module = sys.modules["__main__"]
 
     return Path(main_module.__file__).resolve()
 
 
-# region[Main_Exec]
+def is_dev() -> bool:
+    is_dev_string = os.getenv("IS_DEV", '0').casefold()
+    return str_to_bool(is_dev_string, strict=True) or sys.flags.dev_mode
+
+
+# region [Main_Exec]
 if __name__ == '__main__':
     pass
-# endregion[Main_Exec]
+# endregion [Main_Exec]
```

### Comparing `gidapptools-0.4.4/gidapptools/vendored/atomic_writes.py` & `gidapptools-0.5.0/gidapptools/vendored/atomic_writes.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/gidapptools/vendored/atomic_writes_LICENSE` & `gidapptools-0.5.0/gidapptools/vendored/atomic_writes_LICENSE`

 * *Files identical despite different names*

### Comparing `gidapptools-0.4.4/pyproject.toml` & `gidapptools-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,44 +7,52 @@
 authors = [{ name = "brocaprogs" }]
 classifiers = ["License :: OSI Approved :: MIT License"]
 license = { file = "LICENSE" }
 readme = { file = "README.rst", content-type = "text/x-rst" }
 dynamic = ['version', 'description']
 requires-python = ">=3.9"
 dependencies = [
-    "attrs~=22.1",
-    "frozendict~=2.3",
-    "platformdirs~=2.5",
-    "psutil~=5.9",
-    "pyparsing~=3.0",
-    "tzlocal~=4.2",
-    "yarl~=1.8",
-    "typing-extensions~=4.4",
+    "attrs>=22.1",
+    "frozendict>=2.3",
+    "platformdirs>=2.6",
+    "psutil>=5.9",
+    "pyparsing>=3.0",
+    "tzlocal>=4.2",
+    "yarl>=1.8",
+    "pytz>=2024.1",
+    "filelock>=3.13.4",
+    "orjson>=3.10.3",
 ]
 
 [project.urls]
 Source = "https://github.com/Giddius/GidAppTools"
 
 [project.scripts]
 gidapptools-info = "gidapptools.cli_info:cli_show_info"
 
 
 [project.optional-dependencies]
 
-pyside = ["PySide6~=6.4", "jinja2~=3.1"]
-orm = ["peewee~=3.15"]
-rich = ["rich~=12.6"]
-parsing = ["python-dateutil>=2.8.1"]
+pyside = ["PySide6>=6.4", "pyqtgraph>=0.13", "jinja2>=3.1"]
+orm = ["peewee>=3.15", "apsw>=3.39"]
+rich = ["rich>=13.1"]
+parsing = ["python-dateutil>=2.8"]
+image = ["Pillow>=9.4", "scipy>=1.10", "numpy>=1.24"]
 all = [
-    "PySide6~=6.4",
-    "peewee~=3.15",
-    "cython~=0.29",
-    "rich~=12.6",
-    "jinja2~=3.1",
-    "python-dateutil>=2.8.1",
+    "PySide6>=6.4",
+    "peewee>=3.15",
+    "cython>=0.29",
+    "rich>=13.1",
+    "jinja2>=3.1",
+    "python-dateutil>=2.8",
+    "apsw>=3.39",
+    "Pillow>=9.4",
+    "scipy>=1.10",
+    "numpy>=1.24",
+    "pyqtgraph>=0.13",
 ]
 [tool.flit.sdist]
 exclude = [
     "misc",
     "temp",
     "docs",
     "tools",
@@ -94,17 +102,22 @@
 remove_all_unused_imports = true
 remove_duplicate_keys = false
 remove_unused_variables = false
 ignore_init_module_imports = false
 
 
 [tool.pytest.ini_options]
-addopts = "-rA -vv --durations=0 --capture=tee-sys --show-capture=all --color=auto --code-highlight=yes --cov=gidapptools --cov-report html --html-report=./tools/reports/pytest_report --title='PYTEST REPORT'"
+addopts = "-rA -vv --durations=10 --capture=tee-sys --show-capture=all --color=auto --code-highlight=yes --cov=gidapptools --cov-report html --html-report=./tools/reports/pytest_report --title='PYTEST REPORT'"
+norecursedirs = "manual_*"
 
 [tool.coverage.report]
 omit = ["**/__init__.py"]
 exclude_lines = ["if __name__ == .__main__.:", "def __rich__", "def __repr__"]
 
 [tool.coverage.html]
 directory = "tools/reports/coverage/html"
 
 [tool.mypy]
+
+
+[tool.ruff]
+ignore = ["E501", "E402", "E731"]
```

