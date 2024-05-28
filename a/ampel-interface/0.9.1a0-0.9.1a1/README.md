# Comparing `tmp/ampel_interface-0.9.1a0.tar.gz` & `tmp/ampel_interface-0.9.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_interface-0.9.1a0.tar", max compression
+gzip compressed data, was "ampel_interface-0.9.1a1.tar", max compression
```

## Comparing `ampel_interface-0.9.1a0.tar` & `ampel_interface-0.9.1a1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     1512 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/LICENSE
--rw-r--r--   0        0        0      124 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/README.md
--rw-r--r--   0        0        0      642 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsApplicable.py
--rwxr-xr-x   0        0        0     1050 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsCLIOperation.py
--rwxr-xr-x   0        0        0     1721 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsCustomStateT2Unit.py
--rw-r--r--   0        0        0     1228 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsIdMapper.py
--rwxr-xr-x   0        0        0     2088 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsPointT2Unit.py
--rwxr-xr-x   0        0        0     1109 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsSecretProvider.py
--rwxr-xr-x   0        0        0     1179 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsStateT2Unit.py
--rwxr-xr-x   0        0        0     1042 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsStockT2Unit.py
--rwxr-xr-x   0        0        0     1268 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsT0Unit.py
--rwxr-xr-x   0        0        0     1031 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsT1CombineUnit.py
--rwxr-xr-x   0        0        0      832 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsT1ComputeUnit.py
--rwxr-xr-x   0        0        0     1046 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsT1RetroCombineUnit.py
--rwxr-xr-x   0        0        0     1885 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsT3Unit.py
--rwxr-xr-x   0        0        0      733 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsT4Unit.py
--rwxr-xr-x   0        0        0     1984 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsTiedCustomStateT2Unit.py
--rwxr-xr-x   0        0        0     1345 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsTiedPointT2Unit.py
--rwxr-xr-x   0        0        0     1396 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsTiedStateT2Unit.py
--rwxr-xr-x   0        0        0     1064 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsTiedStockT2Unit.py
--rwxr-xr-x   0        0        0     1123 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/abstract/AbsTiedT2Unit.py
--rwxr-xr-x   0        0        0     4034 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/alert/AmpelAlert.py
--rwxr-xr-x   0        0        0    12019 2023-12-18 12:35:25.630668 ampel_interface-0.9.1a0/ampel/base/AlternativeAmpelBaseModel.py
--rw-r--r--   0        0        0     5987 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/AmpelABC.py
--rw-r--r--   0        0        0     1025 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/AmpelBaseModel.py
--rw-r--r--   0        0        0      615 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/AmpelFlexModel.py
--rw-r--r--   0        0        0     1017 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/AmpelGenericModel.py
--rw-r--r--   0        0        0     7033 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/AmpelUnit.py
--rwxr-xr-x   0        0        0     2858 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/AuxUnitRegister.py
--rwxr-xr-x   0        0        0      386 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/BadConfig.py
--rwxr-xr-x   0        0        0     1832 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/LogicalUnit.py
--rw-r--r--   0        0        0     1970 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/base/decorator.py
--rwxr-xr-x   0        0        0    16556 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/AmpelArgumentParser.py
--rw-r--r--   0        0        0     2349 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/AmpelHelpFormatter.py
--rw-r--r--   0        0        0     6624 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/ArgParserBuilder.py
--rw-r--r--   0        0        0      702 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/LoadAllOfAction.py
--rw-r--r--   0        0        0      702 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/LoadAnyOfAction.py
--rw-r--r--   0        0        0      545 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/LoadJSONAction.py
--rw-r--r--   0        0        0      661 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/MaybeIntAction.py
--rw-r--r--   0        0        0     1256 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/config.py
--rw-r--r--   0        0        0    12099 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/cli/main.py
--rwxr-xr-x   0        0        0     5237 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/config/AmpelConfig.py
--rwxr-xr-x   0        0        0      938 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/DataPoint.py
--rwxr-xr-x   0        0        0     1374 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/EventDocument.py
--rwxr-xr-x   0        0        0     1442 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/JournalRecord.py
--rwxr-xr-x   0        0        0     1791 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/LogDocument.py
--rwxr-xr-x   0        0        0      935 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/MetaActivity.py
--rwxr-xr-x   0        0        0     1470 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/MetaRecord.py
--rwxr-xr-x   0        0        0     1613 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/StockDocument.py
--rwxr-xr-x   0        0        0     1774 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/T1Document.py
--rwxr-xr-x   0        0        0     2150 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/T2Document.py
--rwxr-xr-x   0        0        0     1907 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/T3Document.py
--rwxr-xr-x   0        0        0     1523 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/content/T4Document.py
--rwxr-xr-x   0        0        0     2588 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/enum/DocumentCode.py
--rwxr-xr-x   0        0        0      729 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/enum/EventCode.py
--rwxr-xr-x   0        0        0     1898 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/enum/JournalActionCode.py
--rwxr-xr-x   0        0        0     1138 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/enum/MetaActionCode.py
--rwxr-xr-x   0        0        0     2335 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/model/DPSelection.py
--rwxr-xr-x   0        0        0     1491 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/model/StateT2Dependency.py
--rw-r--r--   0        0        0     1171 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/model/UnitModel.py
--rwxr-xr-x   0        0        0      565 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/model/operator/AllOf.py
--rwxr-xr-x   0        0        0      838 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/model/operator/AnyOf.py
--rw-r--r--   0        0        0      839 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/model/operator/FlatAnyOf.py
--rwxr-xr-x   0        0        0      532 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/model/operator/OneOf.py
--rwxr-xr-x   0        0        0     1292 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/protocol/AmpelAlertProtocol.py
--rwxr-xr-x   0        0        0     1343 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/protocol/LoggerProtocol.py
--rwxr-xr-x   0        0        0      712 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/protocol/LoggingHandlerProtocol.py
--rw-r--r--   0        0        0        0 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/py.typed
--rwxr-xr-x   0        0        0     1368 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/secret/AESecret.py
--rwxr-xr-x   0        0        0     1269 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/secret/AmpelVault.py
--rwxr-xr-x   0        0        0      981 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/secret/NamedSecret.py
--rwxr-xr-x   0        0        0      850 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/secret/Secret.py
--rwxr-xr-x   0        0        0     1382 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/struct/AmpelBuffer.py
--rwxr-xr-x   0        0        0     1965 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/struct/JournalAttributes.py
--rwxr-xr-x   0        0        0     1669 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/struct/Resource.py
--rwxr-xr-x   0        0        0     1236 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/struct/StockAttributes.py
--rwxr-xr-x   0        0        0     1267 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/struct/T1CombineResult.py
--rwxr-xr-x   0        0        0     4149 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/struct/T3Store.py
--rwxr-xr-x   0        0        0     2042 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/struct/UnitResult.py
--rw-r--r--   0        0        0     1856 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/types.py
--rw-r--r--   0        0        0     1089 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/bson.py
--rw-r--r--   0        0        0     1674 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/compression.py
--rwxr-xr-x   0        0        0     2528 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/docstringutils.py
--rw-r--r--   0        0        0     1300 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/freeze.py
--rwxr-xr-x   0        0        0     3838 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/hash.py
--rw-r--r--   0        0        0     3450 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/json.py
--rwxr-xr-x   0        0        0    10572 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/mappings.py
--rw-r--r--   0        0        0     1691 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/recursion.py
--rw-r--r--   0        0        0     2473 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/serialize.py
--rw-r--r--   0        0        0     3181 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/util/tag.py
--rwxr-xr-x   0        0        0      863 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/view/ReadOnlyDict.py
--rwxr-xr-x   0        0        0    10196 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/view/SnapView.py
--rwxr-xr-x   0        0        0     7075 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/view/T2DocView.py
--rwxr-xr-x   0        0        0     3745 2023-12-18 12:35:25.634667 ampel_interface-0.9.1a0/ampel/view/T3DocView.py
--rw-r--r--   0        0        0     1231 2023-12-18 12:35:25.638667 ampel_interface-0.9.1a0/pyproject.toml
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 ampel_interface-0.9.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/LICENSE
+-rw-r--r--   0        0        0      124 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/README.md
+-rw-r--r--   0        0        0      642 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsApplicable.py
+-rwxr-xr-x   0        0        0     1050 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsCLIOperation.py
+-rwxr-xr-x   0        0        0     1721 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsCustomStateT2Unit.py
+-rw-r--r--   0        0        0     1228 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsIdMapper.py
+-rwxr-xr-x   0        0        0     2088 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsPointT2Unit.py
+-rwxr-xr-x   0        0        0     1109 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsSecretProvider.py
+-rwxr-xr-x   0        0        0     1179 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsStateT2Unit.py
+-rwxr-xr-x   0        0        0     1042 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsStockT2Unit.py
+-rwxr-xr-x   0        0        0     1268 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsT0Unit.py
+-rwxr-xr-x   0        0        0     1031 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsT1CombineUnit.py
+-rwxr-xr-x   0        0        0      832 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsT1ComputeUnit.py
+-rwxr-xr-x   0        0        0     1046 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsT1RetroCombineUnit.py
+-rwxr-xr-x   0        0        0     1885 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsT3Unit.py
+-rwxr-xr-x   0        0        0      733 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsT4Unit.py
+-rwxr-xr-x   0        0        0     1984 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsTiedCustomStateT2Unit.py
+-rwxr-xr-x   0        0        0     1345 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsTiedPointT2Unit.py
+-rwxr-xr-x   0        0        0     1396 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsTiedStateT2Unit.py
+-rwxr-xr-x   0        0        0     1064 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsTiedStockT2Unit.py
+-rwxr-xr-x   0        0        0     1123 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/abstract/AbsTiedT2Unit.py
+-rwxr-xr-x   0        0        0     4034 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/alert/AmpelAlert.py
+-rwxr-xr-x   0        0        0    12019 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/AlternativeAmpelBaseModel.py
+-rw-r--r--   0        0        0     5987 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/AmpelABC.py
+-rw-r--r--   0        0        0     1025 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/AmpelBaseModel.py
+-rw-r--r--   0        0        0      615 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/AmpelFlexModel.py
+-rw-r--r--   0        0        0     1017 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/AmpelGenericModel.py
+-rw-r--r--   0        0        0     7033 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/AmpelUnit.py
+-rwxr-xr-x   0        0        0     2858 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/AuxUnitRegister.py
+-rwxr-xr-x   0        0        0      386 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/BadConfig.py
+-rwxr-xr-x   0        0        0     1832 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/LogicalUnit.py
+-rw-r--r--   0        0        0     1970 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/base/decorator.py
+-rwxr-xr-x   0        0        0    16556 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/AmpelArgumentParser.py
+-rw-r--r--   0        0        0     2349 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/AmpelHelpFormatter.py
+-rw-r--r--   0        0        0     6624 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/ArgParserBuilder.py
+-rw-r--r--   0        0        0      702 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/LoadAllOfAction.py
+-rw-r--r--   0        0        0      702 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/LoadAnyOfAction.py
+-rw-r--r--   0        0        0      545 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/LoadJSONAction.py
+-rw-r--r--   0        0        0      661 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/MaybeIntAction.py
+-rw-r--r--   0        0        0     1256 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/config.py
+-rw-r--r--   0        0        0    12210 2023-12-18 19:41:23.817370 ampel_interface-0.9.1a1/ampel/cli/main.py
+-rwxr-xr-x   0        0        0     5237 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/config/AmpelConfig.py
+-rwxr-xr-x   0        0        0      938 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/DataPoint.py
+-rwxr-xr-x   0        0        0     1374 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/EventDocument.py
+-rwxr-xr-x   0        0        0     1442 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/JournalRecord.py
+-rwxr-xr-x   0        0        0     1791 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/LogDocument.py
+-rwxr-xr-x   0        0        0      935 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/MetaActivity.py
+-rwxr-xr-x   0        0        0     1470 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/MetaRecord.py
+-rwxr-xr-x   0        0        0     1613 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/StockDocument.py
+-rwxr-xr-x   0        0        0     1774 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/T1Document.py
+-rwxr-xr-x   0        0        0     2150 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/T2Document.py
+-rwxr-xr-x   0        0        0     1907 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/T3Document.py
+-rwxr-xr-x   0        0        0     1523 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/content/T4Document.py
+-rwxr-xr-x   0        0        0     2588 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/enum/DocumentCode.py
+-rwxr-xr-x   0        0        0      729 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/enum/EventCode.py
+-rwxr-xr-x   0        0        0     1898 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/enum/JournalActionCode.py
+-rwxr-xr-x   0        0        0     1138 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/enum/MetaActionCode.py
+-rwxr-xr-x   0        0        0     2335 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/model/DPSelection.py
+-rwxr-xr-x   0        0        0     1491 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/model/StateT2Dependency.py
+-rw-r--r--   0        0        0     1171 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/model/UnitModel.py
+-rwxr-xr-x   0        0        0      565 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/model/operator/AllOf.py
+-rwxr-xr-x   0        0        0      838 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/model/operator/AnyOf.py
+-rw-r--r--   0        0        0      839 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/model/operator/FlatAnyOf.py
+-rwxr-xr-x   0        0        0      532 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/model/operator/OneOf.py
+-rwxr-xr-x   0        0        0     1292 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/protocol/AmpelAlertProtocol.py
+-rwxr-xr-x   0        0        0     1343 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/protocol/LoggerProtocol.py
+-rwxr-xr-x   0        0        0      712 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/protocol/LoggingHandlerProtocol.py
+-rw-r--r--   0        0        0        0 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/py.typed
+-rwxr-xr-x   0        0        0     1368 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/secret/AESecret.py
+-rwxr-xr-x   0        0        0     1269 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/secret/AmpelVault.py
+-rwxr-xr-x   0        0        0      981 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/secret/NamedSecret.py
+-rwxr-xr-x   0        0        0      850 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/secret/Secret.py
+-rwxr-xr-x   0        0        0     1382 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/struct/AmpelBuffer.py
+-rwxr-xr-x   0        0        0     1965 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/struct/JournalAttributes.py
+-rwxr-xr-x   0        0        0     1669 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/struct/Resource.py
+-rwxr-xr-x   0        0        0     1236 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/struct/StockAttributes.py
+-rwxr-xr-x   0        0        0     1267 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/struct/T1CombineResult.py
+-rwxr-xr-x   0        0        0     4149 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/struct/T3Store.py
+-rwxr-xr-x   0        0        0     2042 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/struct/UnitResult.py
+-rw-r--r--   0        0        0     1856 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/types.py
+-rw-r--r--   0        0        0     1089 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/bson.py
+-rw-r--r--   0        0        0     1674 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/compression.py
+-rwxr-xr-x   0        0        0     2528 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/docstringutils.py
+-rw-r--r--   0        0        0     1300 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/freeze.py
+-rwxr-xr-x   0        0        0     3838 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/hash.py
+-rw-r--r--   0        0        0     3450 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/json.py
+-rwxr-xr-x   0        0        0    10572 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/mappings.py
+-rw-r--r--   0        0        0     1691 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/recursion.py
+-rw-r--r--   0        0        0     2473 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/serialize.py
+-rw-r--r--   0        0        0     3181 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/util/tag.py
+-rwxr-xr-x   0        0        0      863 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/view/ReadOnlyDict.py
+-rwxr-xr-x   0        0        0    10196 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/view/SnapView.py
+-rwxr-xr-x   0        0        0     7075 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/view/T2DocView.py
+-rwxr-xr-x   0        0        0     3745 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/ampel/view/T3DocView.py
+-rw-r--r--   0        0        0     1231 2023-12-18 19:41:23.821370 ampel_interface-0.9.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 ampel_interface-0.9.1a1/PKG-INFO
```

### Comparing `ampel_interface-0.9.1a0/LICENSE` & `ampel_interface-0.9.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsApplicable.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsApplicable.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsCLIOperation.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsCLIOperation.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsCustomStateT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsCustomStateT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsIdMapper.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsIdMapper.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsPointT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsPointT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsSecretProvider.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsSecretProvider.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsStateT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsStateT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsStockT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsStockT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsT0Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsT0Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsT1CombineUnit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsT1CombineUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsT1ComputeUnit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsT1ComputeUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsT1RetroCombineUnit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsT1RetroCombineUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsT3Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsT3Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsT4Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsT4Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsTiedCustomStateT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsTiedCustomStateT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsTiedPointT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsTiedPointT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsTiedStateT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsTiedStateT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsTiedStockT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsTiedStockT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/abstract/AbsTiedT2Unit.py` & `ampel_interface-0.9.1a1/ampel/abstract/AbsTiedT2Unit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/alert/AmpelAlert.py` & `ampel_interface-0.9.1a1/ampel/alert/AmpelAlert.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/AlternativeAmpelBaseModel.py` & `ampel_interface-0.9.1a1/ampel/base/AlternativeAmpelBaseModel.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/AmpelABC.py` & `ampel_interface-0.9.1a1/ampel/base/AmpelABC.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/AmpelBaseModel.py` & `ampel_interface-0.9.1a1/ampel/base/AmpelBaseModel.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/AmpelFlexModel.py` & `ampel_interface-0.9.1a1/ampel/base/AmpelFlexModel.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/AmpelGenericModel.py` & `ampel_interface-0.9.1a1/ampel/base/AmpelGenericModel.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/AmpelUnit.py` & `ampel_interface-0.9.1a1/ampel/base/AmpelUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/AuxUnitRegister.py` & `ampel_interface-0.9.1a1/ampel/base/AuxUnitRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/LogicalUnit.py` & `ampel_interface-0.9.1a1/ampel/base/LogicalUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/base/decorator.py` & `ampel_interface-0.9.1a1/ampel/base/decorator.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/AmpelArgumentParser.py` & `ampel_interface-0.9.1a1/ampel/cli/AmpelArgumentParser.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/AmpelHelpFormatter.py` & `ampel_interface-0.9.1a1/ampel/cli/AmpelHelpFormatter.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/ArgParserBuilder.py` & `ampel_interface-0.9.1a1/ampel/cli/ArgParserBuilder.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/LoadAllOfAction.py` & `ampel_interface-0.9.1a1/ampel/cli/LoadAllOfAction.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/LoadAnyOfAction.py` & `ampel_interface-0.9.1a1/ampel/cli/LoadAnyOfAction.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/LoadJSONAction.py` & `ampel_interface-0.9.1a1/ampel/cli/LoadJSONAction.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/MaybeIntAction.py` & `ampel_interface-0.9.1a1/ampel/cli/MaybeIntAction.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/config.py` & `ampel_interface-0.9.1a1/ampel/cli/config.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/cli/main.py` & `ampel_interface-0.9.1a1/ampel/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,18 @@
 
 	if env_opts := os.environ.get("AMPEL_CLI_OPTS"):
 		if "--debug" in sys.argv:
 			print("[DEBUG] Incorporating options defined by env var AMPEL_CLI_OPTS")
 		for el in env_opts.split(" "):
 			sys.argv.append(el)
 
-	# Convert "-" to "--" for argparse
+	# Convert elements of the form "-option" to "--option" for argparse, skipping things that
+	# look like integers
 	for i in range(len(sys.argv)):
-		if len(sys.argv[i]) > 2 and sys.argv[i][0] == '-' and sys.argv[i][1] != '-':
+		if len(sys.argv[i]) > 2 and sys.argv[i][0] == '-' and sys.argv[i][1] != '-' and not sys.argv[i][1:].isdigit():
 			sys.argv[i] = "-" + sys.argv[i]
 
 	parser = cli_op.get_parser(sub_op)
 	if ambiguous_help and getattr(parser, 'args_not_required', False):
 		del sys.argv[-1]
 	try:
 		args, unknown_args = parser.parse_known_args()
```

### Comparing `ampel_interface-0.9.1a0/ampel/config/AmpelConfig.py` & `ampel_interface-0.9.1a1/ampel/config/AmpelConfig.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/DataPoint.py` & `ampel_interface-0.9.1a1/ampel/content/DataPoint.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/EventDocument.py` & `ampel_interface-0.9.1a1/ampel/content/EventDocument.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/JournalRecord.py` & `ampel_interface-0.9.1a1/ampel/content/JournalRecord.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/LogDocument.py` & `ampel_interface-0.9.1a1/ampel/content/LogDocument.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/MetaActivity.py` & `ampel_interface-0.9.1a1/ampel/content/MetaActivity.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/MetaRecord.py` & `ampel_interface-0.9.1a1/ampel/content/MetaRecord.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/StockDocument.py` & `ampel_interface-0.9.1a1/ampel/content/StockDocument.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/T1Document.py` & `ampel_interface-0.9.1a1/ampel/content/T1Document.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/T2Document.py` & `ampel_interface-0.9.1a1/ampel/content/T2Document.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/T3Document.py` & `ampel_interface-0.9.1a1/ampel/content/T3Document.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/content/T4Document.py` & `ampel_interface-0.9.1a1/ampel/content/T4Document.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/enum/DocumentCode.py` & `ampel_interface-0.9.1a1/ampel/enum/DocumentCode.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/enum/EventCode.py` & `ampel_interface-0.9.1a1/ampel/enum/EventCode.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/enum/JournalActionCode.py` & `ampel_interface-0.9.1a1/ampel/enum/JournalActionCode.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/enum/MetaActionCode.py` & `ampel_interface-0.9.1a1/ampel/enum/MetaActionCode.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/model/DPSelection.py` & `ampel_interface-0.9.1a1/ampel/model/DPSelection.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/model/StateT2Dependency.py` & `ampel_interface-0.9.1a1/ampel/model/StateT2Dependency.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/model/UnitModel.py` & `ampel_interface-0.9.1a1/ampel/model/UnitModel.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/model/operator/AllOf.py` & `ampel_interface-0.9.1a1/ampel/model/operator/AllOf.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/model/operator/AnyOf.py` & `ampel_interface-0.9.1a1/ampel/model/operator/AnyOf.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/model/operator/FlatAnyOf.py` & `ampel_interface-0.9.1a1/ampel/model/operator/FlatAnyOf.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/model/operator/OneOf.py` & `ampel_interface-0.9.1a1/ampel/model/operator/OneOf.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/protocol/AmpelAlertProtocol.py` & `ampel_interface-0.9.1a1/ampel/protocol/AmpelAlertProtocol.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/protocol/LoggerProtocol.py` & `ampel_interface-0.9.1a1/ampel/protocol/LoggerProtocol.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/protocol/LoggingHandlerProtocol.py` & `ampel_interface-0.9.1a1/ampel/protocol/LoggingHandlerProtocol.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/secret/AESecret.py` & `ampel_interface-0.9.1a1/ampel/secret/AESecret.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/secret/AmpelVault.py` & `ampel_interface-0.9.1a1/ampel/secret/AmpelVault.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/secret/NamedSecret.py` & `ampel_interface-0.9.1a1/ampel/secret/NamedSecret.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/secret/Secret.py` & `ampel_interface-0.9.1a1/ampel/secret/Secret.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/struct/AmpelBuffer.py` & `ampel_interface-0.9.1a1/ampel/struct/AmpelBuffer.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/struct/JournalAttributes.py` & `ampel_interface-0.9.1a1/ampel/struct/JournalAttributes.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/struct/Resource.py` & `ampel_interface-0.9.1a1/ampel/struct/Resource.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/struct/StockAttributes.py` & `ampel_interface-0.9.1a1/ampel/struct/StockAttributes.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/struct/T1CombineResult.py` & `ampel_interface-0.9.1a1/ampel/struct/T1CombineResult.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/struct/T3Store.py` & `ampel_interface-0.9.1a1/ampel/struct/T3Store.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/struct/UnitResult.py` & `ampel_interface-0.9.1a1/ampel/struct/UnitResult.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/types.py` & `ampel_interface-0.9.1a1/ampel/types.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/bson.py` & `ampel_interface-0.9.1a1/ampel/util/bson.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/compression.py` & `ampel_interface-0.9.1a1/ampel/util/compression.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/docstringutils.py` & `ampel_interface-0.9.1a1/ampel/util/docstringutils.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/freeze.py` & `ampel_interface-0.9.1a1/ampel/util/freeze.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/hash.py` & `ampel_interface-0.9.1a1/ampel/util/hash.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/json.py` & `ampel_interface-0.9.1a1/ampel/util/json.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/mappings.py` & `ampel_interface-0.9.1a1/ampel/util/mappings.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/recursion.py` & `ampel_interface-0.9.1a1/ampel/util/recursion.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/serialize.py` & `ampel_interface-0.9.1a1/ampel/util/serialize.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/util/tag.py` & `ampel_interface-0.9.1a1/ampel/util/tag.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/view/ReadOnlyDict.py` & `ampel_interface-0.9.1a1/ampel/view/ReadOnlyDict.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/view/SnapView.py` & `ampel_interface-0.9.1a1/ampel/view/SnapView.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/view/T2DocView.py` & `ampel_interface-0.9.1a1/ampel/view/T2DocView.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/ampel/view/T3DocView.py` & `ampel_interface-0.9.1a1/ampel/view/T3DocView.py`

 * *Files identical despite different names*

### Comparing `ampel_interface-0.9.1a0/pyproject.toml` & `ampel_interface-0.9.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-interface"
-version = "0.9.1a0"
+version = "0.9.1a1"
 description = "Base classes for the Ampel analysis platform"
 authors = ["Valery Brinnel"]
 maintainers = ["Jakob van Santen <jakob.van.santen@desy.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://ampelproject.github.io"
 repository = "https://github.com/AmpelProject/Ampel-interface"
```

### Comparing `ampel_interface-0.9.1a0/PKG-INFO` & `ampel_interface-0.9.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampel-interface
-Version: 0.9.1a0
+Version: 0.9.1a1
 Summary: Base classes for the Ampel analysis platform
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Valery Brinnel
 Maintainer: Jakob van Santen
 Maintainer-email: jakob.van.santen@desy.de
 Requires-Python: >=3.10,<4.0
```

