# Comparing `tmp/bell_avr_libraries-0.2.0a2.tar.gz` & `tmp/bell_avr_libraries-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bell_avr_libraries-0.2.0a2.tar", max compression
+gzip compressed data, was "bell_avr_libraries-0.2.0a3.tar", max compression
```

## Comparing `bell_avr_libraries-0.2.0a2.tar` & `bell_avr_libraries-0.2.0a3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/LICENSE
--rw-r--r--   0        0        0     1938 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/README.md
--rw-r--r--   0        0        0      444 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/__init__.py
--rw-r--r--   0        0        0      289 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/__init__.py
--rw-r--r--   0        0        0     8330 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/client.py
--rw-r--r--   0        0        0    23046 2023-05-06 14:31:47.295250 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/constants.py
--rw-r--r--   0        0        0      588 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/dispatcher.py
--rw-r--r--   0        0        0    15050 2023-05-06 14:31:47.287250 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/module.py
--rw-r--r--   0        0        0    28762 2023-05-06 14:31:47.275250 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/payloads.py
--rw-r--r--   0        0        0    12127 2023-05-06 14:31:47.303250 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/qt_widget.py
--rw-r--r--   0        0        0     2534 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/serializer.py
--rw-r--r--   0        0        0      124 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/serial/__init__.py
--rw-r--r--   0        0        0      746 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/serial/client.py
--rw-r--r--   0        0        0    10089 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/serial/pcc.py
--rw-r--r--   0        0        0      935 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/serial/ports.py
--rw-r--r--   0        0        0      206 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/__init__.py
--rw-r--r--   0        0        0     3076 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/decorators.py
--rw-r--r--   0        0        0     1070 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/env.py
--rw-r--r--   0        0        0     2890 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/images.py
--rw-r--r--   0        0        0      726 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/testing.py
--rw-r--r--   0        0        0     1494 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/timing.py
--rw-r--r--   0        0        0     1805 2023-05-06 14:31:27.047232 bell_avr_libraries-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0     3058 1970-01-01 00:00:00.000000 bell_avr_libraries-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/LICENSE
+-rw-r--r--   0        0        0     1885 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/README.md
+-rw-r--r--   0        0        0      444 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/__init__.py
+-rw-r--r--   0        0        0      289 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/__init__.py
+-rw-r--r--   0        0        0     8306 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/client.py
+-rw-r--r--   0        0        0    23046 2023-06-03 17:54:14.739136 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/constants.py
+-rw-r--r--   0        0        0      588 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/dispatcher.py
+-rw-r--r--   0        0        0    15050 2023-06-03 17:54:14.731136 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/module.py
+-rw-r--r--   0        0        0    28762 2023-06-03 17:54:14.727136 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/payloads.py
+-rw-r--r--   0        0        0    12195 2023-06-03 17:54:14.743136 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/qt_widget.py
+-rw-r--r--   0        0        0     2534 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/serializer.py
+-rw-r--r--   0        0        0      124 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/serial/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/serial/client.py
+-rw-r--r--   0        0        0    10661 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/serial/pcc.py
+-rw-r--r--   0        0        0      935 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/serial/ports.py
+-rw-r--r--   0        0        0      206 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/utils/__init__.py
+-rw-r--r--   0        0        0     3076 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/utils/decorators.py
+-rw-r--r--   0        0        0     1070 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/utils/env.py
+-rw-r--r--   0        0        0     3357 2023-06-03 17:53:54.034154 bell_avr_libraries-0.2.0a3/bell/avr/utils/images.py
+-rw-r--r--   0        0        0      726 2023-06-03 17:53:54.034154 bell_avr_libraries-0.2.0a3/bell/avr/utils/testing.py
+-rw-r--r--   0        0        0     1494 2023-06-03 17:53:54.034154 bell_avr_libraries-0.2.0a3/bell/avr/utils/timing.py
+-rw-r--r--   0        0        0     1805 2023-06-03 17:53:54.034154 bell_avr_libraries-0.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 bell_avr_libraries-0.2.0a3/PKG-INFO
```

### Comparing `bell_avr_libraries-0.2.0a2/LICENSE` & `bell_avr_libraries-0.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/README.md` & `bell_avr_libraries-0.2.0a3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -23,47 +23,48 @@
 
 ## Development
 
 It's assumed you have a version of Python installed from
 [python.org](https://python.org) that is the same or newer as
 defined in the [`.python-version`](.python-version) file.
 
-First, install [Poetry](https://python-poetry.org/):
+First, install [Poetry](https://python-poetry.org/) and
+[VS Code Task Runner](https://pypi.org/project/vscode-task-runner/):
 
 ```bash
 python -m pip install pipx --upgrade
 pipx ensurepath
 pipx install poetry
+pipx install vscode-task-runner
 # (Optionally) Add pre-commit plugin
 poetry self add poetry-pre-commit-plugin
 ```
 
 Now, you can clone the repo and install dependencies:
 
 ```bash
 git clone https://github.com/bellflight/AVR-Python-Libraries
 cd AVR-Python-Libraries
-poetry install --sync --all-extras
-poetry run pre-commit install --install-hooks
+vtr install
 ```
 
 Run
 
 ```bash
 poetry shell
 ```
 
 to activate the virtual environment.
 
-Build the auto-generated code with `poetry run python build.py`. From here,
-you can now produce a package with `poetry build`.
+You can now produce a package with `vtr build`, which will automatically
+also run `vtr build-code`.
 
 To add new message definitions, add entries to the `bell/avr/mqtt/asyncapi.yml` file.
 This is an [AsyncAPI](https://www.asyncapi.com/) definition,
 which is primarily [JSONSchema](https://json-schema.org/) with some association
 of classes and topics.
 
 The generator that turns this definition file into Python code is the homebrew
 [build.py](build.py), so double-check that the output makes sense.
 
-To generate the documentation, run the `build.py` script with the `--docs` option.
-This requires that Node.js is installed, and `npm` install has been run.
+To generate the documentation, `vtr build-code-docs`.
+This requires that Node.js is installed.
```

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/client.py` & `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from loguru import logger
 
 from bell.avr.mqtt.constants import _MQTTTopicCallableTypedDict
 from bell.avr.utils.env import get_env_int
 
 
 class MQTTClient:
-    def __init__(self):
-        """
-        This class is *not meant to be used directly*! This meant to serve as the
-        foundation for MQTT interactions. Please use the
-        `bell.avr.mqtt.module.MQTTModule`
-        or `bell.avr.mqtt.qt_widget.MQTTWidget` classes instead.
-        """
+    """
+    This class is *not meant to be used directly*! This meant to serve as the
+    foundation for MQTT interactions. Please use the
+    `bell.avr.mqtt.module.MQTTModule`
+    or `bell.avr.mqtt.qt_widget.MQTTWidget` classes instead.
+    """
 
+    def __init__(self):
         # create the MQTT client
         # Currently using MQTT v3.1.1
         # No reason we can't use v5, just type hinting needs to change
         # for some `on_` functions.
         self._mqtt_client = paho_mqtt.Client(
             client_id=f"{self.__class__.__name__}_{uuid.uuid4()}",
             protocol=paho_mqtt.MQTTv311,
```

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/constants.py` & `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/constants.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/dispatcher.py` & `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/module.py` & `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/module.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/payloads.py` & `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/payloads.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -802,328 +802,328 @@
 
 class AVRAutonomousBuildingDisable(BaseModel):
     building: int = Field(..., ge=0, le=15)
     """
     Building ID. This is 0-indexed.
     """
 
-class _AVRPCMColorSetCallable(Protocol):
+class _AVRFusionCourseCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMColorSet) -> Any:
+    def __call__(self, payload: AVRFusionCourse) -> Any:
         ...
 
-class _AVRFCMPositionLocalCallable(Protocol):
+class _AVRVIOAttitudeQuaternionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionLocal) -> Any:
+    def __call__(self, payload: AVRVIOAttitudeQuaternion) -> Any:
         ...
 
-class _AVRFCMLandedCallable(Protocol):
+class _AVRAutonomousBuildingEnableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMLanded) -> Any:
+    def __call__(self, payload: AVRAutonomousBuildingEnable) -> Any:
         ...
 
-class _AVRPCMServoPercentCallable(Protocol):
+class _AVRFCMHILGPSStatsCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoPercent) -> Any:
+    def __call__(self, payload: AVRFCMHILGPSStats) -> Any:
         ...
 
-class _AVRFusionGroundspeedCallable(Protocol):
+class _AVRPCMServoCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionGroundspeed) -> Any:
+    def __call__(self, payload: AVRPCMServo) -> Any:
         ...
 
-class _AVRFCMFlightModeCallable(Protocol):
+class _AVRFCMBatteryCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMFlightMode) -> Any:
+    def __call__(self, payload: AVRFCMBattery) -> Any:
         ...
 
-class _AVRFusionPositionLocalCallable(Protocol):
+class _AVRAutonomousBuildingDisableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionPositionLocal) -> Any:
+    def __call__(self, payload: AVRAutonomousBuildingDisable) -> Any:
         ...
 
-class _AVRFusionHeadingCallable(Protocol):
+class _AVRAprilTagsVisibleCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionHeading) -> Any:
+    def __call__(self, payload: AVRAprilTagsVisible) -> Any:
         ...
 
-class _AVRFCMPositionHomeCallable(Protocol):
+class _AVRFusionVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionHome) -> Any:
+    def __call__(self, payload: AVRFusionVelocity) -> Any:
         ...
 
-class _AVRFCMGPSInfoCallable(Protocol):
+class _AVRFusionGroundspeedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMGPSInfo) -> Any:
+    def __call__(self, payload: AVRFusionGroundspeed) -> Any:
         ...
 
-class _AVRFCMAttitudeEulerDegreesCallable(Protocol):
+class _AVRVIOAttitudeEulerRadiansCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMAttitudeEulerDegrees) -> Any:
+    def __call__(self, payload: AVRVIOAttitudeEulerRadians) -> Any:
         ...
 
-class _AVRFusionClimbRateCallable(Protocol):
+class _AVRFusionAttitudeQuaternionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionClimbRate) -> Any:
+    def __call__(self, payload: AVRFusionAttitudeQuaternion) -> Any:
         ...
 
-class _AVRFCMHILGPSStatsCallable(Protocol):
+class _AVRFusionAttitudeEulerRadiansCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMHILGPSStats) -> Any:
+    def __call__(self, payload: AVRFusionAttitudeEulerRadians) -> Any:
         ...
 
-class _AVRAprilTagsRawCallable(Protocol):
+class _AVRAprilTagsStatusCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsRaw) -> Any:
+    def __call__(self, payload: AVRAprilTagsStatus) -> Any:
         ...
 
-class _AVRAprilTagsVisibleCallable(Protocol):
+class _AVRAprilTagsVehiclePositionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsVisible) -> Any:
+    def __call__(self, payload: AVRAprilTagsVehiclePosition) -> Any:
         ...
 
-class _AVRVIOHeadingCallable(Protocol):
+class _AVRVIOImageRequestCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOHeading) -> Any:
+    def __call__(self, payload: AVRVIOImageRequest) -> Any:
         ...
 
-class _AVRVIOAttitudeEulerRadiansCallable(Protocol):
+class _AVRFusionHILGPSMessageCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOAttitudeEulerRadians) -> Any:
+    def __call__(self, payload: AVRFusionHILGPSMessage) -> Any:
         ...
 
-class _AVRFusionVelocityCallable(Protocol):
+class _AVRVIOHeadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionVelocity) -> Any:
+    def __call__(self, payload: AVRVIOHeading) -> Any:
         ...
 
-class _AVRVIOAttitudeQuaternionCallable(Protocol):
+class _AVRPCMServoPercentCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOAttitudeQuaternion) -> Any:
+    def __call__(self, payload: AVRPCMServoPercent) -> Any:
         ...
 
-class _AVRAutonomousBuildingEnableCallable(Protocol):
+class _AVRPCMServoPWMCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAutonomousBuildingEnable) -> Any:
+    def __call__(self, payload: AVRPCMServoPWM) -> Any:
         ...
 
-class _AVRVIOResyncCallable(Protocol):
+class _AVRFCMFlightModeCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOResync) -> Any:
+    def __call__(self, payload: AVRFCMFlightMode) -> Any:
         ...
 
-class _AVRVIOImageStreamEnableCallable(Protocol):
+class _AVRFusionPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageStreamEnable) -> Any:
+    def __call__(self, payload: AVRFusionPositionLocal) -> Any:
         ...
 
-class _AVRFCMVelocityCallable(Protocol):
+class _AVRFCMPositionHomeCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMVelocity) -> Any:
+    def __call__(self, payload: AVRFCMPositionHome) -> Any:
         ...
 
-class _AVRFCMPositionGlobalCallable(Protocol):
+class _AVRFCMVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionGlobal) -> Any:
+    def __call__(self, payload: AVRFCMVelocity) -> Any:
         ...
 
-class _AVRVIOImageRequestCallable(Protocol):
+class _AVRFusionHeadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageRequest) -> Any:
+    def __call__(self, payload: AVRFusionHeading) -> Any:
         ...
 
-class _AVRFCMArmedCallable(Protocol):
+class _AVRVIOImageCaptureCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMArmed) -> Any:
+    def __call__(self, payload: AVRVIOImageCapture) -> Any:
         ...
 
-class _AVRAprilTagsStatusCallable(Protocol):
+class _AVRFCMGPSInfoCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsStatus) -> Any:
+    def __call__(self, payload: AVRFCMGPSInfo) -> Any:
         ...
 
-class _AVRPCMColorTimedCallable(Protocol):
+class _AVRFCMPositionGlobalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMColorTimed) -> Any:
+    def __call__(self, payload: AVRFCMPositionGlobal) -> Any:
         ...
 
-class _AVRFusionHILGPSMessageCallable(Protocol):
+class _AVRFCMLandedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionHILGPSMessage) -> Any:
+    def __call__(self, payload: AVRFCMLanded) -> Any:
         ...
 
-class _AVRAutonomousBuildingDisableCallable(Protocol):
+class _AVRVIOConfidenceCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAutonomousBuildingDisable) -> Any:
+    def __call__(self, payload: AVRVIOConfidence) -> Any:
         ...
 
-class _AVRFusionCourseCallable(Protocol):
+class _AVRFCMArmedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionCourse) -> Any:
+    def __call__(self, payload: AVRFCMArmed) -> Any:
         ...
 
-class _AVRFusionAttitudeQuaternionCallable(Protocol):
+class _AVRThermalReadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionAttitudeQuaternion) -> Any:
+    def __call__(self, payload: AVRThermalReading) -> Any:
         ...
 
-class _AVRVIOConfidenceCallable(Protocol):
+class _AVRAprilTagsRawCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOConfidence) -> Any:
+    def __call__(self, payload: AVRAprilTagsRaw) -> Any:
         ...
 
-class _AVRPCMServoAbsoluteCallable(Protocol):
+class _AVRPCMColorTimedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoAbsolute) -> Any:
+    def __call__(self, payload: AVRPCMColorTimed) -> Any:
         ...
 
-class _AVRAprilTagsVehiclePositionCallable(Protocol):
+class _AVRFusionPositionGlobalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsVehiclePosition) -> Any:
+    def __call__(self, payload: AVRFusionPositionGlobal) -> Any:
         ...
 
-class _AVRVIOImageCaptureCallable(Protocol):
+class _AVRVIOVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageCapture) -> Any:
+    def __call__(self, payload: AVRVIOVelocity) -> Any:
         ...
 
-class _AVRFusionPositionGlobalCallable(Protocol):
+class _AVRVIOImageStreamEnableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionPositionGlobal) -> Any:
+    def __call__(self, payload: AVRVIOImageStreamEnable) -> Any:
         ...
 
-class _AVRVIOPositionLocalCallable(Protocol):
+class _AVREmptyMessageCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOPositionLocal) -> Any:
+    def __call__(self) -> Any:
         ...
 
-class _AVRThermalReadingCallable(Protocol):
+class _AVRVIOResyncCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRThermalReading) -> Any:
+    def __call__(self, payload: AVRVIOResync) -> Any:
         ...
 
-class _AVRFCMAirborneCallable(Protocol):
+class _AVRPCMColorSetCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMAirborne) -> Any:
+    def __call__(self, payload: AVRPCMColorSet) -> Any:
         ...
 
-class _AVRFCMBatteryCallable(Protocol):
+class _AVRPCMServoAbsoluteCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMBattery) -> Any:
+    def __call__(self, payload: AVRPCMServoAbsolute) -> Any:
         ...
 
-class _AVRPCMServoCallable(Protocol):
+class _AVRFCMAttitudeEulerDegreesCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServo) -> Any:
+    def __call__(self, payload: AVRFCMAttitudeEulerDegrees) -> Any:
         ...
 
-class _AVRVIOVelocityCallable(Protocol):
+class _AVRVIOPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOVelocity) -> Any:
+    def __call__(self, payload: AVRVIOPositionLocal) -> Any:
         ...
 
-class _AVREmptyMessageCallable(Protocol):
+class _AVRFCMPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self) -> Any:
+    def __call__(self, payload: AVRFCMPositionLocal) -> Any:
         ...
 
-class _AVRPCMServoPWMCallable(Protocol):
+class _AVRFusionClimbRateCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoPWM) -> Any:
+    def __call__(self, payload: AVRFusionClimbRate) -> Any:
         ...
 
-class _AVRFusionAttitudeEulerRadiansCallable(Protocol):
+class _AVRFCMAirborneCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionAttitudeEulerRadians) -> Any:
+    def __call__(self, payload: AVRFCMAirborne) -> Any:
         ...
```

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/qt_widget.py` & `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/qt_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,18 @@
 
 
 class MQTTWidget(QtWidgets.QWidget):
     send_message_signal: QtCore.SignalInstance = QtCore.Signal(str, bytes)  # type: ignore
     """
     This should not be used directly, but rather through `send_message` instead.
 
-    The `send_message_signal` expects a topic, and the str/bytes of the MQTT payload.
-    This should already be serialized with `bell.avr.mqtt.serializer.serialize_payload`
-    and ready for transmission over the network.
+    This is a `QtCore.Signal` that expects a topic, and the str/bytes of the
+    MQTT payload. This should already be serialized with
+    `bell.avr.mqtt.serializer.serialize_payload` and ready for transmission over the
+    network.
     """
 
     def __init__(self, *args, **kwargs):
         """
         This class is desgined for Qt applications where a widget needs to receive and
         send MQTT messages. After the widget is initialized, the signals need to be
         connected.
@@ -96,14 +97,15 @@
 
         # connect the `send_message_signal` signal to the mqtt client to send messages
         thermal_view_control_widget.send_message_signal.connect(
             main_connection_widget.mqtt_connection_widget.mqtt_client._publish
         )
         ```
         """
+        # this docstring is here because of pdoc weirdness
 
         self.topic_callbacks: _MQTTTopicCallableTypedDict = {}
         """
         See `bell.avr.mqtt.client.MQTTClient.topic_callbacks`.
         """
 
         super().__init__(*args, **kwargs)
```

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/serializer.py` & `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/serializer.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/serial/client.py` & `bell_avr_libraries-0.2.0a3/bell/avr/serial/client.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/serial/pcc.py` & `bell_avr_libraries-0.2.0a3/bell/avr/serial/pcc.py`

 * *Files 8% similar despite different names*

```diff
@@ -143,16 +143,19 @@
         data = self._construct_payload(command, length, data)
 
         logger.debug(f"Setting servo open/close: {data}")
         self.ser.write(data)
 
     def set_servo_min(self, servo: int, minimum: float) -> None:
         """
-        Sets the minimum pulse width of a servo. Expects the 0-indexed servo ID and
-        the minimum pulse width between 0 and 1000 non-inclusive.
+        Sets the minimum pulse length of a servo. Expects the 0-indexed servo ID and
+        the minimum pulse length between 0 and 1000 non-inclusive.
+
+        As of writing, the PCC firmware limits this to 150.
+        https://github.com/bellflight/AVR-PCC-Firmware/blob/main/libraries/AVR_ServoDriver/avr_servo.hpp
         """
 
         valid_command = False
 
         command = self.commands.index("SET_SERVO_MIN")
         data = []
 
@@ -167,16 +170,19 @@
         data = self._construct_payload(command, length, data)
 
         logger.debug(f"Setting servo min: {data}")
         self.ser.write(data)
 
     def set_servo_max(self, servo: int, maximum: float) -> None:
         """
-        Sets the maximum pulse width of a servo. Expects the 0-indexed servo ID and
-        the maximum pulse width between 0 and 1000 non-inclusive.
+        Sets the maximum pulse length of a servo. Expects the 0-indexed servo ID and
+        the maximum pulse length between 0 and 1000 non-inclusive.
+
+        As of writing, the PCC firmware limits this to 425.
+        https://github.com/bellflight/AVR-PCC-Firmware/blob/main/libraries/AVR_ServoDriver/avr_servo.hpp
         """
 
         valid_command = False
 
         command = self.commands.index("SET_SERVO_MAX")
         data = []
 
@@ -216,15 +222,18 @@
 
         logger.debug(f"Setting servo percent: {data}")
         self.ser.write(data)
 
     def set_servo_abs(self, servo: int, absolute: int) -> None:
         """
         Sets the absolute position of a servo. Expects the 0-indexed servo ID and
-        the absolute position.
+        the absolute position, which is really the microsecond length of the pulse.
+
+        As of writing, the PCC firmware limits this to between 600 and 2400.
+        https://github.com/bellflight/AVR-PCC-Firmware/blob/main/libraries/AVR_ServoDriver/avr_servo.hpp
         """
 
         valid_command = False
 
         command = self.commands.index("SET_SERVO_ABS")
         data = []
```

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/serial/ports.py` & `bell_avr_libraries-0.2.0a3/bell/avr/serial/ports.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/utils/decorators.py` & `bell_avr_libraries-0.2.0a3/bell/avr/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/utils/env.py` & `bell_avr_libraries-0.2.0a3/bell/avr/utils/env.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/utils/images.py` & `bell_avr_libraries-0.2.0a3/bell/avr/utils/images.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
 import zlib
-from typing import List, TypedDict
+from typing import List, Protocol, TypedDict, Union
 
 import numpy as np
 
 
 class ImageData(TypedDict):
     """
     Data structure to hold image data and metadata.
@@ -38,14 +38,20 @@
     """
     compressed: bool
     """
     Whether or not the image data is compressed.
     """
 
 
+class _ImageDataProtocol(Protocol):
+    data: str
+    shape: List[int]
+    compressed: bool
+
+
 def serialize_image(image: np.ndarray, compress: bool = False) -> ImageData:
     """
     Takes a numpy array of image data, and transforms it into format that can
     be sent over JSON. Expects a 2D or 3D numpy array. If the array does
     not contain integers, all of the values will be rounded to the nearest
     integer. Setting `compress` to `True` enables
     [zlib](https://docs.python.org/3/library/zlib.html) compression.
@@ -69,24 +75,35 @@
 
     # build class
     image_data = ImageData(data=base64_image_data, shape=shape, compressed=compress)
 
     return image_data
 
 
-def deserialize_image(image_data: ImageData) -> np.ndarray:
+def deserialize_image(image_data: Union[ImageData, _ImageDataProtocol]) -> np.ndarray:
     """
     Given an `ImageData` object, will reconstruct the original numpy array.
+    Additionally, an object that has `.data`, `.compressed` and `.shape`
+    attributes is allowed.
     """
+    if isinstance(image_data, dict):
+        data = image_data["data"]
+        compressed = image_data["compressed"]
+        shape = image_data["shape"]
+    else:
+        data = image_data.data
+        compressed = image_data.compressed
+        shape = image_data.shape
+
     # convert the string to bytes, and then undo the base64
-    image_bytes = base64.b64decode(image_data["data"].encode("utf-8"))
+    image_bytes = base64.b64decode(data.encode("utf-8"))
 
     # decompress with zlib
-    if image_data["compressed"]:
+    if compressed:
         image_bytes = zlib.decompress(image_bytes)
 
     # convert bytes to a byte array
     image_byte_array = bytearray(image_bytes)
     # convert the byte array back into a numpy array
     image_array = np.array(image_byte_array)
 
-    return np.reshape(image_array, image_data["shape"])
+    return np.reshape(image_array, shape)
```

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/utils/testing.py` & `bell_avr_libraries-0.2.0a3/bell/avr/utils/testing.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/bell/avr/utils/timing.py` & `bell_avr_libraries-0.2.0a3/bell/avr/utils/timing.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a2/pyproject.toml` & `bell_avr_libraries-0.2.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "bell-avr-libraries"
-    version = "0.2.0a2"
+    version = "0.2.0a3"
     description = "Common Python libraries used by parts of Bell AVR"
     license = "MIT"
     readme = "README.md"
     homepage = "https://roboticseducation.org/bell-advanced-vertical-robotics/"
     repository = "https://github.com/bellflight/AVR-Python-Libraries"
     documentation = "https://bellflight.github.io/AVR-Python-Libraries"
     authors = [
```

### Comparing `bell_avr_libraries-0.2.0a2/PKG-INFO` & `bell_avr_libraries-0.2.0a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bell-avr-libraries
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: Common Python libraries used by parts of Bell AVR
 Home-page: https://roboticseducation.org/bell-advanced-vertical-robotics/
 License: MIT
 Author: Chris Padilla
 Author-email: cpadilla@bellflight.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -50,48 +50,49 @@
 
 ## Development
 
 It's assumed you have a version of Python installed from
 [python.org](https://python.org) that is the same or newer as
 defined in the [`.python-version`](.python-version) file.
 
-First, install [Poetry](https://python-poetry.org/):
+First, install [Poetry](https://python-poetry.org/) and
+[VS Code Task Runner](https://pypi.org/project/vscode-task-runner/):
 
 ```bash
 python -m pip install pipx --upgrade
 pipx ensurepath
 pipx install poetry
+pipx install vscode-task-runner
 # (Optionally) Add pre-commit plugin
 poetry self add poetry-pre-commit-plugin
 ```
 
 Now, you can clone the repo and install dependencies:
 
 ```bash
 git clone https://github.com/bellflight/AVR-Python-Libraries
 cd AVR-Python-Libraries
-poetry install --sync --all-extras
-poetry run pre-commit install --install-hooks
+vtr install
 ```
 
 Run
 
 ```bash
 poetry shell
 ```
 
 to activate the virtual environment.
 
-Build the auto-generated code with `poetry run python build.py`. From here,
-you can now produce a package with `poetry build`.
+You can now produce a package with `vtr build`, which will automatically
+also run `vtr build-code`.
 
 To add new message definitions, add entries to the `bell/avr/mqtt/asyncapi.yml` file.
 This is an [AsyncAPI](https://www.asyncapi.com/) definition,
 which is primarily [JSONSchema](https://json-schema.org/) with some association
 of classes and topics.
 
 The generator that turns this definition file into Python code is the homebrew
 [build.py](build.py), so double-check that the output makes sense.
 
-To generate the documentation, run the `build.py` script with the `--docs` option.
-This requires that Node.js is installed, and `npm` install has been run.
+To generate the documentation, `vtr build-code-docs`.
+This requires that Node.js is installed.
```

