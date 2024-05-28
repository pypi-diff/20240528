# Comparing `tmp/panda_server-0.3.7.tar.gz` & `tmp/panda_server-0.3.8.tar.gz`

## Comparing `panda_server-0.3.7.tar` & `panda_server-0.3.8.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.7/ChangeLog.txt
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.7/Dockerfile
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.7/INSTALL.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.7/INSTALL_ATLAS.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.7/MANIFEST.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.7/PandaPkgInfo.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.7/panda-server.spec
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.7/package/hatch_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/brokerage/broker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/config/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/config/config_utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/config/daemon_config.py
--rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/config/panda_config.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/configurator/Carbon.py
--rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/configurator/Configurator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/configurator/__init__.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/configurator/aux.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/master.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/master_systemd.py
--rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/cache_pilots.py
--rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/cache_schedconfig.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0        0        0    63820 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/AdderSimplePlugin.py
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/DataServiceUtils.py
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/__init__.py
--rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/activator.py
--rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/closer.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/closer_atlas_plugin.py
--rwxr-xr-x   0        0        0    39936 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/ddm.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/ddm_handler.py
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/dyn_data_distributer.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/event_lookup_client_ei.py
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/event_picker.py
--rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/finisher.py
--rwxr-xr-x   0        0        0     7957 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/setupper.py
--rwxr-xr-x   0        0        0   117529 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/setupper_atlas_plugin.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/setupper_dummy_plugin.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/dataservice/setupper_plugin_base.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/jobdispatcher/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/proxycache/__init__.py
--rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/proxycache/panda_proxy_cache.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/server/.gacl
--rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/server/panda.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/srvcore/__init__.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/srvcore/allowed_methods.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/srvcore/panda_request.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/srvcore/srv_msg_utils.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0        0        0  1268846 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/PickleFileSpec.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/PickleJobSpec.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/SQLManager.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0        0        0   143228 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0        0        0    27435 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/task_split_rules.py
--rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/taskbuffer/workflow_processor.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/SchemaChecker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/banUser.py
--rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/boostPrio.py
--rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/boostUser.py
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/callbackDDM.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/daod_on_demand.py
--rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/finishJob.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/finishTaskJEDI.py
--rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/getJobs.py
--rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/killJob.py
--rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/killTask.py
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/killUser.py
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/reassignJobs.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/reassignSite.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/reassignTask.py
--rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/reassignWaiting.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/reloadInputDS.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/setPriority.py
--rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testEvgen.py
--rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testG4sim.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testG4sim17.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testGlobalShares.py
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testReco.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testSiteMap.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/testutils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/alice/README.txt
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/alice/mysetup
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/lsst/README.txt
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
--rwxr-xr-x   0        0        0    80539 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/userinterface/Client.py
--rw-r--r--   0        0        0    91540 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/userinterface/UserIF.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/userinterface/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/psnakemake_container.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/psnakemake_task.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/psnakemake_test.py
--rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.7/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/conda_meta.yaml.template
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/panda_server-httpd.conf.rpmnew.template
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/panda_server.cfg.rpmnew.template
--rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/bin/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/bin/panda_server-vomsrenew.exe.template
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/init.d/panda_server.exe.template
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/logrotate.d/panda_server.logrotate.template
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/sysconfig/panda_server.sysconfig.rpmnew.template
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/sysconfig/panda_server.sysconfig_for_systemd.template
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/sysconfig/panda_server_env.systemd.rpmnew.template
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/systemd/panda.service.template
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/systemd/panda_daemon.service.template
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 panda_server-0.3.7/templates/systemd/panda_httpd.service.template
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.7/LICENSE.txt
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.7/README.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 panda_server-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 panda_server-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.8/ChangeLog.txt
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.8/Dockerfile
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.8/INSTALL.md
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.8/INSTALL_ATLAS.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.8/MANIFEST.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.8/PandaPkgInfo.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.8/panda-server.spec
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.8/package/hatch_build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/brokerage/broker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/config/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/config/config_utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/config/panda_config.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/configurator/Carbon.py
+-rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/configurator/Configurator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/configurator/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/configurator/aux.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/master.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/master_systemd.py
+-rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/cache_pilots.py
+-rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/cache_schedconfig.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0        0        0    63820 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/AdderSimplePlugin.py
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/DataServiceUtils.py
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/__init__.py
+-rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/activator.py
+-rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/closer.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/closer_atlas_plugin.py
+-rwxr-xr-x   0        0        0    39936 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/ddm.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/ddm_handler.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/dyn_data_distributer.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/event_lookup_client_ei.py
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/event_picker.py
+-rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/finisher.py
+-rwxr-xr-x   0        0        0     7957 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/setupper.py
+-rwxr-xr-x   0        0        0   117475 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/setupper_atlas_plugin.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/setupper_dummy_plugin.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/dataservice/setupper_plugin_base.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/jobdispatcher/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/proxycache/__init__.py
+-rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/proxycache/panda_proxy_cache.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/server/.gacl
+-rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/server/panda.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/srvcore/__init__.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/srvcore/allowed_methods.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/srvcore/panda_request.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/srvcore/srv_msg_utils.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0        0        0    28740 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0        0        0  1268846 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/PickleFileSpec.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/PickleJobSpec.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/SQLManager.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0        0        0   143228 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0        0        0    27435 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/task_split_rules.py
+-rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/taskbuffer/workflow_processor.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/banUser.py
+-rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/boostUser.py
+-rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/callbackDDM.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/daod_on_demand.py
+-rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/finishJob.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/finishTaskJEDI.py
+-rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/getJobs.py
+-rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/killJob.py
+-rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/killTask.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/killUser.py
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/reassignJobs.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/reassignSite.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/setPriority.py
+-rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testG4sim.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testG4sim17.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testReco.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testSiteMap.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/testutils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/alice/README.txt
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/alice/mysetup
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/lsst/README.txt
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
+-rwxr-xr-x   0        0        0    80539 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/userinterface/Client.py
+-rw-r--r--   0        0        0    91540 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/userinterface/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/__init__.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/psnakemake_container.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/psnakemake_task.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/psnakemake_test.py
+-rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.8/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/conda_meta.yaml.template
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/panda_server-httpd.conf.rpmnew.template
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/panda_server.cfg.rpmnew.template
+-rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/bin/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/bin/panda_server-vomsrenew.exe.template
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/init.d/panda_server.exe.template
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/logrotate.d/panda_server.logrotate.template
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/sysconfig/panda_server.sysconfig_for_systemd.template
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/sysconfig/panda_server_env.systemd.rpmnew.template
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/systemd/panda.service.template
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/systemd/panda_daemon.service.template
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 panda_server-0.3.8/templates/systemd/panda_httpd.service.template
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.8/LICENSE.txt
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.8/README.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 panda_server-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 panda_server-0.3.8/PKG-INFO
```

### Comparing `panda_server-0.3.7/ChangeLog.txt` & `panda_server-0.3.8/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/Dockerfile` & `panda_server-0.3.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/INSTALL.md` & `panda_server-0.3.8/INSTALL.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/INSTALL_ATLAS.md` & `panda_server-0.3.8/INSTALL_ATLAS.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/panda-server.spec` & `panda_server-0.3.8/panda-server.spec`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/package/hatch_build.py` & `panda_server-0.3.8/package/hatch_build.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/brokerage/SiteMapper.py` & `panda_server-0.3.8/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/brokerage/broker.py` & `panda_server-0.3.8/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/config/daemon_config.py` & `panda_server-0.3.8/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/config/panda_config.py` & `panda_server-0.3.8/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/configurator/Carbon.py` & `panda_server-0.3.8/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/configurator/Configurator.py` & `panda_server-0.3.8/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/configurator/aux.py` & `panda_server-0.3.8/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/master.py` & `panda_server-0.3.8/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/master_systemd.py` & `panda_server-0.3.8/pandaserver/daemons/master_systemd.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/utils.py` & `panda_server-0.3.8/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/add_main.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/add_sub.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/cache_pilots.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/cache_pilots.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/cache_schedconfig.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/cache_schedconfig.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/carbon.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/configurator.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/copyArchive.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/datasetManager.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/evpPD2P.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/metric_collector.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/pilotStreaming.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/task_evaluator.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/tmpwatch.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/daemons/scripts/worker_synchronization.py` & `panda_server-0.3.8/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda_server-0.3.8/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/AdderGen.py` & `panda_server-0.3.8/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/AdderResult.py` & `panda_server-0.3.8/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/AdderSimplePlugin.py` & `panda_server-0.3.8/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/DataServiceUtils.py` & `panda_server-0.3.8/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/ProcessLimiter.py` & `panda_server-0.3.8/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda_server-0.3.8/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/activator.py` & `panda_server-0.3.8/pandaserver/dataservice/activator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/closer.py` & `panda_server-0.3.8/pandaserver/dataservice/closer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/closer_atlas_plugin.py` & `panda_server-0.3.8/pandaserver/dataservice/closer_atlas_plugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/ddm.py` & `panda_server-0.3.8/pandaserver/dataservice/ddm.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/ddm_handler.py` & `panda_server-0.3.8/pandaserver/dataservice/ddm_handler.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/dyn_data_distributer.py` & `panda_server-0.3.8/pandaserver/dataservice/dyn_data_distributer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/event_lookup_client_ei.py` & `panda_server-0.3.8/pandaserver/dataservice/event_lookup_client_ei.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/event_picker.py` & `panda_server-0.3.8/pandaserver/dataservice/event_picker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/finisher.py` & `panda_server-0.3.8/pandaserver/dataservice/finisher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/setupper.py` & `panda_server-0.3.8/pandaserver/dataservice/setupper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/setupper_atlas_plugin.py` & `panda_server-0.3.8/pandaserver/dataservice/setupper_atlas_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,35 +5,34 @@
 
 import datetime
 import re
 import sys
 import time
 import traceback
 import uuid
+from typing import Dict, List, Optional, Tuple
 
-from typing import List, Dict, Tuple, Optional
 from rucio.common.exception import DataIdentifierNotFound
 
 import pandaserver.brokerage.broker
-
 from pandaserver.brokerage.SiteMapper import SiteMapper
 from pandaserver.dataservice import DataServiceUtils, ErrorCode
 from pandaserver.dataservice.DataServiceUtils import select_scope
 from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.dataservice.setupper_plugin_base import SetupperPluginBase
 from pandaserver.taskbuffer import EventServiceUtils, JobUtils
 from pandaserver.taskbuffer.DatasetSpec import DatasetSpec
 
 
-
 class SetupperAtlasPlugin(SetupperPluginBase):
     """
     setup dataset for ATLAS
 
     """
+
     # constructor
     def __init__(self, taskBuffer, jobs: List, logger, **params: Dict) -> None:
         """
         Constructor for the SetupperAtlasPlugin class.
 
         :param taskBuffer: The buffer for tasks.
         :param jobs: The jobs to be processed.
@@ -502,15 +501,15 @@
         dest_error = {}
         dataset_list = {}
         newname_list = {}
         sn_gotten_ds = []
         if start_idx == -1:
             jobs_list = self.jobs
         else:
-            jobs_list = self.jobs[start_idx: start_idx + n_jobs_in_loop]
+            jobs_list = self.jobs[start_idx : start_idx + n_jobs_in_loop]
         for job in jobs_list:
             # ignore failed jobs
             if job.jobStatus in ["failed", "cancelled"] or job.isCancelled():
                 continue
             for file in job.Files:
                 # ignore input files
                 if file.type in ["input", "pseudo_input"]:
@@ -1372,22 +1371,21 @@
                             ):
                                 tmp_input_file_type = tmp_input_items[4]
                 # set input type and project
                 if tmp_job.prodDBlock not in ["", None, "NULL"]:
                     # input project
                     if tmp_input_file_project is not None:
                         tmp_job.inputFileProject = tmp_input_file_project
-                    # input type
-                    if tmp_input_file_type is not None:
-                        tmp_job.inputFileType = tmp_input_file_type
                 # protection
                 max_input_file_bytes = 99999999999
                 tmp_job.inputFileBytes = min(tmp_job.inputFileBytes, max_input_file_bytes)
                 # set background-able flag
                 tmp_job.setBackgroundableFlag()
+                # set input and output file types
+                tmp_job.set_input_output_file_types()
             except Exception:
                 error_type, error_value = sys.exc_info()[:2]
                 self.logger.error(f"failed to set data summary fields for PandaID={tmp_job.PandaID}: {error_type} {error_value}")
         # send jobs to jobs_waiting
         self.task_buffer.keepJobs(jobs_waiting)
         # update failed job
         self.update_failed_jobs(jobs_failed)
@@ -1502,15 +1500,14 @@
             datasets, out = rucioAPI.list_datasets_in_container(container)
             if datasets is not None:
                 return True, datasets
             time.sleep(10)
         self.logger.error(out)
         return False, out
 
-
     # get datasets in container
     def get_list_dataset_replicas_in_container(self, container: str, get_map: bool = False) -> Tuple[int, str]:
         """
         Get list dataset replicas in container method for running the setup process.
 
         :param container: The container to get the list of dataset replicas from.
         :param get_map: Whether to get the map. Defaults to False.
```

### Comparing `panda_server-0.3.7/pandaserver/dataservice/setupper_dummy_plugin.py` & `panda_server-0.3.8/pandaserver/dataservice/setupper_dummy_plugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/dataservice/setupper_plugin_base.py` & `panda_server-0.3.8/pandaserver/dataservice/setupper_plugin_base.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda_server-0.3.8/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/jobdispatcher/JobDispatcher.py` & `panda_server-0.3.8/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/jobdispatcher/Protocol.py` & `panda_server-0.3.8/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/jobdispatcher/Watcher.py` & `panda_server-0.3.8/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/proxycache/panda_proxy_cache.py` & `panda_server-0.3.8/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/server/panda.py` & `panda_server-0.3.8/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/srvcore/CoreUtils.py` & `panda_server-0.3.8/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/srvcore/MailUtils.py` & `panda_server-0.3.8/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/srvcore/allowed_methods.py` & `panda_server-0.3.8/pandaserver/srvcore/allowed_methods.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/srvcore/oidc_utils.py` & `panda_server-0.3.8/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/srvcore/panda_request.py` & `panda_server-0.3.8/pandaserver/srvcore/panda_request.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/srvcore/srv_msg_utils.py` & `panda_server-0.3.8/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/CloudSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/ConBridge.py` & `panda_server-0.3.8/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/DBProxyPool.py` & `panda_server-0.3.8/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/DatasetSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/DdmSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/ErrorCode.py` & `panda_server-0.3.8/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/EventServiceUtils.py` & `panda_server-0.3.8/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/FileSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/GlobalShares.py` & `panda_server-0.3.8/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/Initializer.py` & `panda_server-0.3.8/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/JobSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/JobSpec.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         "memory_leak",
         "memory_leak_x2",
         "container_name",
         "job_label",
         "gco2_regional",
         "gco2_global",
         "cpu_architecture_level",
+        "outputFileType",
     )
     # slots
     __slots__ = _attributes + ("Files", "_changedAttrs", "_reserveChangedState")
     # attributes which have 0 by default
     _zeroAttrs = (
         "assignedPriority",
         "currentPriority",
@@ -177,14 +178,16 @@
         "jobDispatcherErrorDiag": 250,
         "brokerageErrorDiag": 250,
         "pilotErrorDiag": 500,
         "exeErrorDiag": 500,
         "jobSubStatus": 80,
         "supErrorDiag": 250,
         "commandToPilot": 250,
+        "inputFileType": 32,
+        "outputFileType": 32,
     }
     # tag for special handling
     _tagForSH = {
         "altStgOut": "ao",
         "acceptPartial": "ap",
         "allOkEvents": "at",
         "notDiscardEvents": "de",
@@ -876,14 +879,48 @@
         self.__setstate__(job_state[:-1] + [[]])
         # add files
         for file_stat in job_state[-1]:
             file_spec = FileSpec()
             file_spec.__setstate__(file_stat)
             self.addFile(file_spec)
 
+    # set input and output file types
+    def set_input_output_file_types(self) -> None:
+        """
+        Set input and output file types based on the input and output file names
+        """
+        in_types = set()
+        out_types = set()
+        for tmp_file in self.Files:
+            # ignore DBRelease/lib.tgz files
+            if tmp_file.dataset.startswith("ddo") or tmp_file.lfn.endswith(".lib.tgz"):
+                continue
+            # extract type while ignoring user/group/groupXY
+            tmp_items = tmp_file.dataset.split(".")
+            if (
+                len(tmp_items) > 4
+                and (not tmp_items[0] in ["", "NULL", "user", "group", "hc_test"])
+                and (not tmp_items[0].startswith("group"))
+                and not tmp_file.dataset.startswith("panda.um.")
+            ):
+                tmp_type = tmp_items[4]
+            else:
+                continue
+            if tmp_file.type == "input":
+                in_types.add(tmp_type)
+            elif tmp_file.type == "output":
+                out_types.add(tmp_type)
+        # set types
+        if in_types:
+            in_types = sorted(list(in_types))
+            self.inputFileType = ",".join(in_types)[: self._limitLength["inputFileType"]]
+        if out_types:
+            out_types = sorted(list(out_types))
+            self.outputFileType = ",".join(out_types)[: self._limitLength["outputFileType"]]
+
 
 # utils
 
 
 # check if to push status changes without class instance
 def push_status_changes(special_handling):
     if special_handling is not None:
```

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/JobUtils.py` & `panda_server-0.3.8/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/NucleusSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/OraDBProxy.py` & `panda_server-0.3.8/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/PickleFileSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/PickleFileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/PickleJobSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/PickleJobSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/PrioUtil.py` & `panda_server-0.3.8/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/ProcessGroups.py` & `panda_server-0.3.8/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/ResourceSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/SQLDumper.py` & `panda_server-0.3.8/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/SQLManager.py` & `panda_server-0.3.8/pandaserver/taskbuffer/SQLManager.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/SiteSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/TaskBuffer.py` & `panda_server-0.3.8/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda_server-0.3.8/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/Utils.py` & `panda_server-0.3.8/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/WorkerSpec.py` & `panda_server-0.3.8/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/WrappedCursor.py` & `panda_server-0.3.8/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/WrappedPickle.py` & `panda_server-0.3.8/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/retryModule.py` & `panda_server-0.3.8/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/task_split_rules.py` & `panda_server-0.3.8/pandaserver/taskbuffer/task_split_rules.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/taskbuffer/workflow_processor.py` & `panda_server-0.3.8/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/SchemaChecker.py` & `panda_server-0.3.8/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/banUser.py` & `panda_server-0.3.8/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/boostPrio.py` & `panda_server-0.3.8/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/boostUser.py` & `panda_server-0.3.8/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/callbackDDM.py` & `panda_server-0.3.8/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/daod_on_demand.py` & `panda_server-0.3.8/pandaserver/test/daod_on_demand.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/finishJob.py` & `panda_server-0.3.8/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/getJobs.py` & `panda_server-0.3.8/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/killJob.py` & `panda_server-0.3.8/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/killJobLowPrio.py` & `panda_server-0.3.8/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/killJobsInTask.py` & `panda_server-0.3.8/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/killProdJobs.py` & `panda_server-0.3.8/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/killTask.py` & `panda_server-0.3.8/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/killUser.py` & `panda_server-0.3.8/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/reassignSite.py` & `panda_server-0.3.8/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/reassignTask.py` & `panda_server-0.3.8/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/reassignWaiting.py` & `panda_server-0.3.8/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/reloadInputDS.py` & `panda_server-0.3.8/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/sendCommandToJob.py` & `panda_server-0.3.8/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/setDebugMode.py` & `panda_server-0.3.8/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/setPriority.py` & `panda_server-0.3.8/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testEvgen.py` & `panda_server-0.3.8/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testEvgen17.py` & `panda_server-0.3.8/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testG4sim.py` & `panda_server-0.3.8/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testG4sim17.py` & `panda_server-0.3.8/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda_server-0.3.8/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testGlobalShares.py` & `panda_server-0.3.8/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testJobFlowATLAS.py` & `panda_server-0.3.8/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testReco.py` & `panda_server-0.3.8/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testSimulReco14.py` & `panda_server-0.3.8/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testSiteMap.py` & `panda_server-0.3.8/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/testutils.py` & `panda_server-0.3.8/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda_server-0.3.8/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda_server-0.3.8/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/lsst/lsstSubmit.py` & `panda_server-0.3.8/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda_server-0.3.8/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda_server-0.3.8/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh` & `panda_server-0.3.8/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/userinterface/Client.py` & `panda_server-0.3.8/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/userinterface/UserIF.py` & `panda_server-0.3.8/pandaserver/userinterface/UserIF.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/pcwl_test.py` & `panda_server-0.3.8/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/pcwl_utils.py` & `panda_server-0.3.8/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/psnakemake_container.json` & `panda_server-0.3.8/pandaserver/workflow/psnakemake_container.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/psnakemake_task.json` & `panda_server-0.3.8/pandaserver/workflow/psnakemake_task.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/psnakemake_test.py` & `panda_server-0.3.8/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/workflow_utils.py` & `panda_server-0.3.8/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/snakeparser/extensions.py` & `panda_server-0.3.8/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/snakeparser/log.py` & `panda_server-0.3.8/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/snakeparser/parser.py` & `panda_server-0.3.8/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pandaserver/workflow/snakeparser/utils.py` & `panda_server-0.3.8/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/conda_meta.yaml.template` & `panda_server-0.3.8/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda_server-0.3.8/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/panda_server-httpd.conf.rpmnew.template` & `panda_server-0.3.8/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/panda_server.cfg.rpmnew.template` & `panda_server-0.3.8/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/bin/panda_server-makeSlsXml.exe.template` & `panda_server-0.3.8/templates/bin/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/bin/panda_server-vomsrenew.exe.template` & `panda_server-0.3.8/templates/bin/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/init.d/panda_daemon.exe.template` & `panda_server-0.3.8/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/init.d/panda_httpd.exe.template` & `panda_server-0.3.8/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/init.d/panda_server.exe.template` & `panda_server-0.3.8/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/logrotate.d/panda_server.logrotate.template` & `panda_server-0.3.8/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda_server-0.3.8/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/templates/sysconfig/panda_server_env.systemd.rpmnew.template` & `panda_server-0.3.8/templates/sysconfig/panda_server_env.systemd.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/LICENSE.txt` & `panda_server-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/pyproject.toml` & `panda_server-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.7/PKG-INFO` & `panda_server-0.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panda-server
-Version: 0.3.7
+Version: 0.3.8
 Summary: PanDA Server Package
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <panda-support@cern.ch>
 License: Apache-2.0
 License-File: LICENSE.txt
 Requires-Python: >=3.8
 Requires-Dist: cwl-utils>=0.13
```

