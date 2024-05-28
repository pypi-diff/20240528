# Comparing `tmp/ignos-api-client-2024.3.12.8830.tar.gz` & `tmp/ignos_api_client-2024.5.28.9351.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignos-api-client-2024.3.12.8830.tar", last modified: Tue Mar 12 09:55:15 2024, max compression
+gzip compressed data, was "ignos_api_client-2024.5.28.9351.tar", last modified: Tue May 28 10:47:44 2024, max compression
```

## Comparing `ignos-api-client-2024.3.12.8830.tar` & `ignos_api_client-2024.5.28.9351.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.875279 ignos-api-client-2024.3.12.8830/
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-03-12 09:55:15.875279 ignos-api-client-2024.3.12.8830/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.867279 ignos-api-client-2024.3.12.8830/ignos/
--rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.867279 ignos-api-client-2024.3.12.8830/ignos/api/
--rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.867279 ignos-api-client-2024.3.12.8830/ignos/api/client/
--rw-r--r--   0 vsts      (1001) docker     (127)      866 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17574 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2770 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/_patch.py
--rw-r--r--   0 vsts      (1001) docker     (127)    78873 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/_serialization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      495 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.867279 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/
--rw-r--r--   0 vsts      (1001) docker     (127)      813 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17927 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2813 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.871279 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/operations/
--rw-r--r--   0 vsts      (1001) docker     (127)     4381 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)  1212473 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/aio/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.871279 ignos-api-client-2024.3.12.8830/ignos/api/client/models/
--rw-r--r--   0 vsts      (1001) docker     (127)    37069 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10958 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/models/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)   995711 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/models/_models.py
--rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/models/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.875279 ignos-api-client-2024.3.12.8830/ignos/api/client/operations/
--rw-r--r--   0 vsts      (1001) docker     (127)     4381 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)  1473320 2024-03-12 09:55:10.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/operations/_patch.py
--rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/ignos/api/client/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-12 09:55:15.875279 ignos-api-client-2024.3.12.8830/ignos_api_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-03-12 09:55:15.000000 ignos-api-client-2024.3.12.8830/ignos_api_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-03-12 09:55:15.000000 ignos-api-client-2024.3.12.8830/ignos_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-12 09:55:15.000000 ignos-api-client-2024.3.12.8830/ignos_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-03-12 09:55:15.000000 ignos-api-client-2024.3.12.8830/ignos_api_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-03-12 09:55:15.000000 ignos-api-client-2024.3.12.8830/ignos_api_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-03-12 09:55:15.875279 ignos-api-client-2024.3.12.8830/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-03-12 09:55:09.000000 ignos-api-client-2024.3.12.8830/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.097537 ignos_api_client-2024.5.28.9351/
+-rw-r--r--   0 vsts      (1001) docker     (127)      235 2024-05-28 10:47:44.097537 ignos_api_client-2024.5.28.9351/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.089537 ignos_api_client-2024.5.28.9351/ignos/
+-rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.089537 ignos_api_client-2024.5.28.9351/ignos/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.089537 ignos_api_client-2024.5.28.9351/ignos/api/client/
+-rw-r--r--   0 vsts      (1001) docker     (127)      866 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18327 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2770 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    78873 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/_serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      495 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.089537 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/
+-rw-r--r--   0 vsts      (1001) docker     (127)      813 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18692 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2813 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.093537 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/operations/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4591 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  1319758 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/aio/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.093537 ignos_api_client-2024.5.28.9351/ignos/api/client/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)    39007 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11830 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/models/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  1045106 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/models/_models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/models/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.097537 ignos_api_client-2024.5.28.9351/ignos/api/client/operations/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4591 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  1595990 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      674 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/operations/_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/ignos/api/client/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 10:47:44.097537 ignos_api_client-2024.5.28.9351/ignos_api_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      235 2024-05-28 10:47:44.000000 ignos_api_client-2024.5.28.9351/ignos_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-05-28 10:47:44.000000 ignos_api_client-2024.5.28.9351/ignos_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-28 10:47:44.000000 ignos_api_client-2024.5.28.9351/ignos_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-05-28 10:47:44.000000 ignos_api_client-2024.5.28.9351/ignos_api_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-28 10:47:44.000000 ignos_api_client-2024.5.28.9351/ignos_api_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-28 10:47:44.097537 ignos_api_client-2024.5.28.9351/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      944 2024-05-28 10:47:34.000000 ignos_api_client-2024.5.28.9351/setup.py
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/__init__.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/_client.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from . import models as _models
 from ._configuration import IgnosPortalConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     AlertsOperations,
     AssetsOperations,
     AzureRegionsOperations,
+    BookingOperations,
     CdfOperations,
     CncFileTransferOperations,
     CncSetupAgentOperations,
     CncSetupOperations,
     CompaniesOperations,
     CountriesOperations,
     CustomerOrdersOperations,
@@ -31,14 +32,15 @@
     DocumentTypesOperations,
     DocumentsOperations,
     ElectricalOperations,
     ExternalAccessOperations,
     ExternalOperations,
     ExternalServicesOperations,
     LinksOperations,
+    LocationsOperations,
     MachineAlarmsOperations,
     MachineUtilizationOperations,
     MachinesOperations,
     MeOperations,
     MeasurementFormSchemasOperations,
     MeasurementFormsInstancesOperations,
     MeasuringToolsOperations,
@@ -54,14 +56,15 @@
     PowerOperations,
     PresentationOperations,
     ResourcesOperations,
     SuppliersOperations,
     SustainabilityOperations,
     SystemHealthDashboardOperations,
     TraceOperations,
+    TrackingOperations,
     UploadOperations,
     UsersOperations,
     WeldingOperations,
     WorkordersOperations,
     WorkspaceTemplatesAdminOperations,
     WorkspaceTemplatesOperations,
     WorkspacesOperations,
@@ -77,14 +80,16 @@
 
     :ivar alerts: AlertsOperations operations
     :vartype alerts: ignos.api.client.operations.AlertsOperations
     :ivar assets: AssetsOperations operations
     :vartype assets: ignos.api.client.operations.AssetsOperations
     :ivar azure_regions: AzureRegionsOperations operations
     :vartype azure_regions: ignos.api.client.operations.AzureRegionsOperations
+    :ivar booking: BookingOperations operations
+    :vartype booking: ignos.api.client.operations.BookingOperations
     :ivar cdf: CdfOperations operations
     :vartype cdf: ignos.api.client.operations.CdfOperations
     :ivar cnc_file_transfer: CncFileTransferOperations operations
     :vartype cnc_file_transfer: ignos.api.client.operations.CncFileTransferOperations
     :ivar cnc_setup: CncSetupOperations operations
     :vartype cnc_setup: ignos.api.client.operations.CncSetupOperations
     :ivar cnc_setup_agent: CncSetupAgentOperations operations
@@ -113,14 +118,16 @@
     :vartype external_services: ignos.api.client.operations.ExternalServicesOperations
     :ivar electrical: ElectricalOperations operations
     :vartype electrical: ignos.api.client.operations.ElectricalOperations
     :ivar welding: WeldingOperations operations
     :vartype welding: ignos.api.client.operations.WeldingOperations
     :ivar links: LinksOperations operations
     :vartype links: ignos.api.client.operations.LinksOperations
+    :ivar locations: LocationsOperations operations
+    :vartype locations: ignos.api.client.operations.LocationsOperations
     :ivar machine_alarms: MachineAlarmsOperations operations
     :vartype machine_alarms: ignos.api.client.operations.MachineAlarmsOperations
     :ivar machines: MachinesOperations operations
     :vartype machines: ignos.api.client.operations.MachinesOperations
     :ivar machine_utilization: MachineUtilizationOperations operations
     :vartype machine_utilization: ignos.api.client.operations.MachineUtilizationOperations
     :ivar me: MeOperations operations
@@ -158,14 +165,16 @@
     :vartype suppliers: ignos.api.client.operations.SuppliersOperations
     :ivar sustainability: SustainabilityOperations operations
     :vartype sustainability: ignos.api.client.operations.SustainabilityOperations
     :ivar system_health_dashboard: SystemHealthDashboardOperations operations
     :vartype system_health_dashboard: ignos.api.client.operations.SystemHealthDashboardOperations
     :ivar trace: TraceOperations operations
     :vartype trace: ignos.api.client.operations.TraceOperations
+    :ivar tracking: TrackingOperations operations
+    :vartype tracking: ignos.api.client.operations.TrackingOperations
     :ivar upload: UploadOperations operations
     :vartype upload: ignos.api.client.operations.UploadOperations
     :ivar users: UsersOperations operations
     :vartype users: ignos.api.client.operations.UsersOperations
     :ivar workspaces: WorkspacesOperations operations
     :vartype workspaces: ignos.api.client.operations.WorkspacesOperations
     :ivar workspace_templates_admin: WorkspaceTemplatesAdminOperations operations
@@ -203,14 +212,15 @@
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.alerts = AlertsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.assets = AssetsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.azure_regions = AzureRegionsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.booking = BookingOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cdf = CdfOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cnc_file_transfer = CncFileTransferOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.cnc_setup = CncSetupOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cnc_setup_agent = CncSetupAgentOperations(self._client, self._config, self._serialize, self._deserialize)
         self.countries = CountriesOperations(self._client, self._config, self._serialize, self._deserialize)
@@ -225,14 +235,15 @@
         self.external_access = ExternalAccessOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external_services = ExternalServicesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.electrical = ElectricalOperations(self._client, self._config, self._serialize, self._deserialize)
         self.welding = WeldingOperations(self._client, self._config, self._serialize, self._deserialize)
         self.links = LinksOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.locations = LocationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machine_alarms = MachineAlarmsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machines = MachinesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machine_utilization = MachineUtilizationOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.me = MeOperations(self._client, self._config, self._serialize, self._deserialize)
         self.measurement_form_schemas = MeasurementFormSchemasOperations(
@@ -261,14 +272,15 @@
         self.presentation = PresentationOperations(self._client, self._config, self._serialize, self._deserialize)
         self.suppliers = SuppliersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.sustainability = SustainabilityOperations(self._client, self._config, self._serialize, self._deserialize)
         self.system_health_dashboard = SystemHealthDashboardOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.trace = TraceOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.tracking = TrackingOperations(self._client, self._config, self._serialize, self._deserialize)
         self.upload = UploadOperations(self._client, self._config, self._serialize, self._deserialize)
         self.users = UsersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workspaces = WorkspacesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workspace_templates_admin = WorkspaceTemplatesAdminOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.workspace_templates = WorkspaceTemplatesOperations(
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/_configuration.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/_patch.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/_serialization.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/_serialization.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/aio/__init__.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/aio/_client.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/aio/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import IgnosPortalConfiguration
 from .operations import (
     AlertsOperations,
     AssetsOperations,
     AzureRegionsOperations,
+    BookingOperations,
     CdfOperations,
     CncFileTransferOperations,
     CncSetupAgentOperations,
     CncSetupOperations,
     CompaniesOperations,
     CountriesOperations,
     CustomerOrdersOperations,
@@ -31,14 +32,15 @@
     DocumentTypesOperations,
     DocumentsOperations,
     ElectricalOperations,
     ExternalAccessOperations,
     ExternalOperations,
     ExternalServicesOperations,
     LinksOperations,
+    LocationsOperations,
     MachineAlarmsOperations,
     MachineUtilizationOperations,
     MachinesOperations,
     MeOperations,
     MeasurementFormSchemasOperations,
     MeasurementFormsInstancesOperations,
     MeasuringToolsOperations,
@@ -54,14 +56,15 @@
     PowerOperations,
     PresentationOperations,
     ResourcesOperations,
     SuppliersOperations,
     SustainabilityOperations,
     SystemHealthDashboardOperations,
     TraceOperations,
+    TrackingOperations,
     UploadOperations,
     UsersOperations,
     WeldingOperations,
     WorkordersOperations,
     WorkspaceTemplatesAdminOperations,
     WorkspaceTemplatesOperations,
     WorkspacesOperations,
@@ -77,14 +80,16 @@
 
     :ivar alerts: AlertsOperations operations
     :vartype alerts: ignos.api.client.aio.operations.AlertsOperations
     :ivar assets: AssetsOperations operations
     :vartype assets: ignos.api.client.aio.operations.AssetsOperations
     :ivar azure_regions: AzureRegionsOperations operations
     :vartype azure_regions: ignos.api.client.aio.operations.AzureRegionsOperations
+    :ivar booking: BookingOperations operations
+    :vartype booking: ignos.api.client.aio.operations.BookingOperations
     :ivar cdf: CdfOperations operations
     :vartype cdf: ignos.api.client.aio.operations.CdfOperations
     :ivar cnc_file_transfer: CncFileTransferOperations operations
     :vartype cnc_file_transfer: ignos.api.client.aio.operations.CncFileTransferOperations
     :ivar cnc_setup: CncSetupOperations operations
     :vartype cnc_setup: ignos.api.client.aio.operations.CncSetupOperations
     :ivar cnc_setup_agent: CncSetupAgentOperations operations
@@ -113,14 +118,16 @@
     :vartype external_services: ignos.api.client.aio.operations.ExternalServicesOperations
     :ivar electrical: ElectricalOperations operations
     :vartype electrical: ignos.api.client.aio.operations.ElectricalOperations
     :ivar welding: WeldingOperations operations
     :vartype welding: ignos.api.client.aio.operations.WeldingOperations
     :ivar links: LinksOperations operations
     :vartype links: ignos.api.client.aio.operations.LinksOperations
+    :ivar locations: LocationsOperations operations
+    :vartype locations: ignos.api.client.aio.operations.LocationsOperations
     :ivar machine_alarms: MachineAlarmsOperations operations
     :vartype machine_alarms: ignos.api.client.aio.operations.MachineAlarmsOperations
     :ivar machines: MachinesOperations operations
     :vartype machines: ignos.api.client.aio.operations.MachinesOperations
     :ivar machine_utilization: MachineUtilizationOperations operations
     :vartype machine_utilization: ignos.api.client.aio.operations.MachineUtilizationOperations
     :ivar me: MeOperations operations
@@ -161,14 +168,16 @@
     :ivar sustainability: SustainabilityOperations operations
     :vartype sustainability: ignos.api.client.aio.operations.SustainabilityOperations
     :ivar system_health_dashboard: SystemHealthDashboardOperations operations
     :vartype system_health_dashboard:
      ignos.api.client.aio.operations.SystemHealthDashboardOperations
     :ivar trace: TraceOperations operations
     :vartype trace: ignos.api.client.aio.operations.TraceOperations
+    :ivar tracking: TrackingOperations operations
+    :vartype tracking: ignos.api.client.aio.operations.TrackingOperations
     :ivar upload: UploadOperations operations
     :vartype upload: ignos.api.client.aio.operations.UploadOperations
     :ivar users: UsersOperations operations
     :vartype users: ignos.api.client.aio.operations.UsersOperations
     :ivar workspaces: WorkspacesOperations operations
     :vartype workspaces: ignos.api.client.aio.operations.WorkspacesOperations
     :ivar workspace_templates_admin: WorkspaceTemplatesAdminOperations operations
@@ -206,14 +215,15 @@
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.alerts = AlertsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.assets = AssetsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.azure_regions = AzureRegionsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.booking = BookingOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cdf = CdfOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cnc_file_transfer = CncFileTransferOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.cnc_setup = CncSetupOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cnc_setup_agent = CncSetupAgentOperations(self._client, self._config, self._serialize, self._deserialize)
         self.countries = CountriesOperations(self._client, self._config, self._serialize, self._deserialize)
@@ -228,14 +238,15 @@
         self.external_access = ExternalAccessOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external_services = ExternalServicesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.electrical = ElectricalOperations(self._client, self._config, self._serialize, self._deserialize)
         self.welding = WeldingOperations(self._client, self._config, self._serialize, self._deserialize)
         self.links = LinksOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.locations = LocationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machine_alarms = MachineAlarmsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machines = MachinesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machine_utilization = MachineUtilizationOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.me = MeOperations(self._client, self._config, self._serialize, self._deserialize)
         self.measurement_form_schemas = MeasurementFormSchemasOperations(
@@ -264,14 +275,15 @@
         self.presentation = PresentationOperations(self._client, self._config, self._serialize, self._deserialize)
         self.suppliers = SuppliersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.sustainability = SustainabilityOperations(self._client, self._config, self._serialize, self._deserialize)
         self.system_health_dashboard = SystemHealthDashboardOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.trace = TraceOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.tracking = TrackingOperations(self._client, self._config, self._serialize, self._deserialize)
         self.upload = UploadOperations(self._client, self._config, self._serialize, self._deserialize)
         self.users = UsersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workspaces = WorkspacesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workspace_templates_admin = WorkspaceTemplatesAdminOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.workspace_templates = WorkspaceTemplatesOperations(
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/aio/_configuration.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/aio/_patch.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/aio/operations/__init__.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/aio/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import AlertsOperations
 from ._operations import AssetsOperations
 from ._operations import AzureRegionsOperations
+from ._operations import BookingOperations
 from ._operations import CdfOperations
 from ._operations import CncFileTransferOperations
 from ._operations import CncSetupOperations
 from ._operations import CncSetupAgentOperations
 from ._operations import CountriesOperations
 from ._operations import CustomersOperations
 from ._operations import DocumentsOperations
@@ -23,14 +24,15 @@
 from ._operations import WorkordersOperations
 from ._operations import ExternalOperations
 from ._operations import ExternalAccessOperations
 from ._operations import ExternalServicesOperations
 from ._operations import ElectricalOperations
 from ._operations import WeldingOperations
 from ._operations import LinksOperations
+from ._operations import LocationsOperations
 from ._operations import MachineAlarmsOperations
 from ._operations import MachinesOperations
 from ._operations import MachineUtilizationOperations
 from ._operations import MeOperations
 from ._operations import MeasurementFormSchemasOperations
 from ._operations import MeasurementFormsInstancesOperations
 from ._operations import MeasuringToolsOperations
@@ -45,28 +47,30 @@
 from ._operations import OperatorCalculatorsOperations
 from ._operations import PowerOperations
 from ._operations import PresentationOperations
 from ._operations import SuppliersOperations
 from ._operations import SustainabilityOperations
 from ._operations import SystemHealthDashboardOperations
 from ._operations import TraceOperations
+from ._operations import TrackingOperations
 from ._operations import UploadOperations
 from ._operations import UsersOperations
 from ._operations import WorkspacesOperations
 from ._operations import WorkspaceTemplatesAdminOperations
 from ._operations import WorkspaceTemplatesOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AlertsOperations",
     "AssetsOperations",
     "AzureRegionsOperations",
+    "BookingOperations",
     "CdfOperations",
     "CncFileTransferOperations",
     "CncSetupOperations",
     "CncSetupAgentOperations",
     "CountriesOperations",
     "CustomersOperations",
     "DocumentsOperations",
@@ -77,14 +81,15 @@
     "WorkordersOperations",
     "ExternalOperations",
     "ExternalAccessOperations",
     "ExternalServicesOperations",
     "ElectricalOperations",
     "WeldingOperations",
     "LinksOperations",
+    "LocationsOperations",
     "MachineAlarmsOperations",
     "MachinesOperations",
     "MachineUtilizationOperations",
     "MeOperations",
     "MeasurementFormSchemasOperations",
     "MeasurementFormsInstancesOperations",
     "MeasuringToolsOperations",
@@ -99,14 +104,15 @@
     "OperatorCalculatorsOperations",
     "PowerOperations",
     "PresentationOperations",
     "SuppliersOperations",
     "SustainabilityOperations",
     "SystemHealthDashboardOperations",
     "TraceOperations",
+    "TrackingOperations",
     "UploadOperations",
     "UsersOperations",
     "WorkspacesOperations",
     "WorkspaceTemplatesAdminOperations",
     "WorkspaceTemplatesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/aio/operations/_operations.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/aio/operations/_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import datetime
 from io import IOBase
 import sys
-from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
+from typing import Any, Callable, Dict, IO, List, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -36,27 +36,36 @@
     build_assets_get_asset_by_id_request,
     build_assets_get_asset_structure_by_id_request,
     build_assets_list_assets_request,
     build_assets_list_machines_request,
     build_assets_search_assets_request,
     build_assets_update_asset_request,
     build_azure_regions_list_azure_regions_request,
+    build_booking_cancel_booking_request,
+    build_booking_create_booking_request,
+    build_booking_finish_delivery_request,
+    build_booking_get_booking_request,
+    build_booking_list_bookings_request,
+    build_booking_start_delivery_request,
+    build_booking_update_booking_request,
     build_cdf_get_cdf_config_request,
     build_cdf_update_cdf_config_request,
     build_cnc_file_transfer_create_upload_cam_transfer_info_request,
     build_cnc_file_transfer_get_cam_transfer_request,
     build_cnc_file_transfer_get_transfer_status_request,
+    build_cnc_file_transfer_start_cam_transfer_to_machine_from_temp_upload_request,
     build_cnc_file_transfer_start_cam_transfer_to_machine_request,
     build_cnc_file_transfer_start_cnc_machine_operation_transfer_to_cloud_request,
     build_cnc_file_transfer_start_cnc_machine_operation_transfer_to_machine_request,
     build_cnc_setup_agent_create_upload_programs_info_request,
     build_cnc_setup_agent_get_cnc_agent_config_request,
     build_cnc_setup_agent_set_transfer_status_request,
     build_cnc_setup_copy_cnc_machine_operations_request,
     build_cnc_setup_copy_cnc_part_request,
+    build_cnc_setup_copy_tools_cnc_machine_request,
     build_cnc_setup_create_cnc_machine_operation_request,
     build_cnc_setup_create_cnc_machine_operation_tool_request,
     build_cnc_setup_create_cnc_machine_request,
     build_cnc_setup_create_cnc_machine_tool_request,
     build_cnc_setup_create_cnc_part_request,
     build_cnc_setup_create_upload_attachment_info_request,
     build_cnc_setup_create_upload_part_drawing_info_request,
@@ -65,14 +74,15 @@
     build_cnc_setup_delete_cnc_machine_operation_attachment_request,
     build_cnc_setup_delete_cnc_machine_operation_program_request,
     build_cnc_setup_delete_cnc_machine_operation_program_version_request,
     build_cnc_setup_delete_cnc_machine_operation_request,
     build_cnc_setup_delete_cnc_machine_operation_tool_image_request,
     build_cnc_setup_delete_cnc_machine_operation_tool_request,
     build_cnc_setup_delete_cnc_machine_request,
+    build_cnc_setup_delete_cnc_machine_tool_image_request,
     build_cnc_setup_delete_cnc_machine_tool_request,
     build_cnc_setup_delete_cnc_part_drawing_request,
     build_cnc_setup_delete_cnc_part_request,
     build_cnc_setup_get_cnc_machine_communication_settings_request,
     build_cnc_setup_get_cnc_machine_operation_request,
     build_cnc_setup_get_cnc_machine_request,
     build_cnc_setup_get_cnc_part_drawing_request,
@@ -94,14 +104,15 @@
     build_cnc_setup_update_cnc_machine_operation_program_request,
     build_cnc_setup_update_cnc_machine_operation_program_version_request,
     build_cnc_setup_update_cnc_machine_operation_request,
     build_cnc_setup_update_cnc_machine_operation_tool_request,
     build_cnc_setup_update_cnc_machine_request,
     build_cnc_setup_update_cnc_machine_tool_request,
     build_cnc_setup_update_cnc_part_request,
+    build_cnc_setup_upload_cnc_machine_tool_image_request,
     build_cnc_setup_upload_operation_cnc_tool_image_request,
     build_companies_list_production_companies_request,
     build_companies_select_production_company_request,
     build_countries_list_countries_request,
     build_customer_orders_get_customer_order_request,
     build_customer_orders_list_customer_order_lines_request,
     build_customer_orders_list_customer_orders_request,
@@ -145,28 +156,33 @@
     build_external_list_companies_request,
     build_external_list_invites_request,
     build_external_services_get_credential_request,
     build_links_create_link_request,
     build_links_delete_link_request,
     build_links_get_all_link_scopes_request,
     build_links_get_all_links_request,
+    build_locations_search_locations_request,
+    build_locations_suggestions_locations_request,
     build_machine_alarms_count_machine_alarms_request,
     build_machine_alarms_get_machine_alarm_details_request,
     build_machine_alarms_list_alarm_severity_occurrences_request,
     build_machine_alarms_list_alarms_per_machine_request,
     build_machine_alarms_list_machine_alarms_request,
     build_machine_utilization_get_factory_utilization_request,
     build_machine_utilization_get_machine_states_summary_request,
     build_machine_utilization_get_machine_utilization_request,
     build_machine_utilization_get_machine_utilizations_request,
     build_machine_utilization_get_utilization_details_for_machine_request,
     build_machine_utilization_list_machine_states_request,
     build_machine_utilization_list_machine_uptimes_today_request,
     build_machine_utilization_list_power_on_utilization_datapoints_request,
     build_machines_create_machine_group_request,
+    build_machines_create_machine_without_resource_request,
+    build_machines_create_resource_with_machine_request,
+    build_machines_create_resource_without_machine_request,
     build_machines_delete_machine_group_request,
     build_machines_get_machine_erp_data_request,
     build_machines_get_machine_states_summary_request,
     build_machines_get_machine_utilization_summary_request,
     build_machines_list_current_machine_operators_request,
     build_machines_list_current_machine_states_request,
     build_machines_list_machine_erp_data_request,
@@ -290,20 +306,22 @@
     build_measuring_tools_update_whitelisted_measuring_tool_request,
     build_measuring_tools_whitelist_measuring_tool_request,
     build_mes_documents_get_document_request,
     build_mes_get_worker_details_for_current_user_request,
     build_mes_links_add_mes_link_request,
     build_mes_links_delete_mes_link_request,
     build_mes_links_list_mes_links_request,
+    build_mes_links_list_unmapped_mes_links_request,
     build_mes_links_update_mes_link_request,
     build_mes_production_order_check_production_order_for_open_non_conformances_request,
     build_mes_production_order_get_production_order_bom_request,
     build_mes_production_order_get_production_order_open_non_conformances_request,
     build_mes_production_order_get_production_order_pick_list_suggestion_request,
     build_mes_production_order_get_production_order_request,
+    build_mes_production_order_list_production_order_activities_request,
     build_mes_production_order_post_material_pick_list_request,
     build_mes_production_schedule_get_available_production_schedule_filters_request,
     build_mes_production_schedule_get_scheduled_work_summary_request,
     build_mes_production_schedule_list_my_current_work_activities_request,
     build_mes_production_schedule_list_my_current_work_activities_v2_request,
     build_mes_production_schedule_list_production_schedule_operations_request,
     build_mes_production_schedule_post_list_production_schedule_operations_request,
@@ -367,34 +385,43 @@
     build_trace_add_sequence_to_trace_list_request,
     build_trace_generate_trace_request,
     build_trace_get_customer_order_trace_status_request,
     build_trace_get_trace_request,
     build_trace_list_customer_order_line_traces_request,
     build_trace_list_trace_workorders_request,
     build_trace_post_list_trace_workorders_request,
+    build_trace_set_trace_manual_completed_request,
     build_trace_update_trace_request,
+    build_tracking_create_label_request,
+    build_tracking_create_tracking_events_request,
+    build_tracking_create_tracking_history_request,
+    build_tracking_delete_tracking_history_request,
+    build_tracking_list_tracking_history_request,
+    build_tracking_list_work_order_tracking_history_request,
     build_upload_create_upload_info_request,
     build_users_list_users_request,
     build_users_post_list_users_request,
     build_welding_create_welding_iot_config_request,
     build_welding_delete_welding_iot_config_request,
     build_welding_list_electrical_data_configs_request,
     build_welding_list_welding_source_types_request,
     build_workorders_check_resource_status_request,
     build_workorders_create_work_order_mapping_request,
+    build_workorders_delete_work_order_mappings_request,
     build_workorders_delete_workorder_operation_event_request,
     build_workorders_delete_workorder_request,
     build_workorders_filter_workorder_operation_events_request,
     build_workorders_get_work_order_consumption_request,
     build_workorders_get_workorder_operation_event_request,
     build_workorders_get_workorder_request,
     build_workorders_list_active_workorder_operations_request,
     build_workorders_list_workorders_request,
     build_workorders_post_list_workorders_request,
     build_workorders_register_workorder_operation_event_request,
+    build_workorders_search_work_orders_request,
     build_workorders_set_workorder_customer_order_reference_request,
     build_workorders_start_workorder_operation_request,
     build_workorders_start_workorder_operation_v2_request,
     build_workorders_stop_workorder_operation_request,
     build_workorders_stop_workorder_operation_v2_request,
     build_workorders_update_workorder_operation_event_timestamps_request,
     build_workorders_upsert_workorder_consumption_request,
@@ -452,15 +479,15 @@
     async def alert_notification_access(self, **kwargs: Any) -> _models.AlertNotificationAccessDto:
         """alert_notification_access.
 
         :return: AlertNotificationAccessDto
         :rtype: ~ignos.api.client.models.AlertNotificationAccessDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -499,15 +526,15 @@
     async def get_machine_inactivity_alert_type(self, **kwargs: Any) -> _models.MachineInactivityAlertTypeDto:
         """get_machine_inactivity_alert_type.
 
         :return: MachineInactivityAlertTypeDto
         :rtype: ~ignos.api.client.models.MachineInactivityAlertTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -548,15 +575,15 @@
     ) -> List[_models.MachineInactivityCriteriaDtoAlertSubscriptionDto]:
         """list_machine_inactivity_subscriptions.
 
         :return: list of MachineInactivityCriteriaDtoAlertSubscriptionDto
         :rtype: list[~ignos.api.client.models.MachineInactivityCriteriaDtoAlertSubscriptionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -637,15 +664,15 @@
         :param body: Is either a SubscribeToMachineInactivityAlerts type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.SubscribeToMachineInactivityAlerts or IO[bytes]
         :return: MachineInactivityCriteriaDtoAlertSubscriptionDto
         :rtype: ~ignos.api.client.models.MachineInactivityCriteriaDtoAlertSubscriptionDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -751,15 +778,15 @@
         :param body: Is either a UpdateMachineInactivitySubscription type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateMachineInactivitySubscription or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -814,15 +841,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -897,15 +924,15 @@
         :paramtype limit: int
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: AssetDtoPagedResult
         :rtype: ~ignos.api.client.models.AssetDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -986,15 +1013,15 @@
 
         :param body: Is either a CreateAsset type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateAsset or IO[bytes]
         :return: AssetDto
         :rtype: ~ignos.api.client.models.AssetDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1056,15 +1083,15 @@
         :paramtype description: str
         :keyword limit: Default value is 100.
         :paramtype limit: int
         :return: list of AssetDto
         :rtype: list[~ignos.api.client.models.AssetDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1108,15 +1135,15 @@
 
         :param id: Required.
         :type id: int
         :return: AssetDto
         :rtype: ~ignos.api.client.models.AssetDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1204,15 +1231,15 @@
         :type id: int
         :param body: Is either a UpdateAssetRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateAssetRequest or IO[bytes]
         :return: AssetDto
         :rtype: ~ignos.api.client.models.AssetDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1269,15 +1296,15 @@
 
         :param id: Required.
         :type id: int
         :return: AssetStructureDto
         :rtype: ~ignos.api.client.models.AssetStructureDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1317,15 +1344,15 @@
     async def list_machines(self, **kwargs: Any) -> List[_models.MachineDto]:
         """list_machines.
 
         :return: list of MachineDto
         :rtype: list[~ignos.api.client.models.MachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1384,15 +1411,15 @@
     async def list_azure_regions(self, **kwargs: Any) -> List[_models.AzureRegionDto]:
         """list_azure_regions.
 
         :return: list of AzureRegionDto
         :rtype: list[~ignos.api.client.models.AzureRegionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1424,14 +1451,684 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
 
+class BookingOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.aio.IgnosPortal`'s
+        :attr:`booking` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    async def list_bookings(
+        self,
+        body: Optional[_models.BookingRequestListDto] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.BookingResponseListDto:
+        """list_bookings.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestListDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: BookingResponseListDto
+        :rtype: ~ignos.api.client.models.BookingResponseListDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def list_bookings(
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.BookingResponseListDto:
+        """list_bookings.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: BookingResponseListDto
+        :rtype: ~ignos.api.client.models.BookingResponseListDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def list_bookings(
+        self, body: Optional[Union[_models.BookingRequestListDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> _models.BookingResponseListDto:
+        """list_bookings.
+
+        :param body: Is either a BookingRequestListDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestListDto or IO[bytes]
+        :return: BookingResponseListDto
+        :rtype: ~ignos.api.client.models.BookingResponseListDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.BookingResponseListDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingRequestListDto")
+            else:
+                _json = None
+
+        _request = build_booking_list_bookings_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("BookingResponseListDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace_async
+    async def get_booking(self, booking_id: str, **kwargs: Any) -> _models.BookingResponseDto:
+        """get_booking.
+
+        :param booking_id: Required.
+        :type booking_id: str
+        :return: BookingResponseDto
+        :rtype: ~ignos.api.client.models.BookingResponseDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.BookingResponseDto] = kwargs.pop("cls", None)
+
+        _request = build_booking_get_booking_request(
+            booking_id=booking_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("BookingResponseDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    async def update_booking(  # pylint: disable=inconsistent-return-statements
+        self,
+        booking_id: str,
+        body: Optional[_models.BookingRequestDto] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """update_booking.
+
+        :param booking_id: Required.
+        :type booking_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def update_booking(  # pylint: disable=inconsistent-return-statements
+        self,
+        booking_id: str,
+        body: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """update_booking.
+
+        :param booking_id: Required.
+        :type booking_id: str
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def update_booking(  # pylint: disable=inconsistent-return-statements
+        self, booking_id: str, body: Optional[Union[_models.BookingRequestDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """update_booking.
+
+        :param booking_id: Required.
+        :type booking_id: str
+        :param body: Is either a BookingRequestDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingRequestDto")
+            else:
+                _json = None
+
+        _request = build_booking_update_booking_request(
+            booking_id=booking_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    async def create_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[_models.BookingRequestDto] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_booking.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_booking.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.BookingRequestDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_booking.
+
+        :param body: Is either a BookingRequestDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingRequestDto")
+            else:
+                _json = None
+
+        _request = build_booking_create_booking_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    async def cancel_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[_models.BookingUpdateDto] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """cancel_booking.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingUpdateDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def cancel_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """cancel_booking.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def cancel_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.BookingUpdateDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """cancel_booking.
+
+        :param body: Is either a BookingUpdateDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingUpdateDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingUpdateDto")
+            else:
+                _json = None
+
+        _request = build_booking_cancel_booking_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    async def start_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[_models.BookingUpdateDto] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """start_delivery.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingUpdateDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def start_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """start_delivery.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def start_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.BookingUpdateDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """start_delivery.
+
+        :param body: Is either a BookingUpdateDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingUpdateDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingUpdateDto")
+            else:
+                _json = None
+
+        _request = build_booking_start_delivery_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    async def finish_delivery(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.BookingDeliveryUpdateDto] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """finish_delivery.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingDeliveryUpdateDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def finish_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """finish_delivery.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def finish_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.BookingDeliveryUpdateDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """finish_delivery.
+
+        :param body: Is either a BookingDeliveryUpdateDto type or a IO[bytes] type. Default value is
+         None.
+        :type body: ~ignos.api.client.models.BookingDeliveryUpdateDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingDeliveryUpdateDto")
+            else:
+                _json = None
+
+        _request = build_booking_finish_delivery_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+
 class CdfOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.aio.IgnosPortal`'s
@@ -1453,15 +2150,15 @@
 
         Get CDF config.
 
         :return: CdfConfigDto
         :rtype: ~ignos.api.client.models.CdfConfigDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1543,15 +2240,15 @@
 
         :param body: Is either a UpdateCdfConfig type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateCdfConfig or IO[bytes]
         :return: CdfConfigDto
         :rtype: ~ignos.api.client.models.CdfConfigDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1629,15 +2326,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineTransferDto
         :rtype: ~ignos.api.client.models.CncMachineTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1681,15 +2378,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineTransferDto
         :rtype: ~ignos.api.client.models.CncMachineTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1731,15 +2428,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineTransferDto
         :rtype: ~ignos.api.client.models.CncMachineTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1820,15 +2517,15 @@
 
         :param body: Is either a UploadCamFileRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadCamFileRequest or IO[bytes]
         :return: UploadCamFileDto
         :rtype: ~ignos.api.client.models.UploadCamFileDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1884,15 +2581,15 @@
 
         :keyword path: Default value is None.
         :paramtype path: str
         :return: CamTransferDto
         :rtype: ~ignos.api.client.models.CamTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1974,15 +2671,15 @@
         :param body: Is either a StartCamTransferToMachine type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StartCamTransferToMachine or IO[bytes]
         :return: CncMachineTransferDto
         :rtype: ~ignos.api.client.models.CncMachineTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2028,14 +2725,118 @@
         deserialized = self._deserialize("CncMachineTransferDto", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
+    @overload
+    async def start_cam_transfer_to_machine_from_temp_upload(  # pylint: disable=name-too-long
+        self,
+        body: Optional[_models.StartCamTransferToMachineFromTempUpload] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.CncMachineTransferDto:
+        """start_cam_transfer_to_machine_from_temp_upload.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.StartCamTransferToMachineFromTempUpload
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: CncMachineTransferDto
+        :rtype: ~ignos.api.client.models.CncMachineTransferDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def start_cam_transfer_to_machine_from_temp_upload(  # pylint: disable=name-too-long
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.CncMachineTransferDto:
+        """start_cam_transfer_to_machine_from_temp_upload.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: CncMachineTransferDto
+        :rtype: ~ignos.api.client.models.CncMachineTransferDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def start_cam_transfer_to_machine_from_temp_upload(  # pylint: disable=name-too-long
+        self, body: Optional[Union[_models.StartCamTransferToMachineFromTempUpload, IO[bytes]]] = None, **kwargs: Any
+    ) -> _models.CncMachineTransferDto:
+        """start_cam_transfer_to_machine_from_temp_upload.
+
+        :param body: Is either a StartCamTransferToMachineFromTempUpload type or a IO[bytes] type.
+         Default value is None.
+        :type body: ~ignos.api.client.models.StartCamTransferToMachineFromTempUpload or IO[bytes]
+        :return: CncMachineTransferDto
+        :rtype: ~ignos.api.client.models.CncMachineTransferDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CncMachineTransferDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StartCamTransferToMachineFromTempUpload")
+            else:
+                _json = None
+
+        _request = build_cnc_file_transfer_start_cam_transfer_to_machine_from_temp_upload_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("CncMachineTransferDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
 
 class CncSetupOperations:  # pylint: disable=too-many-public-methods
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -2058,15 +2859,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineDto
         :rtype: ~ignos.api.client.models.CncMachineDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2155,15 +2956,15 @@
         :param body: Is either a UpdateCncMachineRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateCncMachineRequest or IO[bytes]
         :return: CncMachineDto
         :rtype: ~ignos.api.client.models.CncMachineDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2222,15 +3023,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2270,15 +3071,15 @@
 
         :keyword name_prefix: Default value is None.
         :paramtype name_prefix: str
         :return: list of CncMachineDto
         :rtype: list[~ignos.api.client.models.CncMachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2355,15 +3156,15 @@
 
         :param body: Is either a CreateCncMachine type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateCncMachine or IO[bytes]
         :return: CncMachineDto
         :rtype: ~ignos.api.client.models.CncMachineDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2421,15 +3222,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineCommunicationSettingsDto
         :rtype: ~ignos.api.client.models.CncMachineCommunicationSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2521,15 +3322,15 @@
         :param body: Is either a UpdateCncMachineCommunicationSettingsRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpdateCncMachineCommunicationSettingsRequest or IO[bytes]
         :return: CncMachineCommunicationSettingsDto
         :rtype: ~ignos.api.client.models.CncMachineCommunicationSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2588,15 +3389,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2669,15 +3470,15 @@
 
         :param body: Is either a CreateCncPart type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateCncPart or IO[bytes]
         :return: CncPartDto
         :rtype: ~ignos.api.client.models.CncPartDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2772,15 +3573,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: CncPartListDtoPagedResult
         :rtype: ~ignos.api.client.models.CncPartListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2879,15 +3680,15 @@
         :type id: str
         :param body: Is either a UpdateCncPartRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateCncPartRequest or IO[bytes]
         :return: CncPartDto
         :rtype: ~ignos.api.client.models.CncPartDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2944,15 +3745,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2990,15 +3791,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncPartDto
         :rtype: ~ignos.api.client.models.CncPartDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3079,15 +3880,15 @@
 
         :param body: Is either a ListCncPartsRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListCncPartsRequest or IO[bytes]
         :return: CncPartListDtoPagedResult
         :rtype: ~ignos.api.client.models.CncPartListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3178,15 +3979,15 @@
 
         :param body: Is either a CopyCncPart type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CopyCncPart or IO[bytes]
         :return: CncPartDto
         :rtype: ~ignos.api.client.models.CncPartDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3289,15 +4090,15 @@
         :param body: Is either a UploadPartDrawingRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UploadPartDrawingRequest or IO[bytes]
         :return: UploadFileDto
         :rtype: ~ignos.api.client.models.UploadFileDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3354,15 +4155,15 @@
 
         :param id: Required.
         :type id: str
         :return: FileDto
         :rtype: ~ignos.api.client.models.FileDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3451,15 +4252,15 @@
         :param body: Is either a DeletePartDrawingRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.DeletePartDrawingRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3552,15 +4353,15 @@
         :param body: Is either a CreateCncMachineOperation type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateCncMachineOperation or IO[bytes]
         :return: CncMachineOperationDto
         :rtype: ~ignos.api.client.models.CncMachineOperationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3658,15 +4459,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: CncMachineOperationSearchResultDtoPagedResult
         :rtype: ~ignos.api.client.models.CncMachineOperationSearchResultDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3760,15 +4561,15 @@
         :param body: Is either a ListCncMachineOperationsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ListCncMachineOperationsRequest or IO[bytes]
         :return: CncMachineOperationSearchResultDtoPagedResult
         :rtype: ~ignos.api.client.models.CncMachineOperationSearchResultDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3871,15 +4672,15 @@
         :param body: Is either a UpdateCncMachineOperationRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateCncMachineOperationRequest or IO[bytes]
         :return: CncMachineOperationDto
         :rtype: ~ignos.api.client.models.CncMachineOperationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3936,15 +4737,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineOperationDto
         :rtype: ~ignos.api.client.models.CncMachineOperationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3988,15 +4789,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4074,15 +4875,15 @@
         :param body: Is either a CopyCncMachineOperations type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CopyCncMachineOperations or IO[bytes]
         :return: list of CncMachineOperationDto
         :rtype: list[~ignos.api.client.models.CncMachineOperationDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4129,14 +4930,117 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
+    async def copy_tools_cnc_machine(
+        self,
+        body: Optional[_models.CopyToolsCncMachine] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> List[_models.CncToolDto]:
+        """copy_tools_cnc_machine.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CopyToolsCncMachine
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: list of CncToolDto
+        :rtype: list[~ignos.api.client.models.CncToolDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def copy_tools_cnc_machine(
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> List[_models.CncToolDto]:
+        """copy_tools_cnc_machine.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: list of CncToolDto
+        :rtype: list[~ignos.api.client.models.CncToolDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def copy_tools_cnc_machine(
+        self, body: Optional[Union[_models.CopyToolsCncMachine, IO[bytes]]] = None, **kwargs: Any
+    ) -> List[_models.CncToolDto]:
+        """copy_tools_cnc_machine.
+
+        :param body: Is either a CopyToolsCncMachine type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.CopyToolsCncMachine or IO[bytes]
+        :return: list of CncToolDto
+        :rtype: list[~ignos.api.client.models.CncToolDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[List[_models.CncToolDto]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CopyToolsCncMachine")
+            else:
+                _json = None
+
+        _request = build_cnc_setup_copy_tools_cnc_machine_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[CncToolDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
     async def create_upload_programs_info(
         self,
         id: str,
         body: Optional[_models.UploadFileRequest] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -4184,15 +5088,15 @@
         :type id: str
         :param body: Is either a UploadFileRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadFileRequest or IO[bytes]
         :return: list of UploadFileDto
         :rtype: list[~ignos.api.client.models.UploadFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4254,15 +5158,15 @@
         :keyword filter_deleted: Known values are: "NoneDeleted", "OnlyDeleted", and "All". Default
          value is None.
         :paramtype filter_deleted: str or ~ignos.api.client.models.CncFilterDeletedDto
         :return: list of ProgramFileDto
         :rtype: list[~ignos.api.client.models.ProgramFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4317,15 +5221,15 @@
         :keyword filter_deleted: Known values are: "NoneDeleted", "OnlyDeleted", and "All". Default
          value is None.
         :paramtype filter_deleted: str or ~ignos.api.client.models.CncFilterDeletedDto
         :return: list of ProgramFileDto
         :rtype: list[~ignos.api.client.models.ProgramFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4433,15 +5337,15 @@
         :param body: Is either a UpdateProgramFileRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateProgramFileRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4499,15 +5403,15 @@
         :type id: str
         :param filename: Required.
         :type filename: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4619,15 +5523,15 @@
         :param body: Is either a UpdateProgramFileRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateProgramFileRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4688,15 +5592,15 @@
         :type filename: str
         :param version_id: Required.
         :type version_id: int
         :return: list of ProgramFileDto
         :rtype: list[~ignos.api.client.models.ProgramFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4786,15 +5690,15 @@
         :type id: str
         :param body: Is either a UploadFileRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadFileRequest or IO[bytes]
         :return: list of UploadFileDto
         :rtype: list[~ignos.api.client.models.UploadFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4851,15 +5755,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of FileDto
         :rtype: list[~ignos.api.client.models.FileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4905,15 +5809,15 @@
         :type operation_id: str
         :param filename: Required.
         :type filename: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4952,15 +5856,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of CncMachineOperationDto
         :rtype: list[~ignos.api.client.models.CncMachineOperationDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5000,15 +5904,15 @@
     async def list_cnc_tool_types(self, **kwargs: Any) -> List[_models.CncToolTypeDto]:
         """list_cnc_tool_types.
 
         :return: list of CncToolTypeDto
         :rtype: list[~ignos.api.client.models.CncToolTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5099,15 +6003,15 @@
         :param body: Is either a CreateCncMachineOperationToolRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateCncMachineOperationToolRequest or IO[bytes]
         :return: CncToolDto
         :rtype: ~ignos.api.client.models.CncToolDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5164,15 +6068,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of CncToolDto
         :rtype: list[~ignos.api.client.models.CncToolDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5278,15 +6182,15 @@
         :param body: Is either a UpdateCncMachineOperationToolRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateCncMachineOperationToolRequest or IO[bytes]
         :return: CncToolDto
         :rtype: ~ignos.api.client.models.CncToolDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5348,15 +6252,15 @@
         :type operation_id: str
         :param id: Required.
         :type id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5459,15 +6363,15 @@
         :param body: Is either a UploadCncToolImageRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UploadCncToolImageRequest or IO[bytes]
         :return: ImageFileDto
         :rtype: ~ignos.api.client.models.ImageFileDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5531,15 +6435,15 @@
         :type id: int
         :param filename: Required.
         :type filename: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5629,15 +6533,15 @@
         :param body: Is either a CreateCncMachineOperationToolRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateCncMachineOperationToolRequest or IO[bytes]
         :return: CncToolDto
         :rtype: ~ignos.api.client.models.CncToolDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5694,15 +6598,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of CncToolDto
         :rtype: list[~ignos.api.client.models.CncToolDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5808,15 +6712,15 @@
         :param body: Is either a UpdateCncMachineToolRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateCncMachineToolRequest or IO[bytes]
         :return: CncToolDto
         :rtype: ~ignos.api.client.models.CncToolDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5878,15 +6782,15 @@
         :type cnc_machine_id: str
         :param id: Required.
         :type id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5916,14 +6820,198 @@
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @overload
+    async def upload_cnc_machine_tool_image(
+        self,
+        machine_id: str,
+        id: int,
+        body: Optional[_models.UploadCncToolImageRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.ImageFileDto:
+        """upload_cnc_machine_tool_image.
+
+        :param machine_id: Required.
+        :type machine_id: str
+        :param id: Required.
+        :type id: int
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.UploadCncToolImageRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: ImageFileDto
+        :rtype: ~ignos.api.client.models.ImageFileDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def upload_cnc_machine_tool_image(
+        self,
+        machine_id: str,
+        id: int,
+        body: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.ImageFileDto:
+        """upload_cnc_machine_tool_image.
+
+        :param machine_id: Required.
+        :type machine_id: str
+        :param id: Required.
+        :type id: int
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: ImageFileDto
+        :rtype: ~ignos.api.client.models.ImageFileDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def upload_cnc_machine_tool_image(
+        self,
+        machine_id: str,
+        id: int,
+        body: Optional[Union[_models.UploadCncToolImageRequest, IO[bytes]]] = None,
+        **kwargs: Any
+    ) -> _models.ImageFileDto:
+        """upload_cnc_machine_tool_image.
+
+        :param machine_id: Required.
+        :type machine_id: str
+        :param id: Required.
+        :type id: int
+        :param body: Is either a UploadCncToolImageRequest type or a IO[bytes] type. Default value is
+         None.
+        :type body: ~ignos.api.client.models.UploadCncToolImageRequest or IO[bytes]
+        :return: ImageFileDto
+        :rtype: ~ignos.api.client.models.ImageFileDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ImageFileDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UploadCncToolImageRequest")
+            else:
+                _json = None
+
+        _request = build_cnc_setup_upload_cnc_machine_tool_image_request(
+            machine_id=machine_id,
+            id=id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("ImageFileDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace_async
+    async def delete_cnc_machine_tool_image(  # pylint: disable=inconsistent-return-statements
+        self, machine_id: str, id: int, filename: str, **kwargs: Any
+    ) -> None:
+        """delete_cnc_machine_tool_image.
+
+        :param machine_id: Required.
+        :type machine_id: str
+        :param id: Required.
+        :type id: int
+        :param filename: Required.
+        :type filename: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        _request = build_cnc_setup_delete_cnc_machine_tool_image_request(
+            machine_id=machine_id,
+            id=id,
+            filename=filename,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
     async def import_operation_with_tools(  # pylint: disable=inconsistent-return-statements
         self,
         body: Optional[_models.ImportOperationWithTool] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
@@ -5965,15 +7053,15 @@
         :param body: Is either a ImportOperationWithTool type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ImportOperationWithTool or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6049,15 +7137,15 @@
         :paramtype agent_id: str
         :keyword agent_version: Default value is None.
         :paramtype agent_version: str
         :return: AgentConfigDto
         :rtype: ~ignos.api.client.models.AgentConfigDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6146,15 +7234,15 @@
         :type id: str
         :param body: Is either a UploadFileRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadFileRequest or IO[bytes]
         :return: list of UploadFileDto
         :rtype: list[~ignos.api.client.models.UploadFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6258,15 +7346,15 @@
         :param body: Is either a SetTransferStatusRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.SetTransferStatusRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6337,15 +7425,15 @@
     async def list_countries(self, **kwargs: Any) -> List[_models.CountryDto]:
         """list_countries.
 
         :return: list of CountryDto
         :rtype: list[~ignos.api.client.models.CountryDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6404,15 +7492,15 @@
     async def get_current_customer(self, **kwargs: Any) -> _models.CurrentCustomerDto:
         """get_current_customer.
 
         :return: CurrentCustomerDto
         :rtype: ~ignos.api.client.models.CurrentCustomerDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6505,15 +7593,15 @@
         :type id: str
         :param body: Is either a UpsertCustomerRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertCustomerRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6568,15 +7656,15 @@
 
         :param id: Customer id. Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6628,15 +7716,15 @@
         :keyword continuation_token_parameter: Continuation token used for pagination. Default value is
          None.
         :paramtype continuation_token_parameter: str
         :return: CustomerDtoPagedResult
         :rtype: ~ignos.api.client.models.CustomerDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6719,15 +7807,15 @@
 
         :param body: Is either a ListCustomersRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListCustomersRequest or IO[bytes]
         :return: CustomerDtoPagedResult
         :rtype: ~ignos.api.client.models.CustomerDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6783,15 +7871,15 @@
 
         List customer groups.
 
         :return: list of CustomerGroupDto
         :rtype: list[~ignos.api.client.models.CustomerGroupDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6834,15 +7922,15 @@
 
         :param id: Customer id. Required.
         :type id: str
         :return: ProblemDetails
         :rtype: ~ignos.api.client.models.ProblemDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6929,15 +8017,15 @@
 
         :param body: Is either a CreateCustomerMapping type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateCustomerMapping or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6989,15 +8077,15 @@
 
         Delete all customer mappings between old customer ids and new customer ids.
 
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7095,15 +8183,15 @@
 
         :param body: Is either a ImportDocument type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ImportDocument or IO[bytes]
         :return: ImportDocumentResultDto
         :rtype: ~ignos.api.client.models.ImportDocumentResultDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7163,15 +8251,15 @@
 
         :keyword imported_reference: Default value is None.
         :paramtype imported_reference: str
         :return: str
         :rtype: str
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7235,15 +8323,15 @@
 
         :keyword include_inactive: Default value is False.
         :paramtype include_inactive: bool
         :return: list of DocumentTypeDto
         :rtype: list[~ignos.api.client.models.DocumentTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7325,15 +8413,15 @@
         :param body: Is either a CreateDocumentTypeRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateDocumentTypeRequest or IO[bytes]
         :return: DocumentTypeDto
         :rtype: ~ignos.api.client.models.DocumentTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7389,15 +8477,15 @@
 
         :param id: Required.
         :type id: str
         :return: DocumentTypeDto
         :rtype: ~ignos.api.client.models.DocumentTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7486,15 +8574,15 @@
         :param body: Is either a UpdateDocumentTypeRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateDocumentTypeRequest or IO[bytes]
         :return: DocumentTypeDto
         :rtype: ~ignos.api.client.models.DocumentTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7555,15 +8643,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7603,15 +8691,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7651,15 +8739,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7697,15 +8785,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of DocumentTypeRuleDto
         :rtype: list[~ignos.api.client.models.DocumentTypeRuleDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7794,15 +8882,15 @@
         :param body: Is either a UpdateDocumentTypeRuleRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateDocumentTypeRuleRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7853,15 +8941,15 @@
     async def list_all_document_rule_types(self, **kwargs: Any) -> List[_models.DocumentTypeRuleTypeDto]:
         """list_all_document_rule_types.
 
         :return: list of DocumentTypeRuleTypeDto
         :rtype: list[~ignos.api.client.models.DocumentTypeRuleTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7900,15 +8988,15 @@
     async def list_document_generators(self, **kwargs: Any) -> List[_models.DocumentGeneratorTypeDto]:
         """list_document_generators.
 
         :return: list of DocumentGeneratorTypeDto
         :rtype: list[~ignos.api.client.models.DocumentGeneratorTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7967,15 +9055,15 @@
     async def list_production_companies(self, **kwargs: Any) -> List[_models.ProductionCompanyDto]:
         """list_production_companies.
 
         :return: list of ProductionCompanyDto
         :rtype: list[~ignos.api.client.models.ProductionCompanyDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8056,15 +9144,15 @@
         :param body: Is either a SelectProductionCompany type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.SelectProductionCompany or IO[bytes]
         :return: ProductionCompanyDto
         :rtype: ~ignos.api.client.models.ProductionCompanyDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8193,15 +9281,15 @@
         :param body: Order details. Is either a UpsertCustomerOrderRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpsertCustomerOrderRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8254,15 +9342,15 @@
 
         :param id: Required.
         :type id: str
         :return: CustomerOrderDto
         :rtype: ~ignos.api.client.models.CustomerOrderDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8370,15 +9458,15 @@
         :param body: Order line details. Is either a CustomerOrderLineDto type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.CustomerOrderLineDto or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8446,15 +9534,15 @@
         :keyword continuation_token_parameter: Continuation token used for pagination. Default value is
          None.
         :paramtype continuation_token_parameter: str
         :return: CustomerOrderDtoPagedResult
         :rtype: ~ignos.api.client.models.CustomerOrderDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8538,15 +9626,15 @@
         :param body: Is either a ListCustomerOrdersRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ListCustomerOrdersRequest or IO[bytes]
         :return: CustomerOrderDtoPagedResult
         :rtype: ~ignos.api.client.models.CustomerOrderDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8602,15 +9690,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of CustomerOrderLineDto
         :rtype: list[~ignos.api.client.models.CustomerOrderLineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8670,15 +9758,15 @@
     async def list_all_machines(self, **kwargs: Any) -> List[_models.MachineDto]:
         """list_all_machines.
 
         :return: list of MachineDto
         :rtype: list[~ignos.api.client.models.MachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8780,15 +9868,15 @@
 
         :param body: Is either a UpsertWorkorder type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertWorkorder or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8881,15 +9969,15 @@
 
         :param body: Is either a UpsertWorkorderV2 type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertWorkorderV2 or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8968,15 +10056,15 @@
         :keyword continuation_token_parameter: Continuation token used for pagination. Default value is
          None.
         :paramtype continuation_token_parameter: str
         :return: WorkorderListDtoPagedResult
         :rtype: ~ignos.api.client.models.WorkorderListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9079,15 +10167,15 @@
         :param body: Consumption details. Is either a UpsertWorkOrderConsumptionsRequest type or a
          IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertWorkOrderConsumptionsRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9140,15 +10228,15 @@
 
         :param id: Required.
         :type id: str
         :return: WorkOrderConsumptionDto
         :rtype: ~ignos.api.client.models.WorkOrderConsumptionDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9243,15 +10331,15 @@
         :param body: Trace details. Is either a UpsertWorkOrderTracesRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpsertWorkOrderTracesRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9354,15 +10442,15 @@
         :param body: Is either a WorkorderCustomerOrderReferenceDto type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.WorkorderCustomerOrderReferenceDto or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9415,15 +10503,15 @@
 
         :param id: Required.
         :type id: str
         :return: ResourceExistDto
         :rtype: ~ignos.api.client.models.ResourceExistDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9535,15 +10623,15 @@
         :param body: Is either a StartWorkOperationRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StartWorkOperationRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9667,15 +10755,15 @@
         :param body: Is either a StopWorkOperationRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StopWorkOperationRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9799,15 +10887,15 @@
         :param body: Is either a RegisterWorkorderOperationEventRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.RegisterWorkorderOperationEventRequest or IO[bytes]
         :return: WorkorderOperationEventDto
         :rtype: ~ignos.api.client.models.WorkorderOperationEventDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9935,15 +11023,15 @@
         :param body: Is either a StartWorkOperationRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StartWorkOperationRequest or IO[bytes]
         :return: WorkorderOperationEventDto
         :rtype: ~ignos.api.client.models.WorkorderOperationEventDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10071,15 +11159,15 @@
         :param body: Is either a StopWorkOperationRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StopWorkOperationRequest or IO[bytes]
         :return: WorkorderOperationEventDto
         :rtype: ~ignos.api.client.models.WorkorderOperationEventDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10135,15 +11223,15 @@
     async def list_active_workorder_operations(self, **kwargs: Any) -> List[_models.WorkorderOperationEventDto]:
         """list_active_workorder_operations.
 
         :return: list of WorkorderOperationEventDto
         :rtype: list[~ignos.api.client.models.WorkorderOperationEventDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10190,15 +11278,15 @@
         :type operation: int
         :param event_id: Required.
         :type event_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10240,15 +11328,15 @@
 
         :param id: The work order ID. Required.
         :type id: str
         :return: WorkorderDto
         :rtype: ~ignos.api.client.models.WorkorderDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10292,15 +11380,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10377,15 +11465,15 @@
 
         :param body: Is either a ListWorkOrdersRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListWorkOrdersRequest or IO[bytes]
         :return: WorkorderListDtoPagedResult
         :rtype: ~ignos.api.client.models.WorkorderListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10443,15 +11531,15 @@
 
         :param event_id: The ID of the event. Required.
         :type event_id: str
         :return: WorkorderOperationEventDto
         :rtype: ~ignos.api.client.models.WorkorderOperationEventDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10549,15 +11637,15 @@
         :param body: Is either a UpdateWorkorderOperationEventTimestamps type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpdateWorkorderOperationEventTimestamps or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10656,15 +11744,15 @@
         :param body: Is either a FilterWorkorderOperationEvents type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.FilterWorkorderOperationEvents or IO[bytes]
         :return: list of WorkorderOperationEventDto
         :rtype: list[~ignos.api.client.models.WorkorderOperationEventDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10766,15 +11854,15 @@
         :param body: Is either a CreateWorkOrderMapping type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateWorkOrderMapping or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10816,14 +11904,111 @@
                 await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
+    @distributed_trace_async
+    async def delete_work_order_mappings(self, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
+        """Deleteds existing work order mappings.
+
+        Deleteds existing work order mappings.
+
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        _request = build_workorders_delete_work_order_mappings_request(
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @distributed_trace_async
+    async def search_work_orders(
+        self, *, input: Optional[str] = None, **kwargs: Any
+    ) -> List[_models.SearchWorkOrderDto]:
+        """search_work_orders.
+
+        :keyword input: Default value is None.
+        :paramtype input: str
+        :return: list of SearchWorkOrderDto
+        :rtype: list[~ignos.api.client.models.SearchWorkOrderDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.SearchWorkOrderDto]] = kwargs.pop("cls", None)
+
+        _request = build_workorders_search_work_orders_request(
+            input=input,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[SearchWorkOrderDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
 
 class ExternalOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -10844,15 +12029,15 @@
     async def list_invites(self, **kwargs: Any) -> List[_models.InviteDto]:
         """list_invites.
 
         :return: list of InviteDto
         :rtype: list[~ignos.api.client.models.InviteDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10933,15 +12118,15 @@
         :param body: Is either a AcceptSupplierInviteRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.AcceptSupplierInviteRequest or IO[bytes]
         :return: CompanyDto
         :rtype: ~ignos.api.client.models.CompanyDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10995,15 +12180,15 @@
     async def list_companies(self, **kwargs: Any) -> List[_models.CompanyDto]:
         """list_companies.
 
         :return: list of CompanyDto
         :rtype: list[~ignos.api.client.models.CompanyDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11064,15 +12249,15 @@
 
         :keyword company_id: Default value is None.
         :paramtype company_id: str
         :return: list of CompanyUserDto
         :rtype: list[~ignos.api.client.models.CompanyUserDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11154,15 +12339,15 @@
         :param body: Is either a CreateCompanyUserRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateCompanyUserRequest or IO[bytes]
         :return: CompanyUserDto
         :rtype: ~ignos.api.client.models.CompanyUserDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11265,15 +12450,15 @@
         :param body: Is either a UpdateCompanyUserRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateCompanyUserRequest or IO[bytes]
         :return: CompanyUserDto
         :rtype: ~ignos.api.client.models.CompanyUserDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11334,15 +12519,15 @@
         :type id: str
         :keyword company_id: Default value is None.
         :paramtype company_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11379,15 +12564,15 @@
     async def list_roles(self, **kwargs: Any) -> List[_models.ExternalRoleDto]:
         """list_roles.
 
         :return: list of ExternalRoleDto
         :rtype: list[~ignos.api.client.models.ExternalRoleDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11426,15 +12611,15 @@
     async def list_company_customers(self, **kwargs: Any) -> List[_models.CompanyCustomerDto]:
         """list_company_customers.
 
         :return: list of CompanyCustomerDto
         :rtype: list[~ignos.api.client.models.CompanyCustomerDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11477,15 +12662,15 @@
 
         :param tenant_id: Required.
         :type tenant_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11546,15 +12731,15 @@
         :param service_name: Known values are: "DbExtractor", "MtConnectExtractor", and
          "MqttConnector". Required.
         :type service_name: str or ~ignos.api.client.models.ExternalServiceName
         :return: ExternalServiceCredentialDto
         :rtype: ~ignos.api.client.models.ExternalServiceCredentialDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11614,15 +12799,15 @@
     async def list_electrical_source_types(self, **kwargs: Any) -> List[_models.IotTypeSourceDto]:
         """list_electrical_source_types.
 
         :return: list of IotTypeSourceDto
         :rtype: list[~ignos.api.client.models.IotTypeSourceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11661,15 +12846,15 @@
     async def list_electrical_data_configs(self, **kwargs: Any) -> List[_models.ElectricalIotConfigDto]:
         """list_electrical_data_configs.
 
         :return: list of ElectricalIotConfigDto
         :rtype: list[~ignos.api.client.models.ElectricalIotConfigDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11750,15 +12935,15 @@
         :param body: Is either a CreateElectricalIotConfig type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateElectricalIotConfig or IO[bytes]
         :return: ElectricalIotConfigDto
         :rtype: ~ignos.api.client.models.ElectricalIotConfigDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11818,15 +13003,15 @@
         :type type_id: str
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11883,15 +13068,15 @@
     async def list_welding_source_types(self, **kwargs: Any) -> List[_models.IotTypeSourceDto]:
         """list_welding_source_types.
 
         :return: list of IotTypeSourceDto
         :rtype: list[~ignos.api.client.models.IotTypeSourceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11930,15 +13115,15 @@
     async def list_electrical_data_configs(self, **kwargs: Any) -> List[JSON]:
         """list_electrical_data_configs.
 
         :return: list of JSON
         :rtype: list[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11979,15 +13164,15 @@
 
         :param body: Default value is None.
         :type body: JSON
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12040,15 +13225,15 @@
         :type type_id: str
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12107,15 +13292,15 @@
 
         :keyword scope: Default value is None.
         :paramtype scope: str
         :return: list of LinkDto
         :rtype: list[~ignos.api.client.models.LinkDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12192,15 +13377,15 @@
 
         :param body: Is either a CreateLinkRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateLinkRequest or IO[bytes]
         :return: LinkDto
         :rtype: ~ignos.api.client.models.LinkDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12254,15 +13439,15 @@
     async def get_all_link_scopes(self, **kwargs: Any) -> List[str]:
         """get_all_link_scopes.
 
         :return: list of str
         :rtype: list[str]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12307,15 +13492,15 @@
         :type id: str
         :keyword scope: Default value is None.
         :paramtype scope: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12345,14 +13530,152 @@
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
 
+class LocationsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.aio.IgnosPortal`'s
+        :attr:`locations` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace_async
+    async def search_locations(
+        self,
+        *,
+        input: Optional[str] = None,
+        location_kinds: Optional[List[Union[str, _models.LocationKindDto]]] = None,
+        **kwargs: Any
+    ) -> List[_models.LocationDto]:
+        """search_locations.
+
+        :keyword input: Default value is None.
+        :paramtype input: str
+        :keyword location_kinds: Default value is None.
+        :paramtype location_kinds: list[str or ~ignos.api.client.models.LocationKindDto]
+        :return: list of LocationDto
+        :rtype: list[~ignos.api.client.models.LocationDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.LocationDto]] = kwargs.pop("cls", None)
+
+        _request = build_locations_search_locations_request(
+            input=input,
+            location_kinds=location_kinds,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[LocationDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace_async
+    async def suggestions_locations(
+        self,
+        *,
+        work_order_id: Optional[str] = None,
+        location_kinds: Optional[List[Union[str, _models.LocationKindDto]]] = None,
+        **kwargs: Any
+    ) -> List[_models.LocationDto]:
+        """suggestions_locations.
+
+        :keyword work_order_id: Default value is None.
+        :paramtype work_order_id: str
+        :keyword location_kinds: Default value is None.
+        :paramtype location_kinds: list[str or ~ignos.api.client.models.LocationKindDto]
+        :return: list of LocationDto
+        :rtype: list[~ignos.api.client.models.LocationDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.LocationDto]] = kwargs.pop("cls", None)
+
+        _request = build_locations_suggestions_locations_request(
+            work_order_id=work_order_id,
+            location_kinds=location_kinds,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[LocationDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+
 class MachineAlarmsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.aio.IgnosPortal`'s
@@ -12415,15 +13738,15 @@
         :paramtype order_by: str
         :keyword sort_direction: Default value is None.
         :paramtype sort_direction: str
         :return: MachineAlarmDtoPagedResult
         :rtype: ~ignos.api.client.models.MachineAlarmDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12485,15 +13808,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: list of MachineAlarmSummaryDto
         :rtype: list[~ignos.api.client.models.MachineAlarmSummaryDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12544,15 +13867,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: list of MachineAlarmSeverityOccurenceDto
         :rtype: list[~ignos.api.client.models.MachineAlarmSeverityOccurenceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12624,15 +13947,15 @@
         :paramtype name: str
         :keyword sequence: Default value is None.
         :paramtype sequence: str
         :return: MachineAlarmCountDto
         :rtype: ~ignos.api.client.models.MachineAlarmCountDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12682,15 +14005,15 @@
 
         :param id: Required.
         :type id: int
         :return: MachineAlarmDetailsDto
         :rtype: ~ignos.api.client.models.MachineAlarmDetailsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12750,15 +14073,15 @@
     async def list_machines(self, **kwargs: Any) -> List[_models.MachineDto]:
         """list_machines.
 
         :return: list of MachineDto
         :rtype: list[~ignos.api.client.models.MachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12797,15 +14120,15 @@
     async def list_machine_groups(self, **kwargs: Any) -> List[_models.MachineGroupDto]:
         """list_machine_groups.
 
         :return: list of MachineGroupDto
         :rtype: list[~ignos.api.client.models.MachineGroupDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12885,15 +14208,15 @@
 
         :param body: Is either a CreateMachineGroup type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateMachineGroup or IO[bytes]
         :return: CreateMachineGroupResponse
         :rtype: ~ignos.api.client.models.CreateMachineGroupResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12995,15 +14318,15 @@
         :type id: str
         :param body: Is either a UpdateMachineGroup type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateMachineGroup or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13058,15 +14381,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13106,15 +14429,15 @@
 
         :keyword asset_id: Default value is None.
         :paramtype asset_id: int
         :return: MachineStateListDto
         :rtype: ~ignos.api.client.models.MachineStateListDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13167,15 +14490,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: list of MachineStateDatapoint
         :rtype: list[~ignos.api.client.models.MachineStateDatapoint]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13230,15 +14553,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: MachineStatesSummaryDto
         :rtype: ~ignos.api.client.models.MachineStatesSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13280,15 +14603,15 @@
     async def list_machine_erp_data(self, **kwargs: Any) -> _models.MachineErpDataListDto:
         """list_machine_erp_data.
 
         :return: MachineErpDataListDto
         :rtype: ~ignos.api.client.models.MachineErpDataListDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13329,15 +14652,15 @@
 
         :param id: Required.
         :type id: int
         :return: MachineErpDataDto
         :rtype: ~ignos.api.client.models.MachineErpDataDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13377,15 +14700,15 @@
     async def get_machine_utilization_summary(self, **kwargs: Any) -> _models.UtilizationSummaryDto:
         """get_machine_utilization_summary.
 
         :return: UtilizationSummaryDto
         :rtype: ~ignos.api.client.models.UtilizationSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13430,15 +14753,15 @@
         :paramtype machine_external_id: str
         :keyword operator_name_query: Default value is None.
         :paramtype operator_name_query: str
         :return: list of OperatorAndMachineDto
         :rtype: list[~ignos.api.client.models.OperatorAndMachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13471,14 +14794,314 @@
         deserialized = self._deserialize("[OperatorAndMachineDto]", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
+    @overload
+    async def create_machine_without_resource(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.CreateMachineWithoutResource] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """create_machine_without_resource.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateMachineWithoutResource
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_machine_without_resource(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_machine_without_resource.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_machine_without_resource(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.CreateMachineWithoutResource, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_machine_without_resource.
+
+        :param body: Is either a CreateMachineWithoutResource type or a IO[bytes] type. Default value
+         is None.
+        :type body: ~ignos.api.client.models.CreateMachineWithoutResource or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateMachineWithoutResource")
+            else:
+                _json = None
+
+        _request = build_machines_create_machine_without_resource_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    async def create_resource_without_machine(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.CreateResourceWithoutMachine] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """create_resource_without_machine.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateResourceWithoutMachine
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_resource_without_machine(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_resource_without_machine.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_resource_without_machine(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.CreateResourceWithoutMachine, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_resource_without_machine.
+
+        :param body: Is either a CreateResourceWithoutMachine type or a IO[bytes] type. Default value
+         is None.
+        :type body: ~ignos.api.client.models.CreateResourceWithoutMachine or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateResourceWithoutMachine")
+            else:
+                _json = None
+
+        _request = build_machines_create_resource_without_machine_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    async def create_resource_with_machine(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.CreateResourceWithMachine] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """create_resource_with_machine.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateResourceWithMachine
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_resource_with_machine(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_resource_with_machine.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_resource_with_machine(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.CreateResourceWithMachine, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_resource_with_machine.
+
+        :param body: Is either a CreateResourceWithMachine type or a IO[bytes] type. Default value is
+         None.
+        :type body: ~ignos.api.client.models.CreateResourceWithMachine or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateResourceWithMachine")
+            else:
+                _json = None
+
+        _request = build_machines_create_resource_with_machine_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
 
 class MachineUtilizationOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -13533,15 +15156,15 @@
         :keyword utc_offset: Explicit UTC offset for start of today's utilization. Default value is
          None.
         :paramtype utc_offset: float
         :return: UtilizationListDto
         :rtype: ~ignos.api.client.models.UtilizationListDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13597,15 +15220,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: UtilizationDetailsDto
         :rtype: ~ignos.api.client.models.UtilizationDetailsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13660,15 +15283,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: MachineStatesSummaryDto
         :rtype: ~ignos.api.client.models.MachineStatesSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13723,15 +15346,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: list of MachineStateDatapoint
         :rtype: list[~ignos.api.client.models.MachineStateDatapoint]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13786,15 +15409,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: MachineStatesSummaryDto
         :rtype: ~ignos.api.client.models.MachineStatesSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13878,15 +15501,15 @@
         :param body: Is either a ListMachineUptimesTodayRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.ListMachineUptimesTodayRequest or IO[bytes]
         :return: MachineUptimesAggregateDto
         :rtype: ~ignos.api.client.models.MachineUptimesAggregateDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13959,15 +15582,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: PowerOnUtilizationList
         :rtype: ~ignos.api.client.models.PowerOnUtilizationList
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14011,15 +15634,15 @@
     async def get_factory_utilization(self, **kwargs: Any) -> _models.PowerOnUtilizationDto:
         """get_factory_utilization.
 
         :return: PowerOnUtilizationDto
         :rtype: ~ignos.api.client.models.PowerOnUtilizationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14078,15 +15701,15 @@
     async def get_my_apps(self, **kwargs: Any) -> List[_models.UserAppDto]:
         """get_my_apps.
 
         :return: list of UserAppDto
         :rtype: list[~ignos.api.client.models.UserAppDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14125,15 +15748,15 @@
     async def get_current_user(self, **kwargs: Any) -> _models.UserDetailsDto:
         """get_current_user.
 
         :return: UserDetailsDto
         :rtype: ~ignos.api.client.models.UserDetailsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14214,15 +15837,15 @@
         :param body: Is either a SetIsBetaTesterRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.SetIsBetaTesterRequest or IO[bytes]
         :return: UserDto
         :rtype: ~ignos.api.client.models.UserDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14278,15 +15901,15 @@
     ) -> None:
         """update_current_user_last_seen.
 
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14372,15 +15995,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14470,15 +16093,15 @@
         :param body: Is either a CreateMeasurementFormSchema type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMeasurementFormSchema or IO[bytes]
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14574,15 +16197,15 @@
         :param body: Is either a ListMeasurementFormSchemasRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormSchemasRequest or IO[bytes]
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14638,15 +16261,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14738,15 +16361,15 @@
         :param body: Is either a UpdateMeasurementFormSchemaRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateMeasurementFormSchemaRequest or IO[bytes]
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14853,15 +16476,15 @@
         :param body: Is either a UpdateSchemaGroupedElementsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateSchemaGroupedElementsRequest or IO[bytes]
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14964,15 +16587,15 @@
         :type id: str
         :param body: Is either a UploadDrawingRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadDrawingRequest or IO[bytes]
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15075,15 +16698,15 @@
         :type id: str
         :param body: Is either a UploadRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadRequest or IO[bytes]
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15142,15 +16765,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormImportStatusDto
         :rtype: ~ignos.api.client.models.MeasurementFormImportStatusDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15238,15 +16861,15 @@
         :type schema_id: str
         :param body: Is either a CreateSchemaElement type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateSchemaElement or IO[bytes]
         :return: MeasurementFormElementDto
         :rtype: ~ignos.api.client.models.MeasurementFormElementDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15317,15 +16940,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15410,15 +17033,15 @@
         :param body: Is either a ListLinkableMeasurementFormSchemasRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.ListLinkableMeasurementFormSchemasRequest or IO[bytes]
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15524,15 +17147,15 @@
         :param body: Is either a CreateMeasurementFormSchemaLinkRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.CreateMeasurementFormSchemaLinkRequest or IO[bytes]
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15593,15 +17216,15 @@
         :type schema_id: str
         :param linked_schema_id: Required.
         :type linked_schema_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15640,15 +17263,15 @@
 
         :param schema_id: Required.
         :type schema_id: str
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15690,15 +17313,15 @@
 
         :param schema_id: Required.
         :type schema_id: str
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15740,15 +17363,15 @@
 
         :param schema_id: Required.
         :type schema_id: str
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15792,15 +17415,15 @@
 
         :param schema_id: Required.
         :type schema_id: str
         :return: bool
         :rtype: bool
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15840,15 +17463,15 @@
     async def get_measurement_form_settings(self, **kwargs: Any) -> _models.MeasurementFormSettingsDto:
         """get_measurement_form_settings.
 
         :return: MeasurementFormSettingsDto
         :rtype: ~ignos.api.client.models.MeasurementFormSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15929,15 +17552,15 @@
         :param body: Is either a UpdateMeasurementFormSettings type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateMeasurementFormSettings or IO[bytes]
         :return: MeasurementFormSettingsDto
         :rtype: ~ignos.api.client.models.MeasurementFormSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15995,15 +17618,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormCustomerSettingsDto
         :rtype: ~ignos.api.client.models.MeasurementFormCustomerSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16085,15 +17708,15 @@
         :param body: Is either a UpdateMeasurementFormCustomerSettings type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpdateMeasurementFormCustomerSettings or IO[bytes]
         :return: MeasurementFormCustomerSettingsDto
         :rtype: ~ignos.api.client.models.MeasurementFormCustomerSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16151,15 +17774,15 @@
 
         :keyword target_id: Required.
         :paramtype target_id: str
         :return: list of MeasurementFormMappingDto
         :rtype: list[~ignos.api.client.models.MeasurementFormMappingDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16244,15 +17867,15 @@
          is None.
         :type body: ~ignos.api.client.models.CreateMeasurementFormMapping or IO[bytes]
         :return: MeasurementFormMappingDto or ProblemDetails
         :rtype: ~ignos.api.client.models.MeasurementFormMappingDto or
          ~ignos.api.client.models.ProblemDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16315,15 +17938,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormMappingDto
         :rtype: ~ignos.api.client.models.MeasurementFormMappingDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16367,15 +17990,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16463,15 +18086,15 @@
         :param body: Is either a [MeasurementFormBalloonMappingRequestDto] type or a IO[bytes] type.
          Default value is None.
         :type body: list[~ignos.api.client.models.MeasurementFormBalloonMappingRequestDto] or IO[bytes]
         :return: MeasurementFormMappingDto
         :rtype: ~ignos.api.client.models.MeasurementFormMappingDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16578,15 +18201,15 @@
         :param body: Is either a SetMeasurementFormMappingBalloonsRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.SetMeasurementFormMappingBalloonsRequest or IO[bytes]
         :return: MeasurementFormMappingDto
         :rtype: ~ignos.api.client.models.MeasurementFormMappingDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16647,15 +18270,15 @@
         :paramtype target_id: str
         :keyword source_id: Default value is None.
         :paramtype source_id: str
         :return: MeasurementFormMappingSuggestionDto
         :rtype: ~ignos.api.client.models.MeasurementFormMappingSuggestionDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16744,15 +18367,15 @@
         :param body: Is either a ImportMeasurementFormSchema type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ImportMeasurementFormSchema or IO[bytes]
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16840,15 +18463,15 @@
         :paramtype continuation_token_parameter: str
         :keyword only_without_drawing_url: Default value is None.
         :paramtype only_without_drawing_url: bool
         :return: MeasurementFormNeedDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormNeedDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16939,15 +18562,15 @@
         :param body: Is either a ListMeasurementFormNeedsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormNeedsRequest or IO[bytes]
         :return: MeasurementFormNeedDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormNeedDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17050,15 +18673,15 @@
         :param body: Is either a SetMeasurementFormNeedUserRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.SetMeasurementFormNeedUserRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17161,15 +18784,15 @@
         :param body: Is either a SetMeasurementFormNeedAsNotNeededRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.SetMeasurementFormNeedAsNotNeededRequest or IO[bytes]
         :return: MeasurementFormSchemaNotNeededDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaNotNeededDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17226,15 +18849,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17322,15 +18945,15 @@
         :type id: str
         :param body: Is either a UploadDrawingRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadDrawingRequest or IO[bytes]
         :return: MeasurementFormNeedDto
         :rtype: ~ignos.api.client.models.MeasurementFormNeedDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17416,15 +19039,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormSchemaNotNeededDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaNotNeededDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17514,15 +19137,15 @@
         :param body: Is either a ListMeasurementFormSchemasNotNeededRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormSchemasNotNeededRequest or IO[bytes]
         :return: MeasurementFormSchemaNotNeededDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaNotNeededDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17580,15 +19203,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17626,15 +19249,15 @@
     ) -> List[_models.MeasurementFormResourceTypeGeneratorDto]:
         """list_resource_types_for_needs_generator.
 
         :return: list of MeasurementFormResourceTypeGeneratorDto
         :rtype: list[~ignos.api.client.models.MeasurementFormResourceTypeGeneratorDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17715,15 +19338,15 @@
         :param body: Is either a AddResourceTypeForNeedsGenerator type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.AddResourceTypeForNeedsGenerator or IO[bytes]
         :return: MeasurementFormResourceTypeGeneratorDto
         :rtype: ~ignos.api.client.models.MeasurementFormResourceTypeGeneratorDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17781,15 +19404,15 @@
 
         :param resource_type: Required.
         :type resource_type: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17825,15 +19448,15 @@
     async def list_frequencies(self, **kwargs: Any) -> List[_models.MeasurementFrequencyDto]:
         """list_frequencies.
 
         :return: list of MeasurementFrequencyDto
         :rtype: list[~ignos.api.client.models.MeasurementFrequencyDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17885,15 +19508,15 @@
         :paramtype search: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: SchemaFeedbackDtoPagedResult
         :rtype: ~ignos.api.client.models.SchemaFeedbackDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17980,15 +19603,15 @@
          type. Default value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormInstanceSchemaFeedbackRequest or
          IO[bytes]
         :return: SchemaFeedbackDtoPagedResult
         :rtype: ~ignos.api.client.models.SchemaFeedbackDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18046,15 +19669,15 @@
 
         :param id: Required.
         :type id: str
         :return: SchemaFeedbackDto
         :rtype: ~ignos.api.client.models.SchemaFeedbackDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18098,15 +19721,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18194,15 +19817,15 @@
         :param body: Is either a SetMeasurementFormSchemaFeedbackUserRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.SetMeasurementFormSchemaFeedbackUserRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18281,15 +19904,15 @@
         :paramtype version: int
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18380,15 +20003,15 @@
         :param body: Is either a ListMeasurementFormSchemasWithHistoryRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormSchemasWithHistoryRequest or IO[bytes]
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18484,15 +20107,15 @@
         :paramtype inactive: bool
         :keyword include_inactive_supplier_access: Default value is None.
         :paramtype include_inactive_supplier_access: bool
         :return: MeasurementFormInstanceOverviewDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceOverviewDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18579,15 +20202,15 @@
         :param body: Is either a ListMeasurementFormsRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ListMeasurementFormsRequest or IO[bytes]
         :return: MeasurementFormInstanceOverviewDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceOverviewDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18664,15 +20287,15 @@
         :paramtype search: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormInstanceDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18759,15 +20382,15 @@
         :param body: Is either a ListMeasurementFormsByStatusRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormsByStatusRequest or IO[bytes]
         :return: MeasurementFormInstanceDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18827,15 +20450,15 @@
         :type id: str
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18878,15 +20501,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18978,15 +20601,15 @@
         :param body: Is either a UpdateMeasurementFormInstanceRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateMeasurementFormInstanceRequest or IO[bytes]
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19045,15 +20668,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of MeasurementFormInstanceFeedbackDto
         :rtype: list[~ignos.api.client.models.MeasurementFormInstanceFeedbackDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19099,15 +20722,15 @@
         :type id: str
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19150,15 +20773,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19200,15 +20823,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19250,15 +20873,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19300,15 +20923,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19358,15 +20981,15 @@
         :paramtype sequence: str
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: MeasurementFormInstanceSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19415,15 +21038,15 @@
         :type id: str
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: MeasurementFormInstanceProgressDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceProgressDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19483,15 +21106,15 @@
         :paramtype sequence: str
         :keyword element_id: Default value is None.
         :paramtype element_id: str
         :return: list of MeasurementFormElementValueAuditDto
         :rtype: list[~ignos.api.client.models.MeasurementFormElementValueAuditDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19535,15 +21158,15 @@
     async def get_validation_rules(self, **kwargs: Any) -> List[_models.ValidationRuleDto]:
         """get_validation_rules.
 
         :return: list of ValidationRuleDto
         :rtype: list[~ignos.api.client.models.ValidationRuleDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19648,15 +21271,15 @@
         :type body: ~ignos.api.client.models.SaveValueRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: SaveValueResponseDto
         :rtype: ~ignos.api.client.models.SaveValueResponseDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19778,15 +21401,15 @@
         :type body: ~ignos.api.client.models.SaveToolRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: SaveValueResponseDto
         :rtype: ~ignos.api.client.models.SaveValueResponseDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19908,15 +21531,15 @@
         :type body: ~ignos.api.client.models.SaveCommentRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20035,15 +21658,15 @@
         :type body: ~ignos.api.client.models.BatchInsertValueRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: BatchInsertValuesResponseDto
         :rtype: ~ignos.api.client.models.BatchInsertValuesResponseDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20176,15 +21799,15 @@
          IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20313,15 +21936,15 @@
         :type body: ~ignos.api.client.models.CreateMeasurementFormSchemaFeedbackRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: SchemaFeedbackCreatedDto
         :rtype: ~ignos.api.client.models.SchemaFeedbackCreatedDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20382,15 +22005,15 @@
 
         :param supplier_id: Required.
         :type supplier_id: str
         :return: list of MeasurementFormSupplierAccessInstanceDto
         :rtype: list[~ignos.api.client.models.MeasurementFormSupplierAccessInstanceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20497,15 +22120,15 @@
          type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertSupplierToMeasurementFormInstanceRequest or
          IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20563,15 +22186,15 @@
         :type id: str
         :param supplier_id: Required.
         :type supplier_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20657,15 +22280,15 @@
         :param body: Is either a ExportDimensionReportRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.ExportDimensionReportRequest or IO[bytes]
         :return: DownloadDto
         :rtype: ~ignos.api.client.models.DownloadDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20786,15 +22409,15 @@
         :param body: Is either a UpdateSchemaInstanceElementsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateSchemaInstanceElementsRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20852,15 +22475,15 @@
         :type id: str
         :param schema_id: Required.
         :type schema_id: str
         :return: list of SchemaInstanceElementDto
         :rtype: list[~ignos.api.client.models.SchemaInstanceElementDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20953,15 +22576,15 @@
         :param body: Is either a ImportMeasurementFormInstanceRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ImportMeasurementFormInstanceRequest or IO[bytes]
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21067,15 +22690,15 @@
         :paramtype sort_direction: str
         :keyword include_deprecated: Default value is False.
         :paramtype include_deprecated: bool
         :return: MeasuringToolDtoPagedData
         :rtype: ~ignos.api.client.models.MeasuringToolDtoPagedData
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21165,15 +22788,15 @@
         :param body: Is either a CreateMeasuringToolRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMeasuringToolRequest or IO[bytes]
         :return: MeasuringToolDetailDto
         :rtype: ~ignos.api.client.models.MeasuringToolDetailDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21276,15 +22899,15 @@
         :param body: Is either a UpdateMeasuringToolRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateMeasuringToolRequest or IO[bytes]
         :return: MeasuringToolDetailDto
         :rtype: ~ignos.api.client.models.MeasuringToolDetailDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21341,15 +22964,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasuringToolDetailDto
         :rtype: ~ignos.api.client.models.MeasuringToolDetailDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21391,15 +23014,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of MeasuringToolCalibrationDto
         :rtype: list[~ignos.api.client.models.MeasuringToolCalibrationDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21491,15 +23114,15 @@
         :param body: Is either a RegisterMeasuringToolCalibrationRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.RegisterMeasuringToolCalibrationRequest or IO[bytes]
         :return: MeasuringToolCalibrationDto
         :rtype: ~ignos.api.client.models.MeasuringToolCalibrationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21620,15 +23243,15 @@
         :param body: Is either a AttachCalibrationCertificateRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.AttachCalibrationCertificateRequest or IO[bytes]
         :return: MeasuringToolCalibrationDto
         :rtype: ~ignos.api.client.models.MeasuringToolCalibrationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21690,15 +23313,15 @@
         :type id: str
         :param calibration_id: Required.
         :type calibration_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21735,15 +23358,15 @@
     async def list_manufacturers(self, **kwargs: Any) -> List[_models.ManufacturerDto]:
         """list_manufacturers.
 
         :return: list of ManufacturerDto
         :rtype: list[~ignos.api.client.models.ManufacturerDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21824,15 +23447,15 @@
         :param body: Is either a CreateMeasuringToolManufacturer type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateMeasuringToolManufacturer or IO[bytes]
         :return: ManufacturerDto
         :rtype: ~ignos.api.client.models.ManufacturerDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21886,15 +23509,15 @@
     async def list_measuring_tool_types(self, **kwargs: Any) -> List[_models.MeasuringToolTypeDto]:
         """list_measuring_tool_types.
 
         :return: list of MeasuringToolTypeDto
         :rtype: list[~ignos.api.client.models.MeasuringToolTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21975,15 +23598,15 @@
         :param body: Is either a CreateMeasuringToolType type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMeasuringToolType or IO[bytes]
         :return: MeasuringToolTypeDto
         :rtype: ~ignos.api.client.models.MeasuringToolTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22086,15 +23709,15 @@
         :param body: Is either a UpdateMeasuringToolTypeRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateMeasuringToolTypeRequest or IO[bytes]
         :return: MeasuringToolTypeDto
         :rtype: ~ignos.api.client.models.MeasuringToolTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22153,15 +23776,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22199,15 +23822,15 @@
 
         :param type_id: Required.
         :type type_id: str
         :return: list of MeasuringToolSubTypeDto
         :rtype: list[~ignos.api.client.models.MeasuringToolSubTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22299,15 +23922,15 @@
         :param body: Is either a CreateMeasuringToolSubTypeRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateMeasuringToolSubTypeRequest or IO[bytes]
         :return: MeasuringToolSubTypeDto
         :rtype: ~ignos.api.client.models.MeasuringToolSubTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22428,15 +24051,15 @@
         :param body: Is either a UpdateMeasuringToolSubTypeRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateMeasuringToolSubTypeRequest or IO[bytes]
         :return: MeasuringToolSubTypeDto
         :rtype: ~ignos.api.client.models.MeasuringToolSubTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22498,15 +24121,15 @@
         :type type_id: str
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22543,15 +24166,15 @@
     async def list_measuring_units(self, **kwargs: Any) -> List[_models.MeasuringUnitDto]:
         """list_measuring_units.
 
         :return: list of MeasuringUnitDto
         :rtype: list[~ignos.api.client.models.MeasuringUnitDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22631,15 +24254,15 @@
 
         :param body: Is either a CreateMeasuringUnit type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateMeasuringUnit or IO[bytes]
         :return: MeasuringUnitDto
         :rtype: ~ignos.api.client.models.MeasuringUnitDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22697,15 +24320,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22760,15 +24383,15 @@
         :paramtype order_by: str
         :keyword sort_direction: Default value is None.
         :paramtype sort_direction: str
         :return: MeasuringToolWhitelistDtoPagedData
         :rtype: ~ignos.api.client.models.MeasuringToolWhitelistDtoPagedData
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22854,15 +24477,15 @@
         :param body: Is either a WhitelistMeasuringTool type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.WhitelistMeasuringTool or IO[bytes]
         :return: MeasuringToolWhitelistDto
         :rtype: ~ignos.api.client.models.MeasuringToolWhitelistDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22965,15 +24588,15 @@
         :param body: Is either a UpdateWhitelistedMeasuringTool type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateWhitelistedMeasuringTool or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23026,15 +24649,15 @@
 
         :param id: Required.
         :type id: str
         :return: ProblemDetails or None
         :rtype: ~ignos.api.client.models.ProblemDetails or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23076,15 +24699,15 @@
     async def list_unregistered_tool_values(self, **kwargs: Any) -> List[_models.UnregisteredToolValueDto]:
         """list_unregistered_tool_values.
 
         :return: list of UnregisteredToolValueDto
         :rtype: list[~ignos.api.client.models.UnregisteredToolValueDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23171,15 +24794,15 @@
         :type id: str
         :param body: Is either a DeprecateToolRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.DeprecateToolRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23234,15 +24857,15 @@
 
         :keyword status: Known values are: "SoonDue" and "Expired". Default value is None.
         :paramtype status: str or ~ignos.api.client.models.CalibrationListStatus
         :return: list of CalibrationListToolDto
         :rtype: list[~ignos.api.client.models.CalibrationListToolDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23323,15 +24946,15 @@
 
         :param body: Is either a ImportMeasuringTool type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ImportMeasuringTool or IO[bytes]
         :return: MeasuringToolDetailDto
         :rtype: ~ignos.api.client.models.MeasuringToolDetailDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23427,15 +25050,15 @@
         :param body: Is either a UpdateMeasuringToolSettings type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateMeasuringToolSettings or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23485,15 +25108,15 @@
     async def get_measuring_tool_settings(self, **kwargs: Any) -> _models.MeasuringToolSettingsDto:
         """get_measuring_tool_settings.
 
         :return: MeasuringToolSettingsDto
         :rtype: ~ignos.api.client.models.MeasuringToolSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23552,15 +25175,15 @@
     async def get_worker_details_for_current_user(self, **kwargs: Any) -> _models.WorkerDto:
         """get_worker_details_for_current_user.
 
         :return: WorkerDto
         :rtype: ~ignos.api.client.models.WorkerDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23623,15 +25246,15 @@
         :type drawing_number: str
         :param id: Required.
         :type id: str
         :return: DocumentLinkDto
         :rtype: ~ignos.api.client.models.DocumentLinkDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23729,15 +25352,15 @@
 
         :param body: Is either a AddMesLink type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.AddMesLink or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23783,48 +25406,95 @@
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace_async
     async def list_mes_links(
         self,
         *,
-        company_id: Optional[str] = None,
-        type: Optional[Union[str, _models.MesLinkTypeDto]] = None,
-        operation_id: Optional[str] = None,
+        types: Optional[List[Union[str, _models.MesLinkTypeDto]]] = None,
+        work_order_id: Optional[str] = None,
+        operation: Optional[int] = None,
         **kwargs: Any
     ) -> List[_models.MesLinkDto]:
         """list_mes_links.
 
-        :keyword company_id: Default value is None.
-        :paramtype company_id: str
-        :keyword type: Known values are: "Static", "Operation", and "WorkOrder". Default value is None.
-        :paramtype type: str or ~ignos.api.client.models.MesLinkTypeDto
-        :keyword operation_id: Default value is None.
-        :paramtype operation_id: str
+        :keyword types: Default value is None.
+        :paramtype types: list[str or ~ignos.api.client.models.MesLinkTypeDto]
+        :keyword work_order_id: Default value is None.
+        :paramtype work_order_id: str
+        :keyword operation: Default value is None.
+        :paramtype operation: int
         :return: list of MesLinkDto
         :rtype: list[~ignos.api.client.models.MesLinkDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.MesLinkDto]] = kwargs.pop("cls", None)
 
         _request = build_mes_links_list_mes_links_request(
-            company_id=company_id,
-            type=type,
-            operation_id=operation_id,
+            types=types,
+            work_order_id=work_order_id,
+            operation=operation,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[MesLinkDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace_async
+    async def list_unmapped_mes_links(self, **kwargs: Any) -> List[_models.MesLinkDto]:
+        """list_unmapped_mes_links.
+
+        :return: list of MesLinkDto
+        :rtype: list[~ignos.api.client.models.MesLinkDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.MesLinkDto]] = kwargs.pop("cls", None)
+
+        _request = build_mes_links_list_unmapped_mes_links_request(
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
@@ -23898,15 +25568,15 @@
         :type id: str
         :param body: Is either a UpdateMesLink type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateMesLink or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23959,15 +25629,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24025,15 +25695,15 @@
 
         :param id: Required.
         :type id: str
         :return: ProductionOrderDto
         :rtype: ~ignos.api.client.models.ProductionOrderDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24079,15 +25749,15 @@
         :type id: str
         :keyword operation: Default value is None.
         :paramtype operation: int
         :return: list of ProductionOrderBomDto
         :rtype: list[~ignos.api.client.models.ProductionOrderBomDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24134,15 +25804,15 @@
         :type id: str
         :keyword operation: Default value is None.
         :paramtype operation: int
         :return: list of PickListSuggestionDto
         :rtype: list[~ignos.api.client.models.PickListSuggestionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24187,15 +25857,15 @@
 
         :param id: Required.
         :type id: str
         :return: bool
         :rtype: bool
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24241,15 +25911,15 @@
         :type id: str
         :keyword only_open: Default value is True.
         :paramtype only_open: bool
         :return: list of NonConformanceDto
         :rtype: list[~ignos.api.client.models.NonConformanceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24345,15 +26015,15 @@
         :type operation_number: int
         :param body: Is either a PostMaterialPickListRequest type or a IO[bytes] type. Required.
         :type body: ~ignos.api.client.models.PostMaterialPickListRequest or IO[bytes]
         :return: MaterialPickListResultDto
         :rtype: ~ignos.api.client.models.MaterialPickListResultDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24398,14 +26068,69 @@
         deserialized = self._deserialize("MaterialPickListResultDto", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
+    @distributed_trace_async
+    async def list_production_order_activities(
+        self, id: str, *, operation: Optional[int] = None, **kwargs: Any
+    ) -> List[_models.ProductionOrderOperationActivityDto]:
+        """list_production_order_activities.
+
+        :param id: Required.
+        :type id: str
+        :keyword operation: Default value is None.
+        :paramtype operation: int
+        :return: list of ProductionOrderOperationActivityDto
+        :rtype: list[~ignos.api.client.models.ProductionOrderOperationActivityDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.ProductionOrderOperationActivityDto]] = kwargs.pop("cls", None)
+
+        _request = build_mes_production_order_list_production_order_activities_request(
+            id=id,
+            operation=operation,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[ProductionOrderOperationActivityDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
 
 class MesProductionScheduleOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -24457,15 +26182,15 @@
         :paramtype part_name: str
         :keyword material: Default value is None.
         :paramtype material: str
         :return: ProductionScheduleOperationDtoPagedResult
         :rtype: ~ignos.api.client.models.ProductionScheduleOperationDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24555,15 +26280,15 @@
         :param body: Is either a ListProductionScheduleOperationsRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.ListProductionScheduleOperationsRequest or IO[bytes]
         :return: ProductionScheduleOperationDtoPagedResult
         :rtype: ~ignos.api.client.models.ProductionScheduleOperationDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24661,15 +26386,15 @@
         :param body: Is either a GetAvailableProductionScheduleFiltersRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.GetAvailableProductionScheduleFiltersRequest or IO[bytes]
         :return: ProductionScheduleFiltersDto
         :rtype: ~ignos.api.client.models.ProductionScheduleFiltersDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24716,33 +26441,33 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
-    async def list_my_current_work_activities(self, **kwargs: Any) -> List[_models.CurrentWorkActivityDto]:
+    async def list_my_current_work_activities(self, **kwargs: Any) -> _models.CurrentWorkActivityDto:
         """list_my_current_work_activities.
 
-        :return: list of CurrentWorkActivityDto
-        :rtype: list[~ignos.api.client.models.CurrentWorkActivityDto]
+        :return: CurrentWorkActivityDto
+        :rtype: ~ignos.api.client.models.CurrentWorkActivityDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[List[_models.CurrentWorkActivityDto]] = kwargs.pop("cls", None)
+        cls: ClsType[_models.CurrentWorkActivityDto] = kwargs.pop("cls", None)
 
         _request = build_mes_production_schedule_list_my_current_work_activities_request(
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -24755,41 +26480,41 @@
 
         if response.status_code not in [200]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
-        deserialized = self._deserialize("[CurrentWorkActivityDto]", pipeline_response)
+        deserialized = self._deserialize("CurrentWorkActivityDto", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace_async
-    async def list_my_current_work_activities_v2(self, **kwargs: Any) -> _models.CurrentWorkActivityV2Dto:
+    async def list_my_current_work_activities_v2(self, **kwargs: Any) -> _models.CurrentWorkActivityDto:
         """list_my_current_work_activities_v2.
 
-        :return: CurrentWorkActivityV2Dto
-        :rtype: ~ignos.api.client.models.CurrentWorkActivityV2Dto
+        :return: CurrentWorkActivityDto
+        :rtype: ~ignos.api.client.models.CurrentWorkActivityDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[_models.CurrentWorkActivityV2Dto] = kwargs.pop("cls", None)
+        cls: ClsType[_models.CurrentWorkActivityDto] = kwargs.pop("cls", None)
 
         _request = build_mes_production_schedule_list_my_current_work_activities_v2_request(
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -24802,15 +26527,15 @@
 
         if response.status_code not in [200]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
-        deserialized = self._deserialize("CurrentWorkActivityV2Dto", pipeline_response)
+        deserialized = self._deserialize("CurrentWorkActivityDto", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -24854,15 +26579,15 @@
 
         :param body: Is either a StartOperations type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.StartOperations or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24954,15 +26679,15 @@
         :param body: Is either a ReportOperationProgress type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ReportOperationProgress or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25018,15 +26743,15 @@
         :paramtype resource_group: str
         :keyword resource_id: Default value is None.
         :paramtype resource_id: str
         :return: ScheduledWorkSummaryDto
         :rtype: ~ignos.api.client.models.ScheduledWorkSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25128,15 +26853,15 @@
 
         :param body: Is either a ListProjectsRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListProjectsRequest or IO[bytes]
         :return: WorkOrderProjectDtoPagedResult
         :rtype: ~ignos.api.client.models.WorkOrderProjectDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25232,15 +26957,15 @@
         :param body: Is either a ListOrderScheduleRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ListOrderScheduleRequest or IO[bytes]
         :return: WorkorderDtoPagedResult
         :rtype: ~ignos.api.client.models.WorkorderDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25318,15 +27043,15 @@
 
         :keyword include_resources: Default value is False.
         :paramtype include_resources: bool
         :return: list of ResourceGroupDto
         :rtype: list[~ignos.api.client.models.ResourceGroupDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25368,15 +27093,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of ProductionResourceDto
         :rtype: list[~ignos.api.client.models.ProductionResourceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25442,15 +27167,15 @@
         :paramtype customer_order: str
         :keyword customer_order_line: Default value is None.
         :paramtype customer_order_line: int
         :return: list of MrbInstanceDto
         :rtype: list[~ignos.api.client.models.MrbInstanceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25528,15 +27253,15 @@
 
         :param body: Is either a CreateMrb type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateMrb or IO[bytes]
         :return: MrbInstanceJobDto
         :rtype: ~ignos.api.client.models.MrbInstanceJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25590,15 +27315,15 @@
     async def list_recent_mrb_intances(self, **kwargs: Any) -> List[_models.MrbInstanceDto]:
         """list_recent_mrb_intances.
 
         :return: list of MrbInstanceDto
         :rtype: list[~ignos.api.client.models.MrbInstanceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25639,15 +27364,15 @@
 
         :param id: Required.
         :type id: str
         :return: MrbInstanceDto
         :rtype: ~ignos.api.client.models.MrbInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25689,15 +27414,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of MrbInstanceRevisionDto
         :rtype: list[~ignos.api.client.models.MrbInstanceRevisionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25786,15 +27511,15 @@
         :param body: Is either a CreateMrbRevisionRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMrbRevisionRequest or IO[bytes]
         :return: MrbInstanceJobDto
         :rtype: ~ignos.api.client.models.MrbInstanceJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25853,15 +27578,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: MrbContentDto
         :rtype: ~ignos.api.client.models.MrbContentDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25908,15 +27633,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25959,15 +27684,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26008,15 +27733,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: MrbPdfExportJobDto
         :rtype: ~ignos.api.client.models.MrbPdfExportJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26061,15 +27786,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: MrbInstanceJobDto
         :rtype: ~ignos.api.client.models.MrbInstanceJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26176,15 +27901,15 @@
         :param body: Is either a IncludeExcludeMrbRevisionContentRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.IncludeExcludeMrbRevisionContentRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26302,15 +28027,15 @@
         :param body: Is either a IncludeExcludeMrbRevisionContentRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.IncludeExcludeMrbRevisionContentRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26427,15 +28152,15 @@
         :type revision_id: int
         :param body: Is either a AttachPdfRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.AttachPdfRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26493,15 +28218,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26542,15 +28267,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: DownloadDto
         :rtype: ~ignos.api.client.models.DownloadDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26593,15 +28318,15 @@
 
         :param job_id: Required.
         :type job_id: str
         :return: MrbInstanceJobDto
         :rtype: ~ignos.api.client.models.MrbInstanceJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26643,15 +28368,15 @@
 
         :param job_id: Required.
         :type job_id: str
         :return: MrbPdfExportJobDto
         :rtype: ~ignos.api.client.models.MrbPdfExportJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26697,15 +28422,15 @@
         :paramtype page_size: int
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MrbInstanceReportDtoPagedResult
         :rtype: ~ignos.api.client.models.MrbInstanceReportDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26788,15 +28513,15 @@
         :param body: Is either a ListMrbInstanceReportsRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.ListMrbInstanceReportsRequest or IO[bytes]
         :return: MrbInstanceReportDtoPagedResult
         :rtype: ~ignos.api.client.models.MrbInstanceReportDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26903,15 +28628,15 @@
         :type template_id: str
         :param body: Is either a AttachPdfRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.AttachPdfRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26966,15 +28691,15 @@
 
         :param template_id: Required.
         :type template_id: str
         :return: MrbTemplateDto
         :rtype: ~ignos.api.client.models.MrbTemplateDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27022,15 +28747,15 @@
         :paramtype customer_id: str
         :keyword customer_group_id: Default value is None.
         :paramtype customer_group_id: str
         :return: list of MrbTemplateDto
         :rtype: list[~ignos.api.client.models.MrbTemplateDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27119,15 +28844,15 @@
         :param body: Is either a CreateMrbTemplateRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMrbTemplateRequest or IO[bytes]
         :return: MrbTemplateDto
         :rtype: ~ignos.api.client.models.MrbTemplateDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27224,15 +28949,15 @@
 
         :param body: Is either a UpdateMrbTemplate type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateMrbTemplate or IO[bytes]
         :return: MrbTemplateDto
         :rtype: ~ignos.api.client.models.MrbTemplateDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27334,15 +29059,15 @@
         :param body: Is either a DeleteMrbTemplateRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.DeleteMrbTemplateRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27392,15 +29117,15 @@
     async def get_mrb_company_settings(self, **kwargs: Any) -> _models.MrbCompanySettingsDto:
         """get_mrb_company_settings.
 
         :return: MrbCompanySettingsDto
         :rtype: ~ignos.api.client.models.MrbCompanySettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27481,15 +29206,15 @@
         :param body: Is either a UpsertMrbCompanySettings type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpsertMrbCompanySettings or IO[bytes]
         :return: MrbCompanySettingsDto
         :rtype: ~ignos.api.client.models.MrbCompanySettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27613,15 +29338,15 @@
         :param body: Contains diameter, and one of cutting speed or spindle speed. Is either a
          CalculateSpindleAndCuttingSpeed type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CalculateSpindleAndCuttingSpeed or IO[bytes]
         :return: SpindleAndCuttingSpeedDto
         :rtype: ~ignos.api.client.models.SpindleAndCuttingSpeedDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27729,15 +29454,15 @@
         :param body: Contains the two parameters to calculate from. Is either a
          CalculateRightAngledTriangle type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CalculateRightAngledTriangle or IO[bytes]
         :return: RightAngledTriangleDto
         :rtype: ~ignos.api.client.models.RightAngledTriangleDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27793,15 +29518,15 @@
 
         List default material types with mass density.
 
         :return: list of MaterialMassDensityDto
         :rtype: list[~ignos.api.client.models.MaterialMassDensityDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27888,15 +29613,15 @@
         :param body: Contains dimensions and mass density for given material. Is either a
          CalculateBarWeight type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CalculateBarWeight or IO[bytes]
         :return: MaterialWeightDto
         :rtype: ~ignos.api.client.models.MaterialWeightDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27972,15 +29697,15 @@
 
         :keyword country: Default value is None.
         :paramtype country: str
         :return: list of PowerRegionDto
         :rtype: list[~ignos.api.client.models.PowerRegionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28042,15 +29767,15 @@
 
         :param component_id: Required.
         :type component_id: str
         :return: ComponentSettingsDto
         :rtype: ~ignos.api.client.models.ComponentSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28110,15 +29835,15 @@
     async def list_supplier_invites(self, **kwargs: Any) -> List[_models.SupplierInviteDto]:
         """list_supplier_invites.
 
         :return: list of SupplierInviteDto
         :rtype: list[~ignos.api.client.models.SupplierInviteDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28198,15 +29923,15 @@
 
         :param body: Is either a CreateSupplierInvite type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateSupplierInvite or IO[bytes]
         :return: SupplierInviteDto
         :rtype: ~ignos.api.client.models.SupplierInviteDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28264,15 +29989,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28308,15 +30033,15 @@
     async def list_suppliers(self, **kwargs: Any) -> List[_models.ExternalSupplierDto]:
         """list_suppliers.
 
         :return: list of ExternalSupplierDto
         :rtype: list[~ignos.api.client.models.ExternalSupplierDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28357,15 +30082,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28438,15 +30163,15 @@
 
         :param body: Is either a ImportSupplier type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ImportSupplier or IO[bytes]
         :return: ExternalSupplierDto
         :rtype: ~ignos.api.client.models.ExternalSupplierDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28547,15 +30272,15 @@
 
         :param body: Is either a CreateSupplierMapping type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateSupplierMapping or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28607,15 +30332,15 @@
 
         Delete all supplier mappings between old supplier ids and new supplier ids.
 
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28670,15 +30395,15 @@
     async def test(self, **kwargs: Any) -> str:
         """test.
 
         :return: str
         :rtype: str
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28754,15 +30479,15 @@
 
         :param body: Is either a GetConsumption type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.GetConsumption or IO[bytes]
         :return: ConsumptionDto
         :rtype: ~ignos.api.client.models.ConsumptionDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28853,15 +30578,15 @@
 
         :param body: Is either a GetPower type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.GetPower or IO[bytes]
         :return: PowerDto
         :rtype: ~ignos.api.client.models.PowerDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28972,15 +30697,15 @@
         :param body: Is either a CustomerOrderConsumptionRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CustomerOrderConsumptionRequest or IO[bytes]
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29037,15 +30762,15 @@
 
         :param external_id: Required.
         :type external_id: str
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29087,15 +30812,15 @@
 
         :param external_id: Required.
         :type external_id: str
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29177,15 +30902,15 @@
         :param body: Is either a CreateCustomerOrderLineGhgReport type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateCustomerOrderLineGhgReport or IO[bytes]
         :return: DownloadDto
         :rtype: ~ignos.api.client.models.DownloadDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29261,15 +30986,15 @@
 
         :keyword asset_id: Default value is None.
         :paramtype asset_id: int
         :return: DataHealthDto
         :rtype: ~ignos.api.client.models.DataHealthDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29331,15 +31056,15 @@
 
         :param id: Required.
         :type id: str
         :return: TraceDto
         :rtype: ~ignos.api.client.models.TraceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29427,15 +31152,15 @@
         :type id: str
         :param body: Is either a UpdateTraceRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateTraceRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29488,15 +31213,15 @@
 
         :param id: Required.
         :type id: str
         :return: TraceDto
         :rtype: ~ignos.api.client.models.TraceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29540,15 +31265,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29576,29 +31301,140 @@
                 await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
+    @overload
+    async def set_trace_manual_completed(  # pylint: disable=inconsistent-return-statements
+        self,
+        id: str,
+        body: Optional[_models.UpdateTraceManualCompletionRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """set_trace_manual_completed.
+
+        :param id: Required.
+        :type id: str
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.UpdateTraceManualCompletionRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def set_trace_manual_completed(  # pylint: disable=inconsistent-return-statements
+        self, id: str, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """set_trace_manual_completed.
+
+        :param id: Required.
+        :type id: str
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def set_trace_manual_completed(  # pylint: disable=inconsistent-return-statements
+        self,
+        id: str,
+        body: Optional[Union[_models.UpdateTraceManualCompletionRequest, IO[bytes]]] = None,
+        **kwargs: Any
+    ) -> None:
+        """set_trace_manual_completed.
+
+        :param id: Required.
+        :type id: str
+        :param body: Is either a UpdateTraceManualCompletionRequest type or a IO[bytes] type. Default
+         value is None.
+        :type body: ~ignos.api.client.models.UpdateTraceManualCompletionRequest or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UpdateTraceManualCompletionRequest")
+            else:
+                _json = None
+
+        _request = build_trace_set_trace_manual_completed_request(
+            id=id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
     @distributed_trace_async
     async def list_customer_order_line_traces(
         self, *, customer_order: Optional[str] = None, customer_order_line: Optional[int] = None, **kwargs: Any
     ) -> List[_models.CustomerOrderLineTraceItemDto]:
         """list_customer_order_line_traces.
 
         :keyword customer_order: Default value is None.
         :paramtype customer_order: str
         :keyword customer_order_line: Default value is None.
         :paramtype customer_order_line: int
         :return: list of CustomerOrderLineTraceItemDto
         :rtype: list[~ignos.api.client.models.CustomerOrderLineTraceItemDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29645,15 +31481,15 @@
         :type id: str
         :keyword line: Default value is None.
         :paramtype line: int
         :return: CustomerOrderTraceStatusDto
         :rtype: ~ignos.api.client.models.CustomerOrderTraceStatusDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29720,15 +31556,15 @@
         :keyword continuation_token_parameter: Continuation token used for pagination. Default value is
          None.
         :paramtype continuation_token_parameter: str
         :return: TraceWorkOrderListDtoPagedResult
         :rtype: ~ignos.api.client.models.TraceWorkOrderListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29814,15 +31650,15 @@
         :param body: Is either a ListTraceWorkordersRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ListTraceWorkordersRequest or IO[bytes]
         :return: TraceWorkOrderListDtoPagedResult
         :rtype: ~ignos.api.client.models.TraceWorkOrderListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29869,14 +31705,484 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
 
+class TrackingOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.aio.IgnosPortal`'s
+        :attr:`tracking` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace_async
+    async def list_tracking_history(self, tracking_id: str, **kwargs: Any) -> _models.TrackingHistoryDto:
+        """list_tracking_history.
+
+        :param tracking_id: Required.
+        :type tracking_id: str
+        :return: TrackingHistoryDto
+        :rtype: ~ignos.api.client.models.TrackingHistoryDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.TrackingHistoryDto] = kwargs.pop("cls", None)
+
+        _request = build_tracking_list_tracking_history_request(
+            tracking_id=tracking_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("TrackingHistoryDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace_async
+    async def list_work_order_tracking_history(self, work_order_id: str, **kwargs: Any) -> _models.TrackingWorkOrderDto:
+        """list_work_order_tracking_history.
+
+        :param work_order_id: Required.
+        :type work_order_id: str
+        :return: TrackingWorkOrderDto
+        :rtype: ~ignos.api.client.models.TrackingWorkOrderDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.TrackingWorkOrderDto] = kwargs.pop("cls", None)
+
+        _request = build_tracking_list_work_order_tracking_history_request(
+            work_order_id=work_order_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("TrackingWorkOrderDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    async def create_tracking_events(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[List[_models.TrackingUpdateDto]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """create_tracking_events.
+
+        :param body: Default value is None.
+        :type body: list[~ignos.api.client.models.TrackingUpdateDto]
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_tracking_events(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_tracking_events.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_tracking_events(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[List[_models.TrackingUpdateDto], IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_tracking_events.
+
+        :param body: Is either a [TrackingUpdateDto] type or a IO[bytes] type. Default value is None.
+        :type body: list[~ignos.api.client.models.TrackingUpdateDto] or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "[TrackingUpdateDto]")
+            else:
+                _json = None
+
+        _request = build_tracking_create_tracking_events_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    async def create_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[List[_models.TrackingHistoryUpdateDto]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """create_tracking_history.
+
+        :param body: Default value is None.
+        :type body: list[~ignos.api.client.models.TrackingHistoryUpdateDto]
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_tracking_history.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[List[_models.TrackingHistoryUpdateDto], IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_tracking_history.
+
+        :param body: Is either a [TrackingHistoryUpdateDto] type or a IO[bytes] type. Default value is
+         None.
+        :type body: list[~ignos.api.client.models.TrackingHistoryUpdateDto] or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "[TrackingHistoryUpdateDto]")
+            else:
+                _json = None
+
+        _request = build_tracking_create_tracking_history_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    async def delete_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[List[_models.TrackingHistoryUpdateDto]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """delete_tracking_history.
+
+        :param body: Default value is None.
+        :type body: list[~ignos.api.client.models.TrackingHistoryUpdateDto]
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def delete_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """delete_tracking_history.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def delete_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[List[_models.TrackingHistoryUpdateDto], IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """delete_tracking_history.
+
+        :param body: Is either a [TrackingHistoryUpdateDto] type or a IO[bytes] type. Default value is
+         None.
+        :type body: list[~ignos.api.client.models.TrackingHistoryUpdateDto] or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "[TrackingHistoryUpdateDto]")
+            else:
+                _json = None
+
+        _request = build_tracking_delete_tracking_history_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @distributed_trace_async
+    async def create_label(  # pylint: disable=inconsistent-return-statements
+        self, work_order_id: str, *, pallet_count: Optional[int] = None, **kwargs: Any
+    ) -> None:
+        """create_label.
+
+        :param work_order_id: Required.
+        :type work_order_id: str
+        :keyword pallet_count: Default value is None.
+        :paramtype pallet_count: int
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        _request = build_tracking_create_label_request(
+            work_order_id=work_order_id,
+            pallet_count=pallet_count,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+
 class UploadOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.aio.IgnosPortal`'s
@@ -29896,15 +32202,15 @@
     async def create_upload_info(self, **kwargs: Any) -> _models.UploadInfoDto:
         """create_upload_info.
 
         :return: UploadInfoDto
         :rtype: ~ignos.api.client.models.UploadInfoDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29976,15 +32282,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: UserDtoPagedResult
         :rtype: ~ignos.api.client.models.UserDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30063,15 +32369,15 @@
 
         :param body: Is either a ListUsersRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListUsersRequest or IO[bytes]
         :return: UserDtoPagedResult
         :rtype: ~ignos.api.client.models.UserDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30145,15 +32451,15 @@
     async def get_my_workspaces(self, **kwargs: Any) -> List[_models.WorkspaceListDto]:
         """get_my_workspaces.
 
         :return: list of WorkspaceListDto
         :rtype: list[~ignos.api.client.models.WorkspaceListDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30229,15 +32535,15 @@
 
         :param body: Is either a CreateWorkspace type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateWorkspace or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30333,15 +32639,15 @@
         :param body: Is either a CreateWorkspaceFromTemplate type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateWorkspaceFromTemplate or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30397,15 +32703,15 @@
 
         :param id: Required.
         :type id: str
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30447,15 +32753,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30540,15 +32846,15 @@
         :param body: Is either a UpdateWorkspaceRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30652,15 +32958,15 @@
         :param body: Is either a UpdateWorkspaceWidgetsRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceWidgetsRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30781,15 +33087,15 @@
         :param body: Is either a UpdateWorkspaceWidgetSettingsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceWidgetSettingsRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30849,15 +33155,15 @@
         :type id: str
         :param widget_id: Required.
         :type widget_id: str
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30960,15 +33266,15 @@
         :param body: Is either a CreateWorkspaceTemplate type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateWorkspaceTemplate or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31024,15 +33330,15 @@
 
         :param id: Required.
         :type id: str
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31076,15 +33382,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31169,15 +33475,15 @@
         :param body: Is either a UpdateWorkspaceRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31281,15 +33587,15 @@
         :param body: Is either a UpdateWorkspaceWidgetsRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceWidgetsRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31410,15 +33716,15 @@
         :param body: Is either a UpdateWorkspaceWidgetSettingsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceWidgetSettingsRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31478,15 +33784,15 @@
         :type id: str
         :param widget_id: Required.
         :type widget_id: str
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31547,15 +33853,15 @@
     async def get_workspace_templates(self, **kwargs: Any) -> List[_models.WorkspaceListDto]:
         """get_workspace_templates.
 
         :return: list of WorkspaceListDto
         :rtype: list[~ignos.api.client.models.WorkspaceListDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/aio/operations/_patch.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/models/__init__.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 from ._models import AssetSimpleStructureDto
 from ._models import AssetStructureDto
 from ._models import AttachCalibrationCertificateRequest
 from ._models import AttachPdfRequest
 from ._models import AzureRegionDto
 from ._models import BatchInsertValueRequest
 from ._models import BatchInsertValuesResponseDto
+from ._models import BookingDeliveryUpdateDto
+from ._models import BookingItemRequestDto
+from ._models import BookingItemResponseDto
+from ._models import BookingRequestDto
+from ._models import BookingRequestListDto
+from ._models import BookingResponseDto
+from ._models import BookingResponseListDto
+from ._models import BookingUpdateDto
 from ._models import CalculateBarWeight
 from ._models import CalculateRightAngledTriangle
 from ._models import CalculateSpindleAndCuttingSpeed
 from ._models import CalibrationListToolDto
 from ._models import CamTransferDto
 from ._models import CdfConfigDto
 from ._models import CncMachineCommunicationSettingsDto
@@ -47,50 +55,53 @@
 from ._models import CompanyDto
 from ._models import CompanyUserDto
 from ._models import ComponentSettingsDto
 from ._models import ConsumptionDto
 from ._models import CopyCncMachineOperationDto
 from ._models import CopyCncMachineOperations
 from ._models import CopyCncPart
+from ._models import CopyToolsCncMachine
 from ._models import CountryDto
 from ._models import CreateAsset
 from ._models import CreateCncMachine
 from ._models import CreateCncMachineOperation
 from ._models import CreateCncMachineOperationToolRequest
 from ._models import CreateCncPart
 from ._models import CreateCompanyUserRequest
 from ._models import CreateCustomerMapping
 from ._models import CreateCustomerOrderLineGhgReport
 from ._models import CreateDocumentTypeRequest
 from ._models import CreateElectricalIotConfig
 from ._models import CreateLinkRequest
 from ._models import CreateMachineGroup
 from ._models import CreateMachineGroupResponse
+from ._models import CreateMachineWithoutResource
 from ._models import CreateMeasurementFormMapping
 from ._models import CreateMeasurementFormSchema
 from ._models import CreateMeasurementFormSchemaFeedbackRequest
 from ._models import CreateMeasurementFormSchemaLinkRequest
 from ._models import CreateMeasuringToolManufacturer
 from ._models import CreateMeasuringToolRequest
 from ._models import CreateMeasuringToolSubTypeRequest
 from ._models import CreateMeasuringToolType
 from ._models import CreateMeasuringUnit
 from ._models import CreateMrb
 from ._models import CreateMrbRevisionRequest
 from ._models import CreateMrbTemplateRequest
+from ._models import CreateResourceWithMachine
+from ._models import CreateResourceWithoutMachine
 from ._models import CreateSchemaElement
 from ._models import CreateSupplierInvite
 from ._models import CreateSupplierMapping
 from ._models import CreateWorkOrderMapping
 from ._models import CreateWorkspace
 from ._models import CreateWorkspaceFromTemplate
 from ._models import CreateWorkspaceTemplate
 from ._models import CurrentCustomerDto
 from ._models import CurrentWorkActivityDto
-from ._models import CurrentWorkActivityV2Dto
 from ._models import CurrentWorkDto
 from ._models import CustomerDto
 from ._models import CustomerDtoPagedResult
 from ._models import CustomerGroupDto
 from ._models import CustomerOrderConsumptionRequest
 from ._models import CustomerOrderDto
 from ._models import CustomerOrderDtoPagedResult
@@ -99,14 +110,15 @@
 from ._models import CustomerOrderLineTraceItemDto
 from ._models import CustomerOrderLineTraceStatusDto
 from ._models import CustomerOrderLineWorkOrderTraceStatusNodeDto
 from ._models import CustomerOrderTraceStatusDto
 from ._models import DataHealthDto
 from ._models import DeleteMrbTemplateRequest
 from ._models import DeletePartDrawingRequest
+from ._models import DepartmentDto
 from ._models import DeprecateToolRequest
 from ._models import DocumentGeneratorTypeDto
 from ._models import DocumentLinkDto
 from ._models import DocumentRevisionApprovalDto
 from ._models import DocumentTagDto
 from ._models import DocumentTypeDto
 from ._models import DocumentTypeRuleDto
@@ -163,14 +175,15 @@
 from ._models import ListMrbInstanceReportsRequest
 from ._models import ListOrderScheduleRequest
 from ._models import ListProductionScheduleOperationsRequest
 from ._models import ListProjectsRequest
 from ._models import ListTraceWorkordersRequest
 from ._models import ListUsersRequest
 from ._models import ListWorkOrdersRequest
+from ._models import LocationDto
 from ._models import Machine
 from ._models import MachineAlarmCountDto
 from ._models import MachineAlarmDetailsDto
 from ._models import MachineAlarmDto
 from ._models import MachineAlarmDtoPagedResult
 from ._models import MachineAlarmSeverityOccurenceDto
 from ._models import MachineAlarmSummaryDto
@@ -291,14 +304,15 @@
 from ._models import PowerOnUtilizationList
 from ._models import PowerOnUtilizationV2Dto
 from ._models import PowerRegionDto
 from ._models import ProblemDetails
 from ._models import ProductionCompanyDto
 from ._models import ProductionOrderBomDto
 from ._models import ProductionOrderDto
+from ._models import ProductionOrderOperationActivityDto
 from ._models import ProductionOrderOperationDto
 from ._models import ProductionResourceDto
 from ._models import ProductionScheduleFiltersDto
 from ._models import ProductionScheduleOperationDto
 from ._models import ProductionScheduleOperationDtoPagedResult
 from ._models import ProgramFileDto
 from ._models import RegisterMeasuringToolCalibrationRequest
@@ -315,24 +329,26 @@
 from ._models import SaveValueRequest
 from ._models import SaveValueResponseDto
 from ._models import ScheduledWorkSummaryDto
 from ._models import SchemaFeedbackCreatedDto
 from ._models import SchemaFeedbackDto
 from ._models import SchemaFeedbackDtoPagedResult
 from ._models import SchemaInstanceElementDto
+from ._models import SearchWorkOrderDto
 from ._models import SelectProductionCompany
 from ._models import SetIsBetaTesterRequest
 from ._models import SetMeasurementFormMappingBalloonsRequest
 from ._models import SetMeasurementFormNeedAsNotNeededRequest
 from ._models import SetMeasurementFormNeedUserRequest
 from ._models import SetMeasurementFormSchemaFeedbackUserRequest
 from ._models import SetTransferStatusRequest
 from ._models import SingleMachineErpDataListDto
 from ._models import SpindleAndCuttingSpeedDto
 from ._models import StartCamTransferToMachine
+from ._models import StartCamTransferToMachineFromTempUpload
 from ._models import StartOperationDto
 from ._models import StartOperations
 from ._models import StartWorkOperationRequest
 from ._models import StateDto
 from ._models import StopWorkOperationRequest
 from ._models import StoppedWorkDto
 from ._models import SubscribeToMachineInactivityAlerts
@@ -346,14 +362,19 @@
 from ._models import TraceDto
 from ._models import TraceItemConsumptionDto
 from ._models import TraceItemDto
 from ._models import TraceListItemDto
 from ._models import TraceMaterialDetailDto
 from ._models import TraceWorkOrderListDto
 from ._models import TraceWorkOrderListDtoPagedResult
+from ._models import TrackingEventDto
+from ._models import TrackingHistoryDto
+from ._models import TrackingHistoryUpdateDto
+from ._models import TrackingUpdateDto
+from ._models import TrackingWorkOrderDto
 from ._models import UnregisteredToolValueDto
 from ._models import UpdateAssetRequest
 from ._models import UpdateCdfConfig
 from ._models import UpdateCncMachineCommunicationSettingsRequest
 from ._models import UpdateCncMachineOperationRequest
 from ._models import UpdateCncMachineOperationToolRequest
 from ._models import UpdateCncMachineRequest
@@ -374,14 +395,15 @@
 from ._models import UpdateMeasuringToolTypeRequest
 from ._models import UpdateMesLink
 from ._models import UpdateMrbTemplate
 from ._models import UpdateProgramFileRequest
 from ._models import UpdateSchemaGroupedElementDto
 from ._models import UpdateSchemaGroupedElementsRequest
 from ._models import UpdateSchemaInstanceElementsRequest
+from ._models import UpdateTraceManualCompletionRequest
 from ._models import UpdateTraceRequest
 from ._models import UpdateWhitelistedMeasuringTool
 from ._models import UpdateWorkorderOperationEventTimestamps
 from ._models import UpdateWorkspaceRequest
 from ._models import UpdateWorkspaceWidgetSettingsRequest
 from ._models import UpdateWorkspaceWidgetsRequest
 from ._models import UploadCamFileDto
@@ -409,16 +431,17 @@
 from ._models import UserDtoPagedResult
 from ._models import UtilizationDetailsDto
 from ._models import UtilizationDto
 from ._models import UtilizationListDto
 from ._models import UtilizationSummaryDto
 from ._models import UtilizationWorkorderDto
 from ._models import ValidationRuleDto
+from ._models import WarehouseLocationDto
 from ._models import WhitelistMeasuringTool
-from ._models import WorkActivityDto
+from ._models import WorkOrderAttachmentDto
 from ._models import WorkOrderConsumptionDto
 from ._models import WorkOrderProjectDto
 from ._models import WorkOrderProjectDtoPagedResult
 from ._models import WorkOrderTraceItemDto
 from ._models import WorkOrderTraceMaterialDto
 from ._models import WorkOrderTraceOperationDto
 from ._models import WorkerDto
@@ -435,14 +458,15 @@
 from ._models import WorkspaceDto
 from ._models import WorkspaceListDto
 from ._models import WorkspaceWidgetBreakpointDto
 from ._models import WorkspaceWidgetDto
 
 from ._enums import AlertNotificationAccessStatusDto
 from ._enums import BonusType
+from ._enums import BookingTypeDto
 from ._enums import CalibrationListStatus
 from ._enums import CalibrationStatusDto
 from ._enums import CncFilterDeletedDto
 from ._enums import CncOperationStatus
 from ._enums import CustomerOrderLineStatus
 from ._enums import CustomerOrderStatus
 from ._enums import DocumentMetadataRequirement
@@ -455,14 +479,15 @@
 from ._enums import DocumentTypeSearchOption
 from ._enums import DocumentWorkflowType
 from ._enums import EmptyChapterStrategy
 from ._enums import ErrorCauseDto
 from ._enums import ExternalServiceName
 from ._enums import FileTransferDirection
 from ._enums import FileTransferStatus
+from ._enums import LocationKindDto
 from ._enums import MachineAlarmType
 from ._enums import MachineState
 from ._enums import MaterialPickStatus
 from ._enums import MaterialStatus
 from ._enums import MaterialStatusDto
 from ._enums import MeasurementFormInstanceStatus
 from ._enums import MeasurementFormSource
@@ -479,15 +504,17 @@
 from ._enums import NotificationChannelDto
 from ._enums import OperationStatusDto
 from ._enums import OrderReferenceTypeDto
 from ._enums import SchemaFeedbackStatus
 from ._enums import SearchTypeDto
 from ._enums import TraceIncludeStatus
 from ._enums import TraceItemStatus
+from ._enums import TraceStatus
 from ._enums import TraceType
+from ._enums import TrackingStatusDto
 from ._enums import UploadStatusDto
 from ._enums import WorkTypeDto
 from ._enums import WorkorderStatus
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
@@ -505,14 +532,22 @@
     "AssetSimpleStructureDto",
     "AssetStructureDto",
     "AttachCalibrationCertificateRequest",
     "AttachPdfRequest",
     "AzureRegionDto",
     "BatchInsertValueRequest",
     "BatchInsertValuesResponseDto",
+    "BookingDeliveryUpdateDto",
+    "BookingItemRequestDto",
+    "BookingItemResponseDto",
+    "BookingRequestDto",
+    "BookingRequestListDto",
+    "BookingResponseDto",
+    "BookingResponseListDto",
+    "BookingUpdateDto",
     "CalculateBarWeight",
     "CalculateRightAngledTriangle",
     "CalculateSpindleAndCuttingSpeed",
     "CalibrationListToolDto",
     "CamTransferDto",
     "CdfConfigDto",
     "CncMachineCommunicationSettingsDto",
@@ -533,50 +568,53 @@
     "CompanyDto",
     "CompanyUserDto",
     "ComponentSettingsDto",
     "ConsumptionDto",
     "CopyCncMachineOperationDto",
     "CopyCncMachineOperations",
     "CopyCncPart",
+    "CopyToolsCncMachine",
     "CountryDto",
     "CreateAsset",
     "CreateCncMachine",
     "CreateCncMachineOperation",
     "CreateCncMachineOperationToolRequest",
     "CreateCncPart",
     "CreateCompanyUserRequest",
     "CreateCustomerMapping",
     "CreateCustomerOrderLineGhgReport",
     "CreateDocumentTypeRequest",
     "CreateElectricalIotConfig",
     "CreateLinkRequest",
     "CreateMachineGroup",
     "CreateMachineGroupResponse",
+    "CreateMachineWithoutResource",
     "CreateMeasurementFormMapping",
     "CreateMeasurementFormSchema",
     "CreateMeasurementFormSchemaFeedbackRequest",
     "CreateMeasurementFormSchemaLinkRequest",
     "CreateMeasuringToolManufacturer",
     "CreateMeasuringToolRequest",
     "CreateMeasuringToolSubTypeRequest",
     "CreateMeasuringToolType",
     "CreateMeasuringUnit",
     "CreateMrb",
     "CreateMrbRevisionRequest",
     "CreateMrbTemplateRequest",
+    "CreateResourceWithMachine",
+    "CreateResourceWithoutMachine",
     "CreateSchemaElement",
     "CreateSupplierInvite",
     "CreateSupplierMapping",
     "CreateWorkOrderMapping",
     "CreateWorkspace",
     "CreateWorkspaceFromTemplate",
     "CreateWorkspaceTemplate",
     "CurrentCustomerDto",
     "CurrentWorkActivityDto",
-    "CurrentWorkActivityV2Dto",
     "CurrentWorkDto",
     "CustomerDto",
     "CustomerDtoPagedResult",
     "CustomerGroupDto",
     "CustomerOrderConsumptionRequest",
     "CustomerOrderDto",
     "CustomerOrderDtoPagedResult",
@@ -585,14 +623,15 @@
     "CustomerOrderLineTraceItemDto",
     "CustomerOrderLineTraceStatusDto",
     "CustomerOrderLineWorkOrderTraceStatusNodeDto",
     "CustomerOrderTraceStatusDto",
     "DataHealthDto",
     "DeleteMrbTemplateRequest",
     "DeletePartDrawingRequest",
+    "DepartmentDto",
     "DeprecateToolRequest",
     "DocumentGeneratorTypeDto",
     "DocumentLinkDto",
     "DocumentRevisionApprovalDto",
     "DocumentTagDto",
     "DocumentTypeDto",
     "DocumentTypeRuleDto",
@@ -649,14 +688,15 @@
     "ListMrbInstanceReportsRequest",
     "ListOrderScheduleRequest",
     "ListProductionScheduleOperationsRequest",
     "ListProjectsRequest",
     "ListTraceWorkordersRequest",
     "ListUsersRequest",
     "ListWorkOrdersRequest",
+    "LocationDto",
     "Machine",
     "MachineAlarmCountDto",
     "MachineAlarmDetailsDto",
     "MachineAlarmDto",
     "MachineAlarmDtoPagedResult",
     "MachineAlarmSeverityOccurenceDto",
     "MachineAlarmSummaryDto",
@@ -777,14 +817,15 @@
     "PowerOnUtilizationList",
     "PowerOnUtilizationV2Dto",
     "PowerRegionDto",
     "ProblemDetails",
     "ProductionCompanyDto",
     "ProductionOrderBomDto",
     "ProductionOrderDto",
+    "ProductionOrderOperationActivityDto",
     "ProductionOrderOperationDto",
     "ProductionResourceDto",
     "ProductionScheduleFiltersDto",
     "ProductionScheduleOperationDto",
     "ProductionScheduleOperationDtoPagedResult",
     "ProgramFileDto",
     "RegisterMeasuringToolCalibrationRequest",
@@ -801,24 +842,26 @@
     "SaveValueRequest",
     "SaveValueResponseDto",
     "ScheduledWorkSummaryDto",
     "SchemaFeedbackCreatedDto",
     "SchemaFeedbackDto",
     "SchemaFeedbackDtoPagedResult",
     "SchemaInstanceElementDto",
+    "SearchWorkOrderDto",
     "SelectProductionCompany",
     "SetIsBetaTesterRequest",
     "SetMeasurementFormMappingBalloonsRequest",
     "SetMeasurementFormNeedAsNotNeededRequest",
     "SetMeasurementFormNeedUserRequest",
     "SetMeasurementFormSchemaFeedbackUserRequest",
     "SetTransferStatusRequest",
     "SingleMachineErpDataListDto",
     "SpindleAndCuttingSpeedDto",
     "StartCamTransferToMachine",
+    "StartCamTransferToMachineFromTempUpload",
     "StartOperationDto",
     "StartOperations",
     "StartWorkOperationRequest",
     "StateDto",
     "StopWorkOperationRequest",
     "StoppedWorkDto",
     "SubscribeToMachineInactivityAlerts",
@@ -832,14 +875,19 @@
     "TraceDto",
     "TraceItemConsumptionDto",
     "TraceItemDto",
     "TraceListItemDto",
     "TraceMaterialDetailDto",
     "TraceWorkOrderListDto",
     "TraceWorkOrderListDtoPagedResult",
+    "TrackingEventDto",
+    "TrackingHistoryDto",
+    "TrackingHistoryUpdateDto",
+    "TrackingUpdateDto",
+    "TrackingWorkOrderDto",
     "UnregisteredToolValueDto",
     "UpdateAssetRequest",
     "UpdateCdfConfig",
     "UpdateCncMachineCommunicationSettingsRequest",
     "UpdateCncMachineOperationRequest",
     "UpdateCncMachineOperationToolRequest",
     "UpdateCncMachineRequest",
@@ -860,14 +908,15 @@
     "UpdateMeasuringToolTypeRequest",
     "UpdateMesLink",
     "UpdateMrbTemplate",
     "UpdateProgramFileRequest",
     "UpdateSchemaGroupedElementDto",
     "UpdateSchemaGroupedElementsRequest",
     "UpdateSchemaInstanceElementsRequest",
+    "UpdateTraceManualCompletionRequest",
     "UpdateTraceRequest",
     "UpdateWhitelistedMeasuringTool",
     "UpdateWorkorderOperationEventTimestamps",
     "UpdateWorkspaceRequest",
     "UpdateWorkspaceWidgetSettingsRequest",
     "UpdateWorkspaceWidgetsRequest",
     "UploadCamFileDto",
@@ -895,16 +944,17 @@
     "UserDtoPagedResult",
     "UtilizationDetailsDto",
     "UtilizationDto",
     "UtilizationListDto",
     "UtilizationSummaryDto",
     "UtilizationWorkorderDto",
     "ValidationRuleDto",
+    "WarehouseLocationDto",
     "WhitelistMeasuringTool",
-    "WorkActivityDto",
+    "WorkOrderAttachmentDto",
     "WorkOrderConsumptionDto",
     "WorkOrderProjectDto",
     "WorkOrderProjectDtoPagedResult",
     "WorkOrderTraceItemDto",
     "WorkOrderTraceMaterialDto",
     "WorkOrderTraceOperationDto",
     "WorkerDto",
@@ -920,14 +970,15 @@
     "WorkorderOperationEventDto",
     "WorkspaceDto",
     "WorkspaceListDto",
     "WorkspaceWidgetBreakpointDto",
     "WorkspaceWidgetDto",
     "AlertNotificationAccessStatusDto",
     "BonusType",
+    "BookingTypeDto",
     "CalibrationListStatus",
     "CalibrationStatusDto",
     "CncFilterDeletedDto",
     "CncOperationStatus",
     "CustomerOrderLineStatus",
     "CustomerOrderStatus",
     "DocumentMetadataRequirement",
@@ -940,14 +991,15 @@
     "DocumentTypeSearchOption",
     "DocumentWorkflowType",
     "EmptyChapterStrategy",
     "ErrorCauseDto",
     "ExternalServiceName",
     "FileTransferDirection",
     "FileTransferStatus",
+    "LocationKindDto",
     "MachineAlarmType",
     "MachineState",
     "MaterialPickStatus",
     "MaterialStatus",
     "MaterialStatusDto",
     "MeasurementFormInstanceStatus",
     "MeasurementFormSource",
@@ -964,14 +1016,16 @@
     "NotificationChannelDto",
     "OperationStatusDto",
     "OrderReferenceTypeDto",
     "SchemaFeedbackStatus",
     "SearchTypeDto",
     "TraceIncludeStatus",
     "TraceItemStatus",
+    "TraceStatus",
     "TraceType",
+    "TrackingStatusDto",
     "UploadStatusDto",
     "WorkTypeDto",
     "WorkorderStatus",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/models/_enums.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/models/_enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,22 @@
     """BonusType."""
 
     NONE = "None"
     POSITIVE = "Positive"
     POSITIVE_AND_NEGATIVE = "PositiveAndNegative"
 
 
+class BookingTypeDto(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """BookingTypeDto."""
+
+    NORMAL_TRUCK = "NormalTruck"
+    LARGE_TRUCK = "LargeTruck"
+    SIDE_LOADING_TRUCK = "SideLoadingTruck"
+
+
 class CalibrationListStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """CalibrationListStatus."""
 
     SOON_DUE = "SoonDue"
     EXPIRED = "Expired"
 
 
@@ -105,15 +113,14 @@
     CUSTOMER_ORDER_LINE = "CustomerOrderLine"
 
 
 class DocumentRuleType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """DocumentRuleType."""
 
     TAG = "Tag"
-    TITLE = "Title"
     SEQUENCES = "Sequences"
     ORDER_LINES = "OrderLines"
     LOT_NUMBERS = "LotNumbers"
 
 
 class DocumentSource(int, Enum, metaclass=CaseInsensitiveEnumMeta):
     """DocumentSource."""
@@ -198,14 +205,22 @@
     """FileTransferStatus."""
 
     IN_PROGRESS = "InProgress"
     SUCCESS = "Success"
     FAILED = "Failed"
 
 
+class LocationKindDto(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """LocationKindDto."""
+
+    WAREHOUSE = "Warehouse"
+    ZONE = "Zone"
+    LOCATION = "Location"
+
+
 class MachineAlarmType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """MachineAlarmType."""
 
     FAULT = "Fault"
     WARNING = "Warning"
 
 
@@ -414,23 +429,43 @@
     """TraceItemStatus."""
 
     NONE = "None"
     OK = "OK"
     SCRAP = "Scrap"
 
 
+class TraceStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """TraceStatus."""
+
+    NONE = "None"
+    UNAVAILABLE = "Unavailable"
+    NOT_NEEDED = "NotNeeded"
+    PARTIAL = "Partial"
+    COMPLETED = "Completed"
+
+
 class TraceType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """TraceType."""
 
     NONE = "None"
     LOT = "Lot"
     BATCH = "Batch"
     SERIAL_NUMBER = "SerialNumber"
 
 
+class TrackingStatusDto(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """TrackingStatusDto."""
+
+    MANUAL = "Manual"
+    BOOKING_PENDING = "BookingPending"
+    BOOKING_CANCELLED = "BookingCancelled"
+    BOOKING_IN_PROGRESS = "BookingInProgress"
+    BOOKING_COMPLETE = "BookingComplete"
+
+
 class UploadStatusDto(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """UploadStatusDto."""
 
     NOT_UPLOADED = "NotUploaded"
     AVAILABLE = "Available"
     DELETED = "Deleted"
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/models/_models.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/models/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -858,14 +858,314 @@
         :paramtype tool_warning: str
         """
         super().__init__(**kwargs)
         self.element_with_values = element_with_values
         self.tool_warning = tool_warning
 
 
+class BookingDeliveryUpdateDto(_serialization.Model):
+    """BookingDeliveryUpdateDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar booking_id: Required.
+    :vartype booking_id: str
+    :ivar to_location_id:
+    :vartype to_location_id: str
+    :ivar comment:
+    :vartype comment: str
+    """
+
+    _validation = {
+        "booking_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "booking_id": {"key": "bookingId", "type": "str"},
+        "to_location_id": {"key": "toLocationId", "type": "str"},
+        "comment": {"key": "comment", "type": "str"},
+    }
+
+    def __init__(
+        self, *, booking_id: str, to_location_id: Optional[str] = None, comment: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword booking_id: Required.
+        :paramtype booking_id: str
+        :keyword to_location_id:
+        :paramtype to_location_id: str
+        :keyword comment:
+        :paramtype comment: str
+        """
+        super().__init__(**kwargs)
+        self.booking_id = booking_id
+        self.to_location_id = to_location_id
+        self.comment = comment
+
+
+class BookingItemRequestDto(_serialization.Model):
+    """BookingItemRequestDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar tracking_id: Required.
+    :vartype tracking_id: str
+    """
+
+    _validation = {
+        "tracking_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "tracking_id": {"key": "trackingId", "type": "str"},
+    }
+
+    def __init__(self, *, tracking_id: str, **kwargs: Any) -> None:
+        """
+        :keyword tracking_id: Required.
+        :paramtype tracking_id: str
+        """
+        super().__init__(**kwargs)
+        self.tracking_id = tracking_id
+
+
+class BookingItemResponseDto(_serialization.Model):
+    """BookingItemResponseDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar tracking_id: Required.
+    :vartype tracking_id: str
+    """
+
+    _validation = {
+        "tracking_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "tracking_id": {"key": "trackingId", "type": "str"},
+    }
+
+    def __init__(self, *, tracking_id: str, **kwargs: Any) -> None:
+        """
+        :keyword tracking_id: Required.
+        :paramtype tracking_id: str
+        """
+        super().__init__(**kwargs)
+        self.tracking_id = tracking_id
+
+
+class BookingRequestDto(_serialization.Model):
+    """BookingRequestDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar booking_type: Required. Known values are: "NormalTruck", "LargeTruck", and
+     "SideLoadingTruck".
+    :vartype booking_type: str or ~ignos.api.client.models.BookingTypeDto
+    :ivar items: Required.
+    :vartype items: list[~ignos.api.client.models.BookingItemRequestDto]
+    :ivar from_location_id: Required.
+    :vartype from_location_id: str
+    :ivar to_location_id: Required.
+    :vartype to_location_id: str
+    """
+
+    _validation = {
+        "booking_type": {"required": True},
+        "items": {"required": True},
+        "from_location_id": {"required": True, "min_length": 1},
+        "to_location_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "booking_type": {"key": "bookingType", "type": "str"},
+        "items": {"key": "items", "type": "[BookingItemRequestDto]"},
+        "from_location_id": {"key": "fromLocationId", "type": "str"},
+        "to_location_id": {"key": "toLocationId", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        booking_type: Union[str, "_models.BookingTypeDto"],
+        items: List["_models.BookingItemRequestDto"],
+        from_location_id: str,
+        to_location_id: str,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword booking_type: Required. Known values are: "NormalTruck", "LargeTruck", and
+         "SideLoadingTruck".
+        :paramtype booking_type: str or ~ignos.api.client.models.BookingTypeDto
+        :keyword items: Required.
+        :paramtype items: list[~ignos.api.client.models.BookingItemRequestDto]
+        :keyword from_location_id: Required.
+        :paramtype from_location_id: str
+        :keyword to_location_id: Required.
+        :paramtype to_location_id: str
+        """
+        super().__init__(**kwargs)
+        self.booking_type = booking_type
+        self.items = items
+        self.from_location_id = from_location_id
+        self.to_location_id = to_location_id
+
+
+class BookingRequestListDto(_serialization.Model):
+    """BookingRequestListDto.
+
+    :ivar continuation_token:
+    :vartype continuation_token: str
+    """
+
+    _attribute_map = {
+        "continuation_token": {"key": "continuationToken", "type": "str"},
+    }
+
+    def __init__(self, *, continuation_token: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword continuation_token:
+        :paramtype continuation_token: str
+        """
+        super().__init__(**kwargs)
+        self.continuation_token = continuation_token
+
+
+class BookingResponseDto(_serialization.Model):
+    """BookingResponseDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar booking_id: Required.
+    :vartype booking_id: str
+    :ivar booking_type: Required. Known values are: "NormalTruck", "LargeTruck", and
+     "SideLoadingTruck".
+    :vartype booking_type: str or ~ignos.api.client.models.BookingTypeDto
+    :ivar items: Required.
+    :vartype items: list[~ignos.api.client.models.BookingItemResponseDto]
+    :ivar from_location_id: Required.
+    :vartype from_location_id: str
+    :ivar to_location_id: Required.
+    :vartype to_location_id: str
+    """
+
+    _validation = {
+        "booking_id": {"required": True, "min_length": 1},
+        "booking_type": {"required": True},
+        "items": {"required": True},
+        "from_location_id": {"required": True, "min_length": 1},
+        "to_location_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "booking_id": {"key": "bookingId", "type": "str"},
+        "booking_type": {"key": "bookingType", "type": "str"},
+        "items": {"key": "items", "type": "[BookingItemResponseDto]"},
+        "from_location_id": {"key": "fromLocationId", "type": "str"},
+        "to_location_id": {"key": "toLocationId", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        booking_id: str,
+        booking_type: Union[str, "_models.BookingTypeDto"],
+        items: List["_models.BookingItemResponseDto"],
+        from_location_id: str,
+        to_location_id: str,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword booking_id: Required.
+        :paramtype booking_id: str
+        :keyword booking_type: Required. Known values are: "NormalTruck", "LargeTruck", and
+         "SideLoadingTruck".
+        :paramtype booking_type: str or ~ignos.api.client.models.BookingTypeDto
+        :keyword items: Required.
+        :paramtype items: list[~ignos.api.client.models.BookingItemResponseDto]
+        :keyword from_location_id: Required.
+        :paramtype from_location_id: str
+        :keyword to_location_id: Required.
+        :paramtype to_location_id: str
+        """
+        super().__init__(**kwargs)
+        self.booking_id = booking_id
+        self.booking_type = booking_type
+        self.items = items
+        self.from_location_id = from_location_id
+        self.to_location_id = to_location_id
+
+
+class BookingResponseListDto(_serialization.Model):
+    """BookingResponseListDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar results: Required.
+    :vartype results: list[~ignos.api.client.models.BookingResponseDto]
+    :ivar continuation_token:
+    :vartype continuation_token: str
+    """
+
+    _validation = {
+        "results": {"required": True},
+    }
+
+    _attribute_map = {
+        "results": {"key": "results", "type": "[BookingResponseDto]"},
+        "continuation_token": {"key": "continuationToken", "type": "str"},
+    }
+
+    def __init__(
+        self, *, results: List["_models.BookingResponseDto"], continuation_token: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword results: Required.
+        :paramtype results: list[~ignos.api.client.models.BookingResponseDto]
+        :keyword continuation_token:
+        :paramtype continuation_token: str
+        """
+        super().__init__(**kwargs)
+        self.results = results
+        self.continuation_token = continuation_token
+
+
+class BookingUpdateDto(_serialization.Model):
+    """BookingUpdateDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar booking_id: Required.
+    :vartype booking_id: str
+    :ivar comment:
+    :vartype comment: str
+    """
+
+    _validation = {
+        "booking_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "booking_id": {"key": "bookingId", "type": "str"},
+        "comment": {"key": "comment", "type": "str"},
+    }
+
+    def __init__(self, *, booking_id: str, comment: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword booking_id: Required.
+        :paramtype booking_id: str
+        :keyword comment:
+        :paramtype comment: str
+        """
+        super().__init__(**kwargs)
+        self.booking_id = booking_id
+        self.comment = comment
+
+
 class CalculateBarWeight(_serialization.Model):
     """CalculateBarWeight.
 
     :ivar inner_diameter:
     :vartype inner_diameter: float
     :ivar outer_diameter:
     :vartype outer_diameter: float
@@ -2129,14 +2429,16 @@
     :vartype size: str
     :ivar diameter:
     :vartype diameter: float
     :ivar grade:
     :vartype grade: str
     :ivar radius:
     :vartype radius: float
+    :ivar chamfer:
+    :vartype chamfer: float
     :ivar width:
     :vartype width: float
     :ivar pitch:
     :vartype pitch: str
     :ivar length:
     :vartype length: float
     :ivar kapr:
@@ -2174,14 +2476,15 @@
         "description": {"key": "description", "type": "str"},
         "holder_description": {"key": "holderDescription", "type": "str"},
         "geometry": {"key": "geometry", "type": "str"},
         "size": {"key": "size", "type": "str"},
         "diameter": {"key": "diameter", "type": "float"},
         "grade": {"key": "grade", "type": "str"},
         "radius": {"key": "radius", "type": "float"},
+        "chamfer": {"key": "chamfer", "type": "float"},
         "width": {"key": "width", "type": "float"},
         "pitch": {"key": "pitch", "type": "str"},
         "length": {"key": "length", "type": "float"},
         "kapr": {"key": "kapr", "type": "float"},
         "teeth": {"key": "teeth", "type": "int"},
         "stick_out": {"key": "stickOut", "type": "float"},
         "apmx": {"key": "apmx", "type": "float"},
@@ -2203,14 +2506,15 @@
         description: Optional[str] = None,
         holder_description: Optional[str] = None,
         geometry: Optional[str] = None,
         size: Optional[str] = None,
         diameter: Optional[float] = None,
         grade: Optional[str] = None,
         radius: Optional[float] = None,
+        chamfer: Optional[float] = None,
         width: Optional[float] = None,
         pitch: Optional[str] = None,
         length: Optional[float] = None,
         kapr: Optional[float] = None,
         teeth: Optional[int] = None,
         stick_out: Optional[float] = None,
         apmx: Optional[float] = None,
@@ -2244,14 +2548,16 @@
         :paramtype size: str
         :keyword diameter:
         :paramtype diameter: float
         :keyword grade:
         :paramtype grade: str
         :keyword radius:
         :paramtype radius: float
+        :keyword chamfer:
+        :paramtype chamfer: float
         :keyword width:
         :paramtype width: float
         :keyword pitch:
         :paramtype pitch: str
         :keyword length:
         :paramtype length: float
         :keyword kapr:
@@ -2280,14 +2586,15 @@
         self.description = description
         self.holder_description = holder_description
         self.geometry = geometry
         self.size = size
         self.diameter = diameter
         self.grade = grade
         self.radius = radius
+        self.chamfer = chamfer
         self.width = width
         self.pitch = pitch
         self.length = length
         self.kapr = kapr
         self.teeth = teeth
         self.stick_out = stick_out
         self.apmx = apmx
@@ -2327,14 +2634,18 @@
     :vartype grade: bool
     :ivar grade_helper_text: Required.
     :vartype grade_helper_text: str
     :ivar radius: Required.
     :vartype radius: bool
     :ivar radius_helper_text: Required.
     :vartype radius_helper_text: str
+    :ivar chamfer: Required.
+    :vartype chamfer: bool
+    :ivar chamfer_helper_text: Required.
+    :vartype chamfer_helper_text: str
     :ivar width: Required.
     :vartype width: bool
     :ivar width_helper_text: Required.
     :vartype width_helper_text: str
     :ivar pitch: Required.
     :vartype pitch: bool
     :ivar pitch_helper_text: Required.
@@ -2380,14 +2691,16 @@
         "size_helper_text": {"required": True, "min_length": 1},
         "diameter": {"required": True},
         "diameter_helper_text": {"required": True, "min_length": 1},
         "grade": {"required": True},
         "grade_helper_text": {"required": True, "min_length": 1},
         "radius": {"required": True},
         "radius_helper_text": {"required": True, "min_length": 1},
+        "chamfer": {"required": True},
+        "chamfer_helper_text": {"required": True, "min_length": 1},
         "width": {"required": True},
         "width_helper_text": {"required": True, "min_length": 1},
         "pitch": {"required": True},
         "pitch_helper_text": {"required": True, "min_length": 1},
         "length": {"required": True},
         "length_helper_text": {"required": True, "min_length": 1},
         "kapr": {"required": True},
@@ -2416,14 +2729,16 @@
         "size_helper_text": {"key": "sizeHelperText", "type": "str"},
         "diameter": {"key": "diameter", "type": "bool"},
         "diameter_helper_text": {"key": "diameterHelperText", "type": "str"},
         "grade": {"key": "grade", "type": "bool"},
         "grade_helper_text": {"key": "gradeHelperText", "type": "str"},
         "radius": {"key": "radius", "type": "bool"},
         "radius_helper_text": {"key": "radiusHelperText", "type": "str"},
+        "chamfer": {"key": "chamfer", "type": "bool"},
+        "chamfer_helper_text": {"key": "chamferHelperText", "type": "str"},
         "width": {"key": "width", "type": "bool"},
         "width_helper_text": {"key": "widthHelperText", "type": "str"},
         "pitch": {"key": "pitch", "type": "bool"},
         "pitch_helper_text": {"key": "pitchHelperText", "type": "str"},
         "length": {"key": "length", "type": "bool"},
         "length_helper_text": {"key": "lengthHelperText", "type": "str"},
         "kapr": {"key": "kapr", "type": "bool"},
@@ -2453,14 +2768,16 @@
         size_helper_text: str,
         diameter: bool,
         diameter_helper_text: str,
         grade: bool,
         grade_helper_text: str,
         radius: bool,
         radius_helper_text: str,
+        chamfer: bool,
+        chamfer_helper_text: str,
         width: bool,
         width_helper_text: str,
         pitch: bool,
         pitch_helper_text: str,
         length: bool,
         length_helper_text: str,
         kapr: bool,
@@ -2505,14 +2822,18 @@
         :paramtype grade: bool
         :keyword grade_helper_text: Required.
         :paramtype grade_helper_text: str
         :keyword radius: Required.
         :paramtype radius: bool
         :keyword radius_helper_text: Required.
         :paramtype radius_helper_text: str
+        :keyword chamfer: Required.
+        :paramtype chamfer: bool
+        :keyword chamfer_helper_text: Required.
+        :paramtype chamfer_helper_text: str
         :keyword width: Required.
         :paramtype width: bool
         :keyword width_helper_text: Required.
         :paramtype width_helper_text: str
         :keyword pitch: Required.
         :paramtype pitch: bool
         :keyword pitch_helper_text: Required.
@@ -2558,14 +2879,16 @@
         self.size_helper_text = size_helper_text
         self.diameter = diameter
         self.diameter_helper_text = diameter_helper_text
         self.grade = grade
         self.grade_helper_text = grade_helper_text
         self.radius = radius
         self.radius_helper_text = radius_helper_text
+        self.chamfer = chamfer
+        self.chamfer_helper_text = chamfer_helper_text
         self.width = width
         self.width_helper_text = width_helper_text
         self.pitch = pitch
         self.pitch_helper_text = pitch_helper_text
         self.length = length
         self.length_helper_text = length_helper_text
         self.kapr = kapr
@@ -3077,14 +3400,56 @@
         self.part_name = part_name
         self.drawing = drawing
         self.drawing_revision = drawing_revision
         self.material = material
         self.description = description
 
 
+class CopyToolsCncMachine(_serialization.Model):
+    """CopyToolsCncMachine.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar source_machine_id: Required.
+    :vartype source_machine_id: str
+    :ivar target_operation_id: Required.
+    :vartype target_operation_id: str
+    :ivar tools_ids: Required.
+    :vartype tools_ids: list[int]
+    """
+
+    _validation = {
+        "source_machine_id": {"required": True, "min_length": 1},
+        "target_operation_id": {"required": True, "min_length": 1},
+        "tools_ids": {"required": True},
+    }
+
+    _attribute_map = {
+        "source_machine_id": {"key": "sourceMachineId", "type": "str"},
+        "target_operation_id": {"key": "targetOperationId", "type": "str"},
+        "tools_ids": {"key": "toolsIds", "type": "[int]"},
+    }
+
+    def __init__(
+        self, *, source_machine_id: str, target_operation_id: str, tools_ids: List[int], **kwargs: Any
+    ) -> None:
+        """
+        :keyword source_machine_id: Required.
+        :paramtype source_machine_id: str
+        :keyword target_operation_id: Required.
+        :paramtype target_operation_id: str
+        :keyword tools_ids: Required.
+        :paramtype tools_ids: list[int]
+        """
+        super().__init__(**kwargs)
+        self.source_machine_id = source_machine_id
+        self.target_operation_id = target_operation_id
+        self.tools_ids = tools_ids
+
+
 class CountryDto(_serialization.Model):
     """CountryDto.
 
     All required parameters must be populated in order to send to server.
 
     :ivar two_letter_iso_region_name: Required.
     :vartype two_letter_iso_region_name: str
@@ -3343,14 +3708,16 @@
     :vartype size: str
     :ivar diameter:
     :vartype diameter: float
     :ivar grade:
     :vartype grade: str
     :ivar radius:
     :vartype radius: float
+    :ivar chamfer:
+    :vartype chamfer: float
     :ivar width:
     :vartype width: float
     :ivar pitch:
     :vartype pitch: str
     :ivar length:
     :vartype length: float
     :ivar kapr:
@@ -3378,14 +3745,15 @@
         "description": {"key": "description", "type": "str"},
         "holder_description": {"key": "holderDescription", "type": "str"},
         "geometry": {"key": "geometry", "type": "str"},
         "size": {"key": "size", "type": "str"},
         "diameter": {"key": "diameter", "type": "float"},
         "grade": {"key": "grade", "type": "str"},
         "radius": {"key": "radius", "type": "float"},
+        "chamfer": {"key": "chamfer", "type": "float"},
         "width": {"key": "width", "type": "float"},
         "pitch": {"key": "pitch", "type": "str"},
         "length": {"key": "length", "type": "float"},
         "kapr": {"key": "kapr", "type": "float"},
         "teeth": {"key": "teeth", "type": "int"},
         "stick_out": {"key": "stickOut", "type": "float"},
         "apmx": {"key": "apmx", "type": "float"},
@@ -3402,14 +3770,15 @@
         description: Optional[str] = None,
         holder_description: Optional[str] = None,
         geometry: Optional[str] = None,
         size: Optional[str] = None,
         diameter: Optional[float] = None,
         grade: Optional[str] = None,
         radius: Optional[float] = None,
+        chamfer: Optional[float] = None,
         width: Optional[float] = None,
         pitch: Optional[str] = None,
         length: Optional[float] = None,
         kapr: Optional[float] = None,
         teeth: Optional[int] = None,
         stick_out: Optional[float] = None,
         apmx: Optional[float] = None,
@@ -3435,14 +3804,16 @@
         :paramtype size: str
         :keyword diameter:
         :paramtype diameter: float
         :keyword grade:
         :paramtype grade: str
         :keyword radius:
         :paramtype radius: float
+        :keyword chamfer:
+        :paramtype chamfer: float
         :keyword width:
         :paramtype width: float
         :keyword pitch:
         :paramtype pitch: str
         :keyword length:
         :paramtype length: float
         :keyword kapr:
@@ -3464,14 +3835,15 @@
         self.description = description
         self.holder_description = holder_description
         self.geometry = geometry
         self.size = size
         self.diameter = diameter
         self.grade = grade
         self.radius = radius
+        self.chamfer = chamfer
         self.width = width
         self.pitch = pitch
         self.length = length
         self.kapr = kapr
         self.teeth = teeth
         self.stick_out = stick_out
         self.apmx = apmx
@@ -3970,14 +4342,110 @@
         :keyword id: Required.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
 
+class CreateMachineWithoutResource(_serialization.Model):
+    """CreateMachineWithoutResource.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar id: Required.
+    :vartype id: str
+    :ivar name: Required.
+    :vartype name: str
+    :ivar description:
+    :vartype description: str
+    :ivar type: Required.
+    :vartype type: str
+    :ivar display_name:
+    :vartype display_name: str
+    :ivar manufacturer:
+    :vartype manufacturer: str
+    :ivar location:
+    :vartype location: str
+    :ivar serial_number:
+    :vartype serial_number: str
+    :ivar year:
+    :vartype year: str
+    :ivar model:
+    :vartype model: str
+    """
+
+    _validation = {
+        "id": {"required": True, "min_length": 1},
+        "name": {"required": True, "min_length": 1},
+        "type": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "display_name": {"key": "displayName", "type": "str"},
+        "manufacturer": {"key": "manufacturer", "type": "str"},
+        "location": {"key": "location", "type": "str"},
+        "serial_number": {"key": "serialNumber", "type": "str"},
+        "year": {"key": "year", "type": "str"},
+        "model": {"key": "model", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: str,  # pylint: disable=redefined-builtin
+        name: str,
+        type: str,
+        description: Optional[str] = None,
+        display_name: Optional[str] = None,
+        manufacturer: Optional[str] = None,
+        location: Optional[str] = None,
+        serial_number: Optional[str] = None,
+        year: Optional[str] = None,
+        model: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id: Required.
+        :paramtype id: str
+        :keyword name: Required.
+        :paramtype name: str
+        :keyword description:
+        :paramtype description: str
+        :keyword type: Required.
+        :paramtype type: str
+        :keyword display_name:
+        :paramtype display_name: str
+        :keyword manufacturer:
+        :paramtype manufacturer: str
+        :keyword location:
+        :paramtype location: str
+        :keyword serial_number:
+        :paramtype serial_number: str
+        :keyword year:
+        :paramtype year: str
+        :keyword model:
+        :paramtype model: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.name = name
+        self.description = description
+        self.type = type
+        self.display_name = display_name
+        self.manufacturer = manufacturer
+        self.location = location
+        self.serial_number = serial_number
+        self.year = year
+        self.model = model
+
+
 class CreateMeasurementFormMapping(_serialization.Model):
     """CreateMeasurementFormMapping.
 
     All required parameters must be populated in order to send to server.
 
     :ivar source_id: Required.
     :vartype source_id: str
@@ -4188,14 +4656,16 @@
     :vartype default_location: str
     :ivar precision:
     :vartype precision: str
     :ivar upload_key:
     :vartype upload_key: str
     :ivar filename:
     :vartype filename: str
+    :ivar initial_calibration_date:
+    :vartype initial_calibration_date: ~datetime.datetime
     """
 
     _validation = {
         "name": {"required": True, "min_length": 1},
         "manufacturer": {"required": True, "min_length": 1},
         "type_id": {"required": True},
         "non_calibration_tool": {"required": True},
@@ -4213,14 +4683,15 @@
         "min": {"key": "min", "type": "float"},
         "max": {"key": "max", "type": "float"},
         "serial_number": {"key": "serialNumber", "type": "str"},
         "default_location": {"key": "defaultLocation", "type": "str"},
         "precision": {"key": "precision", "type": "str"},
         "upload_key": {"key": "uploadKey", "type": "str"},
         "filename": {"key": "filename", "type": "str"},
+        "initial_calibration_date": {"key": "initialCalibrationDate", "type": "iso-8601"},
     }
 
     def __init__(
         self,
         *,
         name: str,
         manufacturer: str,
@@ -4233,14 +4704,15 @@
         min: Optional[float] = None,  # pylint: disable=redefined-builtin
         max: Optional[float] = None,  # pylint: disable=redefined-builtin
         serial_number: Optional[str] = None,
         default_location: Optional[str] = None,
         precision: Optional[str] = None,
         upload_key: Optional[str] = None,
         filename: Optional[str] = None,
+        initial_calibration_date: Optional[datetime.datetime] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword tool_id:
         :paramtype tool_id: str
         :keyword name: Required.
         :paramtype name: str
@@ -4266,14 +4738,16 @@
         :paramtype default_location: str
         :keyword precision:
         :paramtype precision: str
         :keyword upload_key:
         :paramtype upload_key: str
         :keyword filename:
         :paramtype filename: str
+        :keyword initial_calibration_date:
+        :paramtype initial_calibration_date: ~datetime.datetime
         """
         super().__init__(**kwargs)
         self.tool_id = tool_id
         self.name = name
         self.manufacturer = manufacturer
         self.type_id = type_id
         self.sub_type_id = sub_type_id
@@ -4283,14 +4757,15 @@
         self.min = min
         self.max = max
         self.serial_number = serial_number
         self.default_location = default_location
         self.precision = precision
         self.upload_key = upload_key
         self.filename = filename
+        self.initial_calibration_date = initial_calibration_date
 
 
 class CreateMeasuringToolSubTypeRequest(_serialization.Model):
     """CreateMeasuringToolSubTypeRequest.
 
     All required parameters must be populated in order to send to server.
 
@@ -4571,14 +5046,194 @@
         self.customer_name = customer_name
         self.customer_group_id = customer_group_id
         self.customer_group_name = customer_group_name
         self.pdf_upload_key = pdf_upload_key
         self.pdf_filename = pdf_filename
 
 
+class CreateResourceWithMachine(_serialization.Model):  # pylint: disable=too-many-instance-attributes
+    """CreateResourceWithMachine.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar resource_id: Required.
+    :vartype resource_id: str
+    :ivar resource_name: Required.
+    :vartype resource_name: str
+    :ivar resource_description:
+    :vartype resource_description: str
+    :ivar display_name:
+    :vartype display_name: str
+    :ivar machine_id: Required.
+    :vartype machine_id: str
+    :ivar machine_name: Required.
+    :vartype machine_name: str
+    :ivar machine_description:
+    :vartype machine_description: str
+    :ivar machine_type: Required.
+    :vartype machine_type: str
+    :ivar manufacturer:
+    :vartype manufacturer: str
+    :ivar location:
+    :vartype location: str
+    :ivar serial_number:
+    :vartype serial_number: str
+    :ivar year:
+    :vartype year: str
+    :ivar model:
+    :vartype model: str
+    """
+
+    _validation = {
+        "resource_id": {"required": True, "min_length": 1},
+        "resource_name": {"required": True, "min_length": 1},
+        "machine_id": {"required": True, "min_length": 1},
+        "machine_name": {"required": True, "min_length": 1},
+        "machine_type": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "resource_id": {"key": "resourceId", "type": "str"},
+        "resource_name": {"key": "resourceName", "type": "str"},
+        "resource_description": {"key": "resourceDescription", "type": "str"},
+        "display_name": {"key": "displayName", "type": "str"},
+        "machine_id": {"key": "machineId", "type": "str"},
+        "machine_name": {"key": "machineName", "type": "str"},
+        "machine_description": {"key": "machineDescription", "type": "str"},
+        "machine_type": {"key": "machineType", "type": "str"},
+        "manufacturer": {"key": "manufacturer", "type": "str"},
+        "location": {"key": "location", "type": "str"},
+        "serial_number": {"key": "serialNumber", "type": "str"},
+        "year": {"key": "year", "type": "str"},
+        "model": {"key": "model", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        resource_id: str,
+        resource_name: str,
+        machine_id: str,
+        machine_name: str,
+        machine_type: str,
+        resource_description: Optional[str] = None,
+        display_name: Optional[str] = None,
+        machine_description: Optional[str] = None,
+        manufacturer: Optional[str] = None,
+        location: Optional[str] = None,
+        serial_number: Optional[str] = None,
+        year: Optional[str] = None,
+        model: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword resource_id: Required.
+        :paramtype resource_id: str
+        :keyword resource_name: Required.
+        :paramtype resource_name: str
+        :keyword resource_description:
+        :paramtype resource_description: str
+        :keyword display_name:
+        :paramtype display_name: str
+        :keyword machine_id: Required.
+        :paramtype machine_id: str
+        :keyword machine_name: Required.
+        :paramtype machine_name: str
+        :keyword machine_description:
+        :paramtype machine_description: str
+        :keyword machine_type: Required.
+        :paramtype machine_type: str
+        :keyword manufacturer:
+        :paramtype manufacturer: str
+        :keyword location:
+        :paramtype location: str
+        :keyword serial_number:
+        :paramtype serial_number: str
+        :keyword year:
+        :paramtype year: str
+        :keyword model:
+        :paramtype model: str
+        """
+        super().__init__(**kwargs)
+        self.resource_id = resource_id
+        self.resource_name = resource_name
+        self.resource_description = resource_description
+        self.display_name = display_name
+        self.machine_id = machine_id
+        self.machine_name = machine_name
+        self.machine_description = machine_description
+        self.machine_type = machine_type
+        self.manufacturer = manufacturer
+        self.location = location
+        self.serial_number = serial_number
+        self.year = year
+        self.model = model
+
+
+class CreateResourceWithoutMachine(_serialization.Model):
+    """CreateResourceWithoutMachine.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar id: Required.
+    :vartype id: str
+    :ivar name: Required.
+    :vartype name: str
+    :ivar type: Required.
+    :vartype type: str
+    :ivar description:
+    :vartype description: str
+    :ivar display_name:
+    :vartype display_name: str
+    """
+
+    _validation = {
+        "id": {"required": True, "min_length": 1},
+        "name": {"required": True, "min_length": 1},
+        "type": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "display_name": {"key": "displayName", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: str,  # pylint: disable=redefined-builtin
+        name: str,
+        type: str,
+        description: Optional[str] = None,
+        display_name: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id: Required.
+        :paramtype id: str
+        :keyword name: Required.
+        :paramtype name: str
+        :keyword type: Required.
+        :paramtype type: str
+        :keyword description:
+        :paramtype description: str
+        :keyword display_name:
+        :paramtype display_name: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.name = name
+        self.type = type
+        self.description = description
+        self.display_name = display_name
+
+
 class CreateSchemaElement(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """CreateSchemaElement.
 
     :ivar balloon_id:
     :vartype balloon_id: str
     :ivar section:
     :vartype section: str
@@ -5033,53 +5688,14 @@
 
 
 class CurrentWorkActivityDto(_serialization.Model):
     """CurrentWorkActivityDto.
 
     All required parameters must be populated in order to send to server.
 
-    :ivar work_activity: Required.
-    :vartype work_activity: ~ignos.api.client.models.WorkActivityDto
-    :ivar operation: Required.
-    :vartype operation: ~ignos.api.client.models.ProductionScheduleOperationDto
-    """
-
-    _validation = {
-        "work_activity": {"required": True},
-        "operation": {"required": True},
-    }
-
-    _attribute_map = {
-        "work_activity": {"key": "workActivity", "type": "WorkActivityDto"},
-        "operation": {"key": "operation", "type": "ProductionScheduleOperationDto"},
-    }
-
-    def __init__(
-        self,
-        *,
-        work_activity: "_models.WorkActivityDto",
-        operation: "_models.ProductionScheduleOperationDto",
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword work_activity: Required.
-        :paramtype work_activity: ~ignos.api.client.models.WorkActivityDto
-        :keyword operation: Required.
-        :paramtype operation: ~ignos.api.client.models.ProductionScheduleOperationDto
-        """
-        super().__init__(**kwargs)
-        self.work_activity = work_activity
-        self.operation = operation
-
-
-class CurrentWorkActivityV2Dto(_serialization.Model):
-    """CurrentWorkActivityV2Dto.
-
-    All required parameters must be populated in order to send to server.
-
     :ivar active_work: Required.
     :vartype active_work: list[~ignos.api.client.models.ActiveWorkDto]
     :ivar stopped_work: Required.
     :vartype stopped_work: list[~ignos.api.client.models.StoppedWorkDto]
     """
 
     _validation = {
@@ -5109,14 +5725,16 @@
 class CurrentWorkDto(_serialization.Model):
     """CurrentWorkDto.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to server.
 
+    :ivar resource_id: Required.
+    :vartype resource_id: str
     :ivar upn:
     :vartype upn: str
     :ivar personnel_number: Required.
     :vartype personnel_number: str
     :ivar active: Required.
     :vartype active: bool
     :ivar start_time: Required.
@@ -5128,38 +5746,44 @@
     :ivar started_quantity:
     :vartype started_quantity: int
     :ivar work_type: Required. Known values are: "None", "Production", and "Setup".
     :vartype work_type: str or ~ignos.api.client.models.WorkTypeDto
     """
 
     _validation = {
+        "resource_id": {"required": True, "min_length": 1},
         "upn": {"readonly": True},
         "personnel_number": {"required": True, "readonly": True, "min_length": 1},
         "active": {"required": True, "readonly": True},
         "start_time": {"required": True, "readonly": True},
         "end_time": {"readonly": True},
         "user": {"readonly": True},
         "started_quantity": {"readonly": True},
         "work_type": {"required": True, "readonly": True},
     }
 
     _attribute_map = {
+        "resource_id": {"key": "resourceId", "type": "str"},
         "upn": {"key": "upn", "type": "str"},
         "personnel_number": {"key": "personnelNumber", "type": "str"},
         "active": {"key": "active", "type": "bool"},
         "start_time": {"key": "startTime", "type": "iso-8601"},
         "end_time": {"key": "endTime", "type": "iso-8601"},
         "user": {"key": "user", "type": "UserDto"},
         "started_quantity": {"key": "startedQuantity", "type": "int"},
         "work_type": {"key": "workType", "type": "str"},
     }
 
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
+    def __init__(self, *, resource_id: str, **kwargs: Any) -> None:
+        """
+        :keyword resource_id: Required.
+        :paramtype resource_id: str
+        """
         super().__init__(**kwargs)
+        self.resource_id = resource_id
         self.upn = None
         self.personnel_number = None
         self.active = None
         self.start_time = None
         self.end_time = None
         self.user = None
         self.started_quantity = None
@@ -5633,62 +6257,72 @@
     :vartype id: str
     :ivar part: Required.
     :vartype part: ~ignos.api.client.models.PartDto
     :ivar trace_type: Required. Known values are: "None", "Lot", "Batch", and "SerialNumber".
     :vartype trace_type: str or ~ignos.api.client.models.TraceType
     :ivar trace_exists: Required.
     :vartype trace_exists: bool
+    :ivar trace_status: Required. Known values are: "None", "Unavailable", "NotNeeded", "Partial",
+     and "Completed".
+    :vartype trace_status: str or ~ignos.api.client.models.TraceStatus
     :ivar work_orders:
     :vartype work_orders:
      list[~ignos.api.client.models.CustomerOrderLineWorkOrderTraceStatusNodeDto]
     """
 
     _validation = {
         "id": {"required": True, "min_length": 1},
         "part": {"required": True},
         "trace_type": {"required": True},
         "trace_exists": {"required": True},
+        "trace_status": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "part": {"key": "part", "type": "PartDto"},
         "trace_type": {"key": "traceType", "type": "str"},
         "trace_exists": {"key": "traceExists", "type": "bool"},
+        "trace_status": {"key": "traceStatus", "type": "str"},
         "work_orders": {"key": "workOrders", "type": "[CustomerOrderLineWorkOrderTraceStatusNodeDto]"},
     }
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         part: "_models.PartDto",
         trace_type: Union[str, "_models.TraceType"],
         trace_exists: bool,
+        trace_status: Union[str, "_models.TraceStatus"],
         work_orders: Optional[List["_models.CustomerOrderLineWorkOrderTraceStatusNodeDto"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword part: Required.
         :paramtype part: ~ignos.api.client.models.PartDto
         :keyword trace_type: Required. Known values are: "None", "Lot", "Batch", and "SerialNumber".
         :paramtype trace_type: str or ~ignos.api.client.models.TraceType
         :keyword trace_exists: Required.
         :paramtype trace_exists: bool
+        :keyword trace_status: Required. Known values are: "None", "Unavailable", "NotNeeded",
+         "Partial", and "Completed".
+        :paramtype trace_status: str or ~ignos.api.client.models.TraceStatus
         :keyword work_orders:
         :paramtype work_orders:
          list[~ignos.api.client.models.CustomerOrderLineWorkOrderTraceStatusNodeDto]
         """
         super().__init__(**kwargs)
         self.id = id
         self.part = part
         self.trace_type = trace_type
         self.trace_exists = trace_exists
+        self.trace_status = trace_status
         self.work_orders = work_orders
 
 
 class CustomerOrderTraceStatusDto(_serialization.Model):
     """CustomerOrderTraceStatusDto.
 
     All required parameters must be populated in order to send to server.
@@ -5782,14 +6416,47 @@
         :keyword filename: Required.
         :paramtype filename: str
         """
         super().__init__(**kwargs)
         self.filename = filename
 
 
+class DepartmentDto(_serialization.Model):
+    """DepartmentDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar number: Required.
+    :vartype number: str
+    :ivar name: Required.
+    :vartype name: str
+    """
+
+    _validation = {
+        "number": {"required": True, "min_length": 1},
+        "name": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "number": {"key": "number", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+    }
+
+    def __init__(self, *, number: str, name: str, **kwargs: Any) -> None:
+        """
+        :keyword number: Required.
+        :paramtype number: str
+        :keyword name: Required.
+        :paramtype name: str
+        """
+        super().__init__(**kwargs)
+        self.number = number
+        self.name = name
+
+
 class DeprecateToolRequest(_serialization.Model):
     """DeprecateToolRequest.
 
     :ivar date:
     :vartype date: ~datetime.datetime
     """
 
@@ -6128,15 +6795,15 @@
 
     :ivar tag:
     :vartype tag: str
     :ivar requirement: Known values are: "NotAllowed", "Optional", and "Required".
     :vartype requirement: str or ~ignos.api.client.models.DocumentMetadataRequirement
     :ivar mutability: Known values are: "Immutable", "Appendable", and "Mutable".
     :vartype mutability: str or ~ignos.api.client.models.Mutability
-    :ivar rule_type: Known values are: "Tag", "Title", "Sequences", "OrderLines", and "LotNumbers".
+    :ivar rule_type: Known values are: "Tag", "Sequences", "OrderLines", and "LotNumbers".
     :vartype rule_type: str or ~ignos.api.client.models.DocumentRuleType
     """
 
     _attribute_map = {
         "tag": {"key": "tag", "type": "str"},
         "requirement": {"key": "requirement", "type": "str"},
         "mutability": {"key": "mutability", "type": "str"},
@@ -6155,31 +6822,30 @@
         """
         :keyword tag:
         :paramtype tag: str
         :keyword requirement: Known values are: "NotAllowed", "Optional", and "Required".
         :paramtype requirement: str or ~ignos.api.client.models.DocumentMetadataRequirement
         :keyword mutability: Known values are: "Immutable", "Appendable", and "Mutable".
         :paramtype mutability: str or ~ignos.api.client.models.Mutability
-        :keyword rule_type: Known values are: "Tag", "Title", "Sequences", "OrderLines", and
-         "LotNumbers".
+        :keyword rule_type: Known values are: "Tag", "Sequences", "OrderLines", and "LotNumbers".
         :paramtype rule_type: str or ~ignos.api.client.models.DocumentRuleType
         """
         super().__init__(**kwargs)
         self.tag = tag
         self.requirement = requirement
         self.mutability = mutability
         self.rule_type = rule_type
 
 
 class DocumentTypeRuleTypeDto(_serialization.Model):
     """DocumentTypeRuleTypeDto.
 
     :ivar tag:
     :vartype tag: str
-    :ivar rule_type: Known values are: "Tag", "Title", "Sequences", "OrderLines", and "LotNumbers".
+    :ivar rule_type: Known values are: "Tag", "Sequences", "OrderLines", and "LotNumbers".
     :vartype rule_type: str or ~ignos.api.client.models.DocumentRuleType
     :ivar description:
     :vartype description: str
     """
 
     _attribute_map = {
         "tag": {"key": "tag", "type": "str"},
@@ -6194,16 +6860,15 @@
         rule_type: Optional[Union[str, "_models.DocumentRuleType"]] = None,
         description: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword tag:
         :paramtype tag: str
-        :keyword rule_type: Known values are: "Tag", "Title", "Sequences", "OrderLines", and
-         "LotNumbers".
+        :keyword rule_type: Known values are: "Tag", "Sequences", "OrderLines", and "LotNumbers".
         :paramtype rule_type: str or ~ignos.api.client.models.DocumentRuleType
         :keyword description:
         :paramtype description: str
         """
         super().__init__(**kwargs)
         self.tag = tag
         self.rule_type = rule_type
@@ -10109,14 +10774,68 @@
         self.search = search
         self.company_id = company_id
         self.active_orders = active_orders
         self.search_type = search_type
         self.continuation_token = continuation_token
 
 
+class LocationDto(_serialization.Model):
+    """LocationDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar location_id: Required.
+    :vartype location_id: str
+    :ivar location_name: Required.
+    :vartype location_name: str
+    :ivar kind: Required. Known values are: "Warehouse", "Zone", and "Location".
+    :vartype kind: str or ~ignos.api.client.models.LocationKindDto
+    :ivar profile:
+    :vartype profile: str
+    """
+
+    _validation = {
+        "location_id": {"required": True, "min_length": 1},
+        "location_name": {"required": True, "min_length": 1},
+        "kind": {"required": True},
+    }
+
+    _attribute_map = {
+        "location_id": {"key": "locationId", "type": "str"},
+        "location_name": {"key": "locationName", "type": "str"},
+        "kind": {"key": "kind", "type": "str"},
+        "profile": {"key": "profile", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location_id: str,
+        location_name: str,
+        kind: Union[str, "_models.LocationKindDto"],
+        profile: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword location_id: Required.
+        :paramtype location_id: str
+        :keyword location_name: Required.
+        :paramtype location_name: str
+        :keyword kind: Required. Known values are: "Warehouse", "Zone", and "Location".
+        :paramtype kind: str or ~ignos.api.client.models.LocationKindDto
+        :keyword profile:
+        :paramtype profile: str
+        """
+        super().__init__(**kwargs)
+        self.location_id = location_id
+        self.location_name = location_name
+        self.kind = kind
+        self.profile = profile
+
+
 class Machine(_serialization.Model):
     """Machine.
 
     :ivar external_id:
     :vartype external_id: str
     :ivar id:
     :vartype id: int
@@ -11651,39 +12370,59 @@
 
 
 class MachineUtilizationV2Dto(_serialization.Model):
     """MachineUtilizationV2Dto.
 
     All required parameters must be populated in order to send to server.
 
+    :ivar id:
+    :vartype id: int
     :ivar name: Required.
     :vartype name: str
+    :ivar description:
+    :vartype description: str
     :ivar utilization: Required.
     :vartype utilization: ~ignos.api.client.models.UtilizationDto
     """
 
     _validation = {
         "name": {"required": True, "min_length": 1},
         "utilization": {"required": True},
     }
 
     _attribute_map = {
+        "id": {"key": "id", "type": "int"},
         "name": {"key": "name", "type": "str"},
+        "description": {"key": "description", "type": "str"},
         "utilization": {"key": "utilization", "type": "UtilizationDto"},
     }
 
-    def __init__(self, *, name: str, utilization: "_models.UtilizationDto", **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        name: str,
+        utilization: "_models.UtilizationDto",
+        id: Optional[int] = None,  # pylint: disable=redefined-builtin
+        description: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
+        :keyword id:
+        :paramtype id: int
         :keyword name: Required.
         :paramtype name: str
+        :keyword description:
+        :paramtype description: str
         :keyword utilization: Required.
         :paramtype utilization: ~ignos.api.client.models.UtilizationDto
         """
         super().__init__(**kwargs)
+        self.id = id
         self.name = name
+        self.description = description
         self.utilization = utilization
 
 
 class ManufacturerDto(_serialization.Model):
     """ManufacturerDto.
 
     All required parameters must be populated in order to send to server.
@@ -19444,24 +20183,27 @@
     :vartype available_quantity: float
     :ivar drawing:
     :vartype drawing: ~ignos.api.client.models.DrawingDto
     :ivar order_reference:
     :vartype order_reference: ~ignos.api.client.models.OrderReferenceDto
     :ivar status: Required. Known values are: "Unknown", "NotStarted", "Partial", and "Completed".
     :vartype status: str or ~ignos.api.client.models.MaterialStatus
+    :ivar availability_details: Required.
+    :vartype availability_details: list[~ignos.api.client.models.InventoryDto]
     """
 
     _validation = {
         "line_number": {"required": True},
         "part": {"required": True},
         "operation": {"required": True},
         "quantity_per_part": {"required": True},
         "total_required_quantity": {"required": True},
         "used_quantity": {"required": True},
         "status": {"required": True},
+        "availability_details": {"required": True},
     }
 
     _attribute_map = {
         "position": {"key": "position", "type": "str"},
         "line_number": {"key": "lineNumber", "type": "float"},
         "part": {"key": "part", "type": "PartDto"},
         "dimension": {"key": "dimension", "type": "str"},
@@ -19474,26 +20216,28 @@
         "quantity_per_part": {"key": "quantityPerPart", "type": "float"},
         "total_required_quantity": {"key": "totalRequiredQuantity", "type": "float"},
         "used_quantity": {"key": "usedQuantity", "type": "float"},
         "available_quantity": {"key": "availableQuantity", "type": "float"},
         "drawing": {"key": "drawing", "type": "DrawingDto"},
         "order_reference": {"key": "orderReference", "type": "OrderReferenceDto"},
         "status": {"key": "status", "type": "str"},
+        "availability_details": {"key": "availabilityDetails", "type": "[InventoryDto]"},
     }
 
     def __init__(
         self,
         *,
         line_number: float,
         part: "_models.PartDto",
         operation: int,
         quantity_per_part: float,
         total_required_quantity: float,
         used_quantity: float,
         status: Union[str, "_models.MaterialStatus"],
+        availability_details: List["_models.InventoryDto"],
         position: Optional[str] = None,
         dimension: Optional[str] = None,
         operation_name: Optional[str] = None,
         warehouse: Optional[str] = None,
         fixed_location: Optional[str] = None,
         fixed_locations: Optional[List[str]] = None,
         unit: Optional[str] = None,
@@ -19534,14 +20278,16 @@
         :keyword drawing:
         :paramtype drawing: ~ignos.api.client.models.DrawingDto
         :keyword order_reference:
         :paramtype order_reference: ~ignos.api.client.models.OrderReferenceDto
         :keyword status: Required. Known values are: "Unknown", "NotStarted", "Partial", and
          "Completed".
         :paramtype status: str or ~ignos.api.client.models.MaterialStatus
+        :keyword availability_details: Required.
+        :paramtype availability_details: list[~ignos.api.client.models.InventoryDto]
         """
         super().__init__(**kwargs)
         self.position = position
         self.line_number = line_number
         self.part = part
         self.dimension = dimension
         self.operation = operation
@@ -19553,14 +20299,15 @@
         self.quantity_per_part = quantity_per_part
         self.total_required_quantity = total_required_quantity
         self.used_quantity = used_quantity
         self.available_quantity = available_quantity
         self.drawing = drawing
         self.order_reference = order_reference
         self.status = status
+        self.availability_details = availability_details
 
 
 class ProductionOrderDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """ProductionOrderDto.
 
     All required parameters must be populated in order to send to server.
 
@@ -19587,18 +20334,20 @@
     :vartype produced_quantity: float
     :ivar scrapped_quantity: Required.
     :vartype scrapped_quantity: float
     :ivar planner:
     :vartype planner: ~ignos.api.client.models.UserDto
     :ivar project_leader:
     :vartype project_leader: ~ignos.api.client.models.UserDto
-    :ivar end_location:
-    :vartype end_location: str
+    :ivar delivery_location:
+    :vartype delivery_location: ~ignos.api.client.models.WarehouseLocationDto
     :ivar project:
     :vartype project: ~ignos.api.client.models.WorkOrderProjectDto
+    :ivar attachments:
+    :vartype attachments: list[~ignos.api.client.models.WorkOrderAttachmentDto]
     :ivar start_date:
     :vartype start_date: ~datetime.datetime
     :ivar end_date:
     :vartype end_date: ~datetime.datetime
     :ivar bom_position:
     :vartype bom_position: str
     :ivar drawing:
@@ -19628,16 +20377,17 @@
         "operations": {"key": "operations", "type": "[ProductionOrderOperationDto]"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
         "produced_quantity": {"key": "producedQuantity", "type": "float"},
         "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
         "planner": {"key": "planner", "type": "UserDto"},
         "project_leader": {"key": "projectLeader", "type": "UserDto"},
-        "end_location": {"key": "endLocation", "type": "str"},
+        "delivery_location": {"key": "deliveryLocation", "type": "WarehouseLocationDto"},
         "project": {"key": "project", "type": "WorkOrderProjectDto"},
+        "attachments": {"key": "attachments", "type": "[WorkOrderAttachmentDto]"},
         "start_date": {"key": "startDate", "type": "iso-8601"},
         "end_date": {"key": "endDate", "type": "iso-8601"},
         "bom_position": {"key": "bomPosition", "type": "str"},
         "drawing": {"key": "drawing", "type": "DrawingDto"},
         "order_reference": {"key": "orderReference", "type": "OrderReferenceDto"},
     }
 
@@ -19653,16 +20403,17 @@
         produced_quantity: float,
         scrapped_quantity: float,
         unit: Optional[str] = None,
         planned_start: Optional[datetime.datetime] = None,
         planned_end: Optional[datetime.datetime] = None,
         planner: Optional["_models.UserDto"] = None,
         project_leader: Optional["_models.UserDto"] = None,
-        end_location: Optional[str] = None,
+        delivery_location: Optional["_models.WarehouseLocationDto"] = None,
         project: Optional["_models.WorkOrderProjectDto"] = None,
+        attachments: Optional[List["_models.WorkOrderAttachmentDto"]] = None,
         start_date: Optional[datetime.datetime] = None,
         end_date: Optional[datetime.datetime] = None,
         bom_position: Optional[str] = None,
         drawing: Optional["_models.DrawingDto"] = None,
         order_reference: Optional["_models.OrderReferenceDto"] = None,
         **kwargs: Any
     ) -> None:
@@ -19690,18 +20441,20 @@
         :paramtype produced_quantity: float
         :keyword scrapped_quantity: Required.
         :paramtype scrapped_quantity: float
         :keyword planner:
         :paramtype planner: ~ignos.api.client.models.UserDto
         :keyword project_leader:
         :paramtype project_leader: ~ignos.api.client.models.UserDto
-        :keyword end_location:
-        :paramtype end_location: str
+        :keyword delivery_location:
+        :paramtype delivery_location: ~ignos.api.client.models.WarehouseLocationDto
         :keyword project:
         :paramtype project: ~ignos.api.client.models.WorkOrderProjectDto
+        :keyword attachments:
+        :paramtype attachments: list[~ignos.api.client.models.WorkOrderAttachmentDto]
         :keyword start_date:
         :paramtype start_date: ~datetime.datetime
         :keyword end_date:
         :paramtype end_date: ~datetime.datetime
         :keyword bom_position:
         :paramtype bom_position: str
         :keyword drawing:
@@ -19719,33 +20472,148 @@
         self.operations = operations
         self.planned_start = planned_start
         self.planned_end = planned_end
         self.produced_quantity = produced_quantity
         self.scrapped_quantity = scrapped_quantity
         self.planner = planner
         self.project_leader = project_leader
-        self.end_location = end_location
+        self.delivery_location = delivery_location
         self.project = project
+        self.attachments = attachments
         self.start_date = start_date
         self.end_date = end_date
         self.bom_position = bom_position
         self.drawing = drawing
         self.order_reference = order_reference
 
 
+class ProductionOrderOperationActivityDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
+    """ProductionOrderOperationActivityDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar operation: Required.
+    :vartype operation: int
+    :ivar operation_id: Required.
+    :vartype operation_id: str
+    :ivar description:
+    :vartype description: str
+    :ivar resource:
+    :vartype resource: ~ignos.api.client.models.ResourceDto
+    :ivar user:
+    :vartype user: ~ignos.api.client.models.UserDto
+    :ivar start_time: Required.
+    :vartype start_time: ~datetime.datetime
+    :ivar end_time:
+    :vartype end_time: ~datetime.datetime
+    :ivar status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
+     "Stopped".
+    :vartype status: str or ~ignos.api.client.models.OperationStatusDto
+    :ivar active: Required.
+    :vartype active: bool
+    :ivar started_quantity:
+    :vartype started_quantity: float
+    :ivar produced_quantity:
+    :vartype produced_quantity: float
+    :ivar scrapped_quantity:
+    :vartype scrapped_quantity: float
+    """
+
+    _validation = {
+        "operation": {"required": True},
+        "operation_id": {"required": True, "min_length": 1},
+        "start_time": {"required": True},
+        "status": {"required": True},
+        "active": {"required": True},
+    }
+
+    _attribute_map = {
+        "operation": {"key": "operation", "type": "int"},
+        "operation_id": {"key": "operationId", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "resource": {"key": "resource", "type": "ResourceDto"},
+        "user": {"key": "user", "type": "UserDto"},
+        "start_time": {"key": "startTime", "type": "iso-8601"},
+        "end_time": {"key": "endTime", "type": "iso-8601"},
+        "status": {"key": "status", "type": "str"},
+        "active": {"key": "active", "type": "bool"},
+        "started_quantity": {"key": "startedQuantity", "type": "float"},
+        "produced_quantity": {"key": "producedQuantity", "type": "float"},
+        "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
+    }
+
+    def __init__(
+        self,
+        *,
+        operation: int,
+        operation_id: str,
+        start_time: datetime.datetime,
+        status: Union[str, "_models.OperationStatusDto"],
+        active: bool,
+        description: Optional[str] = None,
+        resource: Optional["_models.ResourceDto"] = None,
+        user: Optional["_models.UserDto"] = None,
+        end_time: Optional[datetime.datetime] = None,
+        started_quantity: Optional[float] = None,
+        produced_quantity: Optional[float] = None,
+        scrapped_quantity: Optional[float] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword operation: Required.
+        :paramtype operation: int
+        :keyword operation_id: Required.
+        :paramtype operation_id: str
+        :keyword description:
+        :paramtype description: str
+        :keyword resource:
+        :paramtype resource: ~ignos.api.client.models.ResourceDto
+        :keyword user:
+        :paramtype user: ~ignos.api.client.models.UserDto
+        :keyword start_time: Required.
+        :paramtype start_time: ~datetime.datetime
+        :keyword end_time:
+        :paramtype end_time: ~datetime.datetime
+        :keyword status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
+         "Stopped".
+        :paramtype status: str or ~ignos.api.client.models.OperationStatusDto
+        :keyword active: Required.
+        :paramtype active: bool
+        :keyword started_quantity:
+        :paramtype started_quantity: float
+        :keyword produced_quantity:
+        :paramtype produced_quantity: float
+        :keyword scrapped_quantity:
+        :paramtype scrapped_quantity: float
+        """
+        super().__init__(**kwargs)
+        self.operation = operation
+        self.operation_id = operation_id
+        self.description = description
+        self.resource = resource
+        self.user = user
+        self.start_time = start_time
+        self.end_time = end_time
+        self.status = status
+        self.active = active
+        self.started_quantity = started_quantity
+        self.produced_quantity = produced_quantity
+        self.scrapped_quantity = scrapped_quantity
+
+
 class ProductionOrderOperationDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """ProductionOrderOperationDto.
 
     All required parameters must be populated in order to send to server.
 
-    :ivar operation:
+    :ivar operation: Required.
     :vartype operation: int
     :ivar next_operation:
     :vartype next_operation: int
-    :ivar operation_id:
+    :ivar operation_id: Required.
     :vartype operation_id: str
     :ivar description:
     :vartype description: str
     :ivar total_planned_hours:
     :vartype total_planned_hours: float
     :ivar total_used_hours:
     :vartype total_used_hours: float
@@ -19761,27 +20629,33 @@
     :vartype fixed_time: bool
     :ivar resource:
     :vartype resource: ~ignos.api.client.models.ResourceDto
     :ivar planned_start:
     :vartype planned_start: ~datetime.datetime
     :ivar planned_end:
     :vartype planned_end: ~datetime.datetime
+    :ivar actual_start:
+    :vartype actual_start: ~datetime.datetime
+    :ivar actual_end:
+    :vartype actual_end: ~datetime.datetime
     :ivar status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
      "Stopped".
     :vartype status: str or ~ignos.api.client.models.OperationStatusDto
     :ivar produced_quantity: Required.
     :vartype produced_quantity: float
     :ivar scrapped_quantity: Required.
     :vartype scrapped_quantity: float
     :ivar quantity: Required.
     :vartype quantity: float
     :ivar started_quantity:
     :vartype started_quantity: float
     :ivar ongoing_quantity:
     :vartype ongoing_quantity: float
+    :ivar available_to_start_quantity: Required.
+    :vartype available_to_start_quantity: float
     :ivar work_instructions:
     :vartype work_instructions: str
     :ivar note:
     :vartype note: str
     :ivar fixture:
     :vartype fixture: str
     :ivar program:
@@ -19789,18 +20663,21 @@
     :ivar tool_number:
     :vartype tool_number: str
     :ivar disable_setup_registration: Required.
     :vartype disable_setup_registration: bool
     """
 
     _validation = {
+        "operation": {"required": True},
+        "operation_id": {"required": True, "min_length": 1},
         "status": {"required": True},
         "produced_quantity": {"required": True},
         "scrapped_quantity": {"required": True},
         "quantity": {"required": True},
+        "available_to_start_quantity": {"required": True},
         "disable_setup_registration": {"required": True},
     }
 
     _attribute_map = {
         "operation": {"key": "operation", "type": "int"},
         "next_operation": {"key": "nextOperation", "type": "int"},
         "operation_id": {"key": "operationId", "type": "str"},
@@ -19811,65 +20688,71 @@
         "planned_production_hours": {"key": "plannedProductionHours", "type": "float"},
         "used_setup_hours": {"key": "usedSetupHours", "type": "float"},
         "used_production_hours": {"key": "usedProductionHours", "type": "float"},
         "fixed_time": {"key": "fixedTime", "type": "bool"},
         "resource": {"key": "resource", "type": "ResourceDto"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
+        "actual_start": {"key": "actualStart", "type": "iso-8601"},
+        "actual_end": {"key": "actualEnd", "type": "iso-8601"},
         "status": {"key": "status", "type": "str"},
         "produced_quantity": {"key": "producedQuantity", "type": "float"},
         "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
         "quantity": {"key": "quantity", "type": "float"},
         "started_quantity": {"key": "startedQuantity", "type": "float"},
         "ongoing_quantity": {"key": "ongoingQuantity", "type": "float"},
+        "available_to_start_quantity": {"key": "availableToStartQuantity", "type": "float"},
         "work_instructions": {"key": "workInstructions", "type": "str"},
         "note": {"key": "note", "type": "str"},
         "fixture": {"key": "fixture", "type": "str"},
         "program": {"key": "program", "type": "str"},
         "tool_number": {"key": "toolNumber", "type": "str"},
         "disable_setup_registration": {"key": "disableSetupRegistration", "type": "bool"},
     }
 
     def __init__(  # pylint: disable=too-many-locals
         self,
         *,
+        operation: int,
+        operation_id: str,
         status: Union[str, "_models.OperationStatusDto"],
         produced_quantity: float,
         scrapped_quantity: float,
         quantity: float,
+        available_to_start_quantity: float,
         disable_setup_registration: bool,
-        operation: Optional[int] = None,
         next_operation: Optional[int] = None,
-        operation_id: Optional[str] = None,
         description: Optional[str] = None,
         total_planned_hours: Optional[float] = None,
         total_used_hours: Optional[float] = None,
         planned_setup_hours: Optional[float] = None,
         planned_production_hours: Optional[float] = None,
         used_setup_hours: Optional[float] = None,
         used_production_hours: Optional[float] = None,
         fixed_time: Optional[bool] = None,
         resource: Optional["_models.ResourceDto"] = None,
         planned_start: Optional[datetime.datetime] = None,
         planned_end: Optional[datetime.datetime] = None,
+        actual_start: Optional[datetime.datetime] = None,
+        actual_end: Optional[datetime.datetime] = None,
         started_quantity: Optional[float] = None,
         ongoing_quantity: Optional[float] = None,
         work_instructions: Optional[str] = None,
         note: Optional[str] = None,
         fixture: Optional[str] = None,
         program: Optional[str] = None,
         tool_number: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword operation:
+        :keyword operation: Required.
         :paramtype operation: int
         :keyword next_operation:
         :paramtype next_operation: int
-        :keyword operation_id:
+        :keyword operation_id: Required.
         :paramtype operation_id: str
         :keyword description:
         :paramtype description: str
         :keyword total_planned_hours:
         :paramtype total_planned_hours: float
         :keyword total_used_hours:
         :paramtype total_used_hours: float
@@ -19885,27 +20768,33 @@
         :paramtype fixed_time: bool
         :keyword resource:
         :paramtype resource: ~ignos.api.client.models.ResourceDto
         :keyword planned_start:
         :paramtype planned_start: ~datetime.datetime
         :keyword planned_end:
         :paramtype planned_end: ~datetime.datetime
+        :keyword actual_start:
+        :paramtype actual_start: ~datetime.datetime
+        :keyword actual_end:
+        :paramtype actual_end: ~datetime.datetime
         :keyword status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
          "Stopped".
         :paramtype status: str or ~ignos.api.client.models.OperationStatusDto
         :keyword produced_quantity: Required.
         :paramtype produced_quantity: float
         :keyword scrapped_quantity: Required.
         :paramtype scrapped_quantity: float
         :keyword quantity: Required.
         :paramtype quantity: float
         :keyword started_quantity:
         :paramtype started_quantity: float
         :keyword ongoing_quantity:
         :paramtype ongoing_quantity: float
+        :keyword available_to_start_quantity: Required.
+        :paramtype available_to_start_quantity: float
         :keyword work_instructions:
         :paramtype work_instructions: str
         :keyword note:
         :paramtype note: str
         :keyword fixture:
         :paramtype fixture: str
         :keyword program:
@@ -19926,20 +20815,23 @@
         self.planned_production_hours = planned_production_hours
         self.used_setup_hours = used_setup_hours
         self.used_production_hours = used_production_hours
         self.fixed_time = fixed_time
         self.resource = resource
         self.planned_start = planned_start
         self.planned_end = planned_end
+        self.actual_start = actual_start
+        self.actual_end = actual_end
         self.status = status
         self.produced_quantity = produced_quantity
         self.scrapped_quantity = scrapped_quantity
         self.quantity = quantity
         self.started_quantity = started_quantity
         self.ongoing_quantity = ongoing_quantity
+        self.available_to_start_quantity = available_to_start_quantity
         self.work_instructions = work_instructions
         self.note = note
         self.fixture = fixture
         self.program = program
         self.tool_number = tool_number
         self.disable_setup_registration = disable_setup_registration
 
@@ -19947,37 +20839,44 @@
 class ProductionResourceDto(_serialization.Model):
     """ProductionResourceDto.
 
     :ivar id:
     :vartype id: str
     :ivar name:
     :vartype name: str
+    :ivar department:
+    :vartype department: ~ignos.api.client.models.DepartmentDto
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
+        "department": {"key": "department", "type": "DepartmentDto"},
     }
 
     def __init__(
         self,
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         name: Optional[str] = None,
+        department: Optional["_models.DepartmentDto"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword name:
         :paramtype name: str
+        :keyword department:
+        :paramtype department: ~ignos.api.client.models.DepartmentDto
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
+        self.department = department
 
 
 class ProductionScheduleFiltersDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """ProductionScheduleFiltersDto.
 
     :ivar part_numbers:
     :vartype part_numbers: list[~ignos.api.client.models.FilterValueWithQuantity]
@@ -20084,14 +20983,18 @@
     :vartype operation: int
     :ivar operation_name: Required.
     :vartype operation_name: str
     :ivar planned_start: Required.
     :vartype planned_start: ~datetime.datetime
     :ivar planned_end:
     :vartype planned_end: ~datetime.datetime
+    :ivar actual_start:
+    :vartype actual_start: ~datetime.datetime
+    :ivar actual_end:
+    :vartype actual_end: ~datetime.datetime
     :ivar status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
      "Stopped".
     :vartype status: str or ~ignos.api.client.models.OperationStatusDto
     :ivar total_planned_hours:
     :vartype total_planned_hours: float
     :ivar total_used_hours:
     :vartype total_used_hours: float
@@ -20125,14 +21028,18 @@
     :vartype part_name: str
     :ivar part_material:
     :vartype part_material: str
     :ivar resource_id: Required.
     :vartype resource_id: str
     :ivar resource_name: Required.
     :vartype resource_name: str
+    :ivar resource_department_number:
+    :vartype resource_department_number: str
+    :ivar resource_department_name:
+    :vartype resource_department_name: str
     :ivar bom_position:
     :vartype bom_position: str
     :ivar customer_name:
     :vartype customer_name: str
     :ivar previous_operation:
     :vartype previous_operation: ~ignos.api.client.models.SurroundingOperationDto
     :ivar next_operation:
@@ -20147,16 +21054,16 @@
     :vartype fixture: str
     :ivar program:
     :vartype program: str
     :ivar tool_number:
     :vartype tool_number: str
     :ivar prerequisites: Required.
     :vartype prerequisites: ~ignos.api.client.models.OperationPrerequisitesDto
-    :ivar end_location:
-    :vartype end_location: str
+    :ivar delivery_location:
+    :vartype delivery_location: ~ignos.api.client.models.WarehouseLocationDto
     :ivar drawing:
     :vartype drawing: ~ignos.api.client.models.DrawingDto
     :ivar drawing_number:
     :vartype drawing_number: str
     :ivar disable_setup_registration: Required.
     :vartype disable_setup_registration: bool
     :ivar material_pick_status: Required. Known values are: "NotRequired", "NotStarted", "Started",
@@ -20186,14 +21093,16 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "production_order_number": {"key": "productionOrderNumber", "type": "str"},
         "operation": {"key": "operation", "type": "int"},
         "operation_name": {"key": "operationName", "type": "str"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
+        "actual_start": {"key": "actualStart", "type": "iso-8601"},
+        "actual_end": {"key": "actualEnd", "type": "iso-8601"},
         "status": {"key": "status", "type": "str"},
         "total_planned_hours": {"key": "totalPlannedHours", "type": "float"},
         "total_used_hours": {"key": "totalUsedHours", "type": "float"},
         "planned_setup_hours": {"key": "plannedSetupHours", "type": "float"},
         "planned_production_hours": {"key": "plannedProductionHours", "type": "float"},
         "used_setup_hours": {"key": "usedSetupHours", "type": "float"},
         "used_production_hours": {"key": "usedProductionHours", "type": "float"},
@@ -20206,26 +21115,28 @@
         "project": {"key": "project", "type": "WorkOrderProjectDto"},
         "part_number": {"key": "partNumber", "type": "str"},
         "part_revision": {"key": "partRevision", "type": "str"},
         "part_name": {"key": "partName", "type": "str"},
         "part_material": {"key": "partMaterial", "type": "str"},
         "resource_id": {"key": "resourceId", "type": "str"},
         "resource_name": {"key": "resourceName", "type": "str"},
+        "resource_department_number": {"key": "resourceDepartmentNumber", "type": "str"},
+        "resource_department_name": {"key": "resourceDepartmentName", "type": "str"},
         "bom_position": {"key": "bomPosition", "type": "str"},
         "customer_name": {"key": "customerName", "type": "str"},
         "previous_operation": {"key": "previousOperation", "type": "SurroundingOperationDto"},
         "next_operation": {"key": "nextOperation", "type": "SurroundingOperationDto"},
         "work_instructions": {"key": "workInstructions", "type": "str"},
         "note": {"key": "note", "type": "str"},
         "description": {"key": "description", "type": "str"},
         "fixture": {"key": "fixture", "type": "str"},
         "program": {"key": "program", "type": "str"},
         "tool_number": {"key": "toolNumber", "type": "str"},
         "prerequisites": {"key": "prerequisites", "type": "OperationPrerequisitesDto"},
-        "end_location": {"key": "endLocation", "type": "str"},
+        "delivery_location": {"key": "deliveryLocation", "type": "WarehouseLocationDto"},
         "drawing": {"key": "drawing", "type": "DrawingDto"},
         "drawing_number": {"key": "drawingNumber", "type": "str"},
         "disable_setup_registration": {"key": "disableSetupRegistration", "type": "bool"},
         "material_pick_status": {"key": "materialPickStatus", "type": "str"},
     }
 
     def __init__(  # pylint: disable=too-many-locals
@@ -20244,37 +21155,41 @@
         part_number: str,
         resource_id: str,
         resource_name: str,
         prerequisites: "_models.OperationPrerequisitesDto",
         disable_setup_registration: bool,
         material_pick_status: Union[str, "_models.MaterialPickStatus"],
         planned_end: Optional[datetime.datetime] = None,
+        actual_start: Optional[datetime.datetime] = None,
+        actual_end: Optional[datetime.datetime] = None,
         total_planned_hours: Optional[float] = None,
         total_used_hours: Optional[float] = None,
         planned_setup_hours: Optional[float] = None,
         planned_production_hours: Optional[float] = None,
         used_setup_hours: Optional[float] = None,
         used_production_hours: Optional[float] = None,
         started_quantity: Optional[float] = None,
         ongoing_quantity: Optional[float] = None,
         project: Optional["_models.WorkOrderProjectDto"] = None,
         part_revision: Optional[str] = None,
         part_name: Optional[str] = None,
         part_material: Optional[str] = None,
+        resource_department_number: Optional[str] = None,
+        resource_department_name: Optional[str] = None,
         bom_position: Optional[str] = None,
         customer_name: Optional[str] = None,
         previous_operation: Optional["_models.SurroundingOperationDto"] = None,
         next_operation: Optional["_models.SurroundingOperationDto"] = None,
         work_instructions: Optional[str] = None,
         note: Optional[str] = None,
         description: Optional[str] = None,
         fixture: Optional[str] = None,
         program: Optional[str] = None,
         tool_number: Optional[str] = None,
-        end_location: Optional[str] = None,
+        delivery_location: Optional["_models.WarehouseLocationDto"] = None,
         drawing: Optional["_models.DrawingDto"] = None,
         drawing_number: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
@@ -20284,14 +21199,18 @@
         :paramtype operation: int
         :keyword operation_name: Required.
         :paramtype operation_name: str
         :keyword planned_start: Required.
         :paramtype planned_start: ~datetime.datetime
         :keyword planned_end:
         :paramtype planned_end: ~datetime.datetime
+        :keyword actual_start:
+        :paramtype actual_start: ~datetime.datetime
+        :keyword actual_end:
+        :paramtype actual_end: ~datetime.datetime
         :keyword status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
          "Stopped".
         :paramtype status: str or ~ignos.api.client.models.OperationStatusDto
         :keyword total_planned_hours:
         :paramtype total_planned_hours: float
         :keyword total_used_hours:
         :paramtype total_used_hours: float
@@ -20325,14 +21244,18 @@
         :paramtype part_name: str
         :keyword part_material:
         :paramtype part_material: str
         :keyword resource_id: Required.
         :paramtype resource_id: str
         :keyword resource_name: Required.
         :paramtype resource_name: str
+        :keyword resource_department_number:
+        :paramtype resource_department_number: str
+        :keyword resource_department_name:
+        :paramtype resource_department_name: str
         :keyword bom_position:
         :paramtype bom_position: str
         :keyword customer_name:
         :paramtype customer_name: str
         :keyword previous_operation:
         :paramtype previous_operation: ~ignos.api.client.models.SurroundingOperationDto
         :keyword next_operation:
@@ -20347,16 +21270,16 @@
         :paramtype fixture: str
         :keyword program:
         :paramtype program: str
         :keyword tool_number:
         :paramtype tool_number: str
         :keyword prerequisites: Required.
         :paramtype prerequisites: ~ignos.api.client.models.OperationPrerequisitesDto
-        :keyword end_location:
-        :paramtype end_location: str
+        :keyword delivery_location:
+        :paramtype delivery_location: ~ignos.api.client.models.WarehouseLocationDto
         :keyword drawing:
         :paramtype drawing: ~ignos.api.client.models.DrawingDto
         :keyword drawing_number:
         :paramtype drawing_number: str
         :keyword disable_setup_registration: Required.
         :paramtype disable_setup_registration: bool
         :keyword material_pick_status: Required. Known values are: "NotRequired", "NotStarted",
@@ -20366,14 +21289,16 @@
         super().__init__(**kwargs)
         self.id = id
         self.production_order_number = production_order_number
         self.operation = operation
         self.operation_name = operation_name
         self.planned_start = planned_start
         self.planned_end = planned_end
+        self.actual_start = actual_start
+        self.actual_end = actual_end
         self.status = status
         self.total_planned_hours = total_planned_hours
         self.total_used_hours = total_used_hours
         self.planned_setup_hours = planned_setup_hours
         self.planned_production_hours = planned_production_hours
         self.used_setup_hours = used_setup_hours
         self.used_production_hours = used_production_hours
@@ -20386,26 +21311,28 @@
         self.project = project
         self.part_number = part_number
         self.part_revision = part_revision
         self.part_name = part_name
         self.part_material = part_material
         self.resource_id = resource_id
         self.resource_name = resource_name
+        self.resource_department_number = resource_department_number
+        self.resource_department_name = resource_department_name
         self.bom_position = bom_position
         self.customer_name = customer_name
         self.previous_operation = previous_operation
         self.next_operation = next_operation
         self.work_instructions = work_instructions
         self.note = note
         self.description = description
         self.fixture = fixture
         self.program = program
         self.tool_number = tool_number
         self.prerequisites = prerequisites
-        self.end_location = end_location
+        self.delivery_location = delivery_location
         self.drawing = drawing
         self.drawing_number = drawing_number
         self.disable_setup_registration = disable_setup_registration
         self.material_pick_status = material_pick_status
 
 
 class ProductionScheduleOperationDtoPagedResult(_serialization.Model):  # pylint: disable=name-too-long
@@ -20840,39 +21767,43 @@
     :vartype external: bool
     :ivar description:
     :vartype description: str
     :ivar resource_type:
     :vartype resource_type: str
     :ivar resource_group_id:
     :vartype resource_group_id: str
+    :ivar department:
+    :vartype department: ~ignos.api.client.models.DepartmentDto
     """
 
     _validation = {
         "id": {"required": True, "min_length": 1},
         "external": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "external": {"key": "external", "type": "bool"},
         "description": {"key": "description", "type": "str"},
         "resource_type": {"key": "resourceType", "type": "str"},
         "resource_group_id": {"key": "resourceGroupId", "type": "str"},
+        "department": {"key": "department", "type": "DepartmentDto"},
     }
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         external: bool,
         name: Optional[str] = None,
         description: Optional[str] = None,
         resource_type: Optional[str] = None,
         resource_group_id: Optional[str] = None,
+        department: Optional["_models.DepartmentDto"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword name:
         :paramtype name: str
@@ -20880,22 +21811,25 @@
         :paramtype external: bool
         :keyword description:
         :paramtype description: str
         :keyword resource_type:
         :paramtype resource_type: str
         :keyword resource_group_id:
         :paramtype resource_group_id: str
+        :keyword department:
+        :paramtype department: ~ignos.api.client.models.DepartmentDto
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
         self.external = external
         self.description = description
         self.resource_type = resource_type
         self.resource_group_id = resource_group_id
+        self.department = department
 
 
 class ResourceExistDto(_serialization.Model):
     """ResourceExistDto.
 
     All required parameters must be populated in order to send to server.
 
@@ -20946,46 +21880,53 @@
 
     :ivar id:
     :vartype id: str
     :ivar name:
     :vartype name: str
     :ivar resources: Required.
     :vartype resources: list[~ignos.api.client.models.ProductionResourceDto]
+    :ivar department:
+    :vartype department: ~ignos.api.client.models.DepartmentDto
     """
 
     _validation = {
         "resources": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "resources": {"key": "resources", "type": "[ProductionResourceDto]"},
+        "department": {"key": "department", "type": "DepartmentDto"},
     }
 
     def __init__(
         self,
         *,
         resources: List["_models.ProductionResourceDto"],
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         name: Optional[str] = None,
+        department: Optional["_models.DepartmentDto"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword name:
         :paramtype name: str
         :keyword resources: Required.
         :paramtype resources: list[~ignos.api.client.models.ProductionResourceDto]
+        :keyword department:
+        :paramtype department: ~ignos.api.client.models.DepartmentDto
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
         self.resources = resources
+        self.department = department
 
 
 class RightAngledTriangleDto(_serialization.Model):
     """RightAngledTriangleDto.
 
     All required parameters must be populated in order to send to server.
 
@@ -21676,14 +22617,54 @@
         """
         super().__init__(**kwargs)
         self.element_id = element_id
         self.balloon_id = balloon_id
         self.disabled = disabled
 
 
+class SearchWorkOrderDto(_serialization.Model):
+    """SearchWorkOrderDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar work_order_id: Required.
+    :vartype work_order_id: str
+    :ivar part_name:
+    :vartype part_name: str
+    :ivar part_number:
+    :vartype part_number: str
+    """
+
+    _validation = {
+        "work_order_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "work_order_id": {"key": "workOrderId", "type": "str"},
+        "part_name": {"key": "partName", "type": "str"},
+        "part_number": {"key": "partNumber", "type": "str"},
+    }
+
+    def __init__(
+        self, *, work_order_id: str, part_name: Optional[str] = None, part_number: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword work_order_id: Required.
+        :paramtype work_order_id: str
+        :keyword part_name:
+        :paramtype part_name: str
+        :keyword part_number:
+        :paramtype part_number: str
+        """
+        super().__init__(**kwargs)
+        self.work_order_id = work_order_id
+        self.part_name = part_name
+        self.part_number = part_number
+
+
 class SelectProductionCompany(_serialization.Model):
     """SelectProductionCompany.
 
     All required parameters must be populated in order to send to server.
 
     :ivar id: Required.
     :vartype id: str
@@ -22008,14 +22989,54 @@
         """
         super().__init__(**kwargs)
         self.path = path
         self.content = content
         self.cnc_machine_id = cnc_machine_id
 
 
+class StartCamTransferToMachineFromTempUpload(_serialization.Model):
+    """StartCamTransferToMachineFromTempUpload.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upload_key: Required.
+    :vartype upload_key: str
+    :ivar filename: Required.
+    :vartype filename: str
+    :ivar cnc_machine_id: Required.
+    :vartype cnc_machine_id: str
+    """
+
+    _validation = {
+        "upload_key": {"required": True, "min_length": 1},
+        "filename": {"required": True, "min_length": 1},
+        "cnc_machine_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "upload_key": {"key": "uploadKey", "type": "str"},
+        "filename": {"key": "filename", "type": "str"},
+        "cnc_machine_id": {"key": "cncMachineId", "type": "str"},
+    }
+
+    def __init__(self, *, upload_key: str, filename: str, cnc_machine_id: str, **kwargs: Any) -> None:
+        """
+        :keyword upload_key: Required.
+        :paramtype upload_key: str
+        :keyword filename: Required.
+        :paramtype filename: str
+        :keyword cnc_machine_id: Required.
+        :paramtype cnc_machine_id: str
+        """
+        super().__init__(**kwargs)
+        self.upload_key = upload_key
+        self.filename = filename
+        self.cnc_machine_id = cnc_machine_id
+
+
 class StartOperationDto(_serialization.Model):
     """StartOperationDto.
 
     All required parameters must be populated in order to send to server.
 
     :ivar work_order: Required.
     :vartype work_order: str
@@ -22528,114 +23549,141 @@
 
     :ivar id: Required.
     :vartype id: str
     :ivar operation: Required.
     :vartype operation: int
     :ivar operation_name: Required.
     :vartype operation_name: str
-    :ivar planned_start: Required.
+    :ivar planned_start:
     :vartype planned_start: ~datetime.datetime
     :ivar planned_end:
     :vartype planned_end: ~datetime.datetime
+    :ivar actual_start:
+    :vartype actual_start: ~datetime.datetime
+    :ivar actual_end:
+    :vartype actual_end: ~datetime.datetime
     :ivar status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
      "Stopped".
     :vartype status: str or ~ignos.api.client.models.OperationStatusDto
     :ivar resource_group_id:
     :vartype resource_group_id: str
     :ivar resource_id:
     :vartype resource_id: str
     :ivar resource_name:
     :vartype resource_name: str
+    :ivar resource_department_number:
+    :vartype resource_department_number: str
+    :ivar resource_department_name:
+    :vartype resource_department_name: str
     :ivar produced_quantity: Required.
     :vartype produced_quantity: float
     :ivar scrapped_quantity: Required.
     :vartype scrapped_quantity: float
     :ivar started_quantity:
     :vartype started_quantity: float
     """
 
     _validation = {
         "id": {"required": True, "min_length": 1},
         "operation": {"required": True},
         "operation_name": {"required": True, "min_length": 1},
-        "planned_start": {"required": True},
         "status": {"required": True},
         "produced_quantity": {"required": True},
         "scrapped_quantity": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "operation": {"key": "operation", "type": "int"},
         "operation_name": {"key": "operationName", "type": "str"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
+        "actual_start": {"key": "actualStart", "type": "iso-8601"},
+        "actual_end": {"key": "actualEnd", "type": "iso-8601"},
         "status": {"key": "status", "type": "str"},
         "resource_group_id": {"key": "resourceGroupId", "type": "str"},
         "resource_id": {"key": "resourceId", "type": "str"},
         "resource_name": {"key": "resourceName", "type": "str"},
+        "resource_department_number": {"key": "resourceDepartmentNumber", "type": "str"},
+        "resource_department_name": {"key": "resourceDepartmentName", "type": "str"},
         "produced_quantity": {"key": "producedQuantity", "type": "float"},
         "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
         "started_quantity": {"key": "startedQuantity", "type": "float"},
     }
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         operation: int,
         operation_name: str,
-        planned_start: datetime.datetime,
         status: Union[str, "_models.OperationStatusDto"],
         produced_quantity: float,
         scrapped_quantity: float,
+        planned_start: Optional[datetime.datetime] = None,
         planned_end: Optional[datetime.datetime] = None,
+        actual_start: Optional[datetime.datetime] = None,
+        actual_end: Optional[datetime.datetime] = None,
         resource_group_id: Optional[str] = None,
         resource_id: Optional[str] = None,
         resource_name: Optional[str] = None,
+        resource_department_number: Optional[str] = None,
+        resource_department_name: Optional[str] = None,
         started_quantity: Optional[float] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword operation: Required.
         :paramtype operation: int
         :keyword operation_name: Required.
         :paramtype operation_name: str
-        :keyword planned_start: Required.
+        :keyword planned_start:
         :paramtype planned_start: ~datetime.datetime
         :keyword planned_end:
         :paramtype planned_end: ~datetime.datetime
+        :keyword actual_start:
+        :paramtype actual_start: ~datetime.datetime
+        :keyword actual_end:
+        :paramtype actual_end: ~datetime.datetime
         :keyword status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
          "Stopped".
         :paramtype status: str or ~ignos.api.client.models.OperationStatusDto
         :keyword resource_group_id:
         :paramtype resource_group_id: str
         :keyword resource_id:
         :paramtype resource_id: str
         :keyword resource_name:
         :paramtype resource_name: str
+        :keyword resource_department_number:
+        :paramtype resource_department_number: str
+        :keyword resource_department_name:
+        :paramtype resource_department_name: str
         :keyword produced_quantity: Required.
         :paramtype produced_quantity: float
         :keyword scrapped_quantity: Required.
         :paramtype scrapped_quantity: float
         :keyword started_quantity:
         :paramtype started_quantity: float
         """
         super().__init__(**kwargs)
         self.id = id
         self.operation = operation
         self.operation_name = operation_name
         self.planned_start = planned_start
         self.planned_end = planned_end
+        self.actual_start = actual_start
+        self.actual_end = actual_end
         self.status = status
         self.resource_group_id = resource_group_id
         self.resource_id = resource_id
         self.resource_name = resource_name
+        self.resource_department_number = resource_department_number
+        self.resource_department_name = resource_department_name
         self.produced_quantity = produced_quantity
         self.scrapped_quantity = scrapped_quantity
         self.started_quantity = started_quantity
 
 
 class SustainabilityCustomerOrderDto(_serialization.Model):
     """SustainabilityCustomerOrderDto.
@@ -22839,15 +23887,15 @@
         """
         super().__init__(**kwargs)
         self.part_number = part_number
         self.part_revision = part_revision
         self.part_name = part_name
 
 
-class TraceDto(_serialization.Model):
+class TraceDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """TraceDto.
 
     All required parameters must be populated in order to send to server.
 
     :ivar id: Required.
     :vartype id: str
     :ivar user: Required.
@@ -22862,41 +23910,50 @@
     :vartype items: list[~ignos.api.client.models.TraceItemDto]
     :ivar override_material_details: Required.
     :vartype override_material_details: list[~ignos.api.client.models.TraceMaterialDetailDto]
     :ivar operations: Required.
     :vartype operations: list[~ignos.api.client.models.WorkOrderTraceOperationDto]
     :ivar trace_type: Required. Known values are: "None", "Lot", "Batch", and "SerialNumber".
     :vartype trace_type: str or ~ignos.api.client.models.TraceType
+    :ivar trace_status: Required. Known values are: "None", "Unavailable", "NotNeeded", "Partial",
+     and "Completed".
+    :vartype trace_status: str or ~ignos.api.client.models.TraceStatus
+    :ivar manual_completed: Required.
+    :vartype manual_completed: bool
     :ivar material_lines_missing_trace_information: Required.
     :vartype material_lines_missing_trace_information: list[int]
     """
 
     _validation = {
         "id": {"required": True, "min_length": 1},
         "user": {"required": True},
         "last_changed": {"required": True},
         "part": {"required": True},
         "quantity": {"required": True},
         "items": {"required": True},
         "override_material_details": {"required": True},
         "operations": {"required": True},
         "trace_type": {"required": True},
+        "trace_status": {"required": True},
+        "manual_completed": {"required": True},
         "material_lines_missing_trace_information": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "user": {"key": "user", "type": "UserDto"},
         "last_changed": {"key": "lastChanged", "type": "iso-8601"},
         "part": {"key": "part", "type": "PartDto"},
         "quantity": {"key": "quantity", "type": "float"},
         "items": {"key": "items", "type": "[TraceItemDto]"},
         "override_material_details": {"key": "overrideMaterialDetails", "type": "[TraceMaterialDetailDto]"},
         "operations": {"key": "operations", "type": "[WorkOrderTraceOperationDto]"},
         "trace_type": {"key": "traceType", "type": "str"},
+        "trace_status": {"key": "traceStatus", "type": "str"},
+        "manual_completed": {"key": "manualCompleted", "type": "bool"},
         "material_lines_missing_trace_information": {"key": "materialLinesMissingTraceInformation", "type": "[int]"},
     }
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
@@ -22904,14 +23961,16 @@
         last_changed: datetime.datetime,
         part: "_models.PartDto",
         quantity: float,
         items: List["_models.TraceItemDto"],
         override_material_details: List["_models.TraceMaterialDetailDto"],
         operations: List["_models.WorkOrderTraceOperationDto"],
         trace_type: Union[str, "_models.TraceType"],
+        trace_status: Union[str, "_models.TraceStatus"],
+        manual_completed: bool,
         material_lines_missing_trace_information: List[int],
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword user: Required.
@@ -22926,27 +23985,34 @@
         :paramtype items: list[~ignos.api.client.models.TraceItemDto]
         :keyword override_material_details: Required.
         :paramtype override_material_details: list[~ignos.api.client.models.TraceMaterialDetailDto]
         :keyword operations: Required.
         :paramtype operations: list[~ignos.api.client.models.WorkOrderTraceOperationDto]
         :keyword trace_type: Required. Known values are: "None", "Lot", "Batch", and "SerialNumber".
         :paramtype trace_type: str or ~ignos.api.client.models.TraceType
+        :keyword trace_status: Required. Known values are: "None", "Unavailable", "NotNeeded",
+         "Partial", and "Completed".
+        :paramtype trace_status: str or ~ignos.api.client.models.TraceStatus
+        :keyword manual_completed: Required.
+        :paramtype manual_completed: bool
         :keyword material_lines_missing_trace_information: Required.
         :paramtype material_lines_missing_trace_information: list[int]
         """
         super().__init__(**kwargs)
         self.id = id
         self.user = user
         self.last_changed = last_changed
         self.part = part
         self.quantity = quantity
         self.items = items
         self.override_material_details = override_material_details
         self.operations = operations
         self.trace_type = trace_type
+        self.trace_status = trace_status
+        self.manual_completed = manual_completed
         self.material_lines_missing_trace_information = material_lines_missing_trace_information
 
 
 class TraceItemConsumptionDto(_serialization.Model):
     """TraceItemConsumptionDto.
 
     All required parameters must be populated in order to send to server.
@@ -23326,14 +24392,273 @@
         :paramtype continuation_token: str
         """
         super().__init__(**kwargs)
         self.results = results
         self.continuation_token = continuation_token
 
 
+class TrackingEventDto(_serialization.Model):
+    """TrackingEventDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar id: Required.
+    :vartype id: int
+    :ivar created: Required.
+    :vartype created: ~datetime.datetime
+    :ivar created_by: Required.
+    :vartype created_by: str
+    :ivar location: Required.
+    :vartype location: ~ignos.api.client.models.LocationDto
+    :ivar status: Required. Known values are: "Manual", "BookingPending", "BookingCancelled",
+     "BookingInProgress", and "BookingComplete".
+    :vartype status: str or ~ignos.api.client.models.TrackingStatusDto
+    :ivar booking_id:
+    :vartype booking_id: str
+    :ivar comment:
+    :vartype comment: str
+    """
+
+    _validation = {
+        "id": {"required": True},
+        "created": {"required": True},
+        "created_by": {"required": True, "min_length": 1},
+        "location": {"required": True},
+        "status": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "int"},
+        "created": {"key": "created", "type": "iso-8601"},
+        "created_by": {"key": "createdBy", "type": "str"},
+        "location": {"key": "location", "type": "LocationDto"},
+        "status": {"key": "status", "type": "str"},
+        "booking_id": {"key": "bookingId", "type": "str"},
+        "comment": {"key": "comment", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: int,  # pylint: disable=redefined-builtin
+        created: datetime.datetime,
+        created_by: str,
+        location: "_models.LocationDto",
+        status: Union[str, "_models.TrackingStatusDto"],
+        booking_id: Optional[str] = None,
+        comment: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id: Required.
+        :paramtype id: int
+        :keyword created: Required.
+        :paramtype created: ~datetime.datetime
+        :keyword created_by: Required.
+        :paramtype created_by: str
+        :keyword location: Required.
+        :paramtype location: ~ignos.api.client.models.LocationDto
+        :keyword status: Required. Known values are: "Manual", "BookingPending", "BookingCancelled",
+         "BookingInProgress", and "BookingComplete".
+        :paramtype status: str or ~ignos.api.client.models.TrackingStatusDto
+        :keyword booking_id:
+        :paramtype booking_id: str
+        :keyword comment:
+        :paramtype comment: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.created = created
+        self.created_by = created_by
+        self.location = location
+        self.status = status
+        self.booking_id = booking_id
+        self.comment = comment
+
+
+class TrackingHistoryDto(_serialization.Model):
+    """TrackingHistoryDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar tracking_id: Required.
+    :vartype tracking_id: str
+    :ivar pallet_number: Required.
+    :vartype pallet_number: int
+    :ivar work_order_id: Required.
+    :vartype work_order_id: str
+    :ivar tracking_events: Required.
+    :vartype tracking_events: list[~ignos.api.client.models.TrackingEventDto]
+    """
+
+    _validation = {
+        "tracking_id": {"required": True, "min_length": 1},
+        "pallet_number": {"required": True},
+        "work_order_id": {"required": True, "min_length": 1},
+        "tracking_events": {"required": True},
+    }
+
+    _attribute_map = {
+        "tracking_id": {"key": "trackingId", "type": "str"},
+        "pallet_number": {"key": "palletNumber", "type": "int"},
+        "work_order_id": {"key": "workOrderId", "type": "str"},
+        "tracking_events": {"key": "trackingEvents", "type": "[TrackingEventDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        tracking_id: str,
+        pallet_number: int,
+        work_order_id: str,
+        tracking_events: List["_models.TrackingEventDto"],
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tracking_id: Required.
+        :paramtype tracking_id: str
+        :keyword pallet_number: Required.
+        :paramtype pallet_number: int
+        :keyword work_order_id: Required.
+        :paramtype work_order_id: str
+        :keyword tracking_events: Required.
+        :paramtype tracking_events: list[~ignos.api.client.models.TrackingEventDto]
+        """
+        super().__init__(**kwargs)
+        self.tracking_id = tracking_id
+        self.pallet_number = pallet_number
+        self.work_order_id = work_order_id
+        self.tracking_events = tracking_events
+
+
+class TrackingHistoryUpdateDto(_serialization.Model):
+    """TrackingHistoryUpdateDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar work_order_id: Required.
+    :vartype work_order_id: str
+    :ivar location_id: Required.
+    :vartype location_id: str
+    :ivar comment:
+    :vartype comment: str
+    """
+
+    _validation = {
+        "work_order_id": {"required": True, "min_length": 1},
+        "location_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "work_order_id": {"key": "workOrderId", "type": "str"},
+        "location_id": {"key": "locationId", "type": "str"},
+        "comment": {"key": "comment", "type": "str"},
+    }
+
+    def __init__(self, *, work_order_id: str, location_id: str, comment: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword work_order_id: Required.
+        :paramtype work_order_id: str
+        :keyword location_id: Required.
+        :paramtype location_id: str
+        :keyword comment:
+        :paramtype comment: str
+        """
+        super().__init__(**kwargs)
+        self.work_order_id = work_order_id
+        self.location_id = location_id
+        self.comment = comment
+
+
+class TrackingUpdateDto(_serialization.Model):
+    """TrackingUpdateDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar tracking_id: Required.
+    :vartype tracking_id: str
+    :ivar location_id: Required.
+    :vartype location_id: str
+    :ivar comment:
+    :vartype comment: str
+    """
+
+    _validation = {
+        "tracking_id": {"required": True, "min_length": 1},
+        "location_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "tracking_id": {"key": "trackingId", "type": "str"},
+        "location_id": {"key": "locationId", "type": "str"},
+        "comment": {"key": "comment", "type": "str"},
+    }
+
+    def __init__(self, *, tracking_id: str, location_id: str, comment: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword tracking_id: Required.
+        :paramtype tracking_id: str
+        :keyword location_id: Required.
+        :paramtype location_id: str
+        :keyword comment:
+        :paramtype comment: str
+        """
+        super().__init__(**kwargs)
+        self.tracking_id = tracking_id
+        self.location_id = location_id
+        self.comment = comment
+
+
+class TrackingWorkOrderDto(_serialization.Model):
+    """TrackingWorkOrderDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar work_order_id: Required.
+    :vartype work_order_id: str
+    :ivar part: Required.
+    :vartype part: ~ignos.api.client.models.PartDto
+    :ivar tracking_history: Required.
+    :vartype tracking_history: list[~ignos.api.client.models.TrackingHistoryDto]
+    """
+
+    _validation = {
+        "work_order_id": {"required": True, "min_length": 1},
+        "part": {"required": True},
+        "tracking_history": {"required": True},
+    }
+
+    _attribute_map = {
+        "work_order_id": {"key": "workOrderId", "type": "str"},
+        "part": {"key": "part", "type": "PartDto"},
+        "tracking_history": {"key": "trackingHistory", "type": "[TrackingHistoryDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        work_order_id: str,
+        part: "_models.PartDto",
+        tracking_history: List["_models.TrackingHistoryDto"],
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword work_order_id: Required.
+        :paramtype work_order_id: str
+        :keyword part: Required.
+        :paramtype part: ~ignos.api.client.models.PartDto
+        :keyword tracking_history: Required.
+        :paramtype tracking_history: list[~ignos.api.client.models.TrackingHistoryDto]
+        """
+        super().__init__(**kwargs)
+        self.work_order_id = work_order_id
+        self.part = part
+        self.tracking_history = tracking_history
+
+
 class UnregisteredToolValueDto(_serialization.Model):
     """UnregisteredToolValueDto.
 
     All required parameters must be populated in order to send to server.
 
     :ivar unregistered_tool: Required.
     :vartype unregistered_tool: str
@@ -23663,14 +24988,16 @@
     :vartype size: str
     :ivar diameter:
     :vartype diameter: float
     :ivar grade:
     :vartype grade: str
     :ivar radius:
     :vartype radius: float
+    :ivar chamfer:
+    :vartype chamfer: float
     :ivar width:
     :vartype width: float
     :ivar pitch:
     :vartype pitch: str
     :ivar length:
     :vartype length: float
     :ivar kapr:
@@ -23698,14 +25025,15 @@
         "description": {"key": "description", "type": "str"},
         "holder_description": {"key": "holderDescription", "type": "str"},
         "geometry": {"key": "geometry", "type": "str"},
         "size": {"key": "size", "type": "str"},
         "diameter": {"key": "diameter", "type": "float"},
         "grade": {"key": "grade", "type": "str"},
         "radius": {"key": "radius", "type": "float"},
+        "chamfer": {"key": "chamfer", "type": "float"},
         "width": {"key": "width", "type": "float"},
         "pitch": {"key": "pitch", "type": "str"},
         "length": {"key": "length", "type": "float"},
         "kapr": {"key": "kapr", "type": "float"},
         "teeth": {"key": "teeth", "type": "int"},
         "stick_out": {"key": "stickOut", "type": "float"},
         "apmx": {"key": "apmx", "type": "float"},
@@ -23722,14 +25050,15 @@
         description: Optional[str] = None,
         holder_description: Optional[str] = None,
         geometry: Optional[str] = None,
         size: Optional[str] = None,
         diameter: Optional[float] = None,
         grade: Optional[str] = None,
         radius: Optional[float] = None,
+        chamfer: Optional[float] = None,
         width: Optional[float] = None,
         pitch: Optional[str] = None,
         length: Optional[float] = None,
         kapr: Optional[float] = None,
         teeth: Optional[int] = None,
         stick_out: Optional[float] = None,
         apmx: Optional[float] = None,
@@ -23755,14 +25084,16 @@
         :paramtype size: str
         :keyword diameter:
         :paramtype diameter: float
         :keyword grade:
         :paramtype grade: str
         :keyword radius:
         :paramtype radius: float
+        :keyword chamfer:
+        :paramtype chamfer: float
         :keyword width:
         :paramtype width: float
         :keyword pitch:
         :paramtype pitch: str
         :keyword length:
         :paramtype length: float
         :keyword kapr:
@@ -23784,14 +25115,15 @@
         self.description = description
         self.holder_description = holder_description
         self.geometry = geometry
         self.size = size
         self.diameter = diameter
         self.grade = grade
         self.radius = radius
+        self.chamfer = chamfer
         self.width = width
         self.pitch = pitch
         self.length = length
         self.kapr = kapr
         self.teeth = teeth
         self.stick_out = stick_out
         self.apmx = apmx
@@ -23853,14 +25185,16 @@
     :vartype size: str
     :ivar diameter:
     :vartype diameter: float
     :ivar grade:
     :vartype grade: str
     :ivar radius:
     :vartype radius: float
+    :ivar chamfer:
+    :vartype chamfer: float
     :ivar width:
     :vartype width: float
     :ivar pitch:
     :vartype pitch: str
     :ivar length:
     :vartype length: float
     :ivar kapr:
@@ -23888,14 +25222,15 @@
         "description": {"key": "description", "type": "str"},
         "holder_description": {"key": "holderDescription", "type": "str"},
         "geometry": {"key": "geometry", "type": "str"},
         "size": {"key": "size", "type": "str"},
         "diameter": {"key": "diameter", "type": "float"},
         "grade": {"key": "grade", "type": "str"},
         "radius": {"key": "radius", "type": "float"},
+        "chamfer": {"key": "chamfer", "type": "float"},
         "width": {"key": "width", "type": "float"},
         "pitch": {"key": "pitch", "type": "str"},
         "length": {"key": "length", "type": "float"},
         "kapr": {"key": "kapr", "type": "float"},
         "teeth": {"key": "teeth", "type": "int"},
         "stick_out": {"key": "stickOut", "type": "float"},
         "apmx": {"key": "apmx", "type": "float"},
@@ -23912,14 +25247,15 @@
         description: Optional[str] = None,
         holder_description: Optional[str] = None,
         geometry: Optional[str] = None,
         size: Optional[str] = None,
         diameter: Optional[float] = None,
         grade: Optional[str] = None,
         radius: Optional[float] = None,
+        chamfer: Optional[float] = None,
         width: Optional[float] = None,
         pitch: Optional[str] = None,
         length: Optional[float] = None,
         kapr: Optional[float] = None,
         teeth: Optional[int] = None,
         stick_out: Optional[float] = None,
         apmx: Optional[float] = None,
@@ -23945,14 +25281,16 @@
         :paramtype size: str
         :keyword diameter:
         :paramtype diameter: float
         :keyword grade:
         :paramtype grade: str
         :keyword radius:
         :paramtype radius: float
+        :keyword chamfer:
+        :paramtype chamfer: float
         :keyword width:
         :paramtype width: float
         :keyword pitch:
         :paramtype pitch: str
         :keyword length:
         :paramtype length: float
         :keyword kapr:
@@ -23974,14 +25312,15 @@
         self.description = description
         self.holder_description = holder_description
         self.geometry = geometry
         self.size = size
         self.diameter = diameter
         self.grade = grade
         self.radius = radius
+        self.chamfer = chamfer
         self.width = width
         self.pitch = pitch
         self.length = length
         self.kapr = kapr
         self.teeth = teeth
         self.stick_out = stick_out
         self.apmx = apmx
@@ -25035,14 +26374,40 @@
         :keyword elements:
         :paramtype elements: list[~ignos.api.client.models.SchemaInstanceElementDto]
         """
         super().__init__(**kwargs)
         self.elements = elements
 
 
+class UpdateTraceManualCompletionRequest(_serialization.Model):
+    """UpdateTraceManualCompletionRequest.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar completed: Required.
+    :vartype completed: bool
+    """
+
+    _validation = {
+        "completed": {"required": True},
+    }
+
+    _attribute_map = {
+        "completed": {"key": "completed", "type": "bool"},
+    }
+
+    def __init__(self, *, completed: bool, **kwargs: Any) -> None:
+        """
+        :keyword completed: Required.
+        :paramtype completed: bool
+        """
+        super().__init__(**kwargs)
+        self.completed = completed
+
+
 class UpdateTraceRequest(_serialization.Model):
     """UpdateTraceRequest.
 
     All required parameters must be populated in order to send to server.
 
     :ivar items: Required.
     :vartype items: list[~ignos.api.client.models.TraceItemDto]
@@ -25981,16 +27346,16 @@
     :vartype scrapped_quantity: float
     :ivar customer_order_reference:
     :vartype customer_order_reference: ~ignos.api.client.models.WorkorderCustomerOrderReferenceDto
     :ivar planner:
     :vartype planner: ~ignos.api.client.models.UserDto
     :ivar project_leader:
     :vartype project_leader: ~ignos.api.client.models.UserDto
-    :ivar end_location:
-    :vartype end_location: str
+    :ivar delivery_location:
+    :vartype delivery_location: ~ignos.api.client.models.WarehouseLocationDto
     :ivar project:
     :vartype project: ~ignos.api.client.models.WorkOrderProjectDto
     :ivar start_date:
     :vartype start_date: ~datetime.datetime
     :ivar end_date:
     :vartype end_date: ~datetime.datetime
     :ivar bom_position:
@@ -26018,15 +27383,15 @@
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
         "produced_quantity": {"key": "producedQuantity", "type": "float"},
         "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
         "customer_order_reference": {"key": "customerOrderReference", "type": "WorkorderCustomerOrderReferenceDto"},
         "planner": {"key": "planner", "type": "UserDto"},
         "project_leader": {"key": "projectLeader", "type": "UserDto"},
-        "end_location": {"key": "endLocation", "type": "str"},
+        "delivery_location": {"key": "deliveryLocation", "type": "WarehouseLocationDto"},
         "project": {"key": "project", "type": "WorkOrderProjectDto"},
         "start_date": {"key": "startDate", "type": "iso-8601"},
         "end_date": {"key": "endDate", "type": "iso-8601"},
         "bom_position": {"key": "bomPosition", "type": "str"},
         "trace_type": {"key": "traceType", "type": "str"},
     }
 
@@ -26043,15 +27408,15 @@
         planned_start: Optional[datetime.datetime] = None,
         planned_end: Optional[datetime.datetime] = None,
         produced_quantity: Optional[float] = None,
         scrapped_quantity: Optional[float] = None,
         customer_order_reference: Optional["_models.WorkorderCustomerOrderReferenceDto"] = None,
         planner: Optional["_models.UserDto"] = None,
         project_leader: Optional["_models.UserDto"] = None,
-        end_location: Optional[str] = None,
+        delivery_location: Optional["_models.WarehouseLocationDto"] = None,
         project: Optional["_models.WorkOrderProjectDto"] = None,
         start_date: Optional[datetime.datetime] = None,
         end_date: Optional[datetime.datetime] = None,
         bom_position: Optional[str] = None,
         trace_type: Optional[Union[str, "_models.TraceType"]] = None,
         **kwargs: Any
     ) -> None:
@@ -26082,16 +27447,16 @@
         :keyword customer_order_reference:
         :paramtype customer_order_reference:
          ~ignos.api.client.models.WorkorderCustomerOrderReferenceDto
         :keyword planner:
         :paramtype planner: ~ignos.api.client.models.UserDto
         :keyword project_leader:
         :paramtype project_leader: ~ignos.api.client.models.UserDto
-        :keyword end_location:
-        :paramtype end_location: str
+        :keyword delivery_location:
+        :paramtype delivery_location: ~ignos.api.client.models.WarehouseLocationDto
         :keyword project:
         :paramtype project: ~ignos.api.client.models.WorkOrderProjectDto
         :keyword start_date:
         :paramtype start_date: ~datetime.datetime
         :keyword end_date:
         :paramtype end_date: ~datetime.datetime
         :keyword bom_position:
@@ -26110,15 +27475,15 @@
         self.planned_start = planned_start
         self.planned_end = planned_end
         self.produced_quantity = produced_quantity
         self.scrapped_quantity = scrapped_quantity
         self.customer_order_reference = customer_order_reference
         self.planner = planner
         self.project_leader = project_leader
-        self.end_location = end_location
+        self.delivery_location = delivery_location
         self.project = project
         self.start_date = start_date
         self.end_date = end_date
         self.bom_position = bom_position
         self.trace_type = trace_type
 
 
@@ -26369,48 +27734,55 @@
 
     :ivar id:
     :vartype id: str
     :ivar full_name:
     :vartype full_name: str
     :ivar upn:
     :vartype upn: str
+    :ivar email:
+    :vartype email: str
     :ivar is_beta_tester:
     :vartype is_beta_tester: bool
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "full_name": {"key": "fullName", "type": "str"},
         "upn": {"key": "upn", "type": "str"},
+        "email": {"key": "email", "type": "str"},
         "is_beta_tester": {"key": "isBetaTester", "type": "bool"},
     }
 
     def __init__(
         self,
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         full_name: Optional[str] = None,
         upn: Optional[str] = None,
+        email: Optional[str] = None,
         is_beta_tester: Optional[bool] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword full_name:
         :paramtype full_name: str
         :keyword upn:
         :paramtype upn: str
+        :keyword email:
+        :paramtype email: str
         :keyword is_beta_tester:
         :paramtype is_beta_tester: bool
         """
         super().__init__(**kwargs)
         self.id = id
         self.full_name = full_name
         self.upn = upn
+        self.email = email
         self.is_beta_tester = is_beta_tester
 
 
 class UserDtoPagedResult(_serialization.Model):
     """UserDtoPagedResult.
 
     All required parameters must be populated in order to send to server.
@@ -26752,14 +28124,66 @@
         :paramtype name: str
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
 
 
+class WarehouseLocationDto(_serialization.Model):
+    """WarehouseLocationDto.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar zone:
+    :vartype zone: str
+    :ivar location: Required.
+    :vartype location: str
+    :ivar warehouse:
+    :vartype warehouse: str
+    :ivar site:
+    :vartype site: str
+    """
+
+    _validation = {
+        "location": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "zone": {"key": "zone", "type": "str"},
+        "location": {"key": "location", "type": "str"},
+        "warehouse": {"key": "warehouse", "type": "str"},
+        "site": {"key": "site", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: str,
+        zone: Optional[str] = None,
+        warehouse: Optional[str] = None,
+        site: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword zone:
+        :paramtype zone: str
+        :keyword location: Required.
+        :paramtype location: str
+        :keyword warehouse:
+        :paramtype warehouse: str
+        :keyword site:
+        :paramtype site: str
+        """
+        super().__init__(**kwargs)
+        self.zone = zone
+        self.location = location
+        self.warehouse = warehouse
+        self.site = site
+
+
 class WhitelistMeasuringTool(_serialization.Model):
     """WhitelistMeasuringTool.
 
     All required parameters must be populated in order to send to server.
 
     :ivar value: Required.
     :vartype value: str
@@ -26785,116 +28209,107 @@
         :paramtype description: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.description = description
 
 
-class WorkActivityDto(_serialization.Model):
-    """WorkActivityDto.
-
-    All required parameters must be populated in order to send to server.
+class WorkerDto(_serialization.Model):
+    """WorkerDto.
 
-    :ivar id: Required.
-    :vartype id: str
-    :ivar start_time: Required.
-    :vartype start_time: ~datetime.datetime
-    :ivar end_time:
-    :vartype end_time: ~datetime.datetime
-    :ivar user:
-    :vartype user: ~ignos.api.client.models.UserDto
-    :ivar personnel_number: Required.
+    :ivar personnel_number:
     :vartype personnel_number: str
-    :ivar work_type: Required. Known values are: "None", "Production", and "Setup".
-    :vartype work_type: str or ~ignos.api.client.models.WorkTypeDto
-    :ivar started_quantity:
-    :vartype started_quantity: int
+    :ivar badge_id:
+    :vartype badge_id: str
     """
 
-    _validation = {
-        "id": {"required": True, "min_length": 1},
-        "start_time": {"required": True},
-        "personnel_number": {"required": True, "min_length": 1},
-        "work_type": {"required": True},
-    }
-
     _attribute_map = {
-        "id": {"key": "id", "type": "str"},
-        "start_time": {"key": "startTime", "type": "iso-8601"},
-        "end_time": {"key": "endTime", "type": "iso-8601"},
-        "user": {"key": "user", "type": "UserDto"},
         "personnel_number": {"key": "personnelNumber", "type": "str"},
-        "work_type": {"key": "workType", "type": "str"},
-        "started_quantity": {"key": "startedQuantity", "type": "int"},
+        "badge_id": {"key": "badgeId", "type": "str"},
     }
 
     def __init__(
-        self,
-        *,
-        id: str,  # pylint: disable=redefined-builtin
-        start_time: datetime.datetime,
-        personnel_number: str,
-        work_type: Union[str, "_models.WorkTypeDto"],
-        end_time: Optional[datetime.datetime] = None,
-        user: Optional["_models.UserDto"] = None,
-        started_quantity: Optional[int] = None,
-        **kwargs: Any
+        self, *, personnel_number: Optional[str] = None, badge_id: Optional[str] = None, **kwargs: Any
     ) -> None:
         """
-        :keyword id: Required.
-        :paramtype id: str
-        :keyword start_time: Required.
-        :paramtype start_time: ~datetime.datetime
-        :keyword end_time:
-        :paramtype end_time: ~datetime.datetime
-        :keyword user:
-        :paramtype user: ~ignos.api.client.models.UserDto
-        :keyword personnel_number: Required.
+        :keyword personnel_number:
         :paramtype personnel_number: str
-        :keyword work_type: Required. Known values are: "None", "Production", and "Setup".
-        :paramtype work_type: str or ~ignos.api.client.models.WorkTypeDto
-        :keyword started_quantity:
-        :paramtype started_quantity: int
+        :keyword badge_id:
+        :paramtype badge_id: str
         """
         super().__init__(**kwargs)
-        self.id = id
-        self.start_time = start_time
-        self.end_time = end_time
-        self.user = user
         self.personnel_number = personnel_number
-        self.work_type = work_type
-        self.started_quantity = started_quantity
+        self.badge_id = badge_id
 
 
-class WorkerDto(_serialization.Model):
-    """WorkerDto.
+class WorkOrderAttachmentDto(_serialization.Model):
+    """WorkOrderAttachmentDto.
 
-    :ivar personnel_number:
-    :vartype personnel_number: str
-    :ivar badge_id:
-    :vartype badge_id: str
+    :ivar created_by:
+    :vartype created_by: ~ignos.api.client.models.UserDto
+    :ivar created:
+    :vartype created: ~datetime.datetime
+    :ivar modified_by:
+    :vartype modified_by: ~ignos.api.client.models.UserDto
+    :ivar modified:
+    :vartype modified: ~datetime.datetime
+    :ivar name:
+    :vartype name: str
+    :ivar notes:
+    :vartype notes: str
+    :ivar attachment_type:
+    :vartype attachment_type: str
     """
 
     _attribute_map = {
-        "personnel_number": {"key": "personnelNumber", "type": "str"},
-        "badge_id": {"key": "badgeId", "type": "str"},
+        "created_by": {"key": "createdBy", "type": "UserDto"},
+        "created": {"key": "created", "type": "iso-8601"},
+        "modified_by": {"key": "modifiedBy", "type": "UserDto"},
+        "modified": {"key": "modified", "type": "iso-8601"},
+        "name": {"key": "name", "type": "str"},
+        "notes": {"key": "notes", "type": "str"},
+        "attachment_type": {"key": "attachmentType", "type": "str"},
     }
 
     def __init__(
-        self, *, personnel_number: Optional[str] = None, badge_id: Optional[str] = None, **kwargs: Any
+        self,
+        *,
+        created_by: Optional["_models.UserDto"] = None,
+        created: Optional[datetime.datetime] = None,
+        modified_by: Optional["_models.UserDto"] = None,
+        modified: Optional[datetime.datetime] = None,
+        name: Optional[str] = None,
+        notes: Optional[str] = None,
+        attachment_type: Optional[str] = None,
+        **kwargs: Any
     ) -> None:
         """
-        :keyword personnel_number:
-        :paramtype personnel_number: str
-        :keyword badge_id:
-        :paramtype badge_id: str
+        :keyword created_by:
+        :paramtype created_by: ~ignos.api.client.models.UserDto
+        :keyword created:
+        :paramtype created: ~datetime.datetime
+        :keyword modified_by:
+        :paramtype modified_by: ~ignos.api.client.models.UserDto
+        :keyword modified:
+        :paramtype modified: ~datetime.datetime
+        :keyword name:
+        :paramtype name: str
+        :keyword notes:
+        :paramtype notes: str
+        :keyword attachment_type:
+        :paramtype attachment_type: str
         """
         super().__init__(**kwargs)
-        self.personnel_number = personnel_number
-        self.badge_id = badge_id
+        self.created_by = created_by
+        self.created = created
+        self.modified_by = modified_by
+        self.modified = modified
+        self.name = name
+        self.notes = notes
+        self.attachment_type = attachment_type
 
 
 class WorkOrderConsumptionDto(_serialization.Model):
     """WorkOrderConsumptionDto.
 
     All required parameters must be populated in order to send to server.
 
@@ -27507,14 +28922,18 @@
     :vartype fixed_time: bool
     :ivar resource:
     :vartype resource: ~ignos.api.client.models.ResourceDto
     :ivar planned_start:
     :vartype planned_start: ~datetime.datetime
     :ivar planned_end:
     :vartype planned_end: ~datetime.datetime
+    :ivar actual_start:
+    :vartype actual_start: ~datetime.datetime
+    :ivar actual_end:
+    :vartype actual_end: ~datetime.datetime
     :ivar status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
      "Stopped".
     :vartype status: str or ~ignos.api.client.models.OperationStatusDto
     :ivar produced_quantity: Required.
     :vartype produced_quantity: float
     :ivar scrapped_quantity: Required.
     :vartype scrapped_quantity: float
@@ -27545,14 +28964,16 @@
         "planned_setup_time": {"key": "plannedSetupTime", "type": "float"},
         "planned_production_time_per_part": {"key": "plannedProductionTimePerPart", "type": "float"},
         "planned_production_time": {"key": "plannedProductionTime", "type": "float"},
         "fixed_time": {"key": "fixedTime", "type": "bool"},
         "resource": {"key": "resource", "type": "ResourceDto"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
+        "actual_start": {"key": "actualStart", "type": "iso-8601"},
+        "actual_end": {"key": "actualEnd", "type": "iso-8601"},
         "status": {"key": "status", "type": "str"},
         "produced_quantity": {"key": "producedQuantity", "type": "float"},
         "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
         "used_production_time": {"key": "usedProductionTime", "type": "float"},
         "used_setup_time": {"key": "usedSetupTime", "type": "float"},
         "materials": {"key": "materials", "type": "[WorkorderMaterialDto]"},
     }
@@ -27571,14 +28992,16 @@
         used_setup_time: float,
         materials: List["_models.WorkorderMaterialDto"],
         description: Optional[str] = None,
         fixed_time: Optional[bool] = None,
         resource: Optional["_models.ResourceDto"] = None,
         planned_start: Optional[datetime.datetime] = None,
         planned_end: Optional[datetime.datetime] = None,
+        actual_start: Optional[datetime.datetime] = None,
+        actual_end: Optional[datetime.datetime] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword operation: Required.
         :paramtype operation: int
         :keyword description:
         :paramtype description: str
@@ -27592,14 +29015,18 @@
         :paramtype fixed_time: bool
         :keyword resource:
         :paramtype resource: ~ignos.api.client.models.ResourceDto
         :keyword planned_start:
         :paramtype planned_start: ~datetime.datetime
         :keyword planned_end:
         :paramtype planned_end: ~datetime.datetime
+        :keyword actual_start:
+        :paramtype actual_start: ~datetime.datetime
+        :keyword actual_end:
+        :paramtype actual_end: ~datetime.datetime
         :keyword status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
          "Stopped".
         :paramtype status: str or ~ignos.api.client.models.OperationStatusDto
         :keyword produced_quantity: Required.
         :paramtype produced_quantity: float
         :keyword scrapped_quantity: Required.
         :paramtype scrapped_quantity: float
@@ -27616,14 +29043,16 @@
         self.planned_setup_time = planned_setup_time
         self.planned_production_time_per_part = planned_production_time_per_part
         self.planned_production_time = planned_production_time
         self.fixed_time = fixed_time
         self.resource = resource
         self.planned_start = planned_start
         self.planned_end = planned_end
+        self.actual_start = actual_start
+        self.actual_end = actual_end
         self.status = status
         self.produced_quantity = produced_quantity
         self.scrapped_quantity = scrapped_quantity
         self.used_production_time = used_production_time
         self.used_setup_time = used_setup_time
         self.materials = materials
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/models/_patch.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/operations/__init__.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import AlertsOperations
 from ._operations import AssetsOperations
 from ._operations import AzureRegionsOperations
+from ._operations import BookingOperations
 from ._operations import CdfOperations
 from ._operations import CncFileTransferOperations
 from ._operations import CncSetupOperations
 from ._operations import CncSetupAgentOperations
 from ._operations import CountriesOperations
 from ._operations import CustomersOperations
 from ._operations import DocumentsOperations
@@ -23,14 +24,15 @@
 from ._operations import WorkordersOperations
 from ._operations import ExternalOperations
 from ._operations import ExternalAccessOperations
 from ._operations import ExternalServicesOperations
 from ._operations import ElectricalOperations
 from ._operations import WeldingOperations
 from ._operations import LinksOperations
+from ._operations import LocationsOperations
 from ._operations import MachineAlarmsOperations
 from ._operations import MachinesOperations
 from ._operations import MachineUtilizationOperations
 from ._operations import MeOperations
 from ._operations import MeasurementFormSchemasOperations
 from ._operations import MeasurementFormsInstancesOperations
 from ._operations import MeasuringToolsOperations
@@ -45,28 +47,30 @@
 from ._operations import OperatorCalculatorsOperations
 from ._operations import PowerOperations
 from ._operations import PresentationOperations
 from ._operations import SuppliersOperations
 from ._operations import SustainabilityOperations
 from ._operations import SystemHealthDashboardOperations
 from ._operations import TraceOperations
+from ._operations import TrackingOperations
 from ._operations import UploadOperations
 from ._operations import UsersOperations
 from ._operations import WorkspacesOperations
 from ._operations import WorkspaceTemplatesAdminOperations
 from ._operations import WorkspaceTemplatesOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AlertsOperations",
     "AssetsOperations",
     "AzureRegionsOperations",
+    "BookingOperations",
     "CdfOperations",
     "CncFileTransferOperations",
     "CncSetupOperations",
     "CncSetupAgentOperations",
     "CountriesOperations",
     "CustomersOperations",
     "DocumentsOperations",
@@ -77,14 +81,15 @@
     "WorkordersOperations",
     "ExternalOperations",
     "ExternalAccessOperations",
     "ExternalServicesOperations",
     "ElectricalOperations",
     "WeldingOperations",
     "LinksOperations",
+    "LocationsOperations",
     "MachineAlarmsOperations",
     "MachinesOperations",
     "MachineUtilizationOperations",
     "MeOperations",
     "MeasurementFormSchemasOperations",
     "MeasurementFormsInstancesOperations",
     "MeasuringToolsOperations",
@@ -99,14 +104,15 @@
     "OperatorCalculatorsOperations",
     "PowerOperations",
     "PresentationOperations",
     "SuppliersOperations",
     "SustainabilityOperations",
     "SystemHealthDashboardOperations",
     "TraceOperations",
+    "TrackingOperations",
     "UploadOperations",
     "UsersOperations",
     "WorkspacesOperations",
     "WorkspaceTemplatesAdminOperations",
     "WorkspaceTemplatesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/operations/_operations.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import datetime
 from io import IOBase
 import sys
-from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
+from typing import Any, Callable, Dict, IO, List, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -304,14 +304,125 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
+def build_booking_list_bookings_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/move/booking/list"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_booking_get_booking_request(booking_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/move/booking/{bookingId}"
+    path_format_arguments = {
+        "bookingId": _SERIALIZER.url("booking_id", booking_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_booking_update_booking_request(booking_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/move/booking/{bookingId}"
+    path_format_arguments = {
+        "bookingId": _SERIALIZER.url("booking_id", booking_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
+def build_booking_create_booking_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/move/booking/book"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_booking_cancel_booking_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/move/booking/cancel"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_booking_start_delivery_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/move/booking/startdelivery"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_booking_finish_delivery_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/move/booking/finishdelivery"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 def build_cdf_get_cdf_config_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/admin/cdf/config"
@@ -457,14 +568,33 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_cnc_file_transfer_start_cam_transfer_to_machine_from_temp_upload_request(  # pylint: disable=name-too-long
+    **kwargs: Any,
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/cncfiletransfer/transfers/tempcamfile"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 def build_cnc_setup_get_cnc_machine_request(id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/cncsetup/machines/{id}"
@@ -1008,14 +1138,31 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_cnc_setup_copy_tools_cnc_machine_request(**kwargs: Any) -> HttpRequest:  # pylint: disable=name-too-long
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/cncsetup/operations/copytoolscncmachine"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 def build_cnc_setup_create_upload_programs_info_request(  # pylint: disable=name-too-long
     id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
@@ -1474,14 +1621,55 @@
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     return HttpRequest(method="DELETE", url=_url, **kwargs)
 
 
+def build_cnc_setup_upload_cnc_machine_tool_image_request(  # pylint: disable=name-too-long
+    machine_id: str, id: int, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/cncsetup/machines/{machineId}/tools/{id}/uploadimage"
+    path_format_arguments = {
+        "machineId": _SERIALIZER.url("machine_id", machine_id, "str"),
+        "id": _SERIALIZER.url("id", id, "int"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_cnc_setup_delete_cnc_machine_tool_image_request(  # pylint: disable=name-too-long
+    machine_id: str, id: int, filename: str, **kwargs: Any
+) -> HttpRequest:
+    # Construct URL
+    _url = "/cncsetup/machines/{machineId}/tools/{id}/{filename}"
+    path_format_arguments = {
+        "machineId": _SERIALIZER.url("machine_id", machine_id, "str"),
+        "id": _SERIALIZER.url("id", id, "int"),
+        "filename": _SERIALIZER.url("filename", filename, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    return HttpRequest(method="DELETE", url=_url, **kwargs)
+
+
 def build_cnc_setup_import_operation_with_tools_request(**kwargs: Any) -> HttpRequest:  # pylint: disable=name-too-long
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     # Construct URL
     _url = "/cncsetup/import"
 
@@ -2581,14 +2769,42 @@
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_workorders_delete_work_order_mappings_request(**kwargs: Any) -> HttpRequest:  # pylint: disable=name-too-long
+    # Construct URL
+    _url = "/erp/workorders/mappings"
+
+    return HttpRequest(method="DELETE", url=_url, **kwargs)
+
+
+def build_workorders_search_work_orders_request(  # pylint: disable=name-too-long
+    *, input: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/move/workorders/search"
+
+    # Construct parameters
+    if input is not None:
+        _params["input"] = _SERIALIZER.query("input", input, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 def build_external_list_invites_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/external/invites"
@@ -2965,14 +3181,66 @@
     # Construct parameters
     if scope is not None:
         _params["scope"] = _SERIALIZER.query("scope", scope, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, **kwargs)
 
 
+def build_locations_search_locations_request(
+    *,
+    input: Optional[str] = None,
+    location_kinds: Optional[List[Union[str, _models.LocationKindDto]]] = None,
+    **kwargs: Any,
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/move/locations/search"
+
+    # Construct parameters
+    if input is not None:
+        _params["input"] = _SERIALIZER.query("input", input, "str")
+    if location_kinds is not None:
+        _params["locationKinds"] = _SERIALIZER.query("location_kinds", location_kinds, "[str]")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_locations_suggestions_locations_request(  # pylint: disable=name-too-long
+    *,
+    work_order_id: Optional[str] = None,
+    location_kinds: Optional[List[Union[str, _models.LocationKindDto]]] = None,
+    **kwargs: Any,
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/move/locations/suggestions"
+
+    # Construct parameters
+    if work_order_id is not None:
+        _params["workOrderId"] = _SERIALIZER.query("work_order_id", work_order_id, "str")
+    if location_kinds is not None:
+        _params["locationKinds"] = _SERIALIZER.query("location_kinds", location_kinds, "[str]")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 def build_machine_alarms_list_machine_alarms_request(  # pylint: disable=name-too-long
     *,
     alarm_type: Optional[Union[str, _models.MachineAlarmType]] = None,
     asset_id: Optional[int] = None,
     start_time: Optional[datetime.datetime] = None,
     end_time: Optional[datetime.datetime] = None,
     sub_type: Optional[str] = None,
@@ -3373,14 +3641,60 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_machines_create_machine_without_resource_request(  # pylint: disable=name-too-long
+    **kwargs: Any,
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/machines/machine-without-resource"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_machines_create_resource_without_machine_request(  # pylint: disable=name-too-long
+    **kwargs: Any,
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/machines/resource-without-machine"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_machines_create_resource_with_machine_request(**kwargs: Any) -> HttpRequest:  # pylint: disable=name-too-long
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/machines/resource-with-machine"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 def build_machine_utilization_get_machine_utilizations_request(  # pylint: disable=name-too-long
     *,
     asset_id: Optional[int] = None,
     favorites: bool = False,
     start_time_today: Optional[datetime.datetime] = None,
     utc_offset: Optional[float] = None,
     **kwargs: Any,
@@ -6236,41 +6550,55 @@
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
 def build_mes_links_list_mes_links_request(
     *,
-    company_id: Optional[str] = None,
-    type: Optional[Union[str, _models.MesLinkTypeDto]] = None,
-    operation_id: Optional[str] = None,
+    types: Optional[List[Union[str, _models.MesLinkTypeDto]]] = None,
+    work_order_id: Optional[str] = None,
+    operation: Optional[int] = None,
     **kwargs: Any,
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/mes/links"
 
     # Construct parameters
-    if company_id is not None:
-        _params["companyId"] = _SERIALIZER.query("company_id", company_id, "str")
-    if type is not None:
-        _params["type"] = _SERIALIZER.query("type", type, "str")
-    if operation_id is not None:
-        _params["operationId"] = _SERIALIZER.query("operation_id", operation_id, "str")
+    if types is not None:
+        _params["types"] = _SERIALIZER.query("types", types, "[str]")
+    if work_order_id is not None:
+        _params["workOrderId"] = _SERIALIZER.query("work_order_id", work_order_id, "str")
+    if operation is not None:
+        _params["operation"] = _SERIALIZER.query("operation", operation, "int")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_mes_links_list_unmapped_mes_links_request(**kwargs: Any) -> HttpRequest:  # pylint: disable=name-too-long
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/mes/links/unmapped"
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
 def build_mes_links_update_mes_link_request(id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     # Construct URL
     _url = "/mes/links/{id}"
     path_format_arguments = {
@@ -6439,14 +6767,40 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_mes_production_order_list_production_order_activities_request(  # pylint: disable=name-too-long
+    id: str, *, operation: Optional[int] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/mes/productionorders/{id}/activities"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    if operation is not None:
+        _params["operation"] = _SERIALIZER.query("operation", operation, "int")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 def build_mes_production_schedule_list_production_schedule_operations_request(  # pylint: disable=name-too-long
     *,
     resource_group: Optional[str] = None,
     resource_id: Optional[str] = None,
     page_size: int = 50,
     continuation_token_parameter: Optional[str] = None,
     work_order_id: Optional[str] = None,
@@ -7671,14 +8025,35 @@
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     return HttpRequest(method="POST", url=_url, **kwargs)
 
 
+def build_trace_set_trace_manual_completed_request(  # pylint: disable=name-too-long
+    id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/trace/{id}/manualcompleted"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
 def build_trace_list_customer_order_line_traces_request(  # pylint: disable=name-too-long
     *, customer_order: Optional[str] = None, customer_order_line: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
@@ -7774,14 +8149,118 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_tracking_list_tracking_history_request(  # pylint: disable=name-too-long
+    tracking_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/move/tracking/{trackingId}"
+    path_format_arguments = {
+        "trackingId": _SERIALIZER.url("tracking_id", tracking_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_tracking_list_work_order_tracking_history_request(  # pylint: disable=name-too-long
+    work_order_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/move/tracking/workorder/{workOrderId}"
+    path_format_arguments = {
+        "workOrderId": _SERIALIZER.url("work_order_id", work_order_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_tracking_create_tracking_events_request(**kwargs: Any) -> HttpRequest:  # pylint: disable=name-too-long
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/move/tracking/event"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_tracking_create_tracking_history_request(**kwargs: Any) -> HttpRequest:  # pylint: disable=name-too-long
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/move/tracking/history"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_tracking_delete_tracking_history_request(**kwargs: Any) -> HttpRequest:  # pylint: disable=name-too-long
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/move/tracking/history"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="DELETE", url=_url, headers=_headers, **kwargs)
+
+
+def build_tracking_create_label_request(
+    work_order_id: str, *, pallet_count: Optional[int] = None, **kwargs: Any
+) -> HttpRequest:
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    # Construct URL
+    _url = "/move/tracking/{workOrderId}/label"
+    path_format_arguments = {
+        "workOrderId": _SERIALIZER.url("work_order_id", work_order_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    if pallet_count is not None:
+        _params["palletCount"] = _SERIALIZER.query("pallet_count", pallet_count, "int")
+
+    return HttpRequest(method="POST", url=_url, params=_params, **kwargs)
+
+
 def build_upload_create_upload_info_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/upload"
@@ -8202,15 +8681,15 @@
     def alert_notification_access(self, **kwargs: Any) -> _models.AlertNotificationAccessDto:
         """alert_notification_access.
 
         :return: AlertNotificationAccessDto
         :rtype: ~ignos.api.client.models.AlertNotificationAccessDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8249,15 +8728,15 @@
     def get_machine_inactivity_alert_type(self, **kwargs: Any) -> _models.MachineInactivityAlertTypeDto:
         """get_machine_inactivity_alert_type.
 
         :return: MachineInactivityAlertTypeDto
         :rtype: ~ignos.api.client.models.MachineInactivityAlertTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8298,15 +8777,15 @@
     ) -> List[_models.MachineInactivityCriteriaDtoAlertSubscriptionDto]:
         """list_machine_inactivity_subscriptions.
 
         :return: list of MachineInactivityCriteriaDtoAlertSubscriptionDto
         :rtype: list[~ignos.api.client.models.MachineInactivityCriteriaDtoAlertSubscriptionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8387,15 +8866,15 @@
         :param body: Is either a SubscribeToMachineInactivityAlerts type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.SubscribeToMachineInactivityAlerts or IO[bytes]
         :return: MachineInactivityCriteriaDtoAlertSubscriptionDto
         :rtype: ~ignos.api.client.models.MachineInactivityCriteriaDtoAlertSubscriptionDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8501,15 +8980,15 @@
         :param body: Is either a UpdateMachineInactivitySubscription type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateMachineInactivitySubscription or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8564,15 +9043,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8647,15 +9126,15 @@
         :paramtype limit: int
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: AssetDtoPagedResult
         :rtype: ~ignos.api.client.models.AssetDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8736,15 +9215,15 @@
 
         :param body: Is either a CreateAsset type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateAsset or IO[bytes]
         :return: AssetDto
         :rtype: ~ignos.api.client.models.AssetDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8806,15 +9285,15 @@
         :paramtype description: str
         :keyword limit: Default value is 100.
         :paramtype limit: int
         :return: list of AssetDto
         :rtype: list[~ignos.api.client.models.AssetDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8858,15 +9337,15 @@
 
         :param id: Required.
         :type id: int
         :return: AssetDto
         :rtype: ~ignos.api.client.models.AssetDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8954,15 +9433,15 @@
         :type id: int
         :param body: Is either a UpdateAssetRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateAssetRequest or IO[bytes]
         :return: AssetDto
         :rtype: ~ignos.api.client.models.AssetDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9019,15 +9498,15 @@
 
         :param id: Required.
         :type id: int
         :return: AssetStructureDto
         :rtype: ~ignos.api.client.models.AssetStructureDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9067,15 +9546,15 @@
     def list_machines(self, **kwargs: Any) -> List[_models.MachineDto]:
         """list_machines.
 
         :return: list of MachineDto
         :rtype: list[~ignos.api.client.models.MachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9134,15 +9613,15 @@
     def list_azure_regions(self, **kwargs: Any) -> List[_models.AzureRegionDto]:
         """list_azure_regions.
 
         :return: list of AzureRegionDto
         :rtype: list[~ignos.api.client.models.AzureRegionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9174,14 +9653,684 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
 
+class BookingOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.IgnosPortal`'s
+        :attr:`booking` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    def list_bookings(
+        self,
+        body: Optional[_models.BookingRequestListDto] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> _models.BookingResponseListDto:
+        """list_bookings.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestListDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: BookingResponseListDto
+        :rtype: ~ignos.api.client.models.BookingResponseListDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def list_bookings(
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.BookingResponseListDto:
+        """list_bookings.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: BookingResponseListDto
+        :rtype: ~ignos.api.client.models.BookingResponseListDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def list_bookings(
+        self, body: Optional[Union[_models.BookingRequestListDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> _models.BookingResponseListDto:
+        """list_bookings.
+
+        :param body: Is either a BookingRequestListDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestListDto or IO[bytes]
+        :return: BookingResponseListDto
+        :rtype: ~ignos.api.client.models.BookingResponseListDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.BookingResponseListDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingRequestListDto")
+            else:
+                _json = None
+
+        _request = build_booking_list_bookings_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("BookingResponseListDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace
+    def get_booking(self, booking_id: str, **kwargs: Any) -> _models.BookingResponseDto:
+        """get_booking.
+
+        :param booking_id: Required.
+        :type booking_id: str
+        :return: BookingResponseDto
+        :rtype: ~ignos.api.client.models.BookingResponseDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.BookingResponseDto] = kwargs.pop("cls", None)
+
+        _request = build_booking_get_booking_request(
+            booking_id=booking_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("BookingResponseDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    def update_booking(  # pylint: disable=inconsistent-return-statements
+        self,
+        booking_id: str,
+        body: Optional[_models.BookingRequestDto] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """update_booking.
+
+        :param booking_id: Required.
+        :type booking_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def update_booking(  # pylint: disable=inconsistent-return-statements
+        self,
+        booking_id: str,
+        body: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """update_booking.
+
+        :param booking_id: Required.
+        :type booking_id: str
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def update_booking(  # pylint: disable=inconsistent-return-statements
+        self, booking_id: str, body: Optional[Union[_models.BookingRequestDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """update_booking.
+
+        :param booking_id: Required.
+        :type booking_id: str
+        :param body: Is either a BookingRequestDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingRequestDto")
+            else:
+                _json = None
+
+        _request = build_booking_update_booking_request(
+            booking_id=booking_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    def create_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[_models.BookingRequestDto] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_booking.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_booking.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.BookingRequestDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_booking.
+
+        :param body: Is either a BookingRequestDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingRequestDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingRequestDto")
+            else:
+                _json = None
+
+        _request = build_booking_create_booking_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    def cancel_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[_models.BookingUpdateDto] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """cancel_booking.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingUpdateDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def cancel_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """cancel_booking.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def cancel_booking(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.BookingUpdateDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """cancel_booking.
+
+        :param body: Is either a BookingUpdateDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingUpdateDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingUpdateDto")
+            else:
+                _json = None
+
+        _request = build_booking_cancel_booking_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    def start_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[_models.BookingUpdateDto] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """start_delivery.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingUpdateDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def start_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """start_delivery.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def start_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.BookingUpdateDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """start_delivery.
+
+        :param body: Is either a BookingUpdateDto type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.BookingUpdateDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingUpdateDto")
+            else:
+                _json = None
+
+        _request = build_booking_start_delivery_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    def finish_delivery(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.BookingDeliveryUpdateDto] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """finish_delivery.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.BookingDeliveryUpdateDto
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def finish_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """finish_delivery.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def finish_delivery(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.BookingDeliveryUpdateDto, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """finish_delivery.
+
+        :param body: Is either a BookingDeliveryUpdateDto type or a IO[bytes] type. Default value is
+         None.
+        :type body: ~ignos.api.client.models.BookingDeliveryUpdateDto or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "BookingDeliveryUpdateDto")
+            else:
+                _json = None
+
+        _request = build_booking_finish_delivery_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+
 class CdfOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.IgnosPortal`'s
@@ -9203,15 +10352,15 @@
 
         Get CDF config.
 
         :return: CdfConfigDto
         :rtype: ~ignos.api.client.models.CdfConfigDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9293,15 +10442,15 @@
 
         :param body: Is either a UpdateCdfConfig type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateCdfConfig or IO[bytes]
         :return: CdfConfigDto
         :rtype: ~ignos.api.client.models.CdfConfigDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9379,15 +10528,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineTransferDto
         :rtype: ~ignos.api.client.models.CncMachineTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9431,15 +10580,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineTransferDto
         :rtype: ~ignos.api.client.models.CncMachineTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9481,15 +10630,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineTransferDto
         :rtype: ~ignos.api.client.models.CncMachineTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9570,15 +10719,15 @@
 
         :param body: Is either a UploadCamFileRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadCamFileRequest or IO[bytes]
         :return: UploadCamFileDto
         :rtype: ~ignos.api.client.models.UploadCamFileDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9634,15 +10783,15 @@
 
         :keyword path: Default value is None.
         :paramtype path: str
         :return: CamTransferDto
         :rtype: ~ignos.api.client.models.CamTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9724,15 +10873,15 @@
         :param body: Is either a StartCamTransferToMachine type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StartCamTransferToMachine or IO[bytes]
         :return: CncMachineTransferDto
         :rtype: ~ignos.api.client.models.CncMachineTransferDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9778,14 +10927,118 @@
         deserialized = self._deserialize("CncMachineTransferDto", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
+    @overload
+    def start_cam_transfer_to_machine_from_temp_upload(  # pylint: disable=name-too-long
+        self,
+        body: Optional[_models.StartCamTransferToMachineFromTempUpload] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> _models.CncMachineTransferDto:
+        """start_cam_transfer_to_machine_from_temp_upload.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.StartCamTransferToMachineFromTempUpload
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: CncMachineTransferDto
+        :rtype: ~ignos.api.client.models.CncMachineTransferDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def start_cam_transfer_to_machine_from_temp_upload(  # pylint: disable=name-too-long
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.CncMachineTransferDto:
+        """start_cam_transfer_to_machine_from_temp_upload.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: CncMachineTransferDto
+        :rtype: ~ignos.api.client.models.CncMachineTransferDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def start_cam_transfer_to_machine_from_temp_upload(  # pylint: disable=name-too-long
+        self, body: Optional[Union[_models.StartCamTransferToMachineFromTempUpload, IO[bytes]]] = None, **kwargs: Any
+    ) -> _models.CncMachineTransferDto:
+        """start_cam_transfer_to_machine_from_temp_upload.
+
+        :param body: Is either a StartCamTransferToMachineFromTempUpload type or a IO[bytes] type.
+         Default value is None.
+        :type body: ~ignos.api.client.models.StartCamTransferToMachineFromTempUpload or IO[bytes]
+        :return: CncMachineTransferDto
+        :rtype: ~ignos.api.client.models.CncMachineTransferDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CncMachineTransferDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StartCamTransferToMachineFromTempUpload")
+            else:
+                _json = None
+
+        _request = build_cnc_file_transfer_start_cam_transfer_to_machine_from_temp_upload_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("CncMachineTransferDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
 
 class CncSetupOperations:  # pylint: disable=too-many-public-methods
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -9808,15 +11061,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineDto
         :rtype: ~ignos.api.client.models.CncMachineDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9905,15 +11158,15 @@
         :param body: Is either a UpdateCncMachineRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateCncMachineRequest or IO[bytes]
         :return: CncMachineDto
         :rtype: ~ignos.api.client.models.CncMachineDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9970,15 +11223,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10016,15 +11269,15 @@
 
         :keyword name_prefix: Default value is None.
         :paramtype name_prefix: str
         :return: list of CncMachineDto
         :rtype: list[~ignos.api.client.models.CncMachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10101,15 +11354,15 @@
 
         :param body: Is either a CreateCncMachine type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateCncMachine or IO[bytes]
         :return: CncMachineDto
         :rtype: ~ignos.api.client.models.CncMachineDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10167,15 +11420,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineCommunicationSettingsDto
         :rtype: ~ignos.api.client.models.CncMachineCommunicationSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10267,15 +11520,15 @@
         :param body: Is either a UpdateCncMachineCommunicationSettingsRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpdateCncMachineCommunicationSettingsRequest or IO[bytes]
         :return: CncMachineCommunicationSettingsDto
         :rtype: ~ignos.api.client.models.CncMachineCommunicationSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10334,15 +11587,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10415,15 +11668,15 @@
 
         :param body: Is either a CreateCncPart type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateCncPart or IO[bytes]
         :return: CncPartDto
         :rtype: ~ignos.api.client.models.CncPartDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10518,15 +11771,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: CncPartListDtoPagedResult
         :rtype: ~ignos.api.client.models.CncPartListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10625,15 +11878,15 @@
         :type id: str
         :param body: Is either a UpdateCncPartRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateCncPartRequest or IO[bytes]
         :return: CncPartDto
         :rtype: ~ignos.api.client.models.CncPartDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10690,15 +11943,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10736,15 +11989,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncPartDto
         :rtype: ~ignos.api.client.models.CncPartDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10825,15 +12078,15 @@
 
         :param body: Is either a ListCncPartsRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListCncPartsRequest or IO[bytes]
         :return: CncPartListDtoPagedResult
         :rtype: ~ignos.api.client.models.CncPartListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10924,15 +12177,15 @@
 
         :param body: Is either a CopyCncPart type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CopyCncPart or IO[bytes]
         :return: CncPartDto
         :rtype: ~ignos.api.client.models.CncPartDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11035,15 +12288,15 @@
         :param body: Is either a UploadPartDrawingRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UploadPartDrawingRequest or IO[bytes]
         :return: UploadFileDto
         :rtype: ~ignos.api.client.models.UploadFileDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11100,15 +12353,15 @@
 
         :param id: Required.
         :type id: str
         :return: FileDto
         :rtype: ~ignos.api.client.models.FileDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11197,15 +12450,15 @@
         :param body: Is either a DeletePartDrawingRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.DeletePartDrawingRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11298,15 +12551,15 @@
         :param body: Is either a CreateCncMachineOperation type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateCncMachineOperation or IO[bytes]
         :return: CncMachineOperationDto
         :rtype: ~ignos.api.client.models.CncMachineOperationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11404,15 +12657,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: CncMachineOperationSearchResultDtoPagedResult
         :rtype: ~ignos.api.client.models.CncMachineOperationSearchResultDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11506,15 +12759,15 @@
         :param body: Is either a ListCncMachineOperationsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ListCncMachineOperationsRequest or IO[bytes]
         :return: CncMachineOperationSearchResultDtoPagedResult
         :rtype: ~ignos.api.client.models.CncMachineOperationSearchResultDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11617,15 +12870,15 @@
         :param body: Is either a UpdateCncMachineOperationRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateCncMachineOperationRequest or IO[bytes]
         :return: CncMachineOperationDto
         :rtype: ~ignos.api.client.models.CncMachineOperationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11682,15 +12935,15 @@
 
         :param id: Required.
         :type id: str
         :return: CncMachineOperationDto
         :rtype: ~ignos.api.client.models.CncMachineOperationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11734,15 +12987,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11820,15 +13073,15 @@
         :param body: Is either a CopyCncMachineOperations type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CopyCncMachineOperations or IO[bytes]
         :return: list of CncMachineOperationDto
         :rtype: list[~ignos.api.client.models.CncMachineOperationDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11875,14 +13128,117 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
+    def copy_tools_cnc_machine(
+        self,
+        body: Optional[_models.CopyToolsCncMachine] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> List[_models.CncToolDto]:
+        """copy_tools_cnc_machine.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CopyToolsCncMachine
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: list of CncToolDto
+        :rtype: list[~ignos.api.client.models.CncToolDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def copy_tools_cnc_machine(
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> List[_models.CncToolDto]:
+        """copy_tools_cnc_machine.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: list of CncToolDto
+        :rtype: list[~ignos.api.client.models.CncToolDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def copy_tools_cnc_machine(
+        self, body: Optional[Union[_models.CopyToolsCncMachine, IO[bytes]]] = None, **kwargs: Any
+    ) -> List[_models.CncToolDto]:
+        """copy_tools_cnc_machine.
+
+        :param body: Is either a CopyToolsCncMachine type or a IO[bytes] type. Default value is None.
+        :type body: ~ignos.api.client.models.CopyToolsCncMachine or IO[bytes]
+        :return: list of CncToolDto
+        :rtype: list[~ignos.api.client.models.CncToolDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[List[_models.CncToolDto]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CopyToolsCncMachine")
+            else:
+                _json = None
+
+        _request = build_cnc_setup_copy_tools_cnc_machine_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[CncToolDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
     def create_upload_programs_info(
         self,
         id: str,
         body: Optional[_models.UploadFileRequest] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any,
@@ -11930,15 +13286,15 @@
         :type id: str
         :param body: Is either a UploadFileRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadFileRequest or IO[bytes]
         :return: list of UploadFileDto
         :rtype: list[~ignos.api.client.models.UploadFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12000,15 +13356,15 @@
         :keyword filter_deleted: Known values are: "NoneDeleted", "OnlyDeleted", and "All". Default
          value is None.
         :paramtype filter_deleted: str or ~ignos.api.client.models.CncFilterDeletedDto
         :return: list of ProgramFileDto
         :rtype: list[~ignos.api.client.models.ProgramFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12063,15 +13419,15 @@
         :keyword filter_deleted: Known values are: "NoneDeleted", "OnlyDeleted", and "All". Default
          value is None.
         :paramtype filter_deleted: str or ~ignos.api.client.models.CncFilterDeletedDto
         :return: list of ProgramFileDto
         :rtype: list[~ignos.api.client.models.ProgramFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12179,15 +13535,15 @@
         :param body: Is either a UpdateProgramFileRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateProgramFileRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12245,15 +13601,15 @@
         :type id: str
         :param filename: Required.
         :type filename: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12365,15 +13721,15 @@
         :param body: Is either a UpdateProgramFileRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateProgramFileRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12434,15 +13790,15 @@
         :type filename: str
         :param version_id: Required.
         :type version_id: int
         :return: list of ProgramFileDto
         :rtype: list[~ignos.api.client.models.ProgramFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12532,15 +13888,15 @@
         :type id: str
         :param body: Is either a UploadFileRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadFileRequest or IO[bytes]
         :return: list of UploadFileDto
         :rtype: list[~ignos.api.client.models.UploadFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12597,15 +13953,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of FileDto
         :rtype: list[~ignos.api.client.models.FileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12651,15 +14007,15 @@
         :type operation_id: str
         :param filename: Required.
         :type filename: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12698,15 +14054,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of CncMachineOperationDto
         :rtype: list[~ignos.api.client.models.CncMachineOperationDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12746,15 +14102,15 @@
     def list_cnc_tool_types(self, **kwargs: Any) -> List[_models.CncToolTypeDto]:
         """list_cnc_tool_types.
 
         :return: list of CncToolTypeDto
         :rtype: list[~ignos.api.client.models.CncToolTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12845,15 +14201,15 @@
         :param body: Is either a CreateCncMachineOperationToolRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateCncMachineOperationToolRequest or IO[bytes]
         :return: CncToolDto
         :rtype: ~ignos.api.client.models.CncToolDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12910,15 +14266,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of CncToolDto
         :rtype: list[~ignos.api.client.models.CncToolDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13024,15 +14380,15 @@
         :param body: Is either a UpdateCncMachineOperationToolRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateCncMachineOperationToolRequest or IO[bytes]
         :return: CncToolDto
         :rtype: ~ignos.api.client.models.CncToolDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13094,15 +14450,15 @@
         :type operation_id: str
         :param id: Required.
         :type id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13205,15 +14561,15 @@
         :param body: Is either a UploadCncToolImageRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UploadCncToolImageRequest or IO[bytes]
         :return: ImageFileDto
         :rtype: ~ignos.api.client.models.ImageFileDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13277,15 +14633,15 @@
         :type id: int
         :param filename: Required.
         :type filename: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13375,15 +14731,15 @@
         :param body: Is either a CreateCncMachineOperationToolRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateCncMachineOperationToolRequest or IO[bytes]
         :return: CncToolDto
         :rtype: ~ignos.api.client.models.CncToolDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13440,15 +14796,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of CncToolDto
         :rtype: list[~ignos.api.client.models.CncToolDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13554,15 +14910,15 @@
         :param body: Is either a UpdateCncMachineToolRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateCncMachineToolRequest or IO[bytes]
         :return: CncToolDto
         :rtype: ~ignos.api.client.models.CncToolDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13624,15 +14980,15 @@
         :type cnc_machine_id: str
         :param id: Required.
         :type id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13662,14 +15018,198 @@
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @overload
+    def upload_cnc_machine_tool_image(
+        self,
+        machine_id: str,
+        id: int,
+        body: Optional[_models.UploadCncToolImageRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> _models.ImageFileDto:
+        """upload_cnc_machine_tool_image.
+
+        :param machine_id: Required.
+        :type machine_id: str
+        :param id: Required.
+        :type id: int
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.UploadCncToolImageRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: ImageFileDto
+        :rtype: ~ignos.api.client.models.ImageFileDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def upload_cnc_machine_tool_image(
+        self,
+        machine_id: str,
+        id: int,
+        body: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> _models.ImageFileDto:
+        """upload_cnc_machine_tool_image.
+
+        :param machine_id: Required.
+        :type machine_id: str
+        :param id: Required.
+        :type id: int
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: ImageFileDto
+        :rtype: ~ignos.api.client.models.ImageFileDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def upload_cnc_machine_tool_image(
+        self,
+        machine_id: str,
+        id: int,
+        body: Optional[Union[_models.UploadCncToolImageRequest, IO[bytes]]] = None,
+        **kwargs: Any,
+    ) -> _models.ImageFileDto:
+        """upload_cnc_machine_tool_image.
+
+        :param machine_id: Required.
+        :type machine_id: str
+        :param id: Required.
+        :type id: int
+        :param body: Is either a UploadCncToolImageRequest type or a IO[bytes] type. Default value is
+         None.
+        :type body: ~ignos.api.client.models.UploadCncToolImageRequest or IO[bytes]
+        :return: ImageFileDto
+        :rtype: ~ignos.api.client.models.ImageFileDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ImageFileDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UploadCncToolImageRequest")
+            else:
+                _json = None
+
+        _request = build_cnc_setup_upload_cnc_machine_tool_image_request(
+            machine_id=machine_id,
+            id=id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("ImageFileDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace
+    def delete_cnc_machine_tool_image(  # pylint: disable=inconsistent-return-statements
+        self, machine_id: str, id: int, filename: str, **kwargs: Any
+    ) -> None:
+        """delete_cnc_machine_tool_image.
+
+        :param machine_id: Required.
+        :type machine_id: str
+        :param id: Required.
+        :type id: int
+        :param filename: Required.
+        :type filename: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        _request = build_cnc_setup_delete_cnc_machine_tool_image_request(
+            machine_id=machine_id,
+            id=id,
+            filename=filename,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
     def import_operation_with_tools(  # pylint: disable=inconsistent-return-statements
         self,
         body: Optional[_models.ImportOperationWithTool] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any,
     ) -> None:
@@ -13711,15 +15251,15 @@
         :param body: Is either a ImportOperationWithTool type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ImportOperationWithTool or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13795,15 +15335,15 @@
         :paramtype agent_id: str
         :keyword agent_version: Default value is None.
         :paramtype agent_version: str
         :return: AgentConfigDto
         :rtype: ~ignos.api.client.models.AgentConfigDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -13892,15 +15432,15 @@
         :type id: str
         :param body: Is either a UploadFileRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadFileRequest or IO[bytes]
         :return: list of UploadFileDto
         :rtype: list[~ignos.api.client.models.UploadFileDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14004,15 +15544,15 @@
         :param body: Is either a SetTransferStatusRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.SetTransferStatusRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14083,15 +15623,15 @@
     def list_countries(self, **kwargs: Any) -> List[_models.CountryDto]:
         """list_countries.
 
         :return: list of CountryDto
         :rtype: list[~ignos.api.client.models.CountryDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14150,15 +15690,15 @@
     def get_current_customer(self, **kwargs: Any) -> _models.CurrentCustomerDto:
         """get_current_customer.
 
         :return: CurrentCustomerDto
         :rtype: ~ignos.api.client.models.CurrentCustomerDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14251,15 +15791,15 @@
         :type id: str
         :param body: Is either a UpsertCustomerRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertCustomerRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14314,15 +15854,15 @@
 
         :param id: Customer id. Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14374,15 +15914,15 @@
         :keyword continuation_token_parameter: Continuation token used for pagination. Default value is
          None.
         :paramtype continuation_token_parameter: str
         :return: CustomerDtoPagedResult
         :rtype: ~ignos.api.client.models.CustomerDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14465,15 +16005,15 @@
 
         :param body: Is either a ListCustomersRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListCustomersRequest or IO[bytes]
         :return: CustomerDtoPagedResult
         :rtype: ~ignos.api.client.models.CustomerDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14529,15 +16069,15 @@
 
         List customer groups.
 
         :return: list of CustomerGroupDto
         :rtype: list[~ignos.api.client.models.CustomerGroupDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14580,15 +16120,15 @@
 
         :param id: Customer id. Required.
         :type id: str
         :return: ProblemDetails
         :rtype: ~ignos.api.client.models.ProblemDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14675,15 +16215,15 @@
 
         :param body: Is either a CreateCustomerMapping type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateCustomerMapping or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14735,15 +16275,15 @@
 
         Delete all customer mappings between old customer ids and new customer ids.
 
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14841,15 +16381,15 @@
 
         :param body: Is either a ImportDocument type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ImportDocument or IO[bytes]
         :return: ImportDocumentResultDto
         :rtype: ~ignos.api.client.models.ImportDocumentResultDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14907,15 +16447,15 @@
 
         :keyword imported_reference: Default value is None.
         :paramtype imported_reference: str
         :return: str
         :rtype: str
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -14977,15 +16517,15 @@
 
         :keyword include_inactive: Default value is False.
         :paramtype include_inactive: bool
         :return: list of DocumentTypeDto
         :rtype: list[~ignos.api.client.models.DocumentTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15067,15 +16607,15 @@
         :param body: Is either a CreateDocumentTypeRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateDocumentTypeRequest or IO[bytes]
         :return: DocumentTypeDto
         :rtype: ~ignos.api.client.models.DocumentTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15131,15 +16671,15 @@
 
         :param id: Required.
         :type id: str
         :return: DocumentTypeDto
         :rtype: ~ignos.api.client.models.DocumentTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15228,15 +16768,15 @@
         :param body: Is either a UpdateDocumentTypeRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateDocumentTypeRequest or IO[bytes]
         :return: DocumentTypeDto
         :rtype: ~ignos.api.client.models.DocumentTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15295,15 +16835,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15341,15 +16881,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15389,15 +16929,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15435,15 +16975,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of DocumentTypeRuleDto
         :rtype: list[~ignos.api.client.models.DocumentTypeRuleDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15532,15 +17072,15 @@
         :param body: Is either a UpdateDocumentTypeRuleRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateDocumentTypeRuleRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15591,15 +17131,15 @@
     def list_all_document_rule_types(self, **kwargs: Any) -> List[_models.DocumentTypeRuleTypeDto]:
         """list_all_document_rule_types.
 
         :return: list of DocumentTypeRuleTypeDto
         :rtype: list[~ignos.api.client.models.DocumentTypeRuleTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15638,15 +17178,15 @@
     def list_document_generators(self, **kwargs: Any) -> List[_models.DocumentGeneratorTypeDto]:
         """list_document_generators.
 
         :return: list of DocumentGeneratorTypeDto
         :rtype: list[~ignos.api.client.models.DocumentGeneratorTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15705,15 +17245,15 @@
     def list_production_companies(self, **kwargs: Any) -> List[_models.ProductionCompanyDto]:
         """list_production_companies.
 
         :return: list of ProductionCompanyDto
         :rtype: list[~ignos.api.client.models.ProductionCompanyDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15794,15 +17334,15 @@
         :param body: Is either a SelectProductionCompany type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.SelectProductionCompany or IO[bytes]
         :return: ProductionCompanyDto
         :rtype: ~ignos.api.client.models.ProductionCompanyDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15931,15 +17471,15 @@
         :param body: Order details. Is either a UpsertCustomerOrderRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpsertCustomerOrderRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -15992,15 +17532,15 @@
 
         :param id: Required.
         :type id: str
         :return: CustomerOrderDto
         :rtype: ~ignos.api.client.models.CustomerOrderDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16108,15 +17648,15 @@
         :param body: Order line details. Is either a CustomerOrderLineDto type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.CustomerOrderLineDto or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16184,15 +17724,15 @@
         :keyword continuation_token_parameter: Continuation token used for pagination. Default value is
          None.
         :paramtype continuation_token_parameter: str
         :return: CustomerOrderDtoPagedResult
         :rtype: ~ignos.api.client.models.CustomerOrderDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16276,15 +17816,15 @@
         :param body: Is either a ListCustomerOrdersRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ListCustomerOrdersRequest or IO[bytes]
         :return: CustomerOrderDtoPagedResult
         :rtype: ~ignos.api.client.models.CustomerOrderDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16340,15 +17880,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of CustomerOrderLineDto
         :rtype: list[~ignos.api.client.models.CustomerOrderLineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16408,15 +17948,15 @@
     def list_all_machines(self, **kwargs: Any) -> List[_models.MachineDto]:
         """list_all_machines.
 
         :return: list of MachineDto
         :rtype: list[~ignos.api.client.models.MachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16518,15 +18058,15 @@
 
         :param body: Is either a UpsertWorkorder type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertWorkorder or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16619,15 +18159,15 @@
 
         :param body: Is either a UpsertWorkorderV2 type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertWorkorderV2 or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16706,15 +18246,15 @@
         :keyword continuation_token_parameter: Continuation token used for pagination. Default value is
          None.
         :paramtype continuation_token_parameter: str
         :return: WorkorderListDtoPagedResult
         :rtype: ~ignos.api.client.models.WorkorderListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16817,15 +18357,15 @@
         :param body: Consumption details. Is either a UpsertWorkOrderConsumptionsRequest type or a
          IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertWorkOrderConsumptionsRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16878,15 +18418,15 @@
 
         :param id: Required.
         :type id: str
         :return: WorkOrderConsumptionDto
         :rtype: ~ignos.api.client.models.WorkOrderConsumptionDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -16981,15 +18521,15 @@
         :param body: Trace details. Is either a UpsertWorkOrderTracesRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpsertWorkOrderTracesRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17092,15 +18632,15 @@
         :param body: Is either a WorkorderCustomerOrderReferenceDto type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.WorkorderCustomerOrderReferenceDto or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17153,15 +18693,15 @@
 
         :param id: Required.
         :type id: str
         :return: ResourceExistDto
         :rtype: ~ignos.api.client.models.ResourceExistDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17273,15 +18813,15 @@
         :param body: Is either a StartWorkOperationRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StartWorkOperationRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17405,15 +18945,15 @@
         :param body: Is either a StopWorkOperationRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StopWorkOperationRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17537,15 +19077,15 @@
         :param body: Is either a RegisterWorkorderOperationEventRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.RegisterWorkorderOperationEventRequest or IO[bytes]
         :return: WorkorderOperationEventDto
         :rtype: ~ignos.api.client.models.WorkorderOperationEventDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17673,15 +19213,15 @@
         :param body: Is either a StartWorkOperationRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StartWorkOperationRequest or IO[bytes]
         :return: WorkorderOperationEventDto
         :rtype: ~ignos.api.client.models.WorkorderOperationEventDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17809,15 +19349,15 @@
         :param body: Is either a StopWorkOperationRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.StopWorkOperationRequest or IO[bytes]
         :return: WorkorderOperationEventDto
         :rtype: ~ignos.api.client.models.WorkorderOperationEventDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17873,15 +19413,15 @@
     def list_active_workorder_operations(self, **kwargs: Any) -> List[_models.WorkorderOperationEventDto]:
         """list_active_workorder_operations.
 
         :return: list of WorkorderOperationEventDto
         :rtype: list[~ignos.api.client.models.WorkorderOperationEventDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17928,15 +19468,15 @@
         :type operation: int
         :param event_id: Required.
         :type event_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -17978,15 +19518,15 @@
 
         :param id: The work order ID. Required.
         :type id: str
         :return: WorkorderDto
         :rtype: ~ignos.api.client.models.WorkorderDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18030,15 +19570,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18115,15 +19655,15 @@
 
         :param body: Is either a ListWorkOrdersRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListWorkOrdersRequest or IO[bytes]
         :return: WorkorderListDtoPagedResult
         :rtype: ~ignos.api.client.models.WorkorderListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18181,15 +19721,15 @@
 
         :param event_id: The ID of the event. Required.
         :type event_id: str
         :return: WorkorderOperationEventDto
         :rtype: ~ignos.api.client.models.WorkorderOperationEventDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18287,15 +19827,15 @@
         :param body: Is either a UpdateWorkorderOperationEventTimestamps type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpdateWorkorderOperationEventTimestamps or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18394,15 +19934,15 @@
         :param body: Is either a FilterWorkorderOperationEvents type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.FilterWorkorderOperationEvents or IO[bytes]
         :return: list of WorkorderOperationEventDto
         :rtype: list[~ignos.api.client.models.WorkorderOperationEventDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18504,15 +20044,15 @@
         :param body: Is either a CreateWorkOrderMapping type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateWorkOrderMapping or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18554,14 +20094,109 @@
                 response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
+    @distributed_trace
+    def delete_work_order_mappings(self, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
+        """Deleteds existing work order mappings.
+
+        Deleteds existing work order mappings.
+
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        _request = build_workorders_delete_work_order_mappings_request(
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @distributed_trace
+    def search_work_orders(self, *, input: Optional[str] = None, **kwargs: Any) -> List[_models.SearchWorkOrderDto]:
+        """search_work_orders.
+
+        :keyword input: Default value is None.
+        :paramtype input: str
+        :return: list of SearchWorkOrderDto
+        :rtype: list[~ignos.api.client.models.SearchWorkOrderDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.SearchWorkOrderDto]] = kwargs.pop("cls", None)
+
+        _request = build_workorders_search_work_orders_request(
+            input=input,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[SearchWorkOrderDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
 
 class ExternalOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -18582,15 +20217,15 @@
     def list_invites(self, **kwargs: Any) -> List[_models.InviteDto]:
         """list_invites.
 
         :return: list of InviteDto
         :rtype: list[~ignos.api.client.models.InviteDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18671,15 +20306,15 @@
         :param body: Is either a AcceptSupplierInviteRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.AcceptSupplierInviteRequest or IO[bytes]
         :return: CompanyDto
         :rtype: ~ignos.api.client.models.CompanyDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18733,15 +20368,15 @@
     def list_companies(self, **kwargs: Any) -> List[_models.CompanyDto]:
         """list_companies.
 
         :return: list of CompanyDto
         :rtype: list[~ignos.api.client.models.CompanyDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18802,15 +20437,15 @@
 
         :keyword company_id: Default value is None.
         :paramtype company_id: str
         :return: list of CompanyUserDto
         :rtype: list[~ignos.api.client.models.CompanyUserDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -18892,15 +20527,15 @@
         :param body: Is either a CreateCompanyUserRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateCompanyUserRequest or IO[bytes]
         :return: CompanyUserDto
         :rtype: ~ignos.api.client.models.CompanyUserDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19003,15 +20638,15 @@
         :param body: Is either a UpdateCompanyUserRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateCompanyUserRequest or IO[bytes]
         :return: CompanyUserDto
         :rtype: ~ignos.api.client.models.CompanyUserDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19072,15 +20707,15 @@
         :type id: str
         :keyword company_id: Default value is None.
         :paramtype company_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19117,15 +20752,15 @@
     def list_roles(self, **kwargs: Any) -> List[_models.ExternalRoleDto]:
         """list_roles.
 
         :return: list of ExternalRoleDto
         :rtype: list[~ignos.api.client.models.ExternalRoleDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19164,15 +20799,15 @@
     def list_company_customers(self, **kwargs: Any) -> List[_models.CompanyCustomerDto]:
         """list_company_customers.
 
         :return: list of CompanyCustomerDto
         :rtype: list[~ignos.api.client.models.CompanyCustomerDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19215,15 +20850,15 @@
 
         :param tenant_id: Required.
         :type tenant_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19284,15 +20919,15 @@
         :param service_name: Known values are: "DbExtractor", "MtConnectExtractor", and
          "MqttConnector". Required.
         :type service_name: str or ~ignos.api.client.models.ExternalServiceName
         :return: ExternalServiceCredentialDto
         :rtype: ~ignos.api.client.models.ExternalServiceCredentialDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19352,15 +20987,15 @@
     def list_electrical_source_types(self, **kwargs: Any) -> List[_models.IotTypeSourceDto]:
         """list_electrical_source_types.
 
         :return: list of IotTypeSourceDto
         :rtype: list[~ignos.api.client.models.IotTypeSourceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19399,15 +21034,15 @@
     def list_electrical_data_configs(self, **kwargs: Any) -> List[_models.ElectricalIotConfigDto]:
         """list_electrical_data_configs.
 
         :return: list of ElectricalIotConfigDto
         :rtype: list[~ignos.api.client.models.ElectricalIotConfigDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19488,15 +21123,15 @@
         :param body: Is either a CreateElectricalIotConfig type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateElectricalIotConfig or IO[bytes]
         :return: ElectricalIotConfigDto
         :rtype: ~ignos.api.client.models.ElectricalIotConfigDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19556,15 +21191,15 @@
         :type type_id: str
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19621,15 +21256,15 @@
     def list_welding_source_types(self, **kwargs: Any) -> List[_models.IotTypeSourceDto]:
         """list_welding_source_types.
 
         :return: list of IotTypeSourceDto
         :rtype: list[~ignos.api.client.models.IotTypeSourceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19668,15 +21303,15 @@
     def list_electrical_data_configs(self, **kwargs: Any) -> List[JSON]:
         """list_electrical_data_configs.
 
         :return: list of JSON
         :rtype: list[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19717,15 +21352,15 @@
 
         :param body: Default value is None.
         :type body: JSON
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19778,15 +21413,15 @@
         :type type_id: str
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19845,15 +21480,15 @@
 
         :keyword scope: Default value is None.
         :paramtype scope: str
         :return: list of LinkDto
         :rtype: list[~ignos.api.client.models.LinkDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19930,15 +21565,15 @@
 
         :param body: Is either a CreateLinkRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateLinkRequest or IO[bytes]
         :return: LinkDto
         :rtype: ~ignos.api.client.models.LinkDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -19992,15 +21627,15 @@
     def get_all_link_scopes(self, **kwargs: Any) -> List[str]:
         """get_all_link_scopes.
 
         :return: list of str
         :rtype: list[str]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20045,15 +21680,15 @@
         :type id: str
         :keyword scope: Default value is None.
         :paramtype scope: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20083,14 +21718,152 @@
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
 
+class LocationsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.IgnosPortal`'s
+        :attr:`locations` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace
+    def search_locations(
+        self,
+        *,
+        input: Optional[str] = None,
+        location_kinds: Optional[List[Union[str, _models.LocationKindDto]]] = None,
+        **kwargs: Any,
+    ) -> List[_models.LocationDto]:
+        """search_locations.
+
+        :keyword input: Default value is None.
+        :paramtype input: str
+        :keyword location_kinds: Default value is None.
+        :paramtype location_kinds: list[str or ~ignos.api.client.models.LocationKindDto]
+        :return: list of LocationDto
+        :rtype: list[~ignos.api.client.models.LocationDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.LocationDto]] = kwargs.pop("cls", None)
+
+        _request = build_locations_search_locations_request(
+            input=input,
+            location_kinds=location_kinds,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[LocationDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace
+    def suggestions_locations(
+        self,
+        *,
+        work_order_id: Optional[str] = None,
+        location_kinds: Optional[List[Union[str, _models.LocationKindDto]]] = None,
+        **kwargs: Any,
+    ) -> List[_models.LocationDto]:
+        """suggestions_locations.
+
+        :keyword work_order_id: Default value is None.
+        :paramtype work_order_id: str
+        :keyword location_kinds: Default value is None.
+        :paramtype location_kinds: list[str or ~ignos.api.client.models.LocationKindDto]
+        :return: list of LocationDto
+        :rtype: list[~ignos.api.client.models.LocationDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.LocationDto]] = kwargs.pop("cls", None)
+
+        _request = build_locations_suggestions_locations_request(
+            work_order_id=work_order_id,
+            location_kinds=location_kinds,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[LocationDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+
 class MachineAlarmsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.IgnosPortal`'s
@@ -20153,15 +21926,15 @@
         :paramtype order_by: str
         :keyword sort_direction: Default value is None.
         :paramtype sort_direction: str
         :return: MachineAlarmDtoPagedResult
         :rtype: ~ignos.api.client.models.MachineAlarmDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20223,15 +21996,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: list of MachineAlarmSummaryDto
         :rtype: list[~ignos.api.client.models.MachineAlarmSummaryDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20282,15 +22055,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: list of MachineAlarmSeverityOccurenceDto
         :rtype: list[~ignos.api.client.models.MachineAlarmSeverityOccurenceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20362,15 +22135,15 @@
         :paramtype name: str
         :keyword sequence: Default value is None.
         :paramtype sequence: str
         :return: MachineAlarmCountDto
         :rtype: ~ignos.api.client.models.MachineAlarmCountDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20420,15 +22193,15 @@
 
         :param id: Required.
         :type id: int
         :return: MachineAlarmDetailsDto
         :rtype: ~ignos.api.client.models.MachineAlarmDetailsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20488,15 +22261,15 @@
     def list_machines(self, **kwargs: Any) -> List[_models.MachineDto]:
         """list_machines.
 
         :return: list of MachineDto
         :rtype: list[~ignos.api.client.models.MachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20535,15 +22308,15 @@
     def list_machine_groups(self, **kwargs: Any) -> List[_models.MachineGroupDto]:
         """list_machine_groups.
 
         :return: list of MachineGroupDto
         :rtype: list[~ignos.api.client.models.MachineGroupDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20623,15 +22396,15 @@
 
         :param body: Is either a CreateMachineGroup type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateMachineGroup or IO[bytes]
         :return: CreateMachineGroupResponse
         :rtype: ~ignos.api.client.models.CreateMachineGroupResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20733,15 +22506,15 @@
         :type id: str
         :param body: Is either a UpdateMachineGroup type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateMachineGroup or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20794,15 +22567,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20842,15 +22615,15 @@
 
         :keyword asset_id: Default value is None.
         :paramtype asset_id: int
         :return: MachineStateListDto
         :rtype: ~ignos.api.client.models.MachineStateListDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20903,15 +22676,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: list of MachineStateDatapoint
         :rtype: list[~ignos.api.client.models.MachineStateDatapoint]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -20966,15 +22739,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: MachineStatesSummaryDto
         :rtype: ~ignos.api.client.models.MachineStatesSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21016,15 +22789,15 @@
     def list_machine_erp_data(self, **kwargs: Any) -> _models.MachineErpDataListDto:
         """list_machine_erp_data.
 
         :return: MachineErpDataListDto
         :rtype: ~ignos.api.client.models.MachineErpDataListDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21065,15 +22838,15 @@
 
         :param id: Required.
         :type id: int
         :return: MachineErpDataDto
         :rtype: ~ignos.api.client.models.MachineErpDataDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21113,15 +22886,15 @@
     def get_machine_utilization_summary(self, **kwargs: Any) -> _models.UtilizationSummaryDto:
         """get_machine_utilization_summary.
 
         :return: UtilizationSummaryDto
         :rtype: ~ignos.api.client.models.UtilizationSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21166,15 +22939,15 @@
         :paramtype machine_external_id: str
         :keyword operator_name_query: Default value is None.
         :paramtype operator_name_query: str
         :return: list of OperatorAndMachineDto
         :rtype: list[~ignos.api.client.models.OperatorAndMachineDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21207,14 +22980,314 @@
         deserialized = self._deserialize("[OperatorAndMachineDto]", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
+    @overload
+    def create_machine_without_resource(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.CreateMachineWithoutResource] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """create_machine_without_resource.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateMachineWithoutResource
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create_machine_without_resource(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_machine_without_resource.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create_machine_without_resource(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.CreateMachineWithoutResource, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_machine_without_resource.
+
+        :param body: Is either a CreateMachineWithoutResource type or a IO[bytes] type. Default value
+         is None.
+        :type body: ~ignos.api.client.models.CreateMachineWithoutResource or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateMachineWithoutResource")
+            else:
+                _json = None
+
+        _request = build_machines_create_machine_without_resource_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    def create_resource_without_machine(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.CreateResourceWithoutMachine] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """create_resource_without_machine.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateResourceWithoutMachine
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create_resource_without_machine(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_resource_without_machine.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create_resource_without_machine(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.CreateResourceWithoutMachine, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_resource_without_machine.
+
+        :param body: Is either a CreateResourceWithoutMachine type or a IO[bytes] type. Default value
+         is None.
+        :type body: ~ignos.api.client.models.CreateResourceWithoutMachine or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateResourceWithoutMachine")
+            else:
+                _json = None
+
+        _request = build_machines_create_resource_without_machine_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    def create_resource_with_machine(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.CreateResourceWithMachine] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """create_resource_with_machine.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateResourceWithMachine
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create_resource_with_machine(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_resource_with_machine.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create_resource_with_machine(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.CreateResourceWithMachine, IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_resource_with_machine.
+
+        :param body: Is either a CreateResourceWithMachine type or a IO[bytes] type. Default value is
+         None.
+        :type body: ~ignos.api.client.models.CreateResourceWithMachine or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateResourceWithMachine")
+            else:
+                _json = None
+
+        _request = build_machines_create_resource_with_machine_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
 
 class MachineUtilizationOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -21269,15 +23342,15 @@
         :keyword utc_offset: Explicit UTC offset for start of today's utilization. Default value is
          None.
         :paramtype utc_offset: float
         :return: UtilizationListDto
         :rtype: ~ignos.api.client.models.UtilizationListDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21333,15 +23406,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: UtilizationDetailsDto
         :rtype: ~ignos.api.client.models.UtilizationDetailsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21396,15 +23469,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: MachineStatesSummaryDto
         :rtype: ~ignos.api.client.models.MachineStatesSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21459,15 +23532,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: list of MachineStateDatapoint
         :rtype: list[~ignos.api.client.models.MachineStateDatapoint]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21522,15 +23595,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: MachineStatesSummaryDto
         :rtype: ~ignos.api.client.models.MachineStatesSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21614,15 +23687,15 @@
         :param body: Is either a ListMachineUptimesTodayRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.ListMachineUptimesTodayRequest or IO[bytes]
         :return: MachineUptimesAggregateDto
         :rtype: ~ignos.api.client.models.MachineUptimesAggregateDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21695,15 +23768,15 @@
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: Default value is None.
         :paramtype end_time: ~datetime.datetime
         :return: PowerOnUtilizationList
         :rtype: ~ignos.api.client.models.PowerOnUtilizationList
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21747,15 +23820,15 @@
     def get_factory_utilization(self, **kwargs: Any) -> _models.PowerOnUtilizationDto:
         """get_factory_utilization.
 
         :return: PowerOnUtilizationDto
         :rtype: ~ignos.api.client.models.PowerOnUtilizationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21814,15 +23887,15 @@
     def get_my_apps(self, **kwargs: Any) -> List[_models.UserAppDto]:
         """get_my_apps.
 
         :return: list of UserAppDto
         :rtype: list[~ignos.api.client.models.UserAppDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21861,15 +23934,15 @@
     def get_current_user(self, **kwargs: Any) -> _models.UserDetailsDto:
         """get_current_user.
 
         :return: UserDetailsDto
         :rtype: ~ignos.api.client.models.UserDetailsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -21950,15 +24023,15 @@
         :param body: Is either a SetIsBetaTesterRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.SetIsBetaTesterRequest or IO[bytes]
         :return: UserDto
         :rtype: ~ignos.api.client.models.UserDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22012,15 +24085,15 @@
     def update_current_user_last_seen(self, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
         """update_current_user_last_seen.
 
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22106,15 +24179,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22204,15 +24277,15 @@
         :param body: Is either a CreateMeasurementFormSchema type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMeasurementFormSchema or IO[bytes]
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22308,15 +24381,15 @@
         :param body: Is either a ListMeasurementFormSchemasRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormSchemasRequest or IO[bytes]
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22372,15 +24445,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22472,15 +24545,15 @@
         :param body: Is either a UpdateMeasurementFormSchemaRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateMeasurementFormSchemaRequest or IO[bytes]
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22587,15 +24660,15 @@
         :param body: Is either a UpdateSchemaGroupedElementsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateSchemaGroupedElementsRequest or IO[bytes]
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22698,15 +24771,15 @@
         :type id: str
         :param body: Is either a UploadDrawingRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadDrawingRequest or IO[bytes]
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22809,15 +24882,15 @@
         :type id: str
         :param body: Is either a UploadRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadRequest or IO[bytes]
         :return: MeasurementFormSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22874,15 +24947,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormImportStatusDto
         :rtype: ~ignos.api.client.models.MeasurementFormImportStatusDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -22970,15 +25043,15 @@
         :type schema_id: str
         :param body: Is either a CreateSchemaElement type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateSchemaElement or IO[bytes]
         :return: MeasurementFormElementDto
         :rtype: ~ignos.api.client.models.MeasurementFormElementDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23049,15 +25122,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23142,15 +25215,15 @@
         :param body: Is either a ListLinkableMeasurementFormSchemasRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.ListLinkableMeasurementFormSchemasRequest or IO[bytes]
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23256,15 +25329,15 @@
         :param body: Is either a CreateMeasurementFormSchemaLinkRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.CreateMeasurementFormSchemaLinkRequest or IO[bytes]
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23325,15 +25398,15 @@
         :type schema_id: str
         :param linked_schema_id: Required.
         :type linked_schema_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23372,15 +25445,15 @@
 
         :param schema_id: Required.
         :type schema_id: str
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23422,15 +25495,15 @@
 
         :param schema_id: Required.
         :type schema_id: str
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23472,15 +25545,15 @@
 
         :param schema_id: Required.
         :type schema_id: str
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23524,15 +25597,15 @@
 
         :param schema_id: Required.
         :type schema_id: str
         :return: bool
         :rtype: bool
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23572,15 +25645,15 @@
     def get_measurement_form_settings(self, **kwargs: Any) -> _models.MeasurementFormSettingsDto:
         """get_measurement_form_settings.
 
         :return: MeasurementFormSettingsDto
         :rtype: ~ignos.api.client.models.MeasurementFormSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23661,15 +25734,15 @@
         :param body: Is either a UpdateMeasurementFormSettings type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateMeasurementFormSettings or IO[bytes]
         :return: MeasurementFormSettingsDto
         :rtype: ~ignos.api.client.models.MeasurementFormSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23727,15 +25800,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormCustomerSettingsDto
         :rtype: ~ignos.api.client.models.MeasurementFormCustomerSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23817,15 +25890,15 @@
         :param body: Is either a UpdateMeasurementFormCustomerSettings type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.UpdateMeasurementFormCustomerSettings or IO[bytes]
         :return: MeasurementFormCustomerSettingsDto
         :rtype: ~ignos.api.client.models.MeasurementFormCustomerSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23883,15 +25956,15 @@
 
         :keyword target_id: Required.
         :paramtype target_id: str
         :return: list of MeasurementFormMappingDto
         :rtype: list[~ignos.api.client.models.MeasurementFormMappingDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -23976,15 +26049,15 @@
          is None.
         :type body: ~ignos.api.client.models.CreateMeasurementFormMapping or IO[bytes]
         :return: MeasurementFormMappingDto or ProblemDetails
         :rtype: ~ignos.api.client.models.MeasurementFormMappingDto or
          ~ignos.api.client.models.ProblemDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24047,15 +26120,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormMappingDto
         :rtype: ~ignos.api.client.models.MeasurementFormMappingDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24099,15 +26172,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24195,15 +26268,15 @@
         :param body: Is either a [MeasurementFormBalloonMappingRequestDto] type or a IO[bytes] type.
          Default value is None.
         :type body: list[~ignos.api.client.models.MeasurementFormBalloonMappingRequestDto] or IO[bytes]
         :return: MeasurementFormMappingDto
         :rtype: ~ignos.api.client.models.MeasurementFormMappingDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24310,15 +26383,15 @@
         :param body: Is either a SetMeasurementFormMappingBalloonsRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.SetMeasurementFormMappingBalloonsRequest or IO[bytes]
         :return: MeasurementFormMappingDto
         :rtype: ~ignos.api.client.models.MeasurementFormMappingDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24379,15 +26452,15 @@
         :paramtype target_id: str
         :keyword source_id: Default value is None.
         :paramtype source_id: str
         :return: MeasurementFormMappingSuggestionDto
         :rtype: ~ignos.api.client.models.MeasurementFormMappingSuggestionDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24476,15 +26549,15 @@
         :param body: Is either a ImportMeasurementFormSchema type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ImportMeasurementFormSchema or IO[bytes]
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24572,15 +26645,15 @@
         :paramtype continuation_token_parameter: str
         :keyword only_without_drawing_url: Default value is None.
         :paramtype only_without_drawing_url: bool
         :return: MeasurementFormNeedDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormNeedDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24671,15 +26744,15 @@
         :param body: Is either a ListMeasurementFormNeedsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormNeedsRequest or IO[bytes]
         :return: MeasurementFormNeedDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormNeedDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24782,15 +26855,15 @@
         :param body: Is either a SetMeasurementFormNeedUserRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.SetMeasurementFormNeedUserRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24893,15 +26966,15 @@
         :param body: Is either a SetMeasurementFormNeedAsNotNeededRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.SetMeasurementFormNeedAsNotNeededRequest or IO[bytes]
         :return: MeasurementFormSchemaNotNeededDto
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaNotNeededDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -24958,15 +27031,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormDto
         :rtype: ~ignos.api.client.models.MeasurementFormDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25054,15 +27127,15 @@
         :type id: str
         :param body: Is either a UploadDrawingRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UploadDrawingRequest or IO[bytes]
         :return: MeasurementFormNeedDto
         :rtype: ~ignos.api.client.models.MeasurementFormNeedDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25148,15 +27221,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormSchemaNotNeededDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaNotNeededDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25246,15 +27319,15 @@
         :param body: Is either a ListMeasurementFormSchemasNotNeededRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormSchemasNotNeededRequest or IO[bytes]
         :return: MeasurementFormSchemaNotNeededDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormSchemaNotNeededDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25312,15 +27385,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25358,15 +27431,15 @@
     ) -> List[_models.MeasurementFormResourceTypeGeneratorDto]:
         """list_resource_types_for_needs_generator.
 
         :return: list of MeasurementFormResourceTypeGeneratorDto
         :rtype: list[~ignos.api.client.models.MeasurementFormResourceTypeGeneratorDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25447,15 +27520,15 @@
         :param body: Is either a AddResourceTypeForNeedsGenerator type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.AddResourceTypeForNeedsGenerator or IO[bytes]
         :return: MeasurementFormResourceTypeGeneratorDto
         :rtype: ~ignos.api.client.models.MeasurementFormResourceTypeGeneratorDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25513,15 +27586,15 @@
 
         :param resource_type: Required.
         :type resource_type: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25557,15 +27630,15 @@
     def list_frequencies(self, **kwargs: Any) -> List[_models.MeasurementFrequencyDto]:
         """list_frequencies.
 
         :return: list of MeasurementFrequencyDto
         :rtype: list[~ignos.api.client.models.MeasurementFrequencyDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25617,15 +27690,15 @@
         :paramtype search: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: SchemaFeedbackDtoPagedResult
         :rtype: ~ignos.api.client.models.SchemaFeedbackDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25712,15 +27785,15 @@
          type. Default value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormInstanceSchemaFeedbackRequest or
          IO[bytes]
         :return: SchemaFeedbackDtoPagedResult
         :rtype: ~ignos.api.client.models.SchemaFeedbackDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25778,15 +27851,15 @@
 
         :param id: Required.
         :type id: str
         :return: SchemaFeedbackDto
         :rtype: ~ignos.api.client.models.SchemaFeedbackDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25830,15 +27903,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -25926,15 +27999,15 @@
         :param body: Is either a SetMeasurementFormSchemaFeedbackUserRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.SetMeasurementFormSchemaFeedbackUserRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26013,15 +28086,15 @@
         :paramtype version: int
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26112,15 +28185,15 @@
         :param body: Is either a ListMeasurementFormSchemasWithHistoryRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormSchemasWithHistoryRequest or IO[bytes]
         :return: MeasurementFormListDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26216,15 +28289,15 @@
         :paramtype inactive: bool
         :keyword include_inactive_supplier_access: Default value is None.
         :paramtype include_inactive_supplier_access: bool
         :return: MeasurementFormInstanceOverviewDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceOverviewDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26311,15 +28384,15 @@
         :param body: Is either a ListMeasurementFormsRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ListMeasurementFormsRequest or IO[bytes]
         :return: MeasurementFormInstanceOverviewDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceOverviewDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26396,15 +28469,15 @@
         :paramtype search: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MeasurementFormInstanceDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26491,15 +28564,15 @@
         :param body: Is either a ListMeasurementFormsByStatusRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ListMeasurementFormsByStatusRequest or IO[bytes]
         :return: MeasurementFormInstanceDtoPagedResult
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26559,15 +28632,15 @@
         :type id: str
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26610,15 +28683,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26710,15 +28783,15 @@
         :param body: Is either a UpdateMeasurementFormInstanceRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateMeasurementFormInstanceRequest or IO[bytes]
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26777,15 +28850,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of MeasurementFormInstanceFeedbackDto
         :rtype: list[~ignos.api.client.models.MeasurementFormInstanceFeedbackDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26831,15 +28904,15 @@
         :type id: str
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26882,15 +28955,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26932,15 +29005,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -26982,15 +29055,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27032,15 +29105,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27090,15 +29163,15 @@
         :paramtype sequence: str
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: MeasurementFormInstanceSchemaDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceSchemaDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27147,15 +29220,15 @@
         :type id: str
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: MeasurementFormInstanceProgressDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceProgressDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27215,15 +29288,15 @@
         :paramtype sequence: str
         :keyword element_id: Default value is None.
         :paramtype element_id: str
         :return: list of MeasurementFormElementValueAuditDto
         :rtype: list[~ignos.api.client.models.MeasurementFormElementValueAuditDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27267,15 +29340,15 @@
     def get_validation_rules(self, **kwargs: Any) -> List[_models.ValidationRuleDto]:
         """get_validation_rules.
 
         :return: list of ValidationRuleDto
         :rtype: list[~ignos.api.client.models.ValidationRuleDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27380,15 +29453,15 @@
         :type body: ~ignos.api.client.models.SaveValueRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: SaveValueResponseDto
         :rtype: ~ignos.api.client.models.SaveValueResponseDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27510,15 +29583,15 @@
         :type body: ~ignos.api.client.models.SaveToolRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: SaveValueResponseDto
         :rtype: ~ignos.api.client.models.SaveValueResponseDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27640,15 +29713,15 @@
         :type body: ~ignos.api.client.models.SaveCommentRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27767,15 +29840,15 @@
         :type body: ~ignos.api.client.models.BatchInsertValueRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: BatchInsertValuesResponseDto
         :rtype: ~ignos.api.client.models.BatchInsertValuesResponseDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -27908,15 +29981,15 @@
          IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28045,15 +30118,15 @@
         :type body: ~ignos.api.client.models.CreateMeasurementFormSchemaFeedbackRequest or IO[bytes]
         :keyword tenant_id: Default value is None.
         :paramtype tenant_id: str
         :return: SchemaFeedbackCreatedDto
         :rtype: ~ignos.api.client.models.SchemaFeedbackCreatedDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28114,15 +30187,15 @@
 
         :param supplier_id: Required.
         :type supplier_id: str
         :return: list of MeasurementFormSupplierAccessInstanceDto
         :rtype: list[~ignos.api.client.models.MeasurementFormSupplierAccessInstanceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28229,15 +30302,15 @@
          type. Default value is None.
         :type body: ~ignos.api.client.models.UpsertSupplierToMeasurementFormInstanceRequest or
          IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28295,15 +30368,15 @@
         :type id: str
         :param supplier_id: Required.
         :type supplier_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28389,15 +30462,15 @@
         :param body: Is either a ExportDimensionReportRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.ExportDimensionReportRequest or IO[bytes]
         :return: DownloadDto
         :rtype: ~ignos.api.client.models.DownloadDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28518,15 +30591,15 @@
         :param body: Is either a UpdateSchemaInstanceElementsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateSchemaInstanceElementsRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28584,15 +30657,15 @@
         :type id: str
         :param schema_id: Required.
         :type schema_id: str
         :return: list of SchemaInstanceElementDto
         :rtype: list[~ignos.api.client.models.SchemaInstanceElementDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28685,15 +30758,15 @@
         :param body: Is either a ImportMeasurementFormInstanceRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.ImportMeasurementFormInstanceRequest or IO[bytes]
         :return: MeasurementFormInstanceDto
         :rtype: ~ignos.api.client.models.MeasurementFormInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28799,15 +30872,15 @@
         :paramtype sort_direction: str
         :keyword include_deprecated: Default value is False.
         :paramtype include_deprecated: bool
         :return: MeasuringToolDtoPagedData
         :rtype: ~ignos.api.client.models.MeasuringToolDtoPagedData
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -28897,15 +30970,15 @@
         :param body: Is either a CreateMeasuringToolRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMeasuringToolRequest or IO[bytes]
         :return: MeasuringToolDetailDto
         :rtype: ~ignos.api.client.models.MeasuringToolDetailDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29008,15 +31081,15 @@
         :param body: Is either a UpdateMeasuringToolRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateMeasuringToolRequest or IO[bytes]
         :return: MeasuringToolDetailDto
         :rtype: ~ignos.api.client.models.MeasuringToolDetailDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29073,15 +31146,15 @@
 
         :param id: Required.
         :type id: str
         :return: MeasuringToolDetailDto
         :rtype: ~ignos.api.client.models.MeasuringToolDetailDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29123,15 +31196,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of MeasuringToolCalibrationDto
         :rtype: list[~ignos.api.client.models.MeasuringToolCalibrationDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29223,15 +31296,15 @@
         :param body: Is either a RegisterMeasuringToolCalibrationRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.RegisterMeasuringToolCalibrationRequest or IO[bytes]
         :return: MeasuringToolCalibrationDto
         :rtype: ~ignos.api.client.models.MeasuringToolCalibrationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29352,15 +31425,15 @@
         :param body: Is either a AttachCalibrationCertificateRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.AttachCalibrationCertificateRequest or IO[bytes]
         :return: MeasuringToolCalibrationDto
         :rtype: ~ignos.api.client.models.MeasuringToolCalibrationDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29422,15 +31495,15 @@
         :type id: str
         :param calibration_id: Required.
         :type calibration_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29467,15 +31540,15 @@
     def list_manufacturers(self, **kwargs: Any) -> List[_models.ManufacturerDto]:
         """list_manufacturers.
 
         :return: list of ManufacturerDto
         :rtype: list[~ignos.api.client.models.ManufacturerDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29556,15 +31629,15 @@
         :param body: Is either a CreateMeasuringToolManufacturer type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateMeasuringToolManufacturer or IO[bytes]
         :return: ManufacturerDto
         :rtype: ~ignos.api.client.models.ManufacturerDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29618,15 +31691,15 @@
     def list_measuring_tool_types(self, **kwargs: Any) -> List[_models.MeasuringToolTypeDto]:
         """list_measuring_tool_types.
 
         :return: list of MeasuringToolTypeDto
         :rtype: list[~ignos.api.client.models.MeasuringToolTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29707,15 +31780,15 @@
         :param body: Is either a CreateMeasuringToolType type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMeasuringToolType or IO[bytes]
         :return: MeasuringToolTypeDto
         :rtype: ~ignos.api.client.models.MeasuringToolTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29818,15 +31891,15 @@
         :param body: Is either a UpdateMeasuringToolTypeRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateMeasuringToolTypeRequest or IO[bytes]
         :return: MeasuringToolTypeDto
         :rtype: ~ignos.api.client.models.MeasuringToolTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29885,15 +31958,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -29931,15 +32004,15 @@
 
         :param type_id: Required.
         :type type_id: str
         :return: list of MeasuringToolSubTypeDto
         :rtype: list[~ignos.api.client.models.MeasuringToolSubTypeDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30031,15 +32104,15 @@
         :param body: Is either a CreateMeasuringToolSubTypeRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateMeasuringToolSubTypeRequest or IO[bytes]
         :return: MeasuringToolSubTypeDto
         :rtype: ~ignos.api.client.models.MeasuringToolSubTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30160,15 +32233,15 @@
         :param body: Is either a UpdateMeasuringToolSubTypeRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateMeasuringToolSubTypeRequest or IO[bytes]
         :return: MeasuringToolSubTypeDto
         :rtype: ~ignos.api.client.models.MeasuringToolSubTypeDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30230,15 +32303,15 @@
         :type type_id: str
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30275,15 +32348,15 @@
     def list_measuring_units(self, **kwargs: Any) -> List[_models.MeasuringUnitDto]:
         """list_measuring_units.
 
         :return: list of MeasuringUnitDto
         :rtype: list[~ignos.api.client.models.MeasuringUnitDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30363,15 +32436,15 @@
 
         :param body: Is either a CreateMeasuringUnit type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateMeasuringUnit or IO[bytes]
         :return: MeasuringUnitDto
         :rtype: ~ignos.api.client.models.MeasuringUnitDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30427,15 +32500,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30490,15 +32563,15 @@
         :paramtype order_by: str
         :keyword sort_direction: Default value is None.
         :paramtype sort_direction: str
         :return: MeasuringToolWhitelistDtoPagedData
         :rtype: ~ignos.api.client.models.MeasuringToolWhitelistDtoPagedData
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30584,15 +32657,15 @@
         :param body: Is either a WhitelistMeasuringTool type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.WhitelistMeasuringTool or IO[bytes]
         :return: MeasuringToolWhitelistDto
         :rtype: ~ignos.api.client.models.MeasuringToolWhitelistDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30695,15 +32768,15 @@
         :param body: Is either a UpdateWhitelistedMeasuringTool type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateWhitelistedMeasuringTool or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30756,15 +32829,15 @@
 
         :param id: Required.
         :type id: str
         :return: ProblemDetails or None
         :rtype: ~ignos.api.client.models.ProblemDetails or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30806,15 +32879,15 @@
     def list_unregistered_tool_values(self, **kwargs: Any) -> List[_models.UnregisteredToolValueDto]:
         """list_unregistered_tool_values.
 
         :return: list of UnregisteredToolValueDto
         :rtype: list[~ignos.api.client.models.UnregisteredToolValueDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30901,15 +32974,15 @@
         :type id: str
         :param body: Is either a DeprecateToolRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.DeprecateToolRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -30964,15 +33037,15 @@
 
         :keyword status: Known values are: "SoonDue" and "Expired". Default value is None.
         :paramtype status: str or ~ignos.api.client.models.CalibrationListStatus
         :return: list of CalibrationListToolDto
         :rtype: list[~ignos.api.client.models.CalibrationListToolDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31053,15 +33126,15 @@
 
         :param body: Is either a ImportMeasuringTool type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ImportMeasuringTool or IO[bytes]
         :return: MeasuringToolDetailDto
         :rtype: ~ignos.api.client.models.MeasuringToolDetailDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31157,15 +33230,15 @@
         :param body: Is either a UpdateMeasuringToolSettings type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateMeasuringToolSettings or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31215,15 +33288,15 @@
     def get_measuring_tool_settings(self, **kwargs: Any) -> _models.MeasuringToolSettingsDto:
         """get_measuring_tool_settings.
 
         :return: MeasuringToolSettingsDto
         :rtype: ~ignos.api.client.models.MeasuringToolSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31282,15 +33355,15 @@
     def get_worker_details_for_current_user(self, **kwargs: Any) -> _models.WorkerDto:
         """get_worker_details_for_current_user.
 
         :return: WorkerDto
         :rtype: ~ignos.api.client.models.WorkerDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31353,15 +33426,15 @@
         :type drawing_number: str
         :param id: Required.
         :type id: str
         :return: DocumentLinkDto
         :rtype: ~ignos.api.client.models.DocumentLinkDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31459,15 +33532,15 @@
 
         :param body: Is either a AddMesLink type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.AddMesLink or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31513,48 +33586,95 @@
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def list_mes_links(
         self,
         *,
-        company_id: Optional[str] = None,
-        type: Optional[Union[str, _models.MesLinkTypeDto]] = None,
-        operation_id: Optional[str] = None,
+        types: Optional[List[Union[str, _models.MesLinkTypeDto]]] = None,
+        work_order_id: Optional[str] = None,
+        operation: Optional[int] = None,
         **kwargs: Any,
     ) -> List[_models.MesLinkDto]:
         """list_mes_links.
 
-        :keyword company_id: Default value is None.
-        :paramtype company_id: str
-        :keyword type: Known values are: "Static", "Operation", and "WorkOrder". Default value is None.
-        :paramtype type: str or ~ignos.api.client.models.MesLinkTypeDto
-        :keyword operation_id: Default value is None.
-        :paramtype operation_id: str
+        :keyword types: Default value is None.
+        :paramtype types: list[str or ~ignos.api.client.models.MesLinkTypeDto]
+        :keyword work_order_id: Default value is None.
+        :paramtype work_order_id: str
+        :keyword operation: Default value is None.
+        :paramtype operation: int
         :return: list of MesLinkDto
         :rtype: list[~ignos.api.client.models.MesLinkDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.MesLinkDto]] = kwargs.pop("cls", None)
 
         _request = build_mes_links_list_mes_links_request(
-            company_id=company_id,
-            type=type,
-            operation_id=operation_id,
+            types=types,
+            work_order_id=work_order_id,
+            operation=operation,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[MesLinkDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace
+    def list_unmapped_mes_links(self, **kwargs: Any) -> List[_models.MesLinkDto]:
+        """list_unmapped_mes_links.
+
+        :return: list of MesLinkDto
+        :rtype: list[~ignos.api.client.models.MesLinkDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.MesLinkDto]] = kwargs.pop("cls", None)
+
+        _request = build_mes_links_list_unmapped_mes_links_request(
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
@@ -31628,15 +33748,15 @@
         :type id: str
         :param body: Is either a UpdateMesLink type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateMesLink or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31689,15 +33809,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31755,15 +33875,15 @@
 
         :param id: Required.
         :type id: str
         :return: ProductionOrderDto
         :rtype: ~ignos.api.client.models.ProductionOrderDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31809,15 +33929,15 @@
         :type id: str
         :keyword operation: Default value is None.
         :paramtype operation: int
         :return: list of ProductionOrderBomDto
         :rtype: list[~ignos.api.client.models.ProductionOrderBomDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31864,15 +33984,15 @@
         :type id: str
         :keyword operation: Default value is None.
         :paramtype operation: int
         :return: list of PickListSuggestionDto
         :rtype: list[~ignos.api.client.models.PickListSuggestionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31917,15 +34037,15 @@
 
         :param id: Required.
         :type id: str
         :return: bool
         :rtype: bool
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -31971,15 +34091,15 @@
         :type id: str
         :keyword only_open: Default value is True.
         :paramtype only_open: bool
         :return: list of NonConformanceDto
         :rtype: list[~ignos.api.client.models.NonConformanceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32075,15 +34195,15 @@
         :type operation_number: int
         :param body: Is either a PostMaterialPickListRequest type or a IO[bytes] type. Required.
         :type body: ~ignos.api.client.models.PostMaterialPickListRequest or IO[bytes]
         :return: MaterialPickListResultDto
         :rtype: ~ignos.api.client.models.MaterialPickListResultDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32128,14 +34248,69 @@
         deserialized = self._deserialize("MaterialPickListResultDto", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
+    @distributed_trace
+    def list_production_order_activities(
+        self, id: str, *, operation: Optional[int] = None, **kwargs: Any
+    ) -> List[_models.ProductionOrderOperationActivityDto]:
+        """list_production_order_activities.
+
+        :param id: Required.
+        :type id: str
+        :keyword operation: Default value is None.
+        :paramtype operation: int
+        :return: list of ProductionOrderOperationActivityDto
+        :rtype: list[~ignos.api.client.models.ProductionOrderOperationActivityDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.ProductionOrderOperationActivityDto]] = kwargs.pop("cls", None)
+
+        _request = build_mes_production_order_list_production_order_activities_request(
+            id=id,
+            operation=operation,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[ProductionOrderOperationActivityDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
 
 class MesProductionScheduleOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -32187,15 +34362,15 @@
         :paramtype part_name: str
         :keyword material: Default value is None.
         :paramtype material: str
         :return: ProductionScheduleOperationDtoPagedResult
         :rtype: ~ignos.api.client.models.ProductionScheduleOperationDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32285,15 +34460,15 @@
         :param body: Is either a ListProductionScheduleOperationsRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.ListProductionScheduleOperationsRequest or IO[bytes]
         :return: ProductionScheduleOperationDtoPagedResult
         :rtype: ~ignos.api.client.models.ProductionScheduleOperationDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32391,15 +34566,15 @@
         :param body: Is either a GetAvailableProductionScheduleFiltersRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.GetAvailableProductionScheduleFiltersRequest or IO[bytes]
         :return: ProductionScheduleFiltersDto
         :rtype: ~ignos.api.client.models.ProductionScheduleFiltersDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32446,33 +34621,33 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
-    def list_my_current_work_activities(self, **kwargs: Any) -> List[_models.CurrentWorkActivityDto]:
+    def list_my_current_work_activities(self, **kwargs: Any) -> _models.CurrentWorkActivityDto:
         """list_my_current_work_activities.
 
-        :return: list of CurrentWorkActivityDto
-        :rtype: list[~ignos.api.client.models.CurrentWorkActivityDto]
+        :return: CurrentWorkActivityDto
+        :rtype: ~ignos.api.client.models.CurrentWorkActivityDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[List[_models.CurrentWorkActivityDto]] = kwargs.pop("cls", None)
+        cls: ClsType[_models.CurrentWorkActivityDto] = kwargs.pop("cls", None)
 
         _request = build_mes_production_schedule_list_my_current_work_activities_request(
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -32485,41 +34660,41 @@
 
         if response.status_code not in [200]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
-        deserialized = self._deserialize("[CurrentWorkActivityDto]", pipeline_response)
+        deserialized = self._deserialize("CurrentWorkActivityDto", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     @distributed_trace
-    def list_my_current_work_activities_v2(self, **kwargs: Any) -> _models.CurrentWorkActivityV2Dto:
+    def list_my_current_work_activities_v2(self, **kwargs: Any) -> _models.CurrentWorkActivityDto:
         """list_my_current_work_activities_v2.
 
-        :return: CurrentWorkActivityV2Dto
-        :rtype: ~ignos.api.client.models.CurrentWorkActivityV2Dto
+        :return: CurrentWorkActivityDto
+        :rtype: ~ignos.api.client.models.CurrentWorkActivityDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[_models.CurrentWorkActivityV2Dto] = kwargs.pop("cls", None)
+        cls: ClsType[_models.CurrentWorkActivityDto] = kwargs.pop("cls", None)
 
         _request = build_mes_production_schedule_list_my_current_work_activities_v2_request(
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -32532,15 +34707,15 @@
 
         if response.status_code not in [200]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
-        deserialized = self._deserialize("CurrentWorkActivityV2Dto", pipeline_response)
+        deserialized = self._deserialize("CurrentWorkActivityDto", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     @overload
@@ -32584,15 +34759,15 @@
 
         :param body: Is either a StartOperations type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.StartOperations or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32684,15 +34859,15 @@
         :param body: Is either a ReportOperationProgress type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ReportOperationProgress or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32748,15 +34923,15 @@
         :paramtype resource_group: str
         :keyword resource_id: Default value is None.
         :paramtype resource_id: str
         :return: ScheduledWorkSummaryDto
         :rtype: ~ignos.api.client.models.ScheduledWorkSummaryDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32858,15 +35033,15 @@
 
         :param body: Is either a ListProjectsRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListProjectsRequest or IO[bytes]
         :return: WorkOrderProjectDtoPagedResult
         :rtype: ~ignos.api.client.models.WorkOrderProjectDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -32962,15 +35137,15 @@
         :param body: Is either a ListOrderScheduleRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ListOrderScheduleRequest or IO[bytes]
         :return: WorkorderDtoPagedResult
         :rtype: ~ignos.api.client.models.WorkorderDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33046,15 +35221,15 @@
 
         :keyword include_resources: Default value is False.
         :paramtype include_resources: bool
         :return: list of ResourceGroupDto
         :rtype: list[~ignos.api.client.models.ResourceGroupDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33096,15 +35271,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of ProductionResourceDto
         :rtype: list[~ignos.api.client.models.ProductionResourceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33170,15 +35345,15 @@
         :paramtype customer_order: str
         :keyword customer_order_line: Default value is None.
         :paramtype customer_order_line: int
         :return: list of MrbInstanceDto
         :rtype: list[~ignos.api.client.models.MrbInstanceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33256,15 +35431,15 @@
 
         :param body: Is either a CreateMrb type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateMrb or IO[bytes]
         :return: MrbInstanceJobDto
         :rtype: ~ignos.api.client.models.MrbInstanceJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33318,15 +35493,15 @@
     def list_recent_mrb_intances(self, **kwargs: Any) -> List[_models.MrbInstanceDto]:
         """list_recent_mrb_intances.
 
         :return: list of MrbInstanceDto
         :rtype: list[~ignos.api.client.models.MrbInstanceDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33367,15 +35542,15 @@
 
         :param id: Required.
         :type id: str
         :return: MrbInstanceDto
         :rtype: ~ignos.api.client.models.MrbInstanceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33417,15 +35592,15 @@
 
         :param id: Required.
         :type id: str
         :return: list of MrbInstanceRevisionDto
         :rtype: list[~ignos.api.client.models.MrbInstanceRevisionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33514,15 +35689,15 @@
         :param body: Is either a CreateMrbRevisionRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMrbRevisionRequest or IO[bytes]
         :return: MrbInstanceJobDto
         :rtype: ~ignos.api.client.models.MrbInstanceJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33581,15 +35756,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: MrbContentDto
         :rtype: ~ignos.api.client.models.MrbContentDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33636,15 +35811,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33687,15 +35862,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33736,15 +35911,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: MrbPdfExportJobDto
         :rtype: ~ignos.api.client.models.MrbPdfExportJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33789,15 +35964,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: MrbInstanceJobDto
         :rtype: ~ignos.api.client.models.MrbInstanceJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -33904,15 +36079,15 @@
         :param body: Is either a IncludeExcludeMrbRevisionContentRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.IncludeExcludeMrbRevisionContentRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34030,15 +36205,15 @@
         :param body: Is either a IncludeExcludeMrbRevisionContentRequest type or a IO[bytes] type.
          Default value is None.
         :type body: ~ignos.api.client.models.IncludeExcludeMrbRevisionContentRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34155,15 +36330,15 @@
         :type revision_id: int
         :param body: Is either a AttachPdfRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.AttachPdfRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34221,15 +36396,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34270,15 +36445,15 @@
         :type id: str
         :param revision_id: Required.
         :type revision_id: int
         :return: DownloadDto
         :rtype: ~ignos.api.client.models.DownloadDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34321,15 +36496,15 @@
 
         :param job_id: Required.
         :type job_id: str
         :return: MrbInstanceJobDto
         :rtype: ~ignos.api.client.models.MrbInstanceJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34371,15 +36546,15 @@
 
         :param job_id: Required.
         :type job_id: str
         :return: MrbPdfExportJobDto
         :rtype: ~ignos.api.client.models.MrbPdfExportJobDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34425,15 +36600,15 @@
         :paramtype page_size: int
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: MrbInstanceReportDtoPagedResult
         :rtype: ~ignos.api.client.models.MrbInstanceReportDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34516,15 +36691,15 @@
         :param body: Is either a ListMrbInstanceReportsRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.ListMrbInstanceReportsRequest or IO[bytes]
         :return: MrbInstanceReportDtoPagedResult
         :rtype: ~ignos.api.client.models.MrbInstanceReportDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34631,15 +36806,15 @@
         :type template_id: str
         :param body: Is either a AttachPdfRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.AttachPdfRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34694,15 +36869,15 @@
 
         :param template_id: Required.
         :type template_id: str
         :return: MrbTemplateDto
         :rtype: ~ignos.api.client.models.MrbTemplateDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34750,15 +36925,15 @@
         :paramtype customer_id: str
         :keyword customer_group_id: Default value is None.
         :paramtype customer_group_id: str
         :return: list of MrbTemplateDto
         :rtype: list[~ignos.api.client.models.MrbTemplateDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34847,15 +37022,15 @@
         :param body: Is either a CreateMrbTemplateRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateMrbTemplateRequest or IO[bytes]
         :return: MrbTemplateDto
         :rtype: ~ignos.api.client.models.MrbTemplateDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -34952,15 +37127,15 @@
 
         :param body: Is either a UpdateMrbTemplate type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateMrbTemplate or IO[bytes]
         :return: MrbTemplateDto
         :rtype: ~ignos.api.client.models.MrbTemplateDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35062,15 +37237,15 @@
         :param body: Is either a DeleteMrbTemplateRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.DeleteMrbTemplateRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35120,15 +37295,15 @@
     def get_mrb_company_settings(self, **kwargs: Any) -> _models.MrbCompanySettingsDto:
         """get_mrb_company_settings.
 
         :return: MrbCompanySettingsDto
         :rtype: ~ignos.api.client.models.MrbCompanySettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35209,15 +37384,15 @@
         :param body: Is either a UpsertMrbCompanySettings type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpsertMrbCompanySettings or IO[bytes]
         :return: MrbCompanySettingsDto
         :rtype: ~ignos.api.client.models.MrbCompanySettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35341,15 +37516,15 @@
         :param body: Contains diameter, and one of cutting speed or spindle speed. Is either a
          CalculateSpindleAndCuttingSpeed type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CalculateSpindleAndCuttingSpeed or IO[bytes]
         :return: SpindleAndCuttingSpeedDto
         :rtype: ~ignos.api.client.models.SpindleAndCuttingSpeedDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35457,15 +37632,15 @@
         :param body: Contains the two parameters to calculate from. Is either a
          CalculateRightAngledTriangle type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CalculateRightAngledTriangle or IO[bytes]
         :return: RightAngledTriangleDto
         :rtype: ~ignos.api.client.models.RightAngledTriangleDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35521,15 +37696,15 @@
 
         List default material types with mass density.
 
         :return: list of MaterialMassDensityDto
         :rtype: list[~ignos.api.client.models.MaterialMassDensityDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35616,15 +37791,15 @@
         :param body: Contains dimensions and mass density for given material. Is either a
          CalculateBarWeight type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CalculateBarWeight or IO[bytes]
         :return: MaterialWeightDto
         :rtype: ~ignos.api.client.models.MaterialWeightDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35700,15 +37875,15 @@
 
         :keyword country: Default value is None.
         :paramtype country: str
         :return: list of PowerRegionDto
         :rtype: list[~ignos.api.client.models.PowerRegionDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35770,15 +37945,15 @@
 
         :param component_id: Required.
         :type component_id: str
         :return: ComponentSettingsDto
         :rtype: ~ignos.api.client.models.ComponentSettingsDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35838,15 +38013,15 @@
     def list_supplier_invites(self, **kwargs: Any) -> List[_models.SupplierInviteDto]:
         """list_supplier_invites.
 
         :return: list of SupplierInviteDto
         :rtype: list[~ignos.api.client.models.SupplierInviteDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35926,15 +38101,15 @@
 
         :param body: Is either a CreateSupplierInvite type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateSupplierInvite or IO[bytes]
         :return: SupplierInviteDto
         :rtype: ~ignos.api.client.models.SupplierInviteDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -35990,15 +38165,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36034,15 +38209,15 @@
     def list_suppliers(self, **kwargs: Any) -> List[_models.ExternalSupplierDto]:
         """list_suppliers.
 
         :return: list of ExternalSupplierDto
         :rtype: list[~ignos.api.client.models.ExternalSupplierDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36083,15 +38258,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36164,15 +38339,15 @@
 
         :param body: Is either a ImportSupplier type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ImportSupplier or IO[bytes]
         :return: ExternalSupplierDto
         :rtype: ~ignos.api.client.models.ExternalSupplierDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36273,15 +38448,15 @@
 
         :param body: Is either a CreateSupplierMapping type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateSupplierMapping or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36333,15 +38508,15 @@
 
         Delete all supplier mappings between old supplier ids and new supplier ids.
 
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36396,15 +38571,15 @@
     def test(self, **kwargs: Any) -> str:
         """test.
 
         :return: str
         :rtype: str
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36480,15 +38655,15 @@
 
         :param body: Is either a GetConsumption type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.GetConsumption or IO[bytes]
         :return: ConsumptionDto
         :rtype: ~ignos.api.client.models.ConsumptionDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36577,15 +38752,15 @@
 
         :param body: Is either a GetPower type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.GetPower or IO[bytes]
         :return: PowerDto
         :rtype: ~ignos.api.client.models.PowerDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36696,15 +38871,15 @@
         :param body: Is either a CustomerOrderConsumptionRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CustomerOrderConsumptionRequest or IO[bytes]
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36761,15 +38936,15 @@
 
         :param external_id: Required.
         :type external_id: str
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36811,15 +38986,15 @@
 
         :param external_id: Required.
         :type external_id: str
         :return: JSON
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36901,15 +39076,15 @@
         :param body: Is either a CreateCustomerOrderLineGhgReport type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.CreateCustomerOrderLineGhgReport or IO[bytes]
         :return: DownloadDto
         :rtype: ~ignos.api.client.models.DownloadDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -36985,15 +39160,15 @@
 
         :keyword asset_id: Default value is None.
         :paramtype asset_id: int
         :return: DataHealthDto
         :rtype: ~ignos.api.client.models.DataHealthDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37055,15 +39230,15 @@
 
         :param id: Required.
         :type id: str
         :return: TraceDto
         :rtype: ~ignos.api.client.models.TraceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37151,15 +39326,15 @@
         :type id: str
         :param body: Is either a UpdateTraceRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.UpdateTraceRequest or IO[bytes]
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37212,15 +39387,15 @@
 
         :param id: Required.
         :type id: str
         :return: TraceDto
         :rtype: ~ignos.api.client.models.TraceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37264,15 +39439,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37300,29 +39475,140 @@
                 response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
+    @overload
+    def set_trace_manual_completed(  # pylint: disable=inconsistent-return-statements
+        self,
+        id: str,
+        body: Optional[_models.UpdateTraceManualCompletionRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """set_trace_manual_completed.
+
+        :param id: Required.
+        :type id: str
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.UpdateTraceManualCompletionRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def set_trace_manual_completed(  # pylint: disable=inconsistent-return-statements
+        self, id: str, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """set_trace_manual_completed.
+
+        :param id: Required.
+        :type id: str
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def set_trace_manual_completed(  # pylint: disable=inconsistent-return-statements
+        self,
+        id: str,
+        body: Optional[Union[_models.UpdateTraceManualCompletionRequest, IO[bytes]]] = None,
+        **kwargs: Any,
+    ) -> None:
+        """set_trace_manual_completed.
+
+        :param id: Required.
+        :type id: str
+        :param body: Is either a UpdateTraceManualCompletionRequest type or a IO[bytes] type. Default
+         value is None.
+        :type body: ~ignos.api.client.models.UpdateTraceManualCompletionRequest or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UpdateTraceManualCompletionRequest")
+            else:
+                _json = None
+
+        _request = build_trace_set_trace_manual_completed_request(
+            id=id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
     @distributed_trace
     def list_customer_order_line_traces(
         self, *, customer_order: Optional[str] = None, customer_order_line: Optional[int] = None, **kwargs: Any
     ) -> List[_models.CustomerOrderLineTraceItemDto]:
         """list_customer_order_line_traces.
 
         :keyword customer_order: Default value is None.
         :paramtype customer_order: str
         :keyword customer_order_line: Default value is None.
         :paramtype customer_order_line: int
         :return: list of CustomerOrderLineTraceItemDto
         :rtype: list[~ignos.api.client.models.CustomerOrderLineTraceItemDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37369,15 +39655,15 @@
         :type id: str
         :keyword line: Default value is None.
         :paramtype line: int
         :return: CustomerOrderTraceStatusDto
         :rtype: ~ignos.api.client.models.CustomerOrderTraceStatusDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37444,15 +39730,15 @@
         :keyword continuation_token_parameter: Continuation token used for pagination. Default value is
          None.
         :paramtype continuation_token_parameter: str
         :return: TraceWorkOrderListDtoPagedResult
         :rtype: ~ignos.api.client.models.TraceWorkOrderListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37538,15 +39824,15 @@
         :param body: Is either a ListTraceWorkordersRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.ListTraceWorkordersRequest or IO[bytes]
         :return: TraceWorkOrderListDtoPagedResult
         :rtype: ~ignos.api.client.models.TraceWorkOrderListDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37593,14 +39879,484 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
 
+class TrackingOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.IgnosPortal`'s
+        :attr:`tracking` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace
+    def list_tracking_history(self, tracking_id: str, **kwargs: Any) -> _models.TrackingHistoryDto:
+        """list_tracking_history.
+
+        :param tracking_id: Required.
+        :type tracking_id: str
+        :return: TrackingHistoryDto
+        :rtype: ~ignos.api.client.models.TrackingHistoryDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.TrackingHistoryDto] = kwargs.pop("cls", None)
+
+        _request = build_tracking_list_tracking_history_request(
+            tracking_id=tracking_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("TrackingHistoryDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace
+    def list_work_order_tracking_history(self, work_order_id: str, **kwargs: Any) -> _models.TrackingWorkOrderDto:
+        """list_work_order_tracking_history.
+
+        :param work_order_id: Required.
+        :type work_order_id: str
+        :return: TrackingWorkOrderDto
+        :rtype: ~ignos.api.client.models.TrackingWorkOrderDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.TrackingWorkOrderDto] = kwargs.pop("cls", None)
+
+        _request = build_tracking_list_work_order_tracking_history_request(
+            work_order_id=work_order_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("TrackingWorkOrderDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    def create_tracking_events(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[List[_models.TrackingUpdateDto]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """create_tracking_events.
+
+        :param body: Default value is None.
+        :type body: list[~ignos.api.client.models.TrackingUpdateDto]
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create_tracking_events(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_tracking_events.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create_tracking_events(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[List[_models.TrackingUpdateDto], IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_tracking_events.
+
+        :param body: Is either a [TrackingUpdateDto] type or a IO[bytes] type. Default value is None.
+        :type body: list[~ignos.api.client.models.TrackingUpdateDto] or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "[TrackingUpdateDto]")
+            else:
+                _json = None
+
+        _request = build_tracking_create_tracking_events_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    def create_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[List[_models.TrackingHistoryUpdateDto]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """create_tracking_history.
+
+        :param body: Default value is None.
+        :type body: list[~ignos.api.client.models.TrackingHistoryUpdateDto]
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """create_tracking_history.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[List[_models.TrackingHistoryUpdateDto], IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """create_tracking_history.
+
+        :param body: Is either a [TrackingHistoryUpdateDto] type or a IO[bytes] type. Default value is
+         None.
+        :type body: list[~ignos.api.client.models.TrackingHistoryUpdateDto] or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "[TrackingHistoryUpdateDto]")
+            else:
+                _json = None
+
+        _request = build_tracking_create_tracking_history_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @overload
+    def delete_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[List[_models.TrackingHistoryUpdateDto]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> None:
+        """delete_tracking_history.
+
+        :param body: Default value is None.
+        :type body: list[~ignos.api.client.models.TrackingHistoryUpdateDto]
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def delete_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO[bytes]] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """delete_tracking_history.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def delete_tracking_history(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[List[_models.TrackingHistoryUpdateDto], IO[bytes]]] = None, **kwargs: Any
+    ) -> None:
+        """delete_tracking_history.
+
+        :param body: Is either a [TrackingHistoryUpdateDto] type or a IO[bytes] type. Default value is
+         None.
+        :type body: list[~ignos.api.client.models.TrackingHistoryUpdateDto] or IO[bytes]
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "[TrackingHistoryUpdateDto]")
+            else:
+                _json = None
+
+        _request = build_tracking_delete_tracking_history_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @distributed_trace
+    def create_label(  # pylint: disable=inconsistent-return-statements
+        self, work_order_id: str, *, pallet_count: Optional[int] = None, **kwargs: Any
+    ) -> None:
+        """create_label.
+
+        :param work_order_id: Required.
+        :type work_order_id: str
+        :keyword pallet_count: Default value is None.
+        :paramtype pallet_count: int
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        _request = build_tracking_create_label_request(
+            work_order_id=work_order_id,
+            pallet_count=pallet_count,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+
 class UploadOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.IgnosPortal`'s
@@ -37620,15 +40376,15 @@
     def create_upload_info(self, **kwargs: Any) -> _models.UploadInfoDto:
         """create_upload_info.
 
         :return: UploadInfoDto
         :rtype: ~ignos.api.client.models.UploadInfoDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37700,15 +40456,15 @@
         :paramtype filter: str
         :keyword continuation_token_parameter: Default value is None.
         :paramtype continuation_token_parameter: str
         :return: UserDtoPagedResult
         :rtype: ~ignos.api.client.models.UserDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37787,15 +40543,15 @@
 
         :param body: Is either a ListUsersRequest type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.ListUsersRequest or IO[bytes]
         :return: UserDtoPagedResult
         :rtype: ~ignos.api.client.models.UserDtoPagedResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37869,15 +40625,15 @@
     def get_my_workspaces(self, **kwargs: Any) -> List[_models.WorkspaceListDto]:
         """get_my_workspaces.
 
         :return: list of WorkspaceListDto
         :rtype: list[~ignos.api.client.models.WorkspaceListDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -37953,15 +40709,15 @@
 
         :param body: Is either a CreateWorkspace type or a IO[bytes] type. Default value is None.
         :type body: ~ignos.api.client.models.CreateWorkspace or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38057,15 +40813,15 @@
         :param body: Is either a CreateWorkspaceFromTemplate type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateWorkspaceFromTemplate or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38121,15 +40877,15 @@
 
         :param id: Required.
         :type id: str
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38171,15 +40927,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38264,15 +41020,15 @@
         :param body: Is either a UpdateWorkspaceRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38376,15 +41132,15 @@
         :param body: Is either a UpdateWorkspaceWidgetsRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceWidgetsRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38505,15 +41261,15 @@
         :param body: Is either a UpdateWorkspaceWidgetSettingsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceWidgetSettingsRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38573,15 +41329,15 @@
         :type id: str
         :param widget_id: Required.
         :type widget_id: str
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38684,15 +41440,15 @@
         :param body: Is either a CreateWorkspaceTemplate type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.CreateWorkspaceTemplate or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38748,15 +41504,15 @@
 
         :param id: Required.
         :type id: str
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38800,15 +41556,15 @@
 
         :param id: Required.
         :type id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -38893,15 +41649,15 @@
         :param body: Is either a UpdateWorkspaceRequest type or a IO[bytes] type. Default value is
          None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -39005,15 +41761,15 @@
         :param body: Is either a UpdateWorkspaceWidgetsRequest type or a IO[bytes] type. Default value
          is None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceWidgetsRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -39134,15 +41890,15 @@
         :param body: Is either a UpdateWorkspaceWidgetSettingsRequest type or a IO[bytes] type. Default
          value is None.
         :type body: ~ignos.api.client.models.UpdateWorkspaceWidgetSettingsRequest or IO[bytes]
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -39202,15 +41958,15 @@
         :type id: str
         :param widget_id: Required.
         :type widget_id: str
         :return: WorkspaceDto
         :rtype: ~ignos.api.client.models.WorkspaceDto
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -39271,15 +42027,15 @@
     def get_workspace_templates(self, **kwargs: Any) -> List[_models.WorkspaceListDto]:
         """get_workspace_templates.
 
         :return: list of WorkspaceListDto
         :rtype: list[~ignos.api.client.models.WorkspaceListDto]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `ignos-api-client-2024.3.12.8830/ignos/api/client/operations/_patch.py` & `ignos_api_client-2024.5.28.9351/ignos/api/client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2024.3.12.8830/ignos_api_client.egg-info/SOURCES.txt` & `ignos_api_client-2024.5.28.9351/ignos_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

