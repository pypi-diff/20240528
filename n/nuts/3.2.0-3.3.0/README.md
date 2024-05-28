# Comparing `tmp/nuts-3.2.0.tar.gz` & `tmp/nuts-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuts-3.2.0.tar", max compression
+gzip compressed data, was "nuts-3.3.0.tar", max compression
```

## Comparing `nuts-3.2.0.tar` & `nuts-3.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1108 2023-08-11 15:40:22.153344 nuts-3.2.0/LICENSE
--rw-r--r--   0        0        0     9476 2023-08-11 15:40:22.153344 nuts-3.2.0/README.md
--rw-r--r--   0        0        0        0 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/__init__.py
--rw-r--r--   0        0        0        0 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/base_tests/__init__.py
--rw-r--r--   0        0        0     2929 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/base_tests/napalm_bgp_neighbors.py
--rw-r--r--   0        0        0     1337 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/base_tests/napalm_get_arp.py
--rw-r--r--   0        0        0     1218 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/base_tests/napalm_get_config.py
--rw-r--r--   0        0        0     1691 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/base_tests/napalm_get_users.py
--rw-r--r--   0        0        0     1912 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/base_tests/napalm_get_vlans.py
--rw-r--r--   0        0        0     1900 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/base_tests/napalm_interfaces.py
--rw-r--r--   0        0        0     2638 2023-08-11 15:40:22.157344 nuts-3.2.0/nuts/base_tests/napalm_lldp_neighbors.py
--rw-r--r--   0        0        0     2236 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/base_tests/napalm_network_instances.py
--rw-r--r--   0        0        0     4460 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/base_tests/napalm_ping.py
--rw-r--r--   0        0        0     2143 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/base_tests/netmiko_cdp_neighbors.py
--rw-r--r--   0        0        0     4261 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/base_tests/netmiko_iperf.py
--rw-r--r--   0        0        0     2240 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/base_tests/netmiko_ospf_neighbors.py
--rw-r--r--   0        0        0     7285 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/context.py
--rw-r--r--   0        0        0        0 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/helpers/__init__.py
--rw-r--r--   0        0        0      337 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/helpers/context.py
--rw-r--r--   0        0        0      805 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/helpers/converters.py
--rw-r--r--   0        0        0      479 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/helpers/errors.py
--rw-r--r--   0        0        0     1680 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/helpers/filters.py
--rw-r--r--   0        0        0     8959 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/helpers/result.py
--rw-r--r--   0        0        0     1881 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/index.py
--rw-r--r--   0        0        0     3155 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/plugin.py
--rw-r--r--   0        0        0     8543 2023-08-11 15:40:22.161344 nuts-3.2.0/nuts/yamlloader.py
--rw-r--r--   0        0        0     4136 2023-08-11 15:40:22.161344 nuts-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    10514 1970-01-01 00:00:00.000000 nuts-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-05-28 08:25:28.277246 nuts-3.3.0/LICENSE
+-rw-r--r--   0        0        0     9742 2024-05-28 08:25:28.277246 nuts-3.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/__init__.py
+-rw-r--r--   0        0        0     3369 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_bgp_neighbors.py
+-rw-r--r--   0        0        0     1338 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_get_arp.py
+-rw-r--r--   0        0        0     1219 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_get_config.py
+-rw-r--r--   0        0        0     1692 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_get_users.py
+-rw-r--r--   0        0        0     1913 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_get_vlans.py
+-rw-r--r--   0        0        0     1901 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_interfaces.py
+-rw-r--r--   0        0        0     2641 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_lldp_neighbors.py
+-rw-r--r--   0        0        0     2237 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_network_instances.py
+-rw-r--r--   0        0        0     4461 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/napalm_ping.py
+-rw-r--r--   0        0        0     2144 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/netmiko_cdp_neighbors.py
+-rw-r--r--   0        0        0     4261 2024-05-28 08:25:28.281246 nuts-3.3.0/nuts/base_tests/netmiko_iperf.py
+-rw-r--r--   0        0        0     2241 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/base_tests/netmiko_ospf_neighbors.py
+-rw-r--r--   0        0        0     7357 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/context.py
+-rw-r--r--   0        0        0        0 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/helpers/__init__.py
+-rw-r--r--   0        0        0      338 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/helpers/context.py
+-rw-r--r--   0        0        0      805 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/helpers/converters.py
+-rw-r--r--   0        0        0      479 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/helpers/errors.py
+-rw-r--r--   0        0        0     1681 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/helpers/filters.py
+-rw-r--r--   0        0        0     8979 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/helpers/result.py
+-rw-r--r--   0        0        0      275 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/hooks.py
+-rw-r--r--   0        0        0     1957 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/index.py
+-rw-r--r--   0        0        0     3498 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/plugin.py
+-rw-r--r--   0        0        0     8638 2024-05-28 08:25:28.285246 nuts-3.3.0/nuts/yamlloader.py
+-rw-r--r--   0        0        0     4151 2024-05-28 08:25:28.285246 nuts-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10823 1970-01-01 00:00:00.000000 nuts-3.3.0/PKG-INFO
```

### Comparing `nuts-3.2.0/LICENSE` & `nuts-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nuts-3.2.0/README.md` & `nuts-3.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 Each test bundle contains the following structure:
 ```yaml
 ---
 - test_module: <module that contains the test class> # optional
   test_class: <name of the test class>
   label: <label to uniquely identify the test> # optional 
   test_execution: <additional data used to execute the test> # optional
+  test_extras: <additional data can be provided to the context for custom usage> # optional
   test_data: <data used to generate the test cases>
 ...
 ```
 `test_module`: The full path of the Python module that contains the test class to be used.
 This value is optional if the test class is registered in `index.py` of the pytest-nuts plugin.
 Note that it can be relevant in which directory `pytest` is started if local test modules are used. Using `test_modules` allows you to write your own test classes. **Note: We currently do not support self-written test modules, since upcoming refactorings might introduce breaking changes.**
 
@@ -65,14 +66,17 @@
 
 `test_execution`: Data that is exposed as part of the `nuts_parameters` property. 
 By convention, this contains additional information that is passed directly to the nornir task in the background. 
 Therefore the key-value pairs must be consistent with the key-value pairs of the specific nornir task. 
 As an example, the test definition `napalm_ping.py` calls a nornir task to execute napalm's ping-command. 
 This allows the additional `max_drop` parameter in `test_execution`, since it is in turn pre-defined by napalm.
 
+`test_extras`: Additional data that can be accessed through the `nuts_parameters` property.
+These data are not internally utilized and can be passed for use in custom code.
+
 `test_data`: Data that is used to parametrize the tests in the test class which have the `pytest.mark.nuts` annotation. It is additionally part of the `nuts_parameters` property.
 
 ### Example: CDP Neighbors
 Example of a test bundle for `TestNetmikoCdpNeighbors` which tests that `R1` is a CDP Neighbor of both `R2` and `R3`.
 This example creates three different tests, one for each entry in the `test_data` list.
 
 ```yaml
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_bgp_neighbors.py` & `nuts-3.3.0/nuts/base_tests/napalm_bgp_neighbors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 """Query BGP neighbors of a device or count them."""
-from typing import Dict, Callable, List, Any
+
+from typing import Dict, Callable, List, Any, Tuple
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_napalm.plugins.tasks import napalm_get
 
 from nuts.context import NornirNutsContext
 from nuts.helpers.result import AbstractHostResultExtractor, NutsResult
 
 
 class BgpNeighborsExtractor(AbstractHostResultExtractor):
     def single_transform(
         self, single_result: MultiResult
-    ) -> Dict[str, Dict[str, NutsResult]]:
+    ) -> Dict[Tuple[str, str], Dict[str, NutsResult]]:
+        test_exectuion = self._nuts_ctx.nuts_parameters.get("test_execution")
+        if test_exectuion:
+            vrf = test_exectuion.get("vrf", "global")
+            if not vrf:
+                vrf = "global"
+        else:
+            vrf = "global"
+
         neighbors = self._simple_extract(single_result)["bgp_neighbors"]
-        if "global" not in neighbors:
+        if vrf not in neighbors:
             return {}
-        global_scope = neighbors["global"]
-        router_id = global_scope["router_id"]
+        scope = neighbors[vrf]
+        router_id = scope["router_id"]
         return {
             peer: self._add_local_id(details, router_id)
-            for peer, details in global_scope["peers"].items()
+            for peer, details in scope["peers"].items()
         }
 
     def _add_local_id(self, element: Dict[str, Any], router_id: str) -> Dict[str, Any]:
         element["local_id"] = router_id
         return element
 
 
 class BgpNeighborsContext(NornirNutsContext):
     def nuts_task(self) -> Callable[..., Result]:
         return napalm_get
 
     def nuts_arguments(self) -> Dict[str, List[str]]:
+        # Overrides nuts_arguments.nuts_arguments
+        # "test_execution" is not passed to the nuts_task
         return {"getters": ["bgp_neighbors"]}
 
     def nuts_extractor(self) -> BgpNeighborsExtractor:
         return BgpNeighborsExtractor(self)
 
 
 CONTEXT = BgpNeighborsContext
@@ -44,15 +55,17 @@
 
 class TestNapalmBgpNeighborsCount:
     @pytest.mark.nuts("neighbor_count")
     def test_neighbor_count(
         self, single_result: NutsResult, neighbor_count: int
     ) -> None:
         assert single_result.result is not None
-        assert len(single_result.result) == neighbor_count
+        assert (
+            len(single_result.result) == neighbor_count
+        ), f"Expected {neighbor_count}; got {len(single_result.result)}"
 
 
 class TestNapalmBgpNeighbors:
     @pytest.fixture
     def peer_result(self, single_result: NutsResult, peer: str) -> Dict[str, Any]:
         assert single_result.result is not None
         return single_result.result[peer]
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_get_arp.py` & `nuts-3.3.0/nuts/base_tests/napalm_get_arp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query arp table of a device."""
+
 from typing import Dict, Callable, List, Any, Text
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_napalm.plugins.tasks import napalm_get
 
 from nuts.context import NornirNutsContext
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_get_config.py` & `nuts-3.3.0/nuts/base_tests/napalm_get_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query config of a device."""
+
 from typing import Dict, Callable, List, Any
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_napalm.plugins.tasks import napalm_get
 
 from nuts.context import NornirNutsContext
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_get_users.py` & `nuts-3.3.0/nuts/base_tests/napalm_get_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query users of a device."""
+
 from typing import Dict, Callable, List, Any
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_napalm.plugins.tasks import napalm_get
 
 from nuts.context import NornirNutsContext
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_get_vlans.py` & `nuts-3.3.0/nuts/base_tests/napalm_get_vlans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query vlans of a device."""
+
 from typing import Dict, Callable, List, Any
 
 import pytest
 from nornir.core.filter import F
 from nornir.core.task import MultiResult, Result
 from nornir_napalm.plugins.tasks import napalm_get
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_interfaces.py` & `nuts-3.3.0/nuts/base_tests/napalm_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query interfaces and their information of a device."""
+
 from typing import Dict, Callable, List, Any
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_napalm.plugins.tasks import napalm_get
 
 from nuts.context import NornirNutsContext
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_lldp_neighbors.py` & `nuts-3.3.0/nuts/base_tests/napalm_lldp_neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query LLDP neighbors of a device."""
+
 from typing import Dict, Callable, List, Any
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_napalm.plugins.tasks import napalm_get
 
 from nuts.context import NornirNutsContext
@@ -24,17 +25,17 @@
         return element
 
     def _add_remote_host(self, element: Dict[str, Any]) -> Dict[str, Any]:
         element["remote_host"] = element["remote_system_name"]
         return element
 
     def _add_expanded_remote_port(self, element: Dict[str, Any]) -> Dict[str, Any]:
-        element[
-            "remote_port_expanded"
-        ] = InterfaceNameConverter().expand_interface_name(element["remote_port"])
+        element["remote_port_expanded"] = (
+            InterfaceNameConverter().expand_interface_name(element["remote_port"])
+        )
         return element
 
 
 class LldpNeighborsContext(NornirNutsContext):
     def nuts_task(self) -> Callable[..., Result]:
         return napalm_get
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_network_instances.py` & `nuts-3.3.0/nuts/base_tests/napalm_network_instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query network instances of a device."""
+
 from typing import Dict, List, Callable, Any
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_napalm.plugins.tasks import napalm_get
 
 from nuts.helpers.result import AbstractHostResultExtractor, NutsResult
```

### Comparing `nuts-3.2.0/nuts/base_tests/napalm_ping.py` & `nuts-3.3.0/nuts/base_tests/napalm_ping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Let a device ping another device."""
+
 from enum import Enum
 from typing import Dict, Callable, Any, List
 
 import pytest
 from nornir.core import Task
 from nornir.core.task import Result
 from nornir_napalm.plugins.tasks import napalm_ping
```

### Comparing `nuts-3.2.0/nuts/base_tests/netmiko_cdp_neighbors.py` & `nuts-3.3.0/nuts/base_tests/netmiko_cdp_neighbors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query CDP neighbors of a device."""
+
 from typing import Callable, Dict, Any
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_netmiko import netmiko_send_command
 
 from nuts.helpers.result import AbstractHostResultExtractor, NutsResult
```

### Comparing `nuts-3.2.0/nuts/base_tests/netmiko_iperf.py` & `nuts-3.3.0/nuts/base_tests/netmiko_iperf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query bandwidth performance between two devices."""
+
 import pytest
 import json
 from typing import Dict, Callable, Any
 import shlex
 
 from nornir.core.task import Task, Result
 from nornir.core.filter import F
@@ -102,15 +103,14 @@
         return IperfExtractor(self)
 
 
 CONTEXT = IperfContext
 
 
 class IperfResultError(Error):
-
     """Error in iperf result JSON."""
 
 
 class TestNetmikoIperf:
     @pytest.mark.nuts("min_expected")
     def test_iperf(self, single_result: NutsResult, min_expected: int) -> None:
         assert single_result.result >= min_expected
```

### Comparing `nuts-3.2.0/nuts/base_tests/netmiko_ospf_neighbors.py` & `nuts-3.3.0/nuts/base_tests/netmiko_ospf_neighbors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query OSPF neighbors of a device or count them."""
+
 from typing import Callable, Dict, Any
 
 import pytest
 from nornir.core.task import MultiResult, Result
 from nornir_netmiko import netmiko_send_command
 
 from nuts.context import NornirNutsContext
```

### Comparing `nuts-3.2.0/nuts/context.py` & `nuts-3.3.0/nuts/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provide necessary information that is needed for a specific test."""
+
 import pathlib
 from typing import Any, Callable, Optional, Dict, List
 from pytest import Config
 
 from nornir import InitNornir
 from nornir.core import Nornir
 from nornir.core.task import AggregatedResult, Result
@@ -198,14 +199,15 @@
                 raise NutsSetupError("No Hosts found, is the nornir inventory empty?")
 
         overall_results = selected_hosts.run(
             task=self.nuts_task(), **self.nuts_arguments()
         )
 
         self.teardown()
+        selected_hosts.close_connections(on_good=True, on_failed=True)
         return overall_results
 
     def setup(self) -> None:
         """
         Defines code which is executed before the nornir task.
         """
         pass
```

### Comparing `nuts-3.2.0/nuts/helpers/converters.py` & `nuts-3.3.0/nuts/helpers/converters.py`

 * *Files identical despite different names*

### Comparing `nuts-3.2.0/nuts/helpers/filters.py` & `nuts-3.3.0/nuts/helpers/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Functions to filter the nornir inventory and used in conjunction with
 a context's nornir_filter function.
 """
+
 from typing import Optional, Dict, Any, List, Union
 from nornir.core.filter import F, OR
 
 from nuts.helpers.errors import NutsSetupError
 
 
 def filter_hosts(test_data: Optional[List[Dict[str, Any]]]) -> F:
```

### Comparing `nuts-3.2.0/nuts/helpers/result.py` & `nuts-3.3.0/nuts/helpers/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             header = "".join(
                 traceback.format_exception_only(type(self.exception), self.exception)
             )
             raise NutsNornirError(
                 f"An exception has occurred while executing nornir:\n"
                 f"{header}\n"
                 f"{self._result}"
-            )
+            ) from self.exception
         if self.failed:
             raise NutsNornirError(f"Nornir execution has failed:\n" f"{self._result}")
 
         self._validated = True
 
     @property
     def result(self) -> Any:
```

### Comparing `nuts-3.2.0/nuts/index.py` & `nuts-3.3.0/nuts/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Allows to indicate only the test class name in a test bundle."""
+
 from typing import Optional
 
 default_index = {
     "TestNapalmBgpNeighbors": "nuts.base_tests.napalm_bgp_neighbors",
     "TestNapalmBgpNeighborsCount": "nuts.base_tests.napalm_bgp_neighbors",
     "TestNapalmInterfaces": "nuts.base_tests.napalm_interfaces",
     "TestNapalmLldpNeighbors": "nuts.base_tests.napalm_lldp_neighbors",
     "TestNapalmLldpNeighborsCount": "nuts.base_tests.napalm_lldp_neighbors",
     "TestNapalmNetworkInstances": "nuts.base_tests.napalm_network_instances",
     "TestNapalmPing": "nuts.base_tests.napalm_ping",
     "TestNapalmUsers": "nuts.base_tests.napalm_get_users",
+    "TestNapalmOnlyDefinedUsersExist": "nuts.base_tests.napalm_get_users",
     "TestNapalmConfig": "nuts.base_tests.napalm_get_config",
     "TestNapalmVlans": "nuts.base_tests.napalm_get_vlans",
     "TestNapalmOnlyDefinedVlansExist": "nuts.base_tests.napalm_get_vlans",
     "TestNapalmInterfaceInVlan": "nuts.base_tests.napalm_get_vlans",
     "TestNetmikoCdpNeighbors": "nuts.base_tests.netmiko_cdp_neighbors",
     "TestNetmikoCdpNeighborsCount": "nuts.base_tests.netmiko_cdp_neighbors",
     "TestNetmikoIperf": "nuts.base_tests.netmiko_iperf",
```

### Comparing `nuts-3.2.0/nuts/plugin.py` & `nuts-3.3.0/nuts/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Fixtures"""
+
 from typing import Optional, Dict, Any
 from pathlib import Path
 
 import pytest
 from pytest import Parser
 from pytest import Session
 from pytest import Collector
@@ -12,37 +13,51 @@
 
 from nuts.context import NutsContext
 from nuts.context import NornirNutsContext
 from nuts.helpers.result import NutsResult
 from nuts.yamlloader import NutsYamlFile, get_parametrize_data
 
 
+def pytest_addhooks(pluginmanager):
+    from nuts import hooks
+
+    pluginmanager.add_hookspecs(hooks)
+
+
 @pytest.fixture(scope="class")
 def nuts_ctx(request: FixtureRequest) -> NutsContext:
     params = request.node.params
     context_class = getattr(request.module, "CONTEXT", NutsContext)
     ctx: NutsContext = context_class(params, pytestconfig=request.config)
     ctx.initialize()
     return ctx
 
 
 @pytest.fixture
-def single_result(nuts_ctx: NutsContext, nuts_test_entry: Dict[str, Any]) -> NutsResult:
+def single_result(
+    nuts_ctx: NutsContext, nuts_test_entry: Dict[str, Any], request: FixtureRequest
+) -> NutsResult:
     """
     Returns the result which belongs to a specific host
     out of the overall set of results that has been returned by nornir's task.
     In addition, ensures that the result has no exception and has not failed.
 
     :param nuts_ctx: The context for a test
     :param nuts_test_entry: The entry from the test bundle (yaml-file) for which
         the corresponding result should be returned
     :return: The `NutsResult` that belongs to a host or host/destination pair
     """
     res = nuts_ctx.extractor.single_result(nuts_test_entry)
     res.validate()
+
+    # Invoke the pytest_nuts_single_result hook to extend result reports.
+    request.config.hook.pytest_nuts_single_result(
+        request=request, nuts_ctx=nuts_ctx, result=res
+    )
+
     return res
 
 
 def pytest_configure(config: Config) -> None:
     config.addinivalue_line("markers", "nuts: marks the test for nuts parametrization")
 
 
@@ -60,20 +75,20 @@
 
 
 # https://docs.pytest.org/en/latest/example/nonpython.html#yaml-plugin
 def pytest_collect_file(parent: Session, file_path: Path) -> Optional[Collector]:
     """
     Performs the collection phase for the given pytest session.
     Collects all test bundles if available, i.e. files starting
-    with 'test' and ending in .yaml.
+    with 'test' and ending in .yaml or .yml.
     :param parent: pytest session object
     :param file_path: path to test file(s)
     :return: The pytest collector if found
     """
-    if file_path.suffix == ".yaml" and file_path.name.startswith("test"):
+    if file_path.suffix in [".yaml", ".yml"] and file_path.name.startswith("test"):
         return NutsYamlFile.from_parent(parent, path=file_path)
     return None
 
 
 def pytest_addoption(parser: Parser) -> None:
     """Add pytest command line options to configure nuts"""
```

### Comparing `nuts-3.2.0/nuts/yamlloader.py` & `nuts-3.3.0/nuts/yamlloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Converts a test bundle (YAML file) into a test class for pytest.
 Based on https://docs.pytest.org/en/stable/example/nonpython.html#yaml-plugin
 """
+
 import importlib
 from nuts.helpers.context import load_context
 import types
 from importlib import util
 from typing import Iterable, Union, Any, Optional, List, Set, Dict, Tuple
 
 import yaml
@@ -102,20 +103,22 @@
 
         class_name = self.test_entry["test_class"]
         label = self.test_entry.get("label")
         name = class_name if label is None else f"{class_name} - {label}"
 
         test_data = self.test_entry.get("test_data", [])
         test_execution = self.test_entry.get("test_execution")
+        test_extras = self.test_entry.get("test_extras")
         yield NutsTestClass.from_parent(
             self,
             name=name,
             class_name=class_name,
             test_data=test_data,
             test_execution=test_execution,
+            test_extras=test_extras,
         )
 
 
 class NutsTestClass(pytest.Class):
     """
     Custom nuts test collector for test methods.
     Initialises a corresponding context with externally provided parameters.
```

### Comparing `nuts-3.2.0/pyproject.toml` & `nuts-3.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nuts"
-version = "3.2.0"
+version = "3.3.0"
 description = "Network Unit Testing System"
-authors = ["Lukas Murer, Méline Sieber, Urs Baumann, Matthias Gabriel, Florian Bruhin", "Marco Martinez", "Severin Grimm"]
-maintainers = ["Marco Martinez <marco.maritnez@ost.ch>", "Urs Baumann <github@m.ubaumann.ch>"]
+authors = [
+    "Lukas Murer, Méline Sieber, Urs Baumann, Matthias Gabriel, Florian Bruhin",
+    "Marco Martinez",
+    "Severin Grimm",
+]
+maintainers = [
+    "Marco Martinez <marco.maritnez@ost.ch>",
+    "Urs Baumann <github@m.ubaumann.ch>",
+]
 classifiers = ["Framework :: Pytest", "Topic :: System :: Networking"]
 homepage = "https://github.com/network-unit-testing-system/nuts"
 repository = "https://github.com/network-unit-testing-system/nuts"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-pytest = "^7.3.0"
+pytest = "^7"
 PyYAML = "^6.0"
 nornir = "^3.3.0"
-nornir-napalm = "^0.4.0"
+nornir-napalm = "^0.5.0"
 nornir-netmiko = "^1.0.0"
 nornir-utils = "^0.2.0"
 
 [tool.poetry.dev-dependencies]
 tox = "^4.4.11"
 pytest-cov = "^4.0.0"
-black = "^23.3.0"
-sphinx = "^7.1.2"
+black = "^24.2.0"
+sphinx = "^7"
 mypy = "^1.0.1"
-flake8 = "^6.0.0"
+flake8 = "^7.0.0"
 types-PyYAML = "*"
 types-setuptools = "*"
 types-toml = "*"
 
 [tool.poetry.plugins."pytest11"]
-"nuts"="nuts.plugin"
+"nuts" = "nuts.plugin"
 # why "pytest11": https://github.com/pytest-dev/pytest/commit/ed03eef81b220199a819632a27f9c452b8e1fb81
 # https://docs.pytest.org/en/latest/how-to/writing_plugins.html#making-your-plugin-installable-by-others
 
 [tool.black]
 line-length = 88
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 filterwarnings = [
     "error",
     "ignore:Using or importing the ABCs from 'collections':DeprecationWarning:napalm\\.base\\.helpers",
     "ignore:Using or importing the ABCs from 'collections':DeprecationWarning:jnpr\\.junos\\.factcache",
     "ignore:NutsYamlFile\\.fspath is deprecated and will be replaced by NutsYamlFile\\.path\\.",
 ]
-markers = [
-    "nuts_test_ctx: A NutsContext to be used in tests."
-]
+markers = ["nuts_test_ctx: A NutsContext to be used in tests."]
 
 [tool.mypy]
-python_version = 3.8
+python_version = "3.8"
 
 ### --strict
 warn_unused_configs = true
 disallow_any_generics = true
 disallow_subclassing_any = true
 # disallow_untyped_calls = true
 # disallow_untyped_defs = true
@@ -145,8 +150,7 @@
 deps =
     git+https://github.com/pytest-dev/pytest.git#main
     pytest-cov >= 4.0.0
 commands = pytest {posargs} --junitxml=test-reports/pytest.xml --cov="{envsitepackagesdir}/nuts" --cov=tests --cov-report xml:test-reports/coverage.xml
 # envsitepackagesdir see: https://tox.readthedocs.io/en/latest/example/pytest.html
 
 """
-
```

### Comparing `nuts-3.2.0/PKG-INFO` & `nuts-3.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: nuts
-Version: 3.2.0
+Version: 3.3.0
 Summary: Network Unit Testing System
 Home-page: https://github.com/network-unit-testing-system/nuts
 License: MIT
 Author: Lukas Murer, Méline Sieber, Urs Baumann, Matthias Gabriel, Florian Bruhin
 Maintainer: Marco Martinez
 Maintainer-email: marco.maritnez@ost.ch
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Networking
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: nornir (>=3.3.0,<4.0.0)
-Requires-Dist: nornir-napalm (>=0.4.0,<0.5.0)
+Requires-Dist: nornir-napalm (>=0.5.0,<0.6.0)
 Requires-Dist: nornir-netmiko (>=1.0.0,<2.0.0)
 Requires-Dist: nornir-utils (>=0.2.0,<0.3.0)
-Requires-Dist: pytest (>=7.3.0,<8.0.0)
+Requires-Dist: pytest (>=7,<8)
 Project-URL: Repository, https://github.com/network-unit-testing-system/nuts
 Description-Content-Type: text/markdown
 
 # Network Unit Testing System
 
 ## Introduction
 
@@ -72,14 +73,15 @@
 Each test bundle contains the following structure:
 ```yaml
 ---
 - test_module: <module that contains the test class> # optional
   test_class: <name of the test class>
   label: <label to uniquely identify the test> # optional 
   test_execution: <additional data used to execute the test> # optional
+  test_extras: <additional data can be provided to the context for custom usage> # optional
   test_data: <data used to generate the test cases>
 ...
 ```
 `test_module`: The full path of the Python module that contains the test class to be used.
 This value is optional if the test class is registered in `index.py` of the pytest-nuts plugin.
 Note that it can be relevant in which directory `pytest` is started if local test modules are used. Using `test_modules` allows you to write your own test classes. **Note: We currently do not support self-written test modules, since upcoming refactorings might introduce breaking changes.**
 
@@ -91,14 +93,17 @@
 
 `test_execution`: Data that is exposed as part of the `nuts_parameters` property. 
 By convention, this contains additional information that is passed directly to the nornir task in the background. 
 Therefore the key-value pairs must be consistent with the key-value pairs of the specific nornir task. 
 As an example, the test definition `napalm_ping.py` calls a nornir task to execute napalm's ping-command. 
 This allows the additional `max_drop` parameter in `test_execution`, since it is in turn pre-defined by napalm.
 
+`test_extras`: Additional data that can be accessed through the `nuts_parameters` property.
+These data are not internally utilized and can be passed for use in custom code.
+
 `test_data`: Data that is used to parametrize the tests in the test class which have the `pytest.mark.nuts` annotation. It is additionally part of the `nuts_parameters` property.
 
 ### Example: CDP Neighbors
 Example of a test bundle for `TestNetmikoCdpNeighbors` which tests that `R1` is a CDP Neighbor of both `R2` and `R3`.
 This example creates three different tests, one for each entry in the `test_data` list.
 
 ```yaml
```

