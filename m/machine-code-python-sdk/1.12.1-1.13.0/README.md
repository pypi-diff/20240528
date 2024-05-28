# Comparing `tmp/machine-code-python-sdk-1.12.1.tar.gz` & `tmp/machine_code_python_sdk-1.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machine-code-python-sdk-1.12.1.tar", last modified: Wed Feb 28 22:12:21 2024, max compression
+gzip compressed data, was "machine_code_python_sdk-1.13.0.tar", last modified: Tue May 28 18:52:58 2024, max compression
```

## Comparing `machine-code-python-sdk-1.12.1.tar` & `machine_code_python_sdk-1.13.0.tar`

### file list

```diff
@@ -1,91 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.404887 machine-code-python-sdk-1.12.1/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-02-28 22:12:21.404887 machine-code-python-sdk-1.12.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.404887 machine-code-python-sdk-1.12.1/machine_code_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-02-28 22:12:21.000000 machine-code-python-sdk-1.12.1/machine_code_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-28 22:12:21.000000 machine-code-python-sdk-1.12.1/machine_code_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 22:12:21.000000 machine-code-python-sdk-1.12.1/machine_code_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-28 22:12:21.000000 machine-code-python-sdk-1.12.1/machine_code_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-28 22:12:21.000000 machine-code-python-sdk-1.12.1/machine_code_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.396887 machine-code-python-sdk-1.12.1/machinelogic/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.396887 machine-code-python-sdk-1.12.1/machinelogic/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/decorators/future_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.396887 machine-code-python-sdk-1.12.1/machinelogic/decorators/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/decorators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/decorators/tests/test_future_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/decorators/tests/test_undocumented.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/decorators/undocumented.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.396887 machine-code-python-sdk-1.12.1/machinelogic/ivention/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/iac_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/iactuator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/iactuator_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/ibag_gripper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/icamera.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/idigital_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/idigital_io_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/idigital_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/iestop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/imachine.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/imachine_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/ipneumatic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/irobot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/machine_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/mqtt_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.400887 machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_idigital_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_idigital_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_imachine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_mqtt_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.400887 machine-code-python-sdk-1.12.1/machinelogic/ivention/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/types/ac_motor_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/types/actuator_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/types/bag_gripper_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/types/input_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/types/output_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/types/pneumatic_details.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.400887 machine-code-python-sdk-1.12.1/machinelogic/ivention/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/ivention/util/inheritance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.400887 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/ac_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/actuator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/actuator_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    48469 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/bag_gripper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/digital_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/digital_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/estop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/machine_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/pneumatic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.400887 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/robot/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/robot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/robot/robot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39429 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/robot/vention_ros_client_library.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.404887 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_ac_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_actuator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_bag_gripper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_pneumatic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:12:21.404887 machine-code-python-sdk-1.12.1/machinelogic/state_machine/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/state_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/state_machine/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/state_machine/state_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/machinelogic/state_machine/state_transition.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 22:12:21.404887 machine-code-python-sdk-1.12.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-28 22:11:59.000000 machine-code-python-sdk-1.12.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.920138 machine_code_python_sdk-1.13.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-28 18:52:58.920138 machine_code_python_sdk-1.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.920138 machine_code_python_sdk-1.13.0/machine_code_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-28 18:52:58.000000 machine_code_python_sdk-1.13.0/machine_code_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-28 18:52:58.000000 machine_code_python_sdk-1.13.0/machine_code_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:52:58.000000 machine_code_python_sdk-1.13.0/machine_code_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 18:52:58.000000 machine_code_python_sdk-1.13.0/machine_code_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 18:52:58.000000 machine_code_python_sdk-1.13.0/machine_code_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.908138 machine_code_python_sdk-1.13.0/machinelogic/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.908138 machine_code_python_sdk-1.13.0/machinelogic/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/decorators/future_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.908138 machine_code_python_sdk-1.13.0/machinelogic/decorators/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/decorators/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/decorators/tests/test_future_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/decorators/tests/test_undocumented.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/decorators/undocumented.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.912138 machine_code_python_sdk-1.13.0/machinelogic/ivention/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/iac_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/iactuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/iactuator_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/ibag_gripper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/icamera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/idigital_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/idigital_io_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/idigital_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/iestop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/imachine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/imachine_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/ipath_follower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/ipneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/irobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/machine_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/mqtt_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.912138 machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_idigital_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_idigital_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_imachine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_ipath_follower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_mqtt_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.916138 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/ac_motor_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/actuator_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/bag_gripper_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/input_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/output_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/path_follower_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/path_follower_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/types/pneumatic_details.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.916138 machine_code_python_sdk-1.13.0/machinelogic/ivention/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/ivention/util/inheritance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.916138 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/ac_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/actuator_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53346 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/bag_gripper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/digital_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/digital_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/estop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/machine_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/path_follower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/pneumatic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.920138 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/robot/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/robot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/robot/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39794 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/robot/vention_ros_client_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.920138 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_ac_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_actuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_bag_gripper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_path_follower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_pneumatic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:52:58.920138 machine_code_python_sdk-1.13.0/machinelogic/state_machine/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/state_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/state_machine/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/state_machine/state_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/machinelogic/state_machine/state_transition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:52:58.920138 machine_code_python_sdk-1.13.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-28 18:52:49.000000 machine_code_python_sdk-1.13.0/setup.py
```

### Comparing `machine-code-python-sdk-1.12.1/PKG-INFO` & `machine_code_python_sdk-1.13.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: machine-code-python-sdk
-Version: 1.12.1
+Version: 1.13.0
 Summary: MachineCode SDK for Vention hardware
 Home-page: https://vention.io/resources/guides/machinelogic-python-programming-514
 Author: VentionCo
 Author-email: vention-sw-ci@vention.cc
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: miros==4.2.1
 Requires-Dist: paho-mqtt==1.5.1
 Requires-Dist: types-requests==2.28.11
-Requires-Dist: requests==2.28.2
+Requires-Dist: requests==2.31.0
 Requires-Dist: typing_extensions==4.6.3
 Requires-Dist: parameterized
 Requires-Dist: numpy==1.24.2
 Requires-Dist: roslibpy==1.4.2
-Requires-Dist: scipy==1.9.3
+Requires-Dist: scipy==1.11.1
 Requires-Dist: zope.interface==5.5.2
 
 # machine-code-python-sdk
 
 Provides a programmatic interface in Python to talk to Vention hardware, as well as a generic state machine for coordinating your programs.
 
 ## Table of Contents
```

### Comparing `machine-code-python-sdk-1.12.1/README.md` & `machine_code_python_sdk-1.13.0/README.md`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machine_code_python_sdk.egg-info/PKG-INFO` & `machine_code_python_sdk-1.13.0/machine_code_python_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: machine-code-python-sdk
-Version: 1.12.1
+Version: 1.13.0
 Summary: MachineCode SDK for Vention hardware
 Home-page: https://vention.io/resources/guides/machinelogic-python-programming-514
 Author: VentionCo
 Author-email: vention-sw-ci@vention.cc
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: miros==4.2.1
 Requires-Dist: paho-mqtt==1.5.1
 Requires-Dist: types-requests==2.28.11
-Requires-Dist: requests==2.28.2
+Requires-Dist: requests==2.31.0
 Requires-Dist: typing_extensions==4.6.3
 Requires-Dist: parameterized
 Requires-Dist: numpy==1.24.2
 Requires-Dist: roslibpy==1.4.2
-Requires-Dist: scipy==1.9.3
+Requires-Dist: scipy==1.11.1
 Requires-Dist: zope.interface==5.5.2
 
 # machine-code-python-sdk
 
 Provides a programmatic interface in Python to talk to Vention hardware, as well as a generic state machine for coordinating your programs.
 
 ## Table of Contents
```

### Comparing `machine-code-python-sdk-1.12.1/machine_code_python_sdk.egg-info/SOURCES.txt` & `machine_code_python_sdk-1.13.0/machine_code_python_sdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,30 +25,34 @@
 machinelogic/ivention/icamera.py
 machinelogic/ivention/idigital_input.py
 machinelogic/ivention/idigital_io_shared.py
 machinelogic/ivention/idigital_output.py
 machinelogic/ivention/iestop.py
 machinelogic/ivention/imachine.py
 machinelogic/ivention/imachine_motion.py
+machinelogic/ivention/ipath_follower.py
 machinelogic/ivention/ipneumatic.py
 machinelogic/ivention/irobot.py
 machinelogic/ivention/machine_configuration.py
 machinelogic/ivention/mqtt_client.py
 machinelogic/ivention/tests/__init__.py
 machinelogic/ivention/tests/test_event_listener.py
 machinelogic/ivention/tests/test_idigital_input.py
 machinelogic/ivention/tests/test_idigital_output.py
 machinelogic/ivention/tests/test_imachine.py
+machinelogic/ivention/tests/test_ipath_follower.py
 machinelogic/ivention/tests/test_mqtt_client.py
 machinelogic/ivention/types/__init__.py
 machinelogic/ivention/types/ac_motor_details.py
 machinelogic/ivention/types/actuator_details.py
 machinelogic/ivention/types/bag_gripper_details.py
 machinelogic/ivention/types/input_details.py
 machinelogic/ivention/types/output_details.py
+machinelogic/ivention/types/path_follower_status.py
+machinelogic/ivention/types/path_follower_tool.py
 machinelogic/ivention/types/pneumatic_details.py
 machinelogic/ivention/util/__init__.py
 machinelogic/ivention/util/inheritance.py
 machinelogic/machinelogic/__init__.py
 machinelogic/machinelogic/ac_motor.py
 machinelogic/machinelogic/actuator.py
 machinelogic/machinelogic/actuator_group.py
@@ -56,21 +60,23 @@
 machinelogic/machinelogic/bag_gripper.py
 machinelogic/machinelogic/camera.py
 machinelogic/machinelogic/digital_input.py
 machinelogic/machinelogic/digital_output.py
 machinelogic/machinelogic/estop.py
 machinelogic/machinelogic/machine.py
 machinelogic/machinelogic/machine_motion.py
+machinelogic/machinelogic/path_follower.py
 machinelogic/machinelogic/pneumatic.py
 machinelogic/machinelogic/robot/__init__.py
 machinelogic/machinelogic/robot/robot.py
 machinelogic/machinelogic/robot/vention_ros_client_library.py
 machinelogic/machinelogic/tests/__init__.py
 machinelogic/machinelogic/tests/test_ac_motor.py
 machinelogic/machinelogic/tests/test_actuator.py
 machinelogic/machinelogic/tests/test_bag_gripper.py
 machinelogic/machinelogic/tests/test_machine.py
+machinelogic/machinelogic/tests/test_path_follower.py
 machinelogic/machinelogic/tests/test_pneumatic.py
 machinelogic/state_machine/__init__.py
 machinelogic/state_machine/state_machine.py
 machinelogic/state_machine/state_node.py
 machinelogic/state_machine/state_transition.py
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/decorators/future_api.py` & `machine_code_python_sdk-1.13.0/machinelogic/decorators/future_api.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/decorators/tests/test_future_api.py` & `machine_code_python_sdk-1.13.0/machinelogic/decorators/tests/test_future_api.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/decorators/tests/test_undocumented.py` & `machine_code_python_sdk-1.13.0/machinelogic/decorators/tests/test_undocumented.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/decorators/undocumented.py` & `machine_code_python_sdk-1.13.0/machinelogic/decorators/undocumented.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/event_listener.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/event_listener.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/exception.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,7 +100,14 @@
 
 class BagGripperException(VentionException):
     """An exception thrown by a BagGripper
 
     Args:
         VentionException(__type__): Super class
     """
+
+class PathFollowingException(Exception):
+    """An exception thrown by a path following operation
+
+    Args:
+        VentionException(__type__): Super class
+    """
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/iac_motor.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/iac_motor.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/iactuator.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/iactuator.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,22 +68,24 @@
         uuid: str,
         name: str,
         ip_address: str,
         actuator_type: ActuatorType,
         home_sensor: Literal["A", "B"],
         units: Literal["mm", "deg"],
         brake_present: bool,
+        controller_id: str,
     ) -> None:
         self._uuid: str = uuid
         self._name: str = name
         self._ip_address: str = ip_address
         self._actuator_type: ActuatorType = actuator_type
         self._units: Literal["mm", "deg"] = units
         self._home_sensor: Literal["A", "B"] = home_sensor
         self._brake_present: bool = brake_present
+        self._controller_id: str = controller_id
         self.sensor_event_listener: Optional[Callable[[Tuple[bool, bool]], None]] = None
         self.drive_error_event_listener: Optional[Callable[[int, str], None]] = None
 
     @property
     def uuid(self) -> str:
         """str: The Actuator's ID."""
         return self._uuid
@@ -109,14 +111,19 @@
         return self._home_sensor
 
     @property
     def units(self) -> Literal["deg", "mm"]:
         """Literal["deg", "mm"]: The units that the Actuator functions in."""
         return self._units
 
+    @property
+    def controller_id(self) -> str:
+        """str: The controller id of the Actuator"""
+        return self._controller_id
+
 
 class IActuator(ABC):
     """
     A software representation of an Actuator. An Actuator is defined as a motorized
     axis that can move by discrete distances. It is not recommended that you
     construct this object yourself. Rather, you should query it from a Machine instance:
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/iactuator_group.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/iactuator_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,23 +53,26 @@
 
         for actuator in actuators:
             if not isinstance(actuator, IActuator):
                 raise ActuatorGroupException(
                     "Must only pass Actuators to the ActuatorGroup constructor"
                 )
 
-        ip_address = None
+        controller_id = None
         for actuator in actuators:
-            if ip_address is None:
-                ip_address = actuator.configuration.ip_address
+            if controller_id is None:
+                controller_id = actuator.configuration.controller_id
                 continue
 
-            if ip_address != actuator.configuration.ip_address:
+            if controller_id != actuator.configuration.controller_id:
                 raise ActuatorGroupException(
-                    f"Actuators in an ActuatorGroup must be on the same controller, found an Actuator on ip={ip_address} and another on ip={actuator.configuration.ip_address}"
+                    f"""
+                    Actuators in an ActuatorGroup must be on the same controller,
+                    found an Actuator on controller={controller_id} and another on controller={actuator.configuration.controller_id}
+                    """
                 )
 
         self._actuators: Tuple[IActuator, ...] = actuators
         self._length: int = len(self._actuators)
         self._state: ActuatorGroupState = ActuatorGroupState(
             *[actuator.state for actuator in actuators]
         )
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/ibag_gripper.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/ibag_gripper.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/icamera.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/icamera.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/idigital_input.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/idigital_input.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/idigital_io_shared.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/idigital_io_shared.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/idigital_output.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/idigital_output.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/iestop.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/iestop.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/imachine.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/imachine.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,21 @@
     """
     A software representation of the entire Machine. A Machine is defined as any number of
     MachineMotions, each containing their own set of axes, outputs, inputs, pneumatics,
     bag grippers, and AC Motors. The Machine class offers a global way to retrieve these
     various components using the friendly names that you've defined in your MachineLogic
     configuration.
 
-    To create a new Machine, you can simply write:
+    To create a new Machine with default settings, you can simply write:
         machine = Machine()
-
+    
+    If you need to connect to services running on a different machine or IP address, 
+    you can specify the IP address as follows:
+        machine = Machine("192.168.7.2")
+    
     You should only ever have a single instance of this object in your program.
     """
 
     def __init__(
         self,
         machine_motions: list[IMachineMotion],
         mqtt_client: MqttClient,
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/imachine_motion.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/imachine_motion.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/ipneumatic.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/ipneumatic.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/irobot.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/irobot.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,39 +34,42 @@
 class IRobotAlarm(ABC):
     pass
 
 
 class RobotOperationalState(Enum):
     """The robot's operational state."""
 
-    # operational_state: NORMAL | FREEDRIVE | NON_OPERATIONAL | DISCONNECTED
+    # operational_state: NORMAL | FREEDRIVE | NON_OPERATIONAL | OFFLINE | UNKNOWN | NEED_MANUAL_INTERVENTION
     # uint8 STATE_OFFLINE=0
     # uint8 STATE_NON_OPERATIONAL=1
     # uint8 STATE_FREEDRIVE=2
     # uint8 STATE_NORMAL=3
+    # uint8 STATE_UNKNOWN=4
+    # uint8 STATE_NEED_MANUAL_INTERVENTION=5
     OFFLINE = 0
     NON_OPERATIONAL = 1
     FREEDRIVE = 2
     NORMAL = 3
+    UNKNOWN = 4
+    NEED_MANUAL_INTERVENTION = 5
 
 
 class RobotSafetyState(Enum):
     """The robot's safety state."""
 
-    # safety_state: NORMAL | PROTECTIVE_STOP | ROBOT_EMERGENCY_STOP | REDUCED_SPEED | SAFEGUARD_STOP
+    # safety_state: NORMAL | ROBOT_EMERGENCY_STOP | REDUCED_SPEED | SAFEGUARD_STOP
     # uint8 SAFETY_NORMAL=0
-    # uint8 SAFETY_PROTECTIVE_STOP=1
     # uint8 SAFETY_EMERGENCY_STOP=2
     # uint8 SAFETY_REDUCED_SPEED=3
     # uint8 SAFETY_SAFEGUARD_STOP=4
     # uint8 SAFETY_STATE_UKNOWNN=5
     NORMAL = 0
-    PROTECTIVE_STOP = 1
     EMERGENCY_STOP = 2
     REDUCED_SPEED = 3
+    SAFEGUARD_STOP = 4
     UNKNOWN = 5
 
 
 class RobotConfiguration(ABC):
     """
     A representation of the configuration of a Robot instance.
     This configuration defines what your Robot is and how it
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/machine_configuration.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/machine_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,17 +105,15 @@
         actuator_configuration_json (Any): The actuator configuration in JSON format.
 
     Returns:
         ActuatorConfiguration: The actuator configuration.
     """
     name = actuator_configuration_json["name"]
     uuid = actuator_configuration_json["uuid"]
-    controller_id = actuator_configuration_json[  # pylint: disable=unused-variable
-        "controllerId"
-    ]
+    controller_id = actuator_configuration_json["controllerId"]
     ip_address = actuator_configuration_json["ip"]
     parent_drive = actuator_configuration_json[  # pylint: disable=unused-variable
         "parentDrive"
     ]
     child_drives = actuator_configuration_json[  # pylint: disable=unused-variable
         "childDrives"
     ]
@@ -142,15 +140,22 @@
     control_loop = actuator_configuration_json[  # pylint: disable=unused-variable
         "controlLoop"
     ]
     home_sensor = actuator_configuration_json["homeSensor"]
     units = actuator_configuration_json["units"]
 
     return ActuatorConfiguration(
-        uuid, name, ip_address, actuator_type, home_sensor, units, brake_present
+        uuid,
+        name,
+        ip_address,
+        actuator_type,
+        home_sensor,
+        units,
+        brake_present,
+        controller_id,
     )
 
 
 def _parse_robot_configuration(
     robot_config_json: Any, ros_address: str
 ) -> RobotConfiguration:
     name = robot_config_json["friendlyName"]
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/mqtt_client.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_event_listener.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_event_listener.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_idigital_input.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_idigital_input.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_idigital_output.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_idigital_output.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_imachine.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_imachine.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from unittest.mock import MagicMock
 
 from machinelogic.ivention.exception import MachineException
 from machinelogic.ivention.iactuator import ActuatorConfiguration, IActuator
 from machinelogic.ivention.imachine import IMachine
 from machinelogic.ivention.imachine_motion import IMachineMotion
 from machinelogic.ivention.irobot import (
-  CartesianPose,
-  DegreesPerSecond,
-  DegreesPerSecondSquared,
-  IRobot,
-  IRobotAlarm,
-  IRobotState,
-  ISequenceBuilder,
-  JointAnglesDegrees,
-  Kilograms,
-  MillimetersPerSecond,
-  MillimetersPerSecondSquared,
-  RobotConfiguration,
-  RobotOperationalState,
-  RobotSafetyState,
-  TeachModeContextManager,
+    CartesianPose,
+    DegreesPerSecond,
+    DegreesPerSecondSquared,
+    IRobot,
+    IRobotAlarm,
+    IRobotState,
+    ISequenceBuilder,
+    JointAnglesDegrees,
+    Kilograms,
+    MillimetersPerSecond,
+    MillimetersPerSecondSquared,
+    RobotConfiguration,
+    RobotOperationalState,
+    RobotSafetyState,
+    TeachModeContextManager,
 )
 
 
 class DummyRobotConfiguration(RobotConfiguration):
     @property
     def cartesian_velocity_limit(self) -> MillimetersPerSecond:
         raise NotImplementedError
@@ -47,17 +47,19 @@
         if actuators is not None:
             self._actuator_list.extend(actuators)  # pylint: disable=protected-access
         if robots is not None:
             self._robot_list.extend(robots)  # pylint: disable=protected-access
 
 
 class DummyActuator(IActuator):
-    def __init__(self, name: str):
+    def __init__(self, name: str, controller_id: str = "controller_id"):
         super().__init__(
-            ActuatorConfiguration("uuid", name, "ip", "belt", "A", "mm", False)
+            ActuatorConfiguration(
+                "uuid", name, "ip", "belt", "A", "mm", False, controller_id
+            )
         )
 
     def move_relative_async(self, distance: float) -> None:
         raise NotImplementedError
 
     def move_absolute(self, position: float, timeout: float = 0) -> None:
         raise NotImplementedError
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/tests/test_mqtt_client.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/tests/test_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/types/actuator_details.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/types/actuator_details.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/ivention/util/inheritance.py` & `machine_code_python_sdk-1.13.0/machinelogic/ivention/util/inheritance.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/ac_motor.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/ac_motor.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/actuator.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/actuator.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/actuator_group.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/actuator_group.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/api.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,43 @@
 import warnings
 from enum import Enum
 from typing import Any, Dict, Literal, Optional, Tuple, TypedDict, Union, cast
 
 import requests
 
 from ..ivention.irobot import CartesianPose
-from ..ivention.machine_configuration import MachineConfiguration, parse_machine_configuration
-from ..ivention.types import ac_motor_details, actuator_details, bag_gripper_details, input_details, output_details, pneumatic_details
+from ..ivention.machine_configuration import (
+    MachineConfiguration,
+    parse_machine_configuration,
+)
+from ..ivention.types import (
+    ac_motor_details,
+    actuator_details,
+    bag_gripper_details,
+    input_details,
+    output_details,
+    path_follower_status,
+    path_follower_tool,
+    pneumatic_details,
+)
 
 
 class ApiException(Exception):
     """Thrown by the system when we encounter an error during a request"""
 
 
 class EndstopStateDict(TypedDict):
-    """Dictionary representing the endstop state
-
-    Args:
-        TypedDict (TypedDict): _description_
-    """
+    """Dictionary representing the endstop state"""
 
     home: bool
     end: bool
 
 
 class BrakeState(str, Enum):
-    """_summary_"""
+    """Enum representing brake state"""
 
     LOCKED = "Locked"
     UNLOCKED = "Unlocked"
     UNKNOWN = "Unknown"
 
 
 class Routes(Enum):
@@ -75,25 +83,36 @@
     HOME_ALL = "/v1/python/home_all"
     SET_AXES_POSITIONS = "/v1/python/set_axes_positions"
     STOP_ALL_MOTION = "/v1/python/stop_all_motion"
     MOVE_AC_MOTOR = "/v1/python/move_ac_motor"
     STOP_AC_MOTOR = "/v1/python/stop_ac_motor"
     OPEN_BAG_GRIPPER = "/v1/python/open_bag_gripper"
     CLOSE_BAG_GRIPPER = "/v1/python/close_bag_gripper"
+
+    # PATH FOLLOWING
+    START_PATH = "/v1/python/path"
+    STOP_PATH = "/v1/python/path/stop"
+    GET_PATH_STATUS = "/v1/python/path/status"
+    ADD_PATH_TOOL = "/v1/python/path/add_tool"
+    SET_PATH_AXIS_MAP = "/v1/python/path/set_axis_map"
+
+    # VISION
     VISION_CAMERA_CALIBRATION_SAVE = "/v1/vision/camera/calibration/save"
     VISION_CAMERA_CALIBRATE = "/v1/vision/camera/calibrate"
     VISION_CAMERA_START = "/v1/vision/camera/start"
     VISION_CAMERA_STOP = "/v1/vision/camera/stop"
     VISION_CAMERA_GRAB = "/v1/vision/camera/grab"
     VISION_CAMERA_RESET = "/v1/vision/camera/calibration/reset"
     VISION_CAMERA_PLAY = "/v1/vision/camera/play"
     VISION_CAMERA_RECORD = "/v1/vision/camera/record"
     VISION_CAMERA_TARGET = "/v1/vision/camera/target"
     VISION_CAMERA_POSE = "/v1/vision/camera/pose"
     VISION_VERSION = "/v1/vision/version"
+
+    # ROBOT
     SET_TCP_OFFSET = "/v1/python/set_tcp_offset"
 
 
 DEFAULT_TIMEOUT_SECONDS = 10
 MOVEMENT_TIMEOUT_SECONDS = 300
 
 
@@ -1125,14 +1144,155 @@
             response_dict: dict[str, float] = response.json()
             return response_dict
         except KeyError as err:
             raise ApiException(
                 f"Error while trying to get_axis_actual_torque, no completion value was received from the server. Got: {response_dict}"
             ) from err
 
+    def start_path(
+        self, gcode: str, controller_id: str, wait_on_path_completion: bool
+    ) -> bool:
+        """Load and start a gcode path
+
+        Args:
+            gcode (str): G-code path to start
+            controller_id (str): Id of the controller.
+            waitForMotionComplete (bool, optional):
+                If set True, we wait for the move to complete. Defaults to False.
+
+        Returns:
+            bool: True if we successfully ran G-code path
+        """
+
+        data = {
+            "path": gcode,
+            "acceleration": None,  # uses default from smart-drive server
+            "speedOverride": None,  # uses default from smart-drive server
+            "scaleMultiple": None,  # uses default from smart-drive server
+            "dryRun": None,  # uses default from smart-drive server
+            "controllerUuid": controller_id,
+            "waitOnPathCompletion": wait_on_path_completion,
+        }
+
+        # if we have to wait on completion, we don't know how long it could take.
+        timeout = None if wait_on_path_completion else DEFAULT_TIMEOUT_SECONDS
+
+        response = requests.post(
+            self._make_route(Routes.START_PATH),
+            json=data,
+            timeout=timeout,
+        )
+        if not response.ok:
+            warnings.warn(response.text)
+        return response.ok
+
+    def stop_path(self, controller_id: str) -> dict[str, float]:
+        """
+        Stops the currently running path
+
+        Args:
+            controller_id (str): ID of the controller.
+
+        Returns:
+            bool: True if we successfully stop G-code path
+        """
+        params = {"controllerUuid": controller_id}
+
+        try:
+            response = requests.get(
+                self._make_route(Routes.STOP_PATH),
+                params=params,
+                timeout=DEFAULT_TIMEOUT_SECONDS,
+            )
+            response_dict: dict[str, float] = response.json()
+            return response_dict
+        except KeyError as err:
+            raise ApiException(
+                f"""
+                Error while trying to stop path,
+                no completion value was received from the server. Got: {response_dict}
+                """
+            ) from err
+
+    def get_path_status(
+        self, controller_id: str
+    ) -> path_follower_status.PathFollowerStatus:
+        """Get the status of the current path"
+
+        Args:
+            controller_id (str): Id of controller
+
+        Returns:
+            PathStatusPayload: Payload describing the status of the path
+        """
+        params = {"controllerUuid": controller_id}
+
+        try:
+            response = requests.get(
+                self._make_route(Routes.GET_PATH_STATUS),
+                params=params,
+                timeout=DEFAULT_TIMEOUT_SECONDS,
+            )
+
+            response_dict = response.json()
+            return cast(
+                path_follower_status.PathFollowerStatus, response_dict["status"]
+            )
+        except KeyError as err:
+            raise ApiException(
+                f"""
+                Error while trying to get path status with
+                controller id {controller_id}. Got: {response_dict}"""
+            ) from err
+
+    def add_path_tool(
+        self, tool_id: int, tool: path_follower_tool.PathFollowerTool
+    ) -> bool:
+        """Set a tool ID to a tool payload
+
+        Args:
+            tool_id (int): tool number
+            tool (path_follower_tool.PathFollowerTool): {cw | ccw : {uuid: string, value: number}}
+
+        Returns: bool: True if we successfully set tool
+        """
+        payload = {"toolId": tool_id, "tool": tool}
+
+        response = requests.post(
+            self._make_route(Routes.ADD_PATH_TOOL),
+            json=payload,
+            timeout=DEFAULT_TIMEOUT_SECONDS,
+        )
+        if not response.ok:
+            warnings.warn(response.text)
+        return response.ok
+
+    def set_path_axes_map(
+        self,
+        axis_map: Dict[str, Union[str, None]],
+    ) -> bool:
+        """Set the axis / drive association
+
+        Args:
+            axis_map (Dict[str, str]): A map with at least of the X|Y|Z keys to drive UUIDs
+
+        Returns:
+            bool: True if we successfully set the axis map
+        """
+        payload = {"axisMap": axis_map}
+
+        response = requests.post(
+            self._make_route(Routes.SET_PATH_AXIS_MAP),
+            json=payload,
+            timeout=DEFAULT_TIMEOUT_SECONDS,
+        )
+        if not response.ok:
+            warnings.warn(response.text)
+        return response.ok
+
     def _camera_action(
         self, route: Routes, params: Optional[Dict[str, Any]] = None
     ) -> Union[Dict[str, Any], str]:
         """
         Perform an action with the camera capture pipeline.
 
         Args:
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/bag_gripper.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/bag_gripper.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/camera.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/camera.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/digital_output.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/digital_output.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/estop.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/estop.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/machine.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint: disable=protected-access
 import json
 import warnings
 from os import environ
-from typing import Optional
+from typing import Optional, Union
 
 from ..ivention.iactuator import IActuator
 from ..ivention.icamera import ICameraConfiguration
 from ..ivention.idigital_input import IDigitalInput
 from ..ivention.idigital_output import IDigitalOutput
 from ..ivention.imachine import IMachine
 from ..ivention.imachine_motion import IMachineMotion
@@ -23,28 +23,37 @@
 from .estop import Estop
 from .machine_motion import MachineMotion
 from .pneumatic import Pneumatic
 from .robot import Robot
 
 # Global variables specifying the URL of the execution engine and the MQTT broker
 # This is probably only going to be used in the cloud when spawning remote execution engines and the user doesn't control the ips
-# Otherwise, users would provide their connection strings through the constructor argument.
+# Otherwise, users would provide the machines IP strings through the constructor argument.
+
+MM_EXECUTION_ENGINE_DEFAULT_PORT = "3100"
+MQTT_DEFAULT_PORT = "9001"
+
 MM_EXECUTION_ENGINE_CONNECTION_STR = environ.get(
     "EXECUTION_ENGINE_CONN_STR", "http://localhost:3100"
 )
 MQTT_CONNECTION_STR = environ.get("MQTT_CONN_STR", "ws://localhost:9001")
 
 
 @inherit_docstrings
 class Machine(IMachine):
-    def __init__(
-        self,
-        api_connection_string: str = MM_EXECUTION_ENGINE_CONNECTION_STR,
-        mqtt_connection_string: str = MQTT_CONNECTION_STR,
-    ) -> None:
+    def __init__(self, ip_address: Union[str, None] = None) -> None:
+        if ip_address:
+            api_connection_string = (
+                f"http://{ip_address}:{MM_EXECUTION_ENGINE_DEFAULT_PORT}"
+            )
+            mqtt_connection_string = f"ws://{ip_address}:{MQTT_DEFAULT_PORT}"
+        else:
+            api_connection_string = MM_EXECUTION_ENGINE_CONNECTION_STR
+            mqtt_connection_string = MQTT_CONNECTION_STR
+
         api = Api(api_connection_string)
         machine_configuration = api.get_machine_configuration()
 
         mqtt_client = MqttClient(mqtt_connection_string)
 
         machine_motions = _create_machine_motions(
             machine_configuration, api, mqtt_client
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/pneumatic.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/pneumatic.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/robot/robot.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/robot/robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from collections import namedtuple
 from typing import Callable
 from urllib.parse import urlparse
 
 from machinelogic.decorators.undocumented import undocumented_property
 from machinelogic.ivention.exception import RobotException
 from machinelogic.ivention.irobot import (
-  CartesianPose,
-  DegreesPerSecond,
-  DegreesPerSecondSquared,
-  IRobot,
-  IRobotState,
-  ISequenceBuilder,
-  JointAnglesDegrees,
-  Kilograms,
-  MillimetersPerSecond,
-  MillimetersPerSecondSquared,
-  RobotConfiguration,
-  RobotOperationalState,
-  RobotSafetyState,
+    CartesianPose,
+    DegreesPerSecond,
+    DegreesPerSecondSquared,
+    IRobot,
+    IRobotState,
+    ISequenceBuilder,
+    JointAnglesDegrees,
+    Kilograms,
+    MillimetersPerSecond,
+    MillimetersPerSecondSquared,
+    RobotConfiguration,
+    RobotOperationalState,
+    RobotSafetyState,
 )
 from machinelogic.ivention.util.inheritance import inherit_docstrings  # type: ignore
 
 from ..api import Api
 from .vention_ros_client_library import RobotAlarm
 from .vention_ros_client_library import RosRobotClient as RosRobot
 
@@ -271,16 +271,15 @@
         acceleration: MillimetersPerSecondSquared = 100.0,
         reference_frame: CartesianPose | None = None,
     ) -> None:
         self._robot.movel(target, velocity, acceleration, reference_frame)
 
     def execute_sequence(self, sequence: ISequenceBuilder) -> bool:
         if isinstance(sequence, RosRobot.SequenceBuilder):
-            response = self._robot.execute_sequence(sequence)
-            return bool(response["success"])
+            return self._robot.execute_sequence(sequence)
 
         raise TypeError(
             "The sequence must be a SequenceBuilder, not a SequenceBuilderWrapper."
         )
 
     def teach_mode(self) -> RosRobot._WithTeach:
         return self._robot.teach_mode()
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/robot/vention_ros_client_library.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/robot/vention_ros_client_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Ignore mypy and pylint all errors
 # mypy: ignore-errors
 # pylint: disable-all
 
+
 """nb
 A NOTE ON UNITS:
     All joint angle arguments and return values to methods on class Robot are assumed to be in degrees.
     All cartesian pose arguments and return values are assumed to be of the form
         [x, y, z, rx, ry, rz]
     where:
         x, y, z - millimeters.
@@ -24,14 +25,15 @@
 from enum import Enum
 from typing import Any, Callable, Dict, List, Tuple, Union, cast
 
 import numpy as np
 import requests
 import roslibpy
 from scipy.spatial.transform import Rotation as scipy_rotation
+from machinelogic.ivention.exception import RobotException
 
 from machinelogic.ivention.irobot import (
     CartesianPose,
     Degrees,
     DegreesPerSecond,
     DegreesPerSecondSquared,
     DegreesPerSecondSquaredVector,
@@ -1047,30 +1049,37 @@
             "robot_commands_api/SetPayload",
             dict(payload=payload),
         )
 
     def create_sequence(self) -> "RosRobotClient.SequenceBuilder":
         return RosRobotClient.SequenceBuilder(self)
 
-    def execute_sequence(self, sequence: "RosRobotClient.SequenceBuilder"):
+    def execute_sequence(self, sequence: "RosRobotClient.SequenceBuilder") -> bool:
         moves = sequence.sequence
         if len(moves) == 0:
             raise Exception("no moves in sequence")
         limits = (
             self._joint_velocity_limit,
             self._joint_acceleration_limit,
             self._cartesian_velocity_limit,
             self._cartesian_acceleration_limit,
         )
         blend_radii = self._calculate_blend_radii(moves)
         move_messages = [
             move.message(*limits, blend_radii[index])
             for index, move in enumerate(moves)
         ]
-        return self._move_sequence(move_messages)
+        response = self._move_sequence(move_messages)
+        result = response["result"]
+        status_code, description = result["status_code"], result["description"]
+        if status_code != 1:
+            raise RobotException(
+                f"execute_sequence failed (code: {status_code}): {description}"
+            )
+        return True
 
     def movej(
         self,
         target: JointAnglesDegrees,
         velocity: DegreesPerSecond = 10.0,
         acceleration: DegreesPerSecondSquared = 10.0,
     ):
```

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_ac_motor.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_ac_motor.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_actuator.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_actuator.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_bag_gripper.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_bag_gripper.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_machine.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/machinelogic/tests/test_pneumatic.py` & `machine_code_python_sdk-1.13.0/machinelogic/machinelogic/tests/test_pneumatic.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/state_machine/state_machine.py` & `machine_code_python_sdk-1.13.0/machinelogic/state_machine/state_machine.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/state_machine/state_node.py` & `machine_code_python_sdk-1.13.0/machinelogic/state_machine/state_node.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/machinelogic/state_machine/state_transition.py` & `machine_code_python_sdk-1.13.0/machinelogic/state_machine/state_transition.py`

 * *Files identical despite different names*

### Comparing `machine-code-python-sdk-1.12.1/setup.py` & `machine_code_python_sdk-1.13.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="machine-code-python-sdk",
-    version="1.12.1",
+    version="1.13.0",
     description="MachineCode SDK for Vention hardware",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://vention.io/resources/guides/machinelogic-python-programming-514",
     author="VentionCo",
     author_email="vention-sw-ci@vention.cc",
     packages=find_packages(exclude=["qa*", "tests*"]),
     install_requires=[
         "miros==4.2.1",
         "paho-mqtt==1.5.1",
         "types-requests==2.28.11",
-        "requests==2.28.2",
+        "requests==2.31.0",
         "typing_extensions==4.6.3",
         "parameterized",
         "numpy==1.24.2",
         "roslibpy==1.4.2",
-        "scipy==1.9.3",
+        "scipy==1.11.1",
         "zope.interface==5.5.2",
     ],
     classifiers=[
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.5",
     ],
     python_requires=">=3.6",
```

