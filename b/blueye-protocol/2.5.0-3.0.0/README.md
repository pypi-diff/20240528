# Comparing `tmp/blueye_protocol-2.5.0.tar.gz` & `tmp/blueye.protocol-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueye_protocol-2.5.0.tar", max compression
+gzip compressed data, was "blueye.protocol-3.0.0.tar", max compression
```

## Comparing `blueye_protocol-2.5.0.tar` & `blueye.protocol-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,13 @@
--rw-r--r--   0        0        0     7652 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/LICENSE
--rw-r--r--   0        0        0     2748 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/README.md
--rw-r--r--   0        0        0      128 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/blueye/__init__.py
--rw-r--r--   0        0        0      311 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/blueye/protocol/__init__.py
--rw-r--r--   0        0        0     1329 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/blueye/protocol/exceptions.py
--rw-r--r--   0        0        0    17973 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/blueye/protocol/protos.py
--rw-r--r--   0        0        0    11826 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/blueye/protocol/types/__init__.py
--rw-r--r--   0        0        0    24784 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/blueye/protocol/types/aquatroll.py
--rw-r--r--   0        0        0    12736 2024-05-28 18:35:10.565574 blueye_protocol-2.5.0/blueye/protocol/types/control.py
--rw-r--r--   0        0        0    71389 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/types/message_formats.py
--rw-r--r--   0        0        0    18316 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/types/mission_planning.py
--rw-r--r--   0        0        0    10573 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/types/req_rep.py
--rw-r--r--   0        0        0    18036 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/types/telemetry.py
--rw-r--r--   0        0        0        0 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/v2/__init__.py
--rwxr-xr-x   0        0        0     5219 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/v2/tcp_client.py
--rw-r--r--   0        0        0    37722 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/v2/tcp_protocol_class.py
--rwxr-xr-x   0        0        0     2744 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/v2/udp_client.py
--rw-r--r--   0        0        0    23217 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/v2/udp_protocol_dict.py
--rwxr-xr-x   0        0        0     3738 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/blueye/protocol/v2/udp_protocol_parser.py
--rw-r--r--   0        0        0     1076 2024-05-28 18:35:10.569574 blueye_protocol-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 blueye_protocol-2.5.0/setup.py
--rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 blueye_protocol-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      608 2022-09-15 09:34:34.569966 blueye.protocol-3.0.0/README.md
+-rw-r--r--   0        0        0      173 2022-09-15 09:34:34.569966 blueye.protocol-3.0.0/blueye/__init__.py
+-rw-r--r--   0        0        0    10054 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/__init__.py
+-rw-r--r--   0        0        0       76 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/py.typed
+-rw-r--r--   0        0        0      601 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/services/__init__.py
+-rw-r--r--   0        0        0     6621 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/__init__.py
+-rw-r--r--   0        0        0     8621 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/control.py
+-rw-r--r--   0        0        0    48847 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/message_formats.py
+-rw-r--r--   0        0        0     5985 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/req_rep.py
+-rw-r--r--   0        0        0    10713 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/telemetry.py
+-rw-r--r--   0        0        0      696 2022-09-15 09:34:34.573966 blueye.protocol-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1374 2022-09-15 09:35:00.250462 blueye.protocol-3.0.0/setup.py
+-rw-r--r--   0        0        0     1417 2022-09-15 09:35:00.250781 blueye.protocol-3.0.0/PKG-INFO
```

### Comparing `blueye_protocol-2.5.0/blueye/protocol/types/__init__.py` & `blueye.protocol-3.0.0/blueye/protocol/types/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,49 +15,42 @@
 # limitations under the License.
 #
 
 from .message_formats import (
     BinlogRecord,
     MotionInput,
     Lights,
-    Laser,
     LatLongPosition,
     ConnectionDuration,
     AutoHeadingState,
     AutoDepthState,
     AutoAltitudeState,
     StationKeepingState,
     WeatherVaningState,
-    AutoPilotSurgeYawState,
-    AutoPilotHeaveState,
     ControlMode,
     TiltStabilizationState,
     SystemTime,
     GripperVelocities,
     ClientInfo,
     ConnectedClient,
     RecordState,
-    TimeLapseState,
     WaterDensity,
     PingerConfiguration,
     WaterTemperature,
     CPUTemperature,
     CanisterTemperature,
     CanisterHumidity,
     Battery,
     BatteryBQ40Z50,
     Attitude,
     Altitude,
     ForwardDistance,
     PositionEstimate,
-    ResetPositionSettings,
     Depth,
     Reference,
-    Notification,
-    ControlForce,
     ControllerHealth,
     DiveTime,
     RecordOn,
     StorageSpace,
     CalibrationState,
     IperfStatus,
     NStreamers,
@@ -68,177 +61,88 @@
     CameraParameters,
     OverlayParameters,
     NavigationSensorStatus,
     GuestPortDevice,
     GuestPortDeviceList,
     GuestPortConnectorInfo,
     GuestPortInfo,
-    GuestPortRestartInfo,
     ThicknessGauge,
     CpProbe,
-    GenericServo,
-    MultibeamServo,
-    GuestPortCurrent,
-    Vector3,
-    Imu,
-    MedusaSpectrometerData,
-    IntervalType,
-    HeadingSource,
-    ResetCoordinateSource,
-    NotificationType,
-    NotificationLevel,
     Model,
     PressureSensorType,
     Resolution,
     Framerate,
     Camera,
     TemperatureUnit,
     LogoType,
     DepthUnit,
     ThicknessUnit,
     FontSize,
     GuestPortDeviceID,
-    GuestPortNumber,
     NavigationSensorID,
-    GuestPortDetachStatus,
     GuestPortError,
 )
-from .mission_planning import (
-    Mission,
-    Instruction,
-    DepthSetPoint,
-    Waypoint,
-    ControlModeCommand,
-    WaypointCommand,
-    DepthSetPointCommand,
-    TiltMainCameraCommand,
-    TiltMultibeamCommand,
-    WaitForCommand,
-    CameraCommand,
-    GoToSurfaceCommand,
-    GoToSeabedCommand,
-    GoToHomeCommand,
-    PathSegment,
-    ReferenceAutoPilot,
-    MissionStatus,
-    DepthZeroReference,
-    ControlModeVertical,
-    ControlModeHorizontal,
-    CameraAction,
-    InstructionType,
-    MissionState,
-)
-from .aquatroll import (
-    AquaTrollParameterBlock,
-    AquaTrollSensorMetadata,
-    AquaTrollSensorMetadataArray,
-    AquaTrollProbeMetadata,
-    AquaTrollSensorParameters,
-    AquaTrollSensorParametersArray,
-    SetAquaTrollParameterUnit,
-    SetAquaTrollConnectionStatus,
-    Type,
-    AquaTrollDevice,
-    AquaTrollQuality,
-    AquaTrollParameter,
-    AquaTrollUnit,
-    AquaTrollSensor,
-    AquaTrollSensorStatus,
-    AquaTrollDeviceStatus,
+from .control import (
+    MotionInputCtrl,
+    TiltVelocityCtrl,
+    LightsCtrl,
+    GuestportLightsCtrl,
+    PilotGPSPositionCtrl,
+    WatchdogCtrl,
+    RecordCtrl,
+    TakePictureCtrl,
+    StartCalibrationCtrl,
+    CancelCalibrationCtrl,
+    FinishCalibrationCtrl,
+    AutoHeadingCtrl,
+    AutoDepthCtrl,
+    AutoAltitudeCtrl,
+    StationKeepingCtrl,
+    WeatherVaningCtrl,
+    ResetPositionCtrl,
+    ResetOdometerCtrl,
+    TiltStabilizationCtrl,
+    WaterDensityCtrl,
+    PingerConfigurationCtrl,
+    SystemTimeCtrl,
+    GripperCtrl,
 )
 from .telemetry import (
     AttitudeTel,
     AltitudeTel,
     ForwardDistanceTel,
     PositionEstimateTel,
     DepthTel,
     ReferenceTel,
-    ReferenceAutoPilotTel,
-    MissionStatusTel,
-    NotificationTel,
-    ControlForceTel,
     ControllerHealthTel,
     LightsTel,
     GuestPortLightsTel,
-    LaserTel,
     PilotGPSPositionTel,
     RecordStateTel,
-    TimeLapseStateTel,
     BatteryTel,
     BatteryBQ40Z50Tel,
     DiveTimeTel,
     DroneTimeTel,
     WaterTemperatureTel,
     CPUTemperatureTel,
-    CanisterTopTemperatureTel,
-    CanisterBottomTemperatureTel,
-    CanisterTopHumidityTel,
-    CanisterBottomHumidityTel,
+    CanisterTemperatureTel,
+    CanisterHumidityTel,
     VideoStorageSpaceTel,
     DataStorageSpaceTel,
     CalibrationStateTel,
     TiltStabilizationTel,
     IperfTel,
     NStreamersTel,
     TiltAngleTel,
     DroneInfoTel,
     ErrorFlagsTel,
     ControlModeTel,
     ThicknessGaugeTel,
     CpProbeTel,
-    AquaTrollProbeMetadataTel,
-    AquaTrollSensorMetadataTel,
-    AquaTrollSensorParametersTel,
     ConnectedClientsTel,
-    GenericServoTel,
-    MultibeamServoTel,
-    GuestPortCurrentTel,
-    CalibratedImuTel,
-    Imu1Tel,
-    Imu2Tel,
-    MedusaSpectrometerDataTel,
-)
-from .control import (
-    MotionInputCtrl,
-    TiltVelocityCtrl,
-    LightsCtrl,
-    GuestportLightsCtrl,
-    LaserCtrl,
-    PilotGPSPositionCtrl,
-    WatchdogCtrl,
-    RecordCtrl,
-    TakePictureCtrl,
-    StartCalibrationCtrl,
-    CancelCalibrationCtrl,
-    FinishCalibrationCtrl,
-    AutoHeadingCtrl,
-    AutoDepthCtrl,
-    AutoAltitudeCtrl,
-    StationKeepingCtrl,
-    WeatherVaningCtrl,
-    AutoPilotSurgeYawCtrl,
-    AutoPilotHeaveCtrl,
-    RunMissionCtrl,
-    PauseMissionCtrl,
-    ClearMissionCtrl,
-    ResetPositionCtrl,
-    ResetOdometerCtrl,
-    CalibrateDvlGyroCtrl,
-    TiltStabilizationCtrl,
-    WaterDensityCtrl,
-    PingerConfigurationCtrl,
-    SystemTimeCtrl,
-    GripperCtrl,
-    GenericServoCtrl,
-    MultibeamServoCtrl,
-    DeactivateGuestPortsCtrl,
-    ActivateGuestPortsCtrl,
-    RestartGuestPortsCtrl,
-    SetAquaTrollParameterUnitCtrl,
-    SetAquaTrollConnectionStatusCtrl,
 )
 from .req_rep import (
     SetOverlayParametersReq,
     SetOverlayParametersRep,
     GetOverlayParametersReq,
     GetOverlayParametersRep,
     SetCameraParametersReq,
@@ -249,69 +153,48 @@
     SyncTimeRep,
     PingReq,
     PingRep,
     SetThicknessGaugeParametersReq,
     SetThicknessGaugeParametersRep,
     ConnectClientReq,
     ConnectClientRep,
-    DisconnectClientReq,
-    DisconnectClientRep,
-    GetBatteryReq,
-    GetBatteryRep,
-    SetMissionReq,
-    SetMissionRep,
-    GetMissionReq,
-    GetMissionRep,
-    SetInstructionUpdateReq,
-    SetInstructionUpdateRep,
-    SetPubFrequencyReq,
-    SetPubFrequencyRep,
-    GetTelemetryReq,
-    GetTelemetryRep,
 )
 
 __all__ = (
     'BinlogRecord',
     'MotionInput',
     'Lights',
-    'Laser',
     'LatLongPosition',
     'ConnectionDuration',
     'AutoHeadingState',
     'AutoDepthState',
     'AutoAltitudeState',
     'StationKeepingState',
     'WeatherVaningState',
-    'AutoPilotSurgeYawState',
-    'AutoPilotHeaveState',
     'ControlMode',
     'TiltStabilizationState',
     'SystemTime',
     'GripperVelocities',
     'ClientInfo',
     'ConnectedClient',
     'RecordState',
-    'TimeLapseState',
     'WaterDensity',
     'PingerConfiguration',
     'WaterTemperature',
     'CPUTemperature',
     'CanisterTemperature',
     'CanisterHumidity',
     'Battery',
     'BatteryBQ40Z50',
     'Attitude',
     'Altitude',
     'ForwardDistance',
     'PositionEstimate',
-    'ResetPositionSettings',
     'Depth',
     'Reference',
-    'Notification',
-    'ControlForce',
     'ControllerHealth',
     'DiveTime',
     'RecordOn',
     'StorageSpace',
     'CalibrationState',
     'IperfStatus',
     'NStreamers',
@@ -322,169 +205,84 @@
     'CameraParameters',
     'OverlayParameters',
     'NavigationSensorStatus',
     'GuestPortDevice',
     'GuestPortDeviceList',
     'GuestPortConnectorInfo',
     'GuestPortInfo',
-    'GuestPortRestartInfo',
     'ThicknessGauge',
     'CpProbe',
-    'GenericServo',
-    'MultibeamServo',
-    'GuestPortCurrent',
-    'Vector3',
-    'Imu',
-    'MedusaSpectrometerData',
-    'IntervalType',
-    'HeadingSource',
-    'ResetCoordinateSource',
-    'NotificationType',
-    'NotificationLevel',
     'Model',
     'PressureSensorType',
     'Resolution',
     'Framerate',
     'Camera',
     'TemperatureUnit',
     'LogoType',
     'DepthUnit',
     'ThicknessUnit',
     'FontSize',
     'GuestPortDeviceID',
-    'GuestPortNumber',
     'NavigationSensorID',
-    'GuestPortDetachStatus',
     'GuestPortError',
-    'Mission',
-    'Instruction',
-    'DepthSetPoint',
-    'Waypoint',
-    'ControlModeCommand',
-    'WaypointCommand',
-    'DepthSetPointCommand',
-    'TiltMainCameraCommand',
-    'TiltMultibeamCommand',
-    'WaitForCommand',
-    'CameraCommand',
-    'GoToSurfaceCommand',
-    'GoToSeabedCommand',
-    'GoToHomeCommand',
-    'PathSegment',
-    'ReferenceAutoPilot',
-    'MissionStatus',
-    'DepthZeroReference',
-    'ControlModeVertical',
-    'ControlModeHorizontal',
-    'CameraAction',
-    'InstructionType',
-    'MissionState',
-    'AquaTrollParameterBlock',
-    'AquaTrollSensorMetadata',
-    'AquaTrollSensorMetadataArray',
-    'AquaTrollProbeMetadata',
-    'AquaTrollSensorParameters',
-    'AquaTrollSensorParametersArray',
-    'SetAquaTrollParameterUnit',
-    'SetAquaTrollConnectionStatus',
-    'Type',
-    'AquaTrollDevice',
-    'AquaTrollQuality',
-    'AquaTrollParameter',
-    'AquaTrollUnit',
-    'AquaTrollSensor',
-    'AquaTrollSensorStatus',
-    'AquaTrollDeviceStatus',
+    'MotionInputCtrl',
+    'TiltVelocityCtrl',
+    'LightsCtrl',
+    'GuestportLightsCtrl',
+    'PilotGPSPositionCtrl',
+    'WatchdogCtrl',
+    'RecordCtrl',
+    'TakePictureCtrl',
+    'StartCalibrationCtrl',
+    'CancelCalibrationCtrl',
+    'FinishCalibrationCtrl',
+    'AutoHeadingCtrl',
+    'AutoDepthCtrl',
+    'AutoAltitudeCtrl',
+    'StationKeepingCtrl',
+    'WeatherVaningCtrl',
+    'ResetPositionCtrl',
+    'ResetOdometerCtrl',
+    'TiltStabilizationCtrl',
+    'WaterDensityCtrl',
+    'PingerConfigurationCtrl',
+    'SystemTimeCtrl',
+    'GripperCtrl',
     'AttitudeTel',
     'AltitudeTel',
     'ForwardDistanceTel',
     'PositionEstimateTel',
     'DepthTel',
     'ReferenceTel',
-    'ReferenceAutoPilotTel',
-    'MissionStatusTel',
-    'NotificationTel',
-    'ControlForceTel',
     'ControllerHealthTel',
     'LightsTel',
     'GuestPortLightsTel',
-    'LaserTel',
     'PilotGPSPositionTel',
     'RecordStateTel',
-    'TimeLapseStateTel',
     'BatteryTel',
     'BatteryBQ40Z50Tel',
     'DiveTimeTel',
     'DroneTimeTel',
     'WaterTemperatureTel',
     'CPUTemperatureTel',
-    'CanisterTopTemperatureTel',
-    'CanisterBottomTemperatureTel',
-    'CanisterTopHumidityTel',
-    'CanisterBottomHumidityTel',
+    'CanisterTemperatureTel',
+    'CanisterHumidityTel',
     'VideoStorageSpaceTel',
     'DataStorageSpaceTel',
     'CalibrationStateTel',
     'TiltStabilizationTel',
     'IperfTel',
     'NStreamersTel',
     'TiltAngleTel',
     'DroneInfoTel',
     'ErrorFlagsTel',
     'ControlModeTel',
     'ThicknessGaugeTel',
     'CpProbeTel',
-    'AquaTrollProbeMetadataTel',
-    'AquaTrollSensorMetadataTel',
-    'AquaTrollSensorParametersTel',
     'ConnectedClientsTel',
-    'GenericServoTel',
-    'MultibeamServoTel',
-    'GuestPortCurrentTel',
-    'CalibratedImuTel',
-    'Imu1Tel',
-    'Imu2Tel',
-    'MedusaSpectrometerDataTel',
-    'MotionInputCtrl',
-    'TiltVelocityCtrl',
-    'LightsCtrl',
-    'GuestportLightsCtrl',
-    'LaserCtrl',
-    'PilotGPSPositionCtrl',
-    'WatchdogCtrl',
-    'RecordCtrl',
-    'TakePictureCtrl',
-    'StartCalibrationCtrl',
-    'CancelCalibrationCtrl',
-    'FinishCalibrationCtrl',
-    'AutoHeadingCtrl',
-    'AutoDepthCtrl',
-    'AutoAltitudeCtrl',
-    'StationKeepingCtrl',
-    'WeatherVaningCtrl',
-    'AutoPilotSurgeYawCtrl',
-    'AutoPilotHeaveCtrl',
-    'RunMissionCtrl',
-    'PauseMissionCtrl',
-    'ClearMissionCtrl',
-    'ResetPositionCtrl',
-    'ResetOdometerCtrl',
-    'CalibrateDvlGyroCtrl',
-    'TiltStabilizationCtrl',
-    'WaterDensityCtrl',
-    'PingerConfigurationCtrl',
-    'SystemTimeCtrl',
-    'GripperCtrl',
-    'GenericServoCtrl',
-    'MultibeamServoCtrl',
-    'DeactivateGuestPortsCtrl',
-    'ActivateGuestPortsCtrl',
-    'RestartGuestPortsCtrl',
-    'SetAquaTrollParameterUnitCtrl',
-    'SetAquaTrollConnectionStatusCtrl',
     'SetOverlayParametersReq',
     'SetOverlayParametersRep',
     'GetOverlayParametersReq',
     'GetOverlayParametersRep',
     'SetCameraParametersReq',
     'SetCameraParametersRep',
     'GetCameraParametersReq',
@@ -493,22 +291,8 @@
     'SyncTimeRep',
     'PingReq',
     'PingRep',
     'SetThicknessGaugeParametersReq',
     'SetThicknessGaugeParametersRep',
     'ConnectClientReq',
     'ConnectClientRep',
-    'DisconnectClientReq',
-    'DisconnectClientRep',
-    'GetBatteryReq',
-    'GetBatteryRep',
-    'SetMissionReq',
-    'SetMissionRep',
-    'GetMissionReq',
-    'GetMissionRep',
-    'SetInstructionUpdateReq',
-    'SetInstructionUpdateRep',
-    'SetPubFrequencyReq',
-    'SetPubFrequencyRep',
-    'GetTelemetryReq',
-    'GetTelemetryRep',
 )
```
