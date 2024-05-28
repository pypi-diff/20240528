# Comparing `tmp/ampel_alerts-0.9.0.tar.gz` & `tmp/ampel_alerts-0.9.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_alerts-0.9.0.tar", max compression
+gzip compressed data, was "ampel_alerts-0.9.1a0.tar", max compression
```

## Comparing `ampel_alerts-0.9.0.tar` & `ampel_alerts-0.9.1a0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1512 2023-04-06 20:15:05.586679 ampel_alerts-0.9.0/LICENSE
--rw-r--r--   0        0        0     3417 2023-04-06 20:15:05.586679 ampel_alerts-0.9.0/README.md
--rwxr-xr-x   0        0        0     1075 2023-04-06 20:15:05.586679 ampel_alerts-0.9.0/ampel/abstract/AbsAlertFilter.py
--rwxr-xr-x   0        0        0     1207 2023-04-06 20:15:05.586679 ampel_alerts-0.9.0/ampel/abstract/AbsAlertLoader.py
--rw-r--r--   0        0        0     1024 2023-04-06 20:15:05.586679 ampel_alerts-0.9.0/ampel/abstract/AbsAlertRegister.py
--rwxr-xr-x   0        0        0     1324 2023-04-06 20:15:05.586679 ampel_alerts-0.9.0/ampel/abstract/AbsAlertSupplier.py
--rwxr-xr-x   0        0        0    14569 2023-04-06 20:15:05.586679 ampel_alerts-0.9.0/ampel/alert/AlertConsumer.py
--rw-r--r--   0        0        0      532 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/AlertConsumerError.py
--rw-r--r--   0        0        0     1340 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/AlertConsumerMetrics.py
--rw-r--r--   0        0        0     2550 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/AlertFileList.py
--rwxr-xr-x   0        0        0     2957 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/BaseAlertSupplier.py
--rwxr-xr-x   0        0        0     9978 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/FilterBlock.py
--rwxr-xr-x   0        0        0     4646 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/FilterBlocksHandler.py
--rwxr-xr-x   0        0        0     1691 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/FilteringAlertSupplier.py
--rwxr-xr-x   0        0        0     3434 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/filter/BasicMultiFilter.py
--rwxr-xr-x   0        0        0     3018 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/load/DirAlertLoader.py
--rwxr-xr-x   0        0        0     1417 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/load/DirFileNamesLoader.py
--rwxr-xr-x   0        0        0     1518 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/load/DirTaggedAlertLoader.py
--rwxr-xr-x   0        0        0     1047 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/load/FileAlertLoader.py
--rwxr-xr-x   0        0        0     3371 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/load/TarAlertLoader.py
--rw-r--r--   0        0        0     1056 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/load/TarballWalker.py
--rwxr-xr-x   0        0        0     6946 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/reject/BaseAlertRegister.py
--rwxr-xr-x   0        0        0     5593 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/reject/DBRejectedLogsHandler.py
--rwxr-xr-x   0        0        0     1572 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/reject/FullActiveAlertRegister.py
--rwxr-xr-x   0        0        0     2108 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/reject/FullAlertRegister.py
--rwxr-xr-x   0        0        0     1585 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/reject/GeneralActiveAlertRegister.py
--rwxr-xr-x   0        0        0     1150 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/reject/GeneralAlertRegister.py
--rwxr-xr-x   0        0        0     1258 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/reject/MinimalActiveAlertRegister.py
--rwxr-xr-x   0        0        0     1962 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/alert/reject/MinimalAlertRegister.py
--rwxr-xr-x   0        0        0    12488 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/dev/AutoCompleteBenchmark.py
--rwxr-xr-x   0        0        0     1013 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/dev/UnitTestAlertSupplier.py
--rwxr-xr-x   0        0        0     2018 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/model/AlertConsumerModel.py
--rw-r--r--   0        0        0        0 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/py.typed
--rwxr-xr-x   0        0        0     6204 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/ampel/template/AbsEasyChannelTemplate.py
--rw-r--r--   0        0        0      370 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/conf/ampel-alerts/ampel.yml
--rw-r--r--   0        0        0     1434 2023-04-06 20:15:05.590679 ampel_alerts-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4595 1970-01-01 00:00:00.000000 ampel_alerts-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/LICENSE
+-rw-r--r--   0        0        0     3417 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/README.md
+-rwxr-xr-x   0        0        0     1075 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/abstract/AbsAlertFilter.py
+-rwxr-xr-x   0        0        0     1333 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/abstract/AbsAlertLoader.py
+-rw-r--r--   0        0        0     1024 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/abstract/AbsAlertRegister.py
+-rwxr-xr-x   0        0        0     1467 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/abstract/AbsAlertSupplier.py
+-rwxr-xr-x   0        0        0    14762 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/AlertConsumer.py
+-rw-r--r--   0        0        0      532 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/AlertConsumerError.py
+-rw-r--r--   0        0        0     1340 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/AlertConsumerMetrics.py
+-rw-r--r--   0        0        0     2550 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/AlertFileList.py
+-rwxr-xr-x   0        0        0     2957 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/BaseAlertSupplier.py
+-rwxr-xr-x   0        0        0     9978 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/FilterBlock.py
+-rwxr-xr-x   0        0        0     4646 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/FilterBlocksHandler.py
+-rwxr-xr-x   0        0        0     1691 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/FilteringAlertSupplier.py
+-rwxr-xr-x   0        0        0     3434 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/filter/BasicMultiFilter.py
+-rwxr-xr-x   0        0        0     3018 2023-12-19 10:08:13.150620 ampel_alerts-0.9.1a0/ampel/alert/load/DirAlertLoader.py
+-rwxr-xr-x   0        0        0     1417 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/load/DirFileNamesLoader.py
+-rwxr-xr-x   0        0        0     1518 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/load/DirTaggedAlertLoader.py
+-rwxr-xr-x   0        0        0     1047 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/load/FileAlertLoader.py
+-rwxr-xr-x   0        0        0     3356 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/load/TarAlertLoader.py
+-rw-r--r--   0        0        0     1056 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/load/TarballWalker.py
+-rwxr-xr-x   0        0        0     6946 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/reject/BaseAlertRegister.py
+-rwxr-xr-x   0        0        0     5593 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/reject/DBRejectedLogsHandler.py
+-rwxr-xr-x   0        0        0     1572 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/reject/FullActiveAlertRegister.py
+-rwxr-xr-x   0        0        0     2108 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/reject/FullAlertRegister.py
+-rwxr-xr-x   0        0        0     1585 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/reject/GeneralActiveAlertRegister.py
+-rwxr-xr-x   0        0        0     1150 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/reject/GeneralAlertRegister.py
+-rwxr-xr-x   0        0        0     1258 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/reject/MinimalActiveAlertRegister.py
+-rwxr-xr-x   0        0        0     1962 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/alert/reject/MinimalAlertRegister.py
+-rwxr-xr-x   0        0        0    12488 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/dev/AutoCompleteBenchmark.py
+-rwxr-xr-x   0        0        0     1013 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/dev/UnitTestAlertSupplier.py
+-rwxr-xr-x   0        0        0     2018 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/model/AlertConsumerModel.py
+-rw-r--r--   0        0        0        0 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/py.typed
+-rwxr-xr-x   0        0        0     6204 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/template/AbsEasyChannelTemplate.py
+-rw-r--r--   0        0        0     2902 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/ampel/template/EasyAlertConsumerTemplate.py
+-rw-r--r--   0        0        0      439 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/conf/ampel-alerts/ampel.yml
+-rw-r--r--   0        0        0     1433 2023-12-19 10:08:13.154620 ampel_alerts-0.9.1a0/pyproject.toml
+-rw-r--r--   0        0        0     4651 1970-01-01 00:00:00.000000 ampel_alerts-0.9.1a0/PKG-INFO
```

### Comparing `ampel_alerts-0.9.0/LICENSE` & `ampel_alerts-0.9.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/README.md` & `ampel_alerts-0.9.1a0/README.md`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/abstract/AbsAlertFilter.py` & `ampel_alerts-0.9.1a0/ampel/abstract/AbsAlertFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/abstract/AbsAlertLoader.py` & `ampel_alerts-0.9.1a0/ampel/abstract/AbsAlertSupplier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# File:                Ampel-alerts/ampel/abstract/AbsAlertLoader.py
+# File:                Ampel-alerts/ampel/abstract/AbsAlertSupplier.py
 # License:             BSD-3-Clause
 # Author:              valery brinnel <firstname.lastname@gmail.com>
-# Date:                26.06.2021
+# Date:                23.04.2018
 # Last Modified Date:  19.12.2022
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
-from ampel.types import T
-from typing import Generic
-from collections.abc import Iterator
-from ampel.struct.Resource import Resource
+from typing import Iterator
 from ampel.log.AmpelLogger import AmpelLogger
 from ampel.base.AmpelABC import AmpelABC
 from ampel.base.decorator import abstractmethod
-from ampel.base.AmpelBaseModel import AmpelBaseModel
+from ampel.base.AmpelUnit import AmpelUnit
+from ampel.struct.Resource import Resource
+from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
 
 
-class AbsAlertLoader(Generic[T], AmpelABC, AmpelBaseModel, abstract=True):
+class AbsAlertSupplier(AmpelUnit, AmpelABC, abstract=True):
+	"""
+	Iterable class that, for each alert payload provided by the underlying alert_loader,
+	returns an object that implements :class:`~ampel.protocol.AmpelAlertProtocol`.
+	"""
 
 	def __init__(self, **kwargs) -> None:
 		super().__init__(**kwargs)
 		self.logger: AmpelLogger = AmpelLogger.get_logger()
 		self.resources: dict[str, Resource] = {}
 
 	def set_logger(self, logger: AmpelLogger) -> None:
 		self.logger = logger
 
 	def add_resource(self, name: str, value: Resource) -> None:
 		self.resources[name] = value
 
-	def __iter__(self) -> Iterator[T]: # type: ignore
-		return self
-
 	@abstractmethod
-	def __next__(self) -> T:
+	def __iter__(self) -> Iterator[AmpelAlertProtocol]:
+		...
+
+	def acknowledge(self, alerts: Iterator[AmpelAlertProtocol]) -> None:
+		"""Inform the source that a batch of alerts has been handled"""
 		...
```

### Comparing `ampel_alerts-0.9.0/ampel/abstract/AbsAlertRegister.py` & `ampel_alerts-0.9.1a0/ampel/abstract/AbsAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/AlertConsumer.py` & `ampel_alerts-0.9.1a0/ampel/alert/AlertConsumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,15 @@
 		if db_logging_handler := logger.get_db_logging_handler():
 			db_logging_handler.auto_flush = False
 
 		# Collects and executes pymongo.operations in collection Ampel_data
 		updates_buffer = DBUpdatesBuffer(
 			self._ampel_db, run_id, logger,
 			error_callback = self.set_cancel_run,
+			acknowledge_callback = self.alert_supplier.acknowledge,
 			catch_signals = False, # we do it ourself
 			max_size = self.updates_buffer_size
 		)
 
 		any_filter = any([fb.filter_model for fb in self._fbh.filter_blocks])
 
 		# Set ingesters up
@@ -321,62 +322,66 @@
 									logger.error("Max number of error reached, breaking alert processing")
 									self.set_cancel_run(AlertConsumerError.TOO_MANY_ERRORS)
 				else:
 					# if bypassing filters, track passing rates at top level
 					for counter in stats.filter_accepted:
 						counter.inc()
 
-				if filter_results:
+				with updates_buffer.group_updates():
 
-					stats.accepted.inc()
+					if filter_results:
 
-					try:
-						alert_extra: dict[str, Any] = {'alert': alert.id}
-						if self.include_alert_extra_with_keys and alert.extra:
-							for key, path in self.include_alert_extra_with_keys.items():
-								alert_extra[key] = get_by_path(alert.extra, path)
-						with stat_time.labels("ingest").time():
-							ing_hdlr.ingest(
-								alert.datapoints, filter_results, stock_id, alert.tag,
-								alert_extra, alert.extra.get('stock') if alert.extra else None
-							)
-					except (PyMongoError, AmpelLoggingError) as e:
-						print("%s: abording run() procedure" % e.__class__.__name__)
-						report_ingest_error(e, alert, filter_results)
-						raise e
+						stats.accepted.inc()
 
-					except Exception as e:
-						report_ingest_error(e, alert, filter_results)
-
-						if self.raise_exc:
+						try:
+							alert_extra: dict[str, Any] = {'alert': alert.id}
+							if self.include_alert_extra_with_keys and alert.extra:
+								for key, path in self.include_alert_extra_with_keys.items():
+									alert_extra[key] = get_by_path(alert.extra, path)
+							with stat_time.labels("ingest").time():
+								ing_hdlr.ingest(
+									alert.datapoints, filter_results, stock_id, alert.tag,
+									alert_extra, alert.extra.get('stock') if alert.extra else None
+								)
+						except (PyMongoError, AmpelLoggingError) as e:
+							print("%s: abording run() procedure" % e.__class__.__name__)
+							report_ingest_error(e, alert, filter_results)
 							raise e
 
-						if self.error_max:
-							err += 1
-
-						if err == self.error_max:
-							logger.error("Max number of error reached, breaking alert processing")
-							self.set_cancel_run(AlertConsumerError.TOO_MANY_ERRORS)
+						except Exception as e:
+							report_ingest_error(e, alert, filter_results)
 
-				else:
+							if self.raise_exc:
+								raise e
 
-					# All channels reject this alert
-					# no log entries goes into the main logs collection sinces those are redirected to Ampel_rej.
+							if self.error_max:
+								err += 1
 
-					# So we add a notification manually. For that, we don't use logger
-					# cause rejection messages were alreary logged into the console
-					# by the StreamHandler in channel specific RecordBufferingHandler instances.
-					# So we address directly db_logging_handler, and for that, we create
-					# a LogDocument manually.
-					lr = LightLogRecord(logger.name, LogFlag.INFO | logger.base_flag)
-					lr.stock = stock_id
-					lr.channel = reduced_chan_names # type: ignore[assignment]
-					lr.extra = {'a': alert.id, 'allout': True}
-					if db_logging_handler:
-						db_logging_handler.handle(lr)
+							if err == self.error_max:
+								logger.error("Max number of error reached, breaking alert processing")
+								self.set_cancel_run(AlertConsumerError.TOO_MANY_ERRORS)
+
+					else:
+
+						# All channels reject this alert
+						# no log entries goes into the main logs collection sinces those are redirected to Ampel_rej.
+
+						# So we add a notification manually. For that, we don't use logger
+						# cause rejection messages were alreary logged into the console
+						# by the StreamHandler in channel specific RecordBufferingHandler instances.
+						# So we address directly db_logging_handler, and for that, we create
+						# a LogDocument manually.
+						lr = LightLogRecord(logger.name, LogFlag.INFO | logger.base_flag)
+						lr.stock = stock_id
+						lr.channel = reduced_chan_names # type: ignore[assignment]
+						lr.extra = {'a': alert.id, 'allout': True}
+						if db_logging_handler:
+							db_logging_handler.handle(lr)
+					
+					updates_buffer.acknowledge_on_push(alert)
 
 				iter_count += 1
 				stats.alerts.inc()
 
 				updates_buffer.check_push()
 				if db_logging_handler:
 					db_logging_handler.check_flush()
```

### Comparing `ampel_alerts-0.9.0/ampel/alert/AlertConsumerError.py` & `ampel_alerts-0.9.1a0/ampel/alert/AlertConsumerError.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/AlertConsumerMetrics.py` & `ampel_alerts-0.9.1a0/ampel/alert/AlertConsumerMetrics.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/AlertFileList.py` & `ampel_alerts-0.9.1a0/ampel/alert/AlertFileList.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/BaseAlertSupplier.py` & `ampel_alerts-0.9.1a0/ampel/alert/BaseAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/FilterBlock.py` & `ampel_alerts-0.9.1a0/ampel/alert/FilterBlock.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/FilterBlocksHandler.py` & `ampel_alerts-0.9.1a0/ampel/alert/FilterBlocksHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/FilteringAlertSupplier.py` & `ampel_alerts-0.9.1a0/ampel/alert/FilteringAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/filter/BasicMultiFilter.py` & `ampel_alerts-0.9.1a0/ampel/alert/filter/BasicMultiFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/load/DirAlertLoader.py` & `ampel_alerts-0.9.1a0/ampel/alert/load/DirAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/load/DirFileNamesLoader.py` & `ampel_alerts-0.9.1a0/ampel/alert/load/DirFileNamesLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/load/DirTaggedAlertLoader.py` & `ampel_alerts-0.9.1a0/ampel/alert/load/DirTaggedAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/load/FileAlertLoader.py` & `ampel_alerts-0.9.1a0/ampel/alert/load/FileAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/load/TarAlertLoader.py` & `ampel_alerts-0.9.1a0/ampel/alert/load/TarAlertLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,19 +42,17 @@
 			self.tar_file = tarfile.open(fileobj=self.file_obj, mode=self.tar_mode)
 		elif self.file_path:
 			self.tar_file = tarfile.open(self.file_path, mode=self.tar_mode)
 		else:
 			raise ValueError("Please provide value either for 'file_path' or 'file_obj'")
 
 		if self.start != 0:
-			count = 0
-			for tarinfo in self.tar_file:
-				count += 1
-				if count < self.start:
-					continue
+			for count, _ in enumerate(self.tar_file, 1):
+				if count >= self.start:
+					break
 
 
 	def __iter__(self):
 		return self
 
 
 	def __next__(self) -> IO[bytes]:
```

### Comparing `ampel_alerts-0.9.0/ampel/alert/load/TarballWalker.py` & `ampel_alerts-0.9.1a0/ampel/alert/load/TarballWalker.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/reject/BaseAlertRegister.py` & `ampel_alerts-0.9.1a0/ampel/alert/reject/BaseAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/reject/DBRejectedLogsHandler.py` & `ampel_alerts-0.9.1a0/ampel/alert/reject/DBRejectedLogsHandler.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/reject/FullActiveAlertRegister.py` & `ampel_alerts-0.9.1a0/ampel/alert/reject/FullActiveAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/reject/FullAlertRegister.py` & `ampel_alerts-0.9.1a0/ampel/alert/reject/FullAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/reject/GeneralActiveAlertRegister.py` & `ampel_alerts-0.9.1a0/ampel/alert/reject/GeneralActiveAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/reject/GeneralAlertRegister.py` & `ampel_alerts-0.9.1a0/ampel/alert/reject/GeneralAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/reject/MinimalActiveAlertRegister.py` & `ampel_alerts-0.9.1a0/ampel/alert/reject/MinimalActiveAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/alert/reject/MinimalAlertRegister.py` & `ampel_alerts-0.9.1a0/ampel/alert/reject/MinimalAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/dev/AutoCompleteBenchmark.py` & `ampel_alerts-0.9.1a0/ampel/dev/AutoCompleteBenchmark.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/dev/UnitTestAlertSupplier.py` & `ampel_alerts-0.9.1a0/ampel/dev/UnitTestAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/model/AlertConsumerModel.py` & `ampel_alerts-0.9.1a0/ampel/model/AlertConsumerModel.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/ampel/template/AbsEasyChannelTemplate.py` & `ampel_alerts-0.9.1a0/ampel/template/AbsEasyChannelTemplate.py`

 * *Files identical despite different names*

### Comparing `ampel_alerts-0.9.0/pyproject.toml` & `ampel_alerts-0.9.1a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-alerts"
-version = "0.9.0"
+version = "0.9.1a0"
 description = "Alert support for the Ampel system"
 authors = ["Valery Brinnel"]
 maintainers = ["Jakob van Santen <jakob.van.santen@desy.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://ampelproject.github.io"
 repository = "https://github.com/AmpelProject/Ampel-alerts"
@@ -22,27 +22,27 @@
     'conf/*/*.yaml',
     'conf/*/*/*.yaml',
     'conf/*/*.yml',
     'conf/*/*/*.yml',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
-Sphinx = {version = ">=6.1.2,<6.2.0", optional = true}
+python = "^3.10"
+Sphinx = {version = ">=7.2.0,<7.3.0", optional = true}
 sphinx-autodoc-typehints = {version = "^1.11.1", optional = true}
-tomlkit = {version = "^0.11.0", optional=true}
-ampel-interface = {version = "^0.9.0"}
-ampel-core = {version = "^0.9.0"}
+tomlkit = {version = "^0.12.0", optional=true}
+ampel-interface = {version = "^0.9.1a1"}
+ampel-core = {version = "^0.9.1a0"}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
+pytest = "^7.4.3"
+pytest-cov = "^4.1.0"
+pytest-mock = "^3.12.0"
 mongomock = "^4.1.2"
-mypy = "^1.1.1"
+mypy = "^1.7.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 server = ["fastapi", "uvicorn"]
```

### Comparing `ampel_alerts-0.9.0/PKG-INFO` & `ampel_alerts-0.9.1a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: ampel-alerts
-Version: 0.9.0
+Version: 0.9.1a0
 Summary: Alert support for the Ampel system
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Valery Brinnel
 Maintainer: Jakob van Santen
 Maintainer-email: jakob.van.santen@desy.de
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
 Provides-Extra: docs
 Provides-Extra: server
-Requires-Dist: Sphinx (>=6.1.2,<6.2.0) ; extra == "docs"
-Requires-Dist: ampel-core (>=0.9.0,<0.10.0)
-Requires-Dist: ampel-interface (>=0.9.0,<0.10.0)
+Requires-Dist: Sphinx (>=7.2.0,<7.3.0) ; extra == "docs"
+Requires-Dist: ampel-core (>=0.9.1a0,<0.10.0)
+Requires-Dist: ampel-interface (>=0.9.1a1,<0.10.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.11.1,<2.0.0) ; extra == "docs"
-Requires-Dist: tomlkit (>=0.11.0,<0.12.0) ; extra == "docs"
+Requires-Dist: tomlkit (>=0.12.0,<0.13.0) ; extra == "docs"
 Project-URL: Repository, https://github.com/AmpelProject/Ampel-alerts
 Description-Content-Type: text/markdown
 
 <img align="left" src="https://user-images.githubusercontent.com/17532220/213289600-aa1757d2-44ba-4de2-b12d-520ddb5d39ff.png" width="150" height="150"/>  
 <br>
 
 # Alert support for AMPEL
```

