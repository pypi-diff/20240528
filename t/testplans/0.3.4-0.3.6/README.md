# Comparing `tmp/testplans-0.3.4.tar.gz` & `tmp/testplans-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.3.4.tar", last modified: Thu May 23 14:38:09 2024, max compression
+gzip compressed data, was "testplans-0.3.6.tar", last modified: Tue May 28 14:36:10 2024, max compression
```

## Comparing `testplans-0.3.4.tar` & `testplans-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:38:09.292695 testplans-0.3.4/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 testplans-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-05-23 14:38:09.291704 testplans-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-05-23 14:37:35.000000 testplans-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 14:38:09.293689 testplans-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:38:09.281917 testplans-0.3.4/testplans/
--rw-rw-rw-   0        0        0     1657 2024-05-22 15:02:55.000000 testplans-0.3.4/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.3.4/testplans/_results.py
--rw-rw-rw-   0        0        0     4000 2024-05-22 13:30:32.000000 testplans-0.3.4/testplans/api.py
--rw-rw-rw-   0        0        0     4095 2024-05-23 12:54:47.000000 testplans-0.3.4/testplans/devices.py
--rw-rw-rw-   0        0        0     6708 2024-05-23 13:06:40.000000 testplans-0.3.4/testplans/gui.py
--rw-rw-rw-   0        0        0    12334 2024-05-22 14:48:19.000000 testplans-0.3.4/testplans/main.py
--rw-rw-rw-   0        0        0     1786 2024-05-13 13:45:51.000000 testplans-0.3.4/testplans/models.py
--rw-rw-rw-   0        0        0    13917 2024-05-23 13:06:40.000000 testplans-0.3.4/testplans/tc.py
--rw-rw-rw-   0        0        0     9972 2024-05-22 14:48:19.000000 testplans-0.3.4/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:38:09.291704 testplans-0.3.4/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-05-23 14:38:09.000000 testplans-0.3.4/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-23 14:38:09.000000 testplans-0.3.4/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:38:09.000000 testplans-0.3.4/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 14:38:09.000000 testplans-0.3.4/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 14:36:10.728228 testplans-0.3.6/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 testplans-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0     5508 2024-05-28 14:36:10.728228 testplans-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4598 2024-05-28 14:35:04.000000 testplans-0.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:36:10.730357 testplans-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:36:10.721691 testplans-0.3.6/testplans/
+-rw-rw-rw-   0        0        0     1657 2024-05-22 15:02:55.000000 testplans-0.3.6/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.3.6/testplans/_results.py
+-rw-rw-rw-   0        0        0     4000 2024-05-22 13:30:32.000000 testplans-0.3.6/testplans/api.py
+-rw-rw-rw-   0        0        0     4095 2024-05-23 12:54:47.000000 testplans-0.3.6/testplans/devices.py
+-rw-rw-rw-   0        0        0     6724 2024-05-28 07:24:52.000000 testplans-0.3.6/testplans/gui.py
+-rw-rw-rw-   0        0        0    12402 2024-05-28 07:53:21.000000 testplans-0.3.6/testplans/main.py
+-rw-rw-rw-   0        0        0     1786 2024-05-13 13:45:51.000000 testplans-0.3.6/testplans/models.py
+-rw-rw-rw-   0        0        0    14797 2024-05-28 12:56:32.000000 testplans-0.3.6/testplans/tc.py
+-rw-rw-rw-   0        0        0     9996 2024-05-28 07:24:52.000000 testplans-0.3.6/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:36:10.727181 testplans-0.3.6/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5508 2024-05-28 14:36:10.000000 testplans-0.3.6/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-28 14:36:10.000000 testplans-0.3.6/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:36:10.000000 testplans-0.3.6/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 14:36:10.000000 testplans-0.3.6/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.3.4/LICENSE` & `testplans-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.3.4/PKG-INFO` & `testplans-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.3.4
+Version: 0.3.6
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.3.4)
+# testplans (v0.3.6)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
 
@@ -74,15 +74,15 @@
 1. [THREADS]:  
 	- safe work in independent TCs  
 	- safe stop process at any moment by terminate  
 2. [SKIP]:  
 	- tc  
 	- tc on dut  
 	- dut  
-3. [DEVICES]:  
+3. [DEVICES__BREEDER_INST]:  
 	- keep all in one instance  
 	- use variants: single device for all duts or list for pairing each dut  
 
 
 ********************************************************************************
 ## License
 See the [LICENSE](LICENSE) file for license rights and limitations (MIT).
```

### Comparing `testplans-0.3.4/README.md` & `testplans-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.3.4)
+# testplans (v0.3.6)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
 
@@ -52,15 +52,15 @@
 1. [THREADS]:  
 	- safe work in independent TCs  
 	- safe stop process at any moment by terminate  
 2. [SKIP]:  
 	- tc  
 	- tc on dut  
 	- dut  
-3. [DEVICES]:  
+3. [DEVICES__BREEDER_INST]:  
 	- keep all in one instance  
 	- use variants: single device for all duts or list for pairing each dut  
 
 
 ********************************************************************************
 ## License
 See the [LICENSE](LICENSE) file for license rights and limitations (MIT).
```

### Comparing `testplans-0.3.4/setup.py` & `testplans-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.4/testplans/__init__.py` & `testplans-0.3.6/testplans/__init__.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.4/testplans/_results.py` & `testplans-0.3.6/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.4/testplans/api.py` & `testplans-0.3.6/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.4/testplans/devices.py` & `testplans-0.3.6/testplans/devices.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.4/testplans/gui.py` & `testplans-0.3.6/testplans/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         if index == self.TM.HEADERS.STARTUP:
             pass
 
         if index == self.TM.HEADERS.TEARDOWN:
             pass
 
         if index in self.TM.HEADERS.DUTS:
-            dut = self.DATA.DEVICES__CLS.LIST__DUT[self.TM.HEADERS.DUTS.get_listed_index__by_outer(index)]
+            dut = self.DATA.DEVICES__BREEDER_CLS.LIST__DUT[self.TM.HEADERS.DUTS.get_listed_index__by_outer(index)]
             dut._bebug__SKIP_reverse()
             self.TM._data_reread()
 
     def TV_selectionChanged(self, first: QItemSelection, last: QItemSelection) -> None:
         # print("selectionChanged")
         # print(f"{first=}")  # first=<PyQt5.QtCore.QItemSelection object at 0x000001C79A107460>
         # ObjectInfo(first.indexes()[0]).print(_log_iter=True, skip_fullnames=["takeFirst", "takeLast"])
@@ -159,15 +159,15 @@
 
         tc = list(self.DATA.TCS__CLS)[row]
 
         if col == self.TM.HEADERS.STARTUP:
             self.PTE.setPlainText(str(tc.result__cls_startup))
 
         if col in self.TM.HEADERS.DUTS:
-            dut = self.DATA.DEVICES__CLS.LIST__DUT[col - self.TM.HEADERS.DUTS.START_OUTER]
+            dut = self.DATA.DEVICES__BREEDER_CLS.LIST__DUT[col - self.TM.HEADERS.DUTS.START_OUTER]
             self.PTE.setPlainText(tc.TCS__LIST[dut.INDEX].get__info_pretty())
 
         if col == self.TM.HEADERS.TEARDOWN:
             self.PTE.setPlainText(str(tc.result__cls_teardown))
 
 
 # =====================================================================================================================
```

### Comparing `testplans-0.3.4/testplans/main.py` & `testplans-0.3.6/testplans/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,28 +65,28 @@
     GUI__START: bool = True
     GUI__CLS: Type[TpGuiBase] = TpGuiBase
 
     api_client: Client_RequestsStack = Client_RequestsStack()   # todo: USE CLS!!! + add start
 
     # DIRPATH_TPS: Union[str, Path] = "TESTPLANS"
     DIRPATH_TCS: Union[str, Path] = "TESTCASES"
-    # DIRPATH_DEVS: Union[str, Path] = "DEVICES"
+    # DIRPATH_DEVS: Union[str, Path] = "DEVICES__BREEDER_INST"
     SETTINGS_BASE_NAME: Union[str, Path] = "SETTINGS_BASE.json"
     SETTINGS_BASE_FILEPATH: Path
 
-    DEVICES__CLS: Type[DevicesBreeder_WithDut] = DevicesBreeder_Example
+    DEVICES__BREEDER_CLS: Type[DevicesBreeder_WithDut] = DevicesBreeder_Example
 
     # AUX -----------------------------------------------------------
     TCS__CLS: Dict[Union[str, Type[TestCaseBase]], Optional[bool]] = {}     # todo: RENAME TO clss!!!
     # {
     #     Tc1: True,
     #     Tc2: True
     # }
 
-    # DEVICES: List[Union[str, Type[DeviceBase]]]    # settings
+    # DEVICES__BREEDER_INST: List[Union[str, Type[DeviceBase]]]    # settings
     # [
     #     Dev1,
     #     Dev2
     # ]
 
     tc_active: Optional[Type[TestCaseBase]] = None      # TODO:FIXME: use as PROPERTY!!!! not attribute!
     progress: int = 0   # todo: use as property? by getting from TCS???
@@ -99,15 +99,15 @@
         self.SETTINGS_BASE_FILEPATH = self.DIRPATH_TCS.joinpath(self.SETTINGS_BASE_NAME)
 
         if not self.DIRPATH_TCS.exists():
             msg = f"[ERROR] not found path {self.DIRPATH_TCS.name=}"
             print(msg)
             raise Exx__TcsPathNotExists(msg)
 
-        self.DEVICES__CLS.generate__objects()
+        self.DEVICES__BREEDER_CLS.generate__objects()
 
         self.tcs__reinit()
         self.slots_connect()
 
         if self.START__GUI_AND_API:
             self.start__gui_and_api()
 
@@ -130,15 +130,15 @@
             self.gui.run()
         elif self.API_SERVER__START:
             self.api_server.wait()  # it is ok!!!
 
     def slots_connect(self) -> None:
         self.signal__tp_start.connect(self.start)
         self.signal__tp_stop.connect(self.terminate)
-        self._signal__tp_reset_duts_sn.connect(self.DEVICES__CLS._debug__duts__reset_sn)
+        self._signal__tp_reset_duts_sn.connect(self.DEVICES__BREEDER_CLS._debug__duts__reset_sn)
 
         TestCaseBase.signals.signal__tc_state_changed.connect(self.post__tc_results)
 
     # =================================================================================================================
     def tcs__reinit(self) -> None:
         if not self.TCS__CLS:
             self._tcs__load_from_files()
@@ -194,15 +194,15 @@
                 print(f"{settings_tc_filepath=} NOT_EXISTS")
                 pass
 
         # print(f"{tc_cls.SETTINGS=}")
 
     def _tcs__apply_devices(self) -> None:
         for tc in self.TCS__CLS:
-            tc.devices__apply(self.DEVICES__CLS)
+            tc.devices__apply(self.DEVICES__BREEDER_CLS)
 
     # =================================================================================================================
     def tp__check_active(self) -> bool:
         result = self.tc_active is not None and self.progress not in [0, 100]
         return result
 
     # =================================================================================================================
@@ -221,15 +221,15 @@
             self.tc_active.terminate__cls()
         self.tc_active = None
 
         if progress is None:
             progress = 100
         self.progress = progress
 
-        self.DEVICES__CLS.disconnect__cls()
+        self.DEVICES__BREEDER_CLS.disconnect__cls()
 
         self.signal__tp_finished.emit()
 
     # =================================================================================================================
     def terminate(self) -> None:
         super().terminate()
```

### Comparing `testplans-0.3.4/testplans/models.py` & `testplans-0.3.6/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.4/testplans/tc.py` & `testplans-0.3.6/testplans/tc.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,80 +43,109 @@
     DESCRIPTION: str = ""
     SKIP: Optional[bool] = None     # access only over CLASS attribute! not instance!!!
     skip_tc_dut: Optional[bool] = None
     ASYNC: Optional[bool] = True
     # STOP_IF_FALSE_RESULT: Optional[bool] = None     # NOT USED NOW! MAYBE NOT IMPORTANT!!!
     SETTINGS_FILES: Union[None, pathlib.Path, List[pathlib.Path]] = None
 
+    DEVICES__BREEDER_CLS: Type['DevicesBreeder'] = None
+
     # AUXILIARY -----------------------------------
     signals: Signals = Signals()  # FIXME: need signal ON BASE CLASS! need only one SlotConnection! need Singleton?
-    TCS__LIST: List['_TestCaseBase'] = None
-
-    # INSTANCE ------------------------------------
-    DEVICES__CLS: Type['DevicesBreeder'] = None
-    DEVICES: 'DevicesBreeder' = None
-
-    SETTINGS: PrivateJson = None
-    INDEX: int = 0
+    TCS__LIST: List['_TestCaseBase'] = []
+    _INSTS_DICT_CLS: dict[Any, dict[Any, Any]]
 
     result__cls_startup: Optional[bool] = None
     result__cls_teardown: Optional[bool] = None
-    __result: Optional[bool]
-    __timestamp_last: float | None = None
-    timestamp_start: float | None = None
-    details: Dict[str, Any]
+
+    # INSTANCE ------------------------------------
+    _inst_inited: Optional[bool] = None
+
+    INDEX: int
+    SETTINGS: PrivateJson
+    DEVICES__BREEDER_INST: 'DevicesBreeder'
+
+    _result: Optional[bool] = None
+    _timestamp_last: Optional[float]
+    timestamp_start: Optional[float]
+    details: dict[str, Any]
     exx: Optional[Exception]
     progress: int
 
     # =================================================================================================================
-    # def __init__(self, dut: Any, _settings_files: Union[None, pathlib.Path, List[pathlib.Path]] = None):
-    def __init__(self, index: int = 0):
-        super().__init__()
-        self.INDEX = index
-
-        if self.DEVICES__CLS:
-            self.DEVICES = self.DEVICES__CLS(self.INDEX)
-
-        self.clear()
-
-        # if _settings_files is not None:
-        #     self.SETTINGS_FILES = _settings_files
-
-        self.SETTINGS = PrivateJson(_dict=self.settings_read())
-
     @classmethod
     def devices__apply(cls, devices_cls: Type['DevicesBreeder'] = None) -> None:
         if devices_cls is not None:
-            cls.DEVICES__CLS = devices_cls
-        if cls.DEVICES__CLS:
-            cls._objects__generate()
+            cls.DEVICES__BREEDER_CLS = devices_cls
+            cls.TCS__LIST = []
+
+        if cls.DEVICES__BREEDER_CLS:
+            cls.DEVICES__BREEDER_CLS.generate__objects()
+            cls._TCS__LIST__generate()
 
     @classmethod
-    def _objects__generate(cls) -> None:
+    def _TCS__LIST__generate(cls) -> None:
         """
         create tc objects for all DUTs, if not existed - create it in all DUTs
         """
-        cls.TCS__LIST = []
-        for index in range(cls.DEVICES__CLS.COUNT):
-            tc_on_dut = cls(index=index)
-            cls.TCS__LIST.append(tc_on_dut)
+        if cls.TCS__LIST:
+            return
+
+        for index in range(cls.DEVICES__BREEDER_CLS.COUNT):
+            tc_inst = cls(index=index)
+            cls.TCS__LIST.append(tc_inst)
 
         # FIXME: check if some TC on one base - it would be incorrect!!!???
 
     # =================================================================================================================
+    def __new__(cls, index: int, *args, **kwargs):
+        print(f"{cls.__name__}.__NEW__={index=}/{args=}/{kwargs=}")
+
+        if not hasattr(cls, "_INSTS_DICT_CLS"):
+            setattr(cls, "_INSTS_DICT_CLS", {})
+
+        if cls not in cls._INSTS_DICT_CLS:
+            cls._INSTS_DICT_CLS.update({cls: {}})
+
+        INSTS_DICT = cls._INSTS_DICT_CLS[cls]
+
+        try:
+            INST = INSTS_DICT[index]
+        except:
+            INST = super().__new__(cls)
+            INSTS_DICT[index] = INST
+
+        return INST
+
+    def __init__(self, index: int):
+        if self._inst_inited:
+            return
+
+        # NEW INSTANCE -----------------------------
+        self.INDEX = index
+        self.clear()
+        super().__init__()
+
+        if self.DEVICES__BREEDER_CLS:
+            self.DEVICES__BREEDER_INST = self.DEVICES__BREEDER_CLS(index)
+
+        self.SETTINGS = PrivateJson(_dict=self.settings_read())
+        self._inst_inited = True
+
+    # =================================================================================================================
     @property
     def timestamp_last(self) -> float | None:
         """
         None - not even started
         float - was started!
             stable - finished
             UnStable - in progress (active thread)
         """
-        if self.__timestamp_last:
-            return self.__timestamp_last
+        if self._timestamp_last:
+            return self._timestamp_last
 
         if self.isRunning():
             return time.time()
 
     # =================================================================================================================
     @classmethod
     def settings_read(cls, files: Union[None, pathlib.Path, List[pathlib.Path]] = None) -> dict:
@@ -131,19 +160,17 @@
                 for file in _settings_files:
                     if file.exists():
                         file_data = json.loads(file.read_text())
                         result.update(file_data)
         return result
 
     def clear(self) -> None:
-        self.LOGGER.debug("clear")
-
-        self.__timestamp_last = None
-        self.timestamp_start = None
         self.result = None
+        self._timestamp_last = None
+        self.timestamp_start = None
         self.details = {}
         self.exx = None
         self.progress = 0
 
     @classmethod
     def clear__cls(cls):
         cls.result__cls_startup = None
@@ -156,19 +183,19 @@
     # def NAME(cls):
     #     return cls.__name__
     #     # return pathlib.Path(__file__).name    # work as last destination where property starts!
 
     # RESULT ----------------------------------------------------------------------------------------------------------
     @property
     def result(self) -> TYPE__RESULT:
-        return self.__result
+        return self._result
 
     @result.setter
     def result(self, value: TYPE__RESULT) -> None:
-        self.__result = value
+        self._result = value
         self.signals.signal__tc_state_changed.emit(self)
 
     # # ---------------------------------------------------------
     # @classmethod
     # @property
     # def result__cls_startup(cls) -> Optional[bool]:
     #     return cls.__result__cls_startup
@@ -209,15 +236,15 @@
     # =================================================================================================================
     def run(self) -> None:
         self.LOGGER.debug("run")
 
         # PREPARE --------
         self.clear()
         self.timestamp_start = time.time()
-        if not self.DEVICES.DUT or not self.DEVICES.DUT.connect() or self.DEVICES.DUT.SKIP:
+        if not self.DEVICES__BREEDER_INST.DUT or not self.DEVICES__BREEDER_INST.DUT.connect() or self.DEVICES__BREEDER_INST.DUT.SKIP:
             return
 
         # WORK --------
         self.LOGGER.debug("run-startup")
         if self.startup():
             try:
                 self.LOGGER.debug("run-run_wrapped START")
@@ -229,15 +256,15 @@
         self.teardown()
 
     @classmethod
     def run__cls(cls) -> None:
         """run TC on batch duts(??? may be INDEXES???)
         prefered using in thread on upper level!
         """
-        # if not cls.DEVICES__CLS.LIST__DUT:
+        # if not cls.DEVICES__BREEDER_CLS.LIST__DUT:
         #     return
 
         print(f"run__cls=START={cls.NAME=}={'='*50}")
         if cls.SKIP:
             print(f"run__cls=SKIP={cls.NAME=}={'='*50}")
             return
 
@@ -280,15 +307,15 @@
     def startup(self) -> TYPE__RESULT:
         self.LOGGER.debug("")
         self.progress = 1
         return self.startup__wrapped()
 
     def teardown(self) -> TYPE__RESULT:
         self.LOGGER.debug("")
-        self.__timestamp_last = time.time()
+        self._timestamp_last = time.time()
         self.progress = 99
         result = self.teardown__wrapped()
         self.progress = 100
         return result
 
     @classmethod
     def teardown__cls(cls) -> TYPE__RESULT:
@@ -333,15 +360,15 @@
     """
     # =================================================================================================================
     def get__info_pretty(self) -> str:
         # fixme: ref from info_get
         result = ""
 
         result += f"DUT_INDEX={self.INDEX}\n"
-        result += f"DUT_SN={self.DEVICES.DUT.SN}\n"
+        result += f"DUT_SN={self.DEVICES__BREEDER_INST.DUT.SN}\n"
         result += f"TC_NAME={self.NAME}\n"
         result += f"TC_DESCRIPTION={self.DESCRIPTION}\n"
         result += f"TC_SKIP={self.SKIP}\n"
         result += f"tc_skip_dut={self.skip_tc_dut}\n"
         result += f"TC_ASYNC={self.ASYNC}\n"
         result += f"tc_result={self.result}\n"
         result += f"tc_progress={self.progress}\n"
@@ -376,15 +403,15 @@
 
     # =================================================================================================================
     def get__results(self) -> ModelTcResultFull:
         self.LOGGER.debug("")
 
         result = {
             **self.get__info().dict(),
-            **self.DEVICES.DUT.get__info().dict(),
+            **self.DEVICES__BREEDER_INST.DUT.get__info().dict(),
 
             # RESULTS
             "tc_timestamp": self.timestamp_last,
             "tc_active": self.isRunning(),
             "tc_progress": self.progress,
             "tc_result": bool(self.result),
             "tc_details": self.details,
```

### Comparing `testplans-0.3.4/testplans/tm.py` & `testplans-0.3.6/testplans/tm.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         class Headers(BreederStrStack):
             TESTCASE: int = 0
             ASYNC: None = None
             STARTUP: None = None
-            DUTS: BreederStrSeries = BreederStrSeries(None, self.DATA.DEVICES__CLS.COUNT)
+            DUTS: BreederStrSeries = BreederStrSeries(None, self.DATA.DEVICES__BREEDER_CLS.COUNT)
             TEARDOWN: None = None
             # FIXME: need resolve COUNT over DevicesIndexed!!!
 
         self.HEADERS = Headers()
 
     def rowCount(self, parent: QModelIndex = None, *args, **kwargs) -> int:
         return len(self.DATA.TCS__CLS)
@@ -68,15 +68,15 @@
         col = index.column()
         row = index.row()
         tc = list(self.DATA.TCS__CLS)[row]
 
         dut = None
         tc_inst = None
         if col in self.HEADERS.DUTS:
-            dut = self.DATA.DEVICES__CLS.LIST__DUT[col - self.HEADERS.DUTS.START_OUTER]
+            dut = self.DATA.DEVICES__BREEDER_CLS.LIST__DUT[col - self.HEADERS.DUTS.START_OUTER]
             tc_inst = tc.TCS__LIST[dut.INDEX]
 
         # -------------------------------------------------------------------------------------------------------------
         if role == Qt.DisplayRole:
             if col == self.HEADERS.TESTCASE:
                 return f'{tc.NAME}\n{tc.DESCRIPTION}'
             if col == self.HEADERS.ASYNC:
@@ -214,15 +214,15 @@
         row = index.row()
         col = index.column()
         tc = list(self.DATA.TCS__CLS)[row]
 
         dut = None
         tc_inst = None
         if col in self.HEADERS.DUTS:
-            dut = self.DATA.DEVICES__CLS.LIST__DUT[col - self.HEADERS.DUTS.START_OUTER]
+            dut = self.DATA.DEVICES__BREEDER_CLS.LIST__DUT[col - self.HEADERS.DUTS.START_OUTER]
             tc_inst = tc.TCS__LIST[dut.INDEX]
 
         # -------------------------------------------------------------------------------------------------------------
         if role == Qt.CheckStateRole:
             if col == self.HEADERS.TESTCASE:
                 tc.SKIP = value == Qt.Unchecked
```

### Comparing `testplans-0.3.4/testplans.egg-info/PKG-INFO` & `testplans-0.3.6/testplans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.3.4
+Version: 0.3.6
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.3.4)
+# testplans (v0.3.6)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
 
@@ -74,15 +74,15 @@
 1. [THREADS]:  
 	- safe work in independent TCs  
 	- safe stop process at any moment by terminate  
 2. [SKIP]:  
 	- tc  
 	- tc on dut  
 	- dut  
-3. [DEVICES]:  
+3. [DEVICES__BREEDER_INST]:  
 	- keep all in one instance  
 	- use variants: single device for all duts or list for pairing each dut  
 
 
 ********************************************************************************
 ## License
 See the [LICENSE](LICENSE) file for license rights and limitations (MIT).
```

