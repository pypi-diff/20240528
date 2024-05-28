# Comparing `tmp/ccdexplorer_fundamentals-0.2.8.tar.gz` & `tmp/ccdexplorer_fundamentals-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdexplorer_fundamentals-0.2.8.tar", last modified: Sun May  5 15:45:06 2024, max compression
+gzip compressed data, was "ccdexplorer_fundamentals-0.2.9.tar", last modified: Thu May  9 06:03:04 2024, max compression
```

## Comparing `ccdexplorer_fundamentals-0.2.8.tar` & `ccdexplorer_fundamentals-0.2.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.804548 ccdexplorer_fundamentals-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-05 15:45:06.804548 ccdexplorer_fundamentals-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.792548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.796548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.796548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/CCD_Types/
--rw-r--r--   0 runner    (1001) docker     (127)    38515 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.796548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/concordium/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/concordium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.796548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/concordium/health/
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.796548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/concordium/v2/
--rw-r--r--   0 runner    (1001) docker     (127)   190426 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.800548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)    38653 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    99596 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)   131737 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   198939 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/wadze.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.804548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20427 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    43542 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/cis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/cns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.804548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_store_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/rewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/tooter.py
--rw-r--r--   0 runner    (1001) docker     (127)    46983 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/user_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.804548 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-05 15:45:06.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-05 15:45:06.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:45:06.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 15:45:06.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 15:45:06.000000 ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 15:45:06.804548 ccdexplorer_fundamentals-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:06.804548 ccdexplorer_fundamentals-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-05 15:45:02.000000 ccdexplorer_fundamentals-0.2.8/tests/whats_wrong.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.303258 ccdexplorer_fundamentals-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-09 06:03:04.303258 ccdexplorer_fundamentals-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.287257 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.291257 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.291257 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/CCD_Types/
+-rw-r--r--   0 runner    (1001) docker     (127)    38528 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.291257 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/concordium/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/concordium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.291257 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/concordium/health/
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.291257 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/concordium/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)   190426 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.295257 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38653 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    99596 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131737 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198939 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/wadze.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.299258 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20427 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43542 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/cis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/cns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.303258 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_store_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/tooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46983 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/user_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.303258 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-09 06:03:04.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-09 06:03:04.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:03:04.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 06:03:04.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 06:03:04.000000 ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:03:04.303258 ccdexplorer_fundamentals-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:04.303258 ccdexplorer_fundamentals-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-09 06:03:00.000000 ccdexplorer_fundamentals-0.2.9/tests/whats_wrong.py
```

### Comparing `ccdexplorer_fundamentals-0.2.8/LICENSE.md` & `ccdexplorer_fundamentals-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/PKG-INFO` & `ccdexplorer_fundamentals-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdexplorer-fundamentals
-Version: 0.2.8
+Version: 0.2.9
 Summary: Shared code for CCDExplorer.io and its Notification Bot.
 Home-page: https://github.com/ccdexplorer/ccdexplorer-fundamentals
 Author: Sander de Ruiter
 Author-email: sdr@ccdexplorer.io
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ccdexplorer_fundamentals-0.2.8/README.md` & `ccdexplorer_fundamentals-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     idDocType = 6
     idDocNo = 7
     idDocIssuer = 8
     idDocIssuedAt = 9
     idDocExpiresAt = 10
     nationalIdNo = 11
     taxIdNo = 12
+    lei = 13
 
 
 class CredentialDocType(Enum):
     na = "0"
     Passport = "1"
     National_ID_Card = "2"
     Driving_License = "3"
```

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/__init__.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/health_pb2.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/health_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/service_pb2.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/types_pb2.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/types_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/GRPCClient/wadze.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/GRPCClient/wadze.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/block.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/block.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_search.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_search.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/cis.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/cis.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/cns.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/cns.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/credential.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/credential.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/env.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/env.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_store_block.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_store_block.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/node.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/node.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/pool.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/pool.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/tooter.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/tooter.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/transaction.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/transaction.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals/user_v2.py` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals/user_v2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals.egg-info/PKG-INFO` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdexplorer-fundamentals
-Version: 0.2.8
+Version: 0.2.9
 Summary: Shared code for CCDExplorer.io and its Notification Bot.
 Home-page: https://github.com/ccdexplorer/ccdexplorer-fundamentals
 Author: Sander de Ruiter
 Author-email: sdr@ccdexplorer.io
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ccdexplorer_fundamentals-0.2.8/ccdexplorer_fundamentals.egg-info/SOURCES.txt` & `ccdexplorer_fundamentals-0.2.9/ccdexplorer_fundamentals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.8/setup.py` & `ccdexplorer_fundamentals-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="ccdexplorer-fundamentals",
-    version="0.2.8",
+    version="0.2.9",
     author="Sander de Ruiter",
     author_email="sdr@ccdexplorer.io",
     description="Shared code for CCDExplorer.io and its Notification Bot.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ccdexplorer/ccdexplorer-fundamentals",
     project_urls={},
```

