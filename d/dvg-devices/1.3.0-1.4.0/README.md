# Comparing `tmp/dvg-devices-1.3.0.tar.gz` & `tmp/dvg-devices-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvg-devices-1.3.0.tar", last modified: Thu Feb 23 19:21:48 2023, max compression
+gzip compressed data, was "dvg-devices-1.4.0.tar", last modified: Tue May 28 12:06:04 2024, max compression
```

## Comparing `dvg-devices-1.3.0.tar` & `dvg-devices-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 19:21:48.003796 dvg-devices-1.3.0/
--rw-rw-rw-   0        0        0      736 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/.readthedocs.yml
--rw-rw-rw-   0        0        0       76 2020-07-01 17:41:38.000000 dvg-devices-1.3.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     2848 2023-02-23 19:08:22.000000 dvg-devices-1.3.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     2511 2020-07-23 18:29:32.000000 dvg-devices-1.3.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1098 2022-02-01 21:32:50.000000 dvg-devices-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      289 2020-07-01 17:41:38.000000 dvg-devices-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7401 2023-02-23 19:21:48.002796 dvg-devices-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2932 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-23 19:21:47.975796 dvg-devices-1.3.0/docs/
--rw-rw-rw-   0        0        0      654 2020-06-10 12:56:24.000000 dvg-devices-1.3.0/docs/Makefile
--rw-rw-rw-   0        0        0      155 2020-07-15 22:53:33.000000 dvg-devices-1.3.0/docs/api-arduinoprotocolserial.rst
--rw-rw-rw-   0        0        0      965 2023-02-23 19:09:28.000000 dvg-devices-1.3.0/docs/api-serialdevice.rst
--rw-rw-rw-   0        0        0       27 2020-06-17 17:34:08.000000 dvg-devices-1.3.0/docs/authors.rst
--rw-rw-rw-   0        0        0       29 2020-06-17 17:34:49.000000 dvg-devices-1.3.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     3760 2023-02-23 19:09:00.000000 dvg-devices-1.3.0/docs/conf.py
--rw-rw-rw-   0        0        0       32 2020-06-17 17:36:57.000000 dvg-devices-1.3.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       45 2020-06-17 17:41:53.000000 dvg-devices-1.3.0/docs/genindex.rst
--rw-rw-rw-   0        0        0     2239 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/docs/index.rst
--rwxrwxrwx   0        0        0      795 2020-06-18 15:36:35.000000 dvg-devices-1.3.0/docs/make.bat
--rw-rw-rw-   0        0        0       54 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/docs/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-23 19:21:48.003796 dvg-devices-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     3311 2023-02-23 19:06:27.000000 dvg-devices-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 19:21:47.893795 dvg-devices-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-23 19:21:47.997797 dvg-devices-1.3.0/src/dvg_devices/
--rw-rw-rw-   0        0        0     5291 2023-01-26 23:20:39.000000 dvg-devices-1.3.0/src/dvg_devices/Aim_TTi_PSU_demo.py
--rw-rw-rw-   0        0        0    24939 2023-01-26 23:20:39.000000 dvg-devices-1.3.0/src/dvg_devices/Aim_TTi_PSU_protocol_RS232.py
--rw-rw-rw-   0        0        0    21081 2023-01-26 23:20:39.000000 dvg-devices-1.3.0/src/dvg_devices/Aim_TTi_PSU_qdev.py
--rw-rw-rw-   0        0        0     3804 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/src/dvg_devices/Arduino_protocol_serial.py
--rw-rw-rw-   0        0        0    34260 2023-02-23 19:04:20.000000 dvg-devices-1.3.0/src/dvg_devices/BaseDevice.py
--rw-rw-rw-   0        0        0     5805 2023-01-26 23:20:39.000000 dvg-devices-1.3.0/src/dvg_devices/Bronkhorst_MFC_demo.py
--rw-rw-rw-   0        0        0    12135 2023-01-26 23:20:39.000000 dvg-devices-1.3.0/src/dvg_devices/Bronkhorst_MFC_protocol_RS232.py
--rw-rw-rw-   0        0        0    12556 2023-01-26 23:20:39.000000 dvg-devices-1.3.0/src/dvg_devices/Bronkhorst_MFC_qdev.py
--rw-rw-rw-   0        0        0    10647 2023-01-26 23:20:39.000000 dvg-devices-1.3.0/src/dvg_devices/Compax3_servo_demo.py
--rw-rw-rw-   0        0        0    21500 2023-01-26 23:20:39.000000 dvg-devices-1.3.0/src/dvg_devices/Compax3_servo_protocol_RS232.py
--rw-rw-rw-   0        0        0    14922 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Compax3_servo_qdev.py
--rw-rw-rw-   0        0        0    10274 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Compax3_servo_step_navigator_GUI.py
--rw-rw-rw-   0        0        0     5330 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Julabo_circulator_demo.py
--rw-rw-rw-   0        0        0    31795 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Julabo_circulator_protocol_RS232.py
--rw-rw-rw-   0        0        0    14898 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Julabo_circulator_qdev.py
--rw-rw-rw-   0        0        0     6961 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Keysight_3497xA_demo.py
--rw-rw-rw-   0        0        0    18137 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Keysight_3497xA_demo_logger.py
--rw-rw-rw-   0        0        0    26067 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/src/dvg_devices/Keysight_3497xA_protocol_SCPI.py
--rw-rw-rw-   0        0        0    22323 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Keysight_3497xA_qdev.py
--rw-rw-rw-   0        0        0     8106 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Keysight_N8700_demo.py
--rw-rw-rw-   0        0        0    32530 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/src/dvg_devices/Keysight_N8700_protocol_SCPI.py
--rw-rw-rw-   0        0        0    28407 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Keysight_N8700_qdev.py
--rw-rw-rw-   0        0        0     5851 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Picotech_PT104_demo.py
--rw-rw-rw-   0        0        0    19003 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/src/dvg_devices/Picotech_PT104_protocol_UDP.py
--rw-rw-rw-   0        0        0     7886 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/Picotech_PT104_qdev.py
--rw-rw-rw-   0        0        0     9319 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/PolyScience_PD_bath_protocol_RS232.py
--rw-rw-rw-   0        0        0     5958 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/ThermoFlex_chiller_demo.py
--rw-rw-rw-   0        0        0    35891 2022-09-14 21:08:37.000000 dvg-devices-1.3.0/src/dvg_devices/ThermoFlex_chiller_protocol_RS232.py
--rw-rw-rw-   0        0        0    26750 2023-01-26 23:20:40.000000 dvg-devices-1.3.0/src/dvg_devices/ThermoFlex_chiller_qdev.py
--rw-rw-rw-   0        0        0     4426 2018-12-06 19:33:08.000000 dvg-devices-1.3.0/src/dvg_devices/Traverse_layout.png
--rw-rw-rw-   0        0        0        0 2020-07-02 09:38:51.000000 dvg-devices-1.3.0/src/dvg_devices/_init_.py
-drwxrwxrwx   0        0        0        0 2023-02-23 19:21:48.002796 dvg-devices-1.3.0/src/dvg_devices.egg-info/
--rw-rw-rw-   0        0        0     7401 2023-02-23 19:21:47.000000 dvg-devices-1.3.0/src/dvg_devices.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1862 2023-02-23 19:21:47.000000 dvg-devices-1.3.0/src/dvg_devices.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 19:21:47.000000 dvg-devices-1.3.0/src/dvg_devices.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-08-11 20:45:36.000000 dvg-devices-1.3.0/src/dvg_devices.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      275 2023-02-23 19:21:47.000000 dvg-devices-1.3.0/src/dvg_devices.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-23 19:21:47.000000 dvg-devices-1.3.0/src/dvg_devices.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 12:06:04.544378 dvg-devices-1.4.0/
+-rw-rw-rw-   0        0        0      798 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/.readthedocs.yml
+-rw-rw-rw-   0        0        0       76 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3409 2024-05-23 16:13:20.000000 dvg-devices-1.4.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     2511 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1098 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      289 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8820 2024-05-28 12:06:04.544378 dvg-devices-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3256 2024-05-23 16:17:54.000000 dvg-devices-1.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-28 12:06:04.522724 dvg-devices-1.4.0/docs/
+-rw-rw-rw-   0        0        0      654 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/Makefile
+-rw-rw-rw-   0        0        0      155 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/api-arduinoprotocolserial.rst
+-rw-rw-rw-   0        0        0      965 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/api-serialdevice.rst
+-rw-rw-rw-   0        0        0       27 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/authors.rst
+-rw-rw-rw-   0        0        0       29 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/changelog.rst
+-rw-rw-rw-   0        0        0     3760 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/conf.py
+-rw-rw-rw-   0        0        0       32 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       45 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/genindex.rst
+-rw-rw-rw-   0        0        0     2239 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/index.rst
+-rwxrwxrwx   0        0        0      795 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/make.bat
+-rw-rw-rw-   0        0        0       54 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/docs/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 12:06:04.544378 dvg-devices-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     3329 2024-05-23 13:53:52.000000 dvg-devices-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:06:04.512718 dvg-devices-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 12:06:04.528747 dvg-devices-1.4.0/src/dvg_devices/
+-rw-rw-rw-   0        0        0     3952 2024-05-23 15:37:14.000000 dvg-devices-1.4.0/src/dvg_devices/Aim_TTi_PSU_demo.py
+-rw-rw-rw-   0        0        0    25563 2024-05-23 15:20:48.000000 dvg-devices-1.4.0/src/dvg_devices/Aim_TTi_PSU_protocol_RS232.py
+-rw-rw-rw-   0        0        0    19770 2024-05-23 15:38:47.000000 dvg-devices-1.4.0/src/dvg_devices/Aim_TTi_PSU_qdev.py
+-rw-rw-rw-   0        0        0     4129 2024-05-23 15:20:55.000000 dvg-devices-1.4.0/src/dvg_devices/Arduino_protocol_serial.py
+-rw-rw-rw-   0        0        0    34703 2024-05-23 15:20:59.000000 dvg-devices-1.4.0/src/dvg_devices/BaseDevice.py
+-rw-rw-rw-   0        0        0     4515 2024-05-23 15:40:40.000000 dvg-devices-1.4.0/src/dvg_devices/Bronkhorst_MFC_demo.py
+-rw-rw-rw-   0        0        0    12567 2024-05-23 15:21:03.000000 dvg-devices-1.4.0/src/dvg_devices/Bronkhorst_MFC_protocol_RS232.py
+-rw-rw-rw-   0        0        0    10586 2024-05-23 15:44:05.000000 dvg-devices-1.4.0/src/dvg_devices/Bronkhorst_MFC_qdev.py
+-rw-rw-rw-   0        0        0     9016 2024-05-23 15:43:13.000000 dvg-devices-1.4.0/src/dvg_devices/Compax3_servo_demo.py
+-rw-rw-rw-   0        0        0    21339 2024-05-23 15:21:25.000000 dvg-devices-1.4.0/src/dvg_devices/Compax3_servo_protocol_RS232.py
+-rw-rw-rw-   0        0        0    13168 2024-05-23 15:44:45.000000 dvg-devices-1.4.0/src/dvg_devices/Compax3_servo_qdev.py
+-rw-rw-rw-   0        0        0     8634 2024-05-23 15:46:07.000000 dvg-devices-1.4.0/src/dvg_devices/Compax3_servo_step_navigator_GUI.py
+-rw-rw-rw-   0        0        0     3973 2024-05-23 15:47:23.000000 dvg-devices-1.4.0/src/dvg_devices/Julabo_circulator_demo.py
+-rw-rw-rw-   0        0        0    32210 2024-05-23 15:21:35.000000 dvg-devices-1.4.0/src/dvg_devices/Julabo_circulator_protocol_RS232.py
+-rw-rw-rw-   0        0        0    13160 2024-05-23 15:48:25.000000 dvg-devices-1.4.0/src/dvg_devices/Julabo_circulator_qdev.py
+-rw-rw-rw-   0        0        0     5698 2024-05-23 15:55:15.000000 dvg-devices-1.4.0/src/dvg_devices/Keysight_3497xA_demo.py
+-rw-rw-rw-   0        0        0    15963 2024-05-23 15:53:18.000000 dvg-devices-1.4.0/src/dvg_devices/Keysight_3497xA_demo_logger.py
+-rw-rw-rw-   0        0        0    27353 2024-05-23 15:22:18.000000 dvg-devices-1.4.0/src/dvg_devices/Keysight_3497xA_protocol_SCPI.py
+-rw-rw-rw-   0        0        0    21673 2024-05-23 15:57:13.000000 dvg-devices-1.4.0/src/dvg_devices/Keysight_3497xA_qdev.py
+-rw-rw-rw-   0        0        0     6642 2024-05-23 15:59:00.000000 dvg-devices-1.4.0/src/dvg_devices/Keysight_N8700_demo.py
+-rw-rw-rw-   0        0        0    33813 2024-05-23 15:22:23.000000 dvg-devices-1.4.0/src/dvg_devices/Keysight_N8700_protocol_SCPI.py
+-rw-rw-rw-   0        0        0    27439 2024-05-23 16:00:22.000000 dvg-devices-1.4.0/src/dvg_devices/Keysight_N8700_qdev.py
+-rw-rw-rw-   0        0        0     3057 2024-05-23 13:53:51.000000 dvg-devices-1.4.0/src/dvg_devices/MDrive_example_motion_program_x.mxt
+-rw-rw-rw-   0        0        0     3057 2024-05-23 13:53:51.000000 dvg-devices-1.4.0/src/dvg_devices/MDrive_example_motion_program_z.mxt
+-rw-rw-rw-   0        0        0     5418 2024-05-23 15:22:26.000000 dvg-devices-1.4.0/src/dvg_devices/MDrive_stepper_demo.py
+-rw-rw-rw-   0        0        0    55474 2024-05-23 15:22:28.000000 dvg-devices-1.4.0/src/dvg_devices/MDrive_stepper_protocol_RS422.py
+-rw-rw-rw-   0        0        0    42947 2024-05-23 16:01:36.000000 dvg-devices-1.4.0/src/dvg_devices/MDrive_stepper_qdev.py
+-rw-rw-rw-   0        0        0     4432 2024-05-23 16:02:35.000000 dvg-devices-1.4.0/src/dvg_devices/Picotech_PT104_demo.py
+-rw-rw-rw-   0        0        0    19986 2024-05-23 15:22:34.000000 dvg-devices-1.4.0/src/dvg_devices/Picotech_PT104_protocol_UDP.py
+-rw-rw-rw-   0        0        0     6328 2024-05-23 16:03:35.000000 dvg-devices-1.4.0/src/dvg_devices/Picotech_PT104_qdev.py
+-rw-rw-rw-   0        0        0     9198 2024-05-23 15:22:37.000000 dvg-devices-1.4.0/src/dvg_devices/PolyScience_PD_bath_protocol_RS232.py
+-rw-rw-rw-   0        0        0     4468 2024-05-23 16:04:37.000000 dvg-devices-1.4.0/src/dvg_devices/ThermoFlex_chiller_demo.py
+-rw-rw-rw-   0        0        0    37693 2024-05-23 15:22:40.000000 dvg-devices-1.4.0/src/dvg_devices/ThermoFlex_chiller_protocol_RS232.py
+-rw-rw-rw-   0        0        0    24826 2024-05-23 16:05:53.000000 dvg-devices-1.4.0/src/dvg_devices/ThermoFlex_chiller_qdev.py
+-rw-rw-rw-   0        0        0     4426 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/src/dvg_devices/Traverse_layout.png
+-rw-rw-rw-   0        0        0     4830 2024-05-23 15:22:43.000000 dvg-devices-1.4.0/src/dvg_devices/XylemHydrovarHVL_CRC_tools.py
+-rw-rw-rw-   0        0        0     4449 2024-05-23 16:07:14.000000 dvg-devices-1.4.0/src/dvg_devices/XylemHydrovarHVL_demo.py
+-rw-rw-rw-   0        0        0    41159 2024-05-23 15:22:47.000000 dvg-devices-1.4.0/src/dvg_devices/XylemHydrovarHVL_protocol_RTU.py
+-rw-rw-rw-   0        0        0    21179 2024-05-23 16:09:03.000000 dvg-devices-1.4.0/src/dvg_devices/XylemHydrovarHVL_qdev.py
+-rw-rw-rw-   0        0        0     3460 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/src/dvg_devices/_Qt_tests.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 11:08:14.000000 dvg-devices-1.4.0/src/dvg_devices/_init_.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:06:04.528747 dvg-devices-1.4.0/src/dvg_devices.egg-info/
+-rw-rw-rw-   0        0        0     8820 2024-05-28 12:06:04.000000 dvg-devices-1.4.0/src/dvg_devices.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2299 2024-05-28 12:06:04.000000 dvg-devices-1.4.0/src/dvg_devices.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 12:06:04.000000 dvg-devices-1.4.0/src/dvg_devices.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-23 09:09:21.000000 dvg-devices-1.4.0/src/dvg_devices.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      280 2024-05-28 12:06:04.000000 dvg-devices-1.4.0/src/dvg_devices.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 12:06:04.000000 dvg-devices-1.4.0/src/dvg_devices.egg-info/top_level.txt
```

### Comparing `dvg-devices-1.3.0/.readthedocs.yml` & `dvg-devices-1.4.0/.readthedocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # .readthedocs.yml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
 
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.11"
+
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
 # Build documentation with MkDocs
 #mkdocs:
 #  configuration: mkdocs.yml
@@ -23,8 +28,8 @@
       - requirements: docs/requirements.txt
       - method: pip
         path: .
         extra_requirements:
            - docs
       #- method: setuptools
       #  path: .
-   system_packages: true
+   # system_packages: true
```

### Comparing `dvg-devices-1.3.0/CONTRIBUTING.rst` & `dvg-devices-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvg-devices-1.3.0/LICENSE.txt` & `dvg-devices-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dvg-devices-1.3.0/PKG-INFO` & `dvg-devices-1.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 Metadata-Version: 2.1
 Name: dvg-devices
-Version: 1.3.0
+Version: 1.4.0
 Summary: Collection of I/O interfaces to communicate with microcontroller boards and laboratory devices, with optional PyQt/PySide multithread support and graphical user-interfaces.
 Home-page: https://python-dvg-devices.readthedocs.io
 Author: Dennis van Gils
 Author-email: vangils.dennis@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Dennis-van-Gils/python-dvg-devices/issues
 Keywords: PyQt5,PyQt6,PySide2,PySide6,device I/O,automation,laboratory,science,control,experiment,multithread,Arduino,serial,VISA
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering 
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+Requires-Dist: dvg-debug-functions~=2.4
+Requires-Dist: dvg-pid-controller~=2.1
+Requires-Dist: dvg-pyqt-controls~=1.3
+Requires-Dist: dvg-pyqt-filelogger~=1.3
+Requires-Dist: dvg-pyqtgraph-threadsafe~=3.3
+Requires-Dist: dvg-qdeviceio~=1.2
+Requires-Dist: matplotlib~=3.1
+Requires-Dist: numpy~=1.15
+Requires-Dist: pyserial~=3.4
+Requires-Dist: pyvisa~=1.11
+Requires-Dist: qtpy
 Provides-Extra: pyqt5
+Requires-Dist: pyqt5~=5.12; extra == "pyqt5"
 Provides-Extra: pyqt6
+Requires-Dist: pyqt6; extra == "pyqt6"
 Provides-Extra: pyside2
+Requires-Dist: pyside2; extra == "pyside2"
 Provides-Extra: pyside6
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
+Requires-Dist: pyside6; extra == "pyside6"
 
-.. image:: https://img.shields.io/pypi/v/dvg-devices
+|pypi| |python| |readthedocs| |black| |license|
+
+.. |pypi| image:: https://img.shields.io/pypi/v/dvg-devices
     :target: https://pypi.org/project/dvg-devices
-.. image:: https://img.shields.io/pypi/pyversions/dvg-devices
+.. |python| image:: https://img.shields.io/pypi/pyversions/dvg-devices
     :target: https://pypi.org/project/dvg-devices
-.. image:: https://requires.io/github/Dennis-van-Gils/python-dvg-devices/requirements.svg?branch=master
-    :target: https://requires.io/github/Dennis-van-Gils/python-dvg-devices/requirements/?branch=master
-    :alt: Requirements Status
-.. image:: https://readthedocs.org/projects/python-dvg-devices/badge/?version=latest
+.. |readthedocs| image:: https://readthedocs.org/projects/python-dvg-devices/badge/?version=latest
     :target: https://python-dvg-devices.readthedocs.io/en/latest/?badge=latest
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
-.. image:: https://img.shields.io/badge/License-MIT-purple.svg
+.. |license| image:: https://img.shields.io/badge/License-MIT-purple.svg
     :target: https://github.com/Dennis-van-Gils/python-dvg-devices/blob/master/LICENSE.txt
 
 DvG_Devices
 =============
 *Collection of I/O interfaces to communicate with microcontroller boards and
 laboratory devices, with optional PyQt/PySide multithread support and graphical
 user-interfaces.*
@@ -59,33 +72,37 @@
 - Github: https://github.com/Dennis-van-Gils/python-dvg-devices
 - PyPI: https://pypi.org/project/dvg-devices
 
 Installation::
 
     pip install dvg-devices
 
-Installation with an optional Qt-library::
+To be able to run the several provided graphical user-interfaces, one has to install an additional Qt-library. This can be either PyQt5, PyQt6, PySide2 or PySide6. Installation with an optional Qt-library::
 
     pip install dvg-devices[pyqt5/pyqt6/pyside2/pyside6]
 
+If you wish to interface with an GPIB device you need to additionally install a Visa backend. See https://pyvisa.readthedocs.io/en/latest/introduction/getting.html
+
 Supported devices
 -----------------
 
-    =======================    =======================
-    Arduino, or similar        microcontroller board
-    Aim TTi QL series II       power supply
-    Bronkhorst EL-FLOW         mass flow controller
-    Julabo circulator          recirculating bath
-    Keysight 3497xA            digital multimeter
-    Keysight N8700             power supply
-    Parker Compax3             servo controller
-    Picotech PT104             temperature logger
-    PolyScience PD             recirculating bath
-    ThermoFisher ThermoFlex    chiller
-    =======================    =======================
+    =======================    ==============================
+    Arduino, or similar        Microcontroller board
+    Aim TTi QL series II       Power supply
+    Bronkhorst EL-FLOW         Mass flow controller
+    Julabo circulator          Recirculating bath
+    Keysight 3497xA            Digital multimeter
+    Keysight N8700             Power supply
+    Novanta IMS MDrive         Stepper motor controller
+    Parker Compax3             Servo controller
+    Picotech PT104             Temperature logger
+    PolyScience PD             Recirculating bath
+    ThermoFisher ThermoFlex    Chiller
+    Xylem Hydrovar HVL         Variable speed pump controller
+    =======================    ==============================
 
 Highlights
 ----------
 * Class ``SerialDevice()`` offering higher-level general I/O methods for
   a serial device, such as ``auto_connect()``, ``write()`` and ``query()``.
 
 * Class ``Arduino()`` which wraps around ``SerialDevice()``. In combination with
@@ -99,14 +116,31 @@
 
 * Ready-to-run PyQt/PySide demos to directly control many of the supported
   devices with a graphical user-interface.
 
 Changelog
 =========
 
+1.4.0 (2024-05-23)
+------------------
+Major clean-up and streamlining:
+
+* Using `qtpy` library instead of my own Qt5/6 mechanism
+* Changed all string formatting to f-strings
+* Extended type hinting and checking
+* Made demos uniform and passing `qdev` arguments to `MainWindow` now
+* Individual source files now follow the PyPi package version
+* Resolved nearly all Pylint / Pylance warnings
+* Removed Python 3.6 support
+
+New devices added:
+
+* Xylem Hydrovar HVL - Variable speed pump controller
+* Novanta IMS MDrive - Stepper motor controller
+
 1.3.0 (2023-02-23)
 ------------------
 * Added method ``BaseDevice.SerialDevice.query_bytes()``
 * Fixed type hints in ``BaseDevice.SerialDevice``
 
 1.2.0 (2022-09-14)
 ------------------
@@ -193,9 +227,7 @@
 ------------------
 * Major restructuring PyPI package
 * Implemented ``DvG_QDeviceIO``
 
 0.0.1 (2020-07-01)
 ------------------
 * First release on PyPI
-
-
```

### Comparing `dvg-devices-1.3.0/README.rst` & `dvg-devices-1.4.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,19 @@
-.. image:: https://img.shields.io/pypi/v/dvg-devices
-    :target: https://pypi.org/project/dvg-devices
-.. image:: https://img.shields.io/pypi/pyversions/dvg-devices
-    :target: https://pypi.org/project/dvg-devices
-.. image:: https://requires.io/github/Dennis-van-Gils/python-dvg-devices/requirements.svg?branch=master
-    :target: https://requires.io/github/Dennis-van-Gils/python-dvg-devices/requirements/?branch=master
-    :alt: Requirements Status
-.. image:: https://readthedocs.org/projects/python-dvg-devices/badge/?version=latest
-    :target: https://python-dvg-devices.readthedocs.io/en/latest/?badge=latest
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-.. image:: https://img.shields.io/badge/License-MIT-purple.svg
-    :target: https://github.com/Dennis-van-Gils/python-dvg-devices/blob/master/LICENSE.txt
-
 DvG_Devices
 =============
 *Collection of I/O interfaces to communicate with microcontroller boards and
 laboratory devices, with optional PyQt/PySide multithread support and graphical
 user-interfaces.*
 
-Supports PyQt5, PyQt6, PySide2 and PySide6.
-
 - Documentation: https://python-dvg-devices.readthedocs.io
 - Github: https://github.com/Dennis-van-Gils/python-dvg-devices
 - PyPI: https://pypi.org/project/dvg-devices
 
+Supports PyQt5, PyQt6, PySide2 and PySide6.
+
 Installation::
 
     pip install dvg-devices
 
 Installation with an optional Qt-library::
 
     pip install dvg-devices[pyqt5/pyqt6/pyside2/pyside6]
@@ -60,7 +46,25 @@
 
 * Separate PyQt/PySide interfaces are provided for each of these devices,
   offering out-of-the-box multithreaded data acquisition and communication. It
   relies on `DvG_QDeviceIO <https://python-dvg-qdeviceio.readthedocs.io>`_.
 
 * Ready-to-run PyQt/PySide demos to directly control many of the supported
   devices with a graphical user-interface.
+
+
+.. toctree::
+   :caption: API
+
+   api-serialdevice
+   api-arduinoprotocolserial
+
+
+
+.. toctree::
+   :maxdepth: 1
+   :caption: Other
+
+   authors
+   changelog
+   contributing
+   genindex
```

### Comparing `dvg-devices-1.3.0/docs/Makefile` & `dvg-devices-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dvg-devices-1.3.0/docs/api-serialdevice.rst` & `dvg-devices-1.4.0/docs/api-serialdevice.rst`

 * *Files identical despite different names*

### Comparing `dvg-devices-1.3.0/docs/conf.py` & `dvg-devices-1.4.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "DvG_Devices"
 copyright = "2022, Dennis van Gils"
 author = "Dennis van Gils"
 
 # The full version, including alpha/beta/rc tags
-release = "1.3.0"
+release = "1.4.0"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `dvg-devices-1.3.0/docs/index.rst` & `dvg-devices-1.4.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,59 @@
+|pypi| |python| |readthedocs| |black| |license|
+
+.. |pypi| image:: https://img.shields.io/pypi/v/dvg-devices
+    :target: https://pypi.org/project/dvg-devices
+.. |python| image:: https://img.shields.io/pypi/pyversions/dvg-devices
+    :target: https://pypi.org/project/dvg-devices
+.. |readthedocs| image:: https://readthedocs.org/projects/python-dvg-devices/badge/?version=latest
+    :target: https://python-dvg-devices.readthedocs.io/en/latest/?badge=latest
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. |license| image:: https://img.shields.io/badge/License-MIT-purple.svg
+    :target: https://github.com/Dennis-van-Gils/python-dvg-devices/blob/master/LICENSE.txt
+
 DvG_Devices
 =============
 *Collection of I/O interfaces to communicate with microcontroller boards and
 laboratory devices, with optional PyQt/PySide multithread support and graphical
 user-interfaces.*
 
+Supports PyQt5, PyQt6, PySide2 and PySide6.
+
 - Documentation: https://python-dvg-devices.readthedocs.io
 - Github: https://github.com/Dennis-van-Gils/python-dvg-devices
 - PyPI: https://pypi.org/project/dvg-devices
 
-Supports PyQt5, PyQt6, PySide2 and PySide6.
-
 Installation::
 
     pip install dvg-devices
 
-Installation with an optional Qt-library::
+To be able to run the several provided graphical user-interfaces, one has to install an additional Qt-library. This can be either PyQt5, PyQt6, PySide2 or PySide6. Installation with an optional Qt-library::
 
     pip install dvg-devices[pyqt5/pyqt6/pyside2/pyside6]
 
+If you wish to interface with an GPIB device you need to additionally install a Visa backend. See https://pyvisa.readthedocs.io/en/latest/introduction/getting.html
+
 Supported devices
 -----------------
 
-    =======================    =======================
-    Arduino, or similar        microcontroller board
-    Aim TTi QL series II       power supply
-    Bronkhorst EL-FLOW         mass flow controller
-    Julabo circulator          recirculating bath
-    Keysight 3497xA            digital multimeter
-    Keysight N8700             power supply
-    Parker Compax3             servo controller
-    Picotech PT104             temperature logger
-    PolyScience PD             recirculating bath
-    ThermoFisher ThermoFlex    chiller
-    =======================    =======================
+    =======================    ==============================
+    Arduino, or similar        Microcontroller board
+    Aim TTi QL series II       Power supply
+    Bronkhorst EL-FLOW         Mass flow controller
+    Julabo circulator          Recirculating bath
+    Keysight 3497xA            Digital multimeter
+    Keysight N8700             Power supply
+    Novanta IMS MDrive         Stepper motor controller
+    Parker Compax3             Servo controller
+    Picotech PT104             Temperature logger
+    PolyScience PD             Recirculating bath
+    ThermoFisher ThermoFlex    Chiller
+    Xylem Hydrovar HVL         Variable speed pump controller
+    =======================    ==============================
 
 Highlights
 ----------
 * Class ``SerialDevice()`` offering higher-level general I/O methods for
   a serial device, such as ``auto_connect()``, ``write()`` and ``query()``.
 
 * Class ``Arduino()`` which wraps around ``SerialDevice()``. In combination with
@@ -46,25 +63,7 @@
 
 * Separate PyQt/PySide interfaces are provided for each of these devices,
   offering out-of-the-box multithreaded data acquisition and communication. It
   relies on `DvG_QDeviceIO <https://python-dvg-qdeviceio.readthedocs.io>`_.
 
 * Ready-to-run PyQt/PySide demos to directly control many of the supported
   devices with a graphical user-interface.
-
-
-.. toctree::
-   :caption: API
-
-   api-serialdevice
-   api-arduinoprotocolserial
-
-
-
-.. toctree::
-   :maxdepth: 1
-   :caption: Other
-
-   authors
-   changelog
-   contributing
-   genindex
```

### Comparing `dvg-devices-1.3.0/docs/make.bat` & `dvg-devices-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dvg-devices-1.3.0/setup.py` & `dvg-devices-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="dvg-devices",
-    version="1.3.0",
+    version="1.4.0",
     license="MIT",
     description="Collection of I/O interfaces to communicate with microcontroller boards and laboratory devices, with optional PyQt/PySide multithread support and graphical user-interfaces.",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
@@ -48,19 +48,19 @@
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering ",
         "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
         "Topic :: Scientific/Engineering :: Physics",
     ],
     project_urls={
         "Issue Tracker": "https://github.com/Dennis-van-Gils/python-dvg-devices/issues",
     },
@@ -76,26 +76,27 @@
         "control",
         "experiment",
         "multithread",
         "Arduino",
         "serial",
         "VISA",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=[
-        "dvg-debug-functions~=2.2",
-        "dvg-pid-controller~=2.0",
-        "dvg-pyqt-controls~=1.2",
-        "dvg-pyqt-filelogger~=1.2",
-        "dvg-pyqtgraph-threadsafe~=3.2",
-        "dvg-qdeviceio~=1.1",
+        "dvg-debug-functions~=2.4",
+        "dvg-pid-controller~=2.1",
+        "dvg-pyqt-controls~=1.3",
+        "dvg-pyqt-filelogger~=1.3",
+        "dvg-pyqtgraph-threadsafe~=3.3",
+        "dvg-qdeviceio~=1.2",
         "matplotlib~=3.1",
         "numpy~=1.15",
         "pyserial~=3.4",
         "pyvisa~=1.11",
+        "qtpy",
     ],
     extras_require={
         "pyqt5": ["pyqt5~=5.12"],
         "pyqt6": ["pyqt6"],
         "pyside2": ["pyside2"],
         "pyside6": ["pyside6"],
     },
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Aim_TTi_PSU_demo.py` & `dvg-devices-1.4.0/src/dvg_devices/Keysight_3497xA_demo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,163 +1,170 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""Multithreaded PyQt/PySide GUI to interface with a a Keysight (former HP or
+Agilent) 34970A/34972A data acquisition/switch unit.
+"""
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+print(__url__)
+# pylint: disable=wrong-import-position, missing-function-docstring, bare-except
 
-import os
 import sys
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
+import qtpy
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+import pyvisa
+
+import dvg_pyqt_controls as controls
+from dvg_devices.Keysight_3497xA_protocol_SCPI import Keysight_3497xA
+from dvg_devices.Keysight_3497xA_qdev import Keysight_3497xA_qdev
+
+# VISA address of the Keysight 3497xA data acquisition/switch unit containing a
+# multiplexer plug-in module. Hence, we simply call this device a 'mux'.
+# MUX_VISA_ADDRESS = "USB0::0x0957::0x2007::MY49018071::INSTR"
+MUX_VISA_ADDRESS = "GPIB0::9::INSTR"
+
+# SCPI commands to be send to the mux to set up the scan cycle.
+"""
+scan_list = "(@101:112)"
+MUX_SCPI_COMMANDS = [
+            f"rout:open {scan_list}",
+            f"conf:temp TC,J,{scan_list}",
+            f"unit:temp C,{scan_list}",
+            f"sens:temp:tran:tc:rjun:type INT,{scan_list}",
+            f"sens:temp:tran:tc:check ON,{scan_list}",
+            f"sens:temp:nplc 1,{scan_list}",
+            f"rout:scan {scan_list}",
+]
+"""
+
+scan_list = "(@101:110)"
+MUX_SCPI_COMMANDS = [
+    f"rout:open {scan_list}",
+    f"conf:res 1e6,{scan_list}",
+    f"sens:res:nplc 1,{scan_list}",
+    f"rout:scan {scan_list}",
+]
 
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-# Parse optional cli argument to enfore a QT_LIB
-# cli example: python benchmark.py pyside6
-if len(sys.argv) > 1:
-    arg1 = str(sys.argv[1]).upper()
-    for i, lib in enumerate(QT_LIB_ORDER):
-        if arg1 == lib.upper():
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
-from dvg_pyqt_controls import SS_TEXTBOX_READ_ONLY, SS_GROUP
-from dvg_devices.Aim_TTi_PSU_protocol_RS232 import Aim_TTi_PSU
-from dvg_devices.Aim_TTi_PSU_qdev import Aim_TTi_PSU_qdev
+# A scan will be performed by the mux every N milliseconds
+DAQ_INTERVAL_MS = 1000  # [ms]
 
 # Show debug info in terminal? Warning: Slow! Do not leave on unintentionally.
 DEBUG = False
 
 # ------------------------------------------------------------------------------
 #   MainWindow
 # ------------------------------------------------------------------------------
 
 
 class MainWindow(QtWid.QWidget):
-    def __init__(self, parent=None, **kwargs):
+    def __init__(self, qdev: Keysight_3497xA_qdev, parent=None, **kwargs):
         super().__init__(parent, **kwargs)
 
-        self.setGeometry(600, 120, 0, 0)
-        self.setWindowTitle("Aim TTi power supply control")
+        self.setWindowTitle("Keysight 3497xA control")
+        self.setGeometry(40, 60, 0, 0)
+        self.setFont(QtGui.QFont("Arial", 9))
+        self.setStyleSheet(
+            controls.SS_TEXTBOX_READ_ONLY
+            + controls.SS_GROUP
+            + controls.SS_HOVER
+        )
 
-        self.pbtn_exit = QtWid.QPushButton("Exit")
-        self.pbtn_exit.clicked.connect(self.close)
-        self.pbtn_exit.setMinimumHeight(30)
-
-        hbox = QtWid.QHBoxLayout()
-        hbox.addWidget(psu_qdev.grpb)
-        hbox.addWidget(
-            self.pbtn_exit, alignment=QtCore.Qt.AlignmentFlag.AlignTop
+        # Top grid
+        self.qlbl_title = QtWid.QLabel("Keysight 3497xA control")
+        self.qlbl_title.setFont(
+            QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold)
         )
-        hbox.addStretch(1)
+        self.qpbt_exit = QtWid.QPushButton("Exit")
+        self.qpbt_exit.clicked.connect(self.close)
+        self.qpbt_exit.setMinimumHeight(30)
+
+        grid_top = QtWid.QGridLayout()
+        grid_top.addWidget(self.qlbl_title, 0, 0)
+        grid_top.addWidget(
+            self.qpbt_exit, 0, 1, QtCore.Qt.AlignmentFlag.AlignRight
+        )
+
+        # Bottom grid
+        hbox1 = QtWid.QHBoxLayout()
+        hbox1.addWidget(qdev.qgrp)
+        hbox1.addStretch(1)
+        hbox1.setAlignment(qdev.qgrp, QtCore.Qt.AlignmentFlag.AlignTop)
 
+        # Round up full window
         vbox = QtWid.QVBoxLayout(self)
-        vbox.addLayout(hbox)
+        vbox.addLayout(grid_top)
+        vbox.addLayout(hbox1)
         vbox.addStretch(1)
 
 
 # ------------------------------------------------------------------------------
-#   about_to_quit
-# ------------------------------------------------------------------------------
-
-
-def about_to_quit():
-    print("About to quit")
-    app.processEvents()
-    psu_qdev.quit()
-    psu.close()
-
-
-# ------------------------------------------------------------------------------
 #   Main
 # ------------------------------------------------------------------------------
 
 if __name__ == "__main__":
-    # Config file containing COM port address
-    PATH_PORT = "config/port_Aim_TTi_PSU.txt"
-
-    # The state of the PSU is polled with this time interval
-    DAQ_INTERVAL_MS = 200  # [ms]
 
     # --------------------------------------------------------------------------
-    #   Connect to power supply
+    #   Connect to Keysight 3497xA (mux)
     # --------------------------------------------------------------------------
 
-    psu = Aim_TTi_PSU(name="Aim TTi PSU")
-    if psu.auto_connect(filepath_last_known_port=PATH_PORT):
-        psu.begin()
+    rm = pyvisa.ResourceManager()
+    mux = Keysight_3497xA(MUX_VISA_ADDRESS, "MUX")
+
+    try:
+        if mux.connect(rm):
+            mux.begin(MUX_SCPI_COMMANDS)
+    except ValueError as e:
+        # No connection could be made to the VISA device because module
+        # dependencies are missing. Print error, not raise and continue to
+        # show the GUI.
+        print(e)
 
     # --------------------------------------------------------------------------
     #   Create application
     # --------------------------------------------------------------------------
-    QtCore.QThread.currentThread().setObjectName("MAIN")  # For DEBUG info
 
+    main_thread = QtCore.QThread.currentThread()
+    if isinstance(main_thread, QtCore.QThread):
+        main_thread.setObjectName("MAIN")  # For DEBUG info
+
+    if qtpy.PYQT6 or qtpy.PYSIDE6:
+        sys.argv += ["-platform", "windows:darkmode=0"]
     app = QtWid.QApplication(sys.argv)
-    app.setFont(QtGui.QFont("Arial", 9))
-    app.setStyleSheet(SS_TEXTBOX_READ_ONLY + SS_GROUP)
-    app.aboutToQuit.connect(about_to_quit)
+    app.setStyle("Fusion")
 
     # --------------------------------------------------------------------------
-    #   Set up communication threads for the PSU
+    #   Set up communication threads for the mux
     # --------------------------------------------------------------------------
 
-    psu_qdev = Aim_TTi_PSU_qdev(
-        dev=psu, DAQ_interval_ms=DAQ_INTERVAL_MS, debug=DEBUG
+    mux_qdev = Keysight_3497xA_qdev(
+        dev=mux,
+        DAQ_interval_ms=DAQ_INTERVAL_MS,
+        debug=DEBUG,
     )
-    psu_qdev.start()
+    mux_qdev.start()
 
     # --------------------------------------------------------------------------
     #   Start the main GUI event loop
     # --------------------------------------------------------------------------
 
-    window = MainWindow()
+    def about_to_quit():
+        print("About to quit")
+        app.processEvents()
+        mux_qdev.quit()
+        try:
+            mux.close()
+        except:
+            pass
+        try:
+            rm.close()
+        except:
+            pass
+
+    app.aboutToQuit.connect(about_to_quit)
+    window = MainWindow(qdev=mux_qdev)
     window.show()
-    if QT_LIB in (PYQT5, PYSIDE2):
-        sys.exit(app.exec_())
-    else:
-        sys.exit(app.exec())
+
+    sys.exit(app.exec())
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Aim_TTi_PSU_protocol_RS232.py` & `dvg-devices-1.4.0/src/dvg_devices/Aim_TTi_PSU_protocol_RS232.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,64 +5,64 @@
 Note:
     * Only one channel implemented (channel 1)
     * Limited error reporting
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except, broad-except, try-except-raise
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=broad-except, missing-function-docstring, multiple-statements
 
 import os
 import sys
 import time
-from typing import AnyStr, Tuple
+from typing import Union, Tuple
 from pathlib import Path
 
 import numpy as np
 
 from dvg_debug_functions import print_fancy_traceback as pft
 from dvg_devices.BaseDevice import SerialDevice
 
 
 class Aim_TTi_PSU(SerialDevice):
     class State:
         """Container for the process and measurement variables."""
 
         # fmt: off
-        V_source = 0            # Voltage to be sourced         [V]
-        I_source = 0            # Current to be sourced (limit) [A]
+        V_source: float = 0            # Voltage to be sourced         [V]
+        I_source: float = 0            # Current to be sourced (limit) [A]
 
-        V_meas = np.nan         # Measured output voltage [V]
-        I_meas = np.nan         # Measured output current [A]
-        P_meas = np.nan         # Derived output power    [W]
-
-        OVP_level  = np.nan     # Over-voltage protection level [V]
-        OCP_level  = np.nan     # Over-current protection level [A]
-        ENA_output = False      # Is power output enabled (by software)?
+        V_meas: float = np.nan         # Measured output voltage [V]
+        I_meas: float = np.nan         # Measured output current [A]
+        P_meas: float = np.nan         # Derived output power    [W]
+
+        OVP_level:  float = np.nan      # Over-voltage protection level [V]
+        OCP_level:  float = np.nan      # Over-current protection level [A]
+        ENA_output: bool  = False       # Is power output enabled (by software)?
 
         # Limit Event Status Register (LSR)
-        LSR_is_tripped = False    # True if any LSR tripped, ignoring mode
-        LSR_TRIP_AUX = False      # Aux output trip                   , bit 7
-        LSR_MODE_AUX_CC = False   # Aux output constant-current mode  , bit 6
-        LSR_TRIP_SENSE = False    # Sense trip                        , bit 5
-        LSR_TRIP_OTP = False      # Over-temperature trip             , bit 4
-        LSR_TRIP_OCP = False      # Over-current trip                 , bit 3
-        LSR_TRIP_OVP = False      # Over-voltage trip                 , bit 2
-        LSR_MODE_CC = False       # Constant-current mode             , bit 1
-        LSR_MODE_CV = False       # Constant-voltage mode             , bit 0
+        LSR_is_tripped:  bool = False  # True if any LSR tripped, ignoring mode
+        LSR_TRIP_AUX:    bool = False  # Aux output trip                 , bit 7
+        LSR_MODE_AUX_CC: bool = False  # Aux output constant-current mode, bit 6
+        LSR_TRIP_SENSE:  bool = False  # Sense trip                      , bit 5
+        LSR_TRIP_OTP:    bool = False  # Over-temperature trip           , bit 4
+        LSR_TRIP_OCP:    bool = False  # Over-current trip               , bit 3
+        LSR_TRIP_OVP:    bool = False  # Over-voltage trip               , bit 2
+        LSR_MODE_CC:     bool = False  # Constant-current mode           , bit 1
+        LSR_MODE_CV:     bool = False  # Constant-voltage mode           , bit 0
         # fmt: on
 
     class Config:
         # fmt: off
-        V_source  = 10   # Voltage to be sourced         [V]
-        I_source  = 0.5  # Current to be sourced (limit) [A]
-        OVP_level = 12   # Over-voltage protection level [V]
-        OCP_level = 1    # Over-current protection level [A]
+        V_source:  float = 10   # Voltage to be sourced         [V]
+        I_source:  float = 0.5  # Current to be sourced (limit) [A]
+        OVP_level: float = 12   # Over-voltage protection level [V]
+        OCP_level: float = 1    # Over-current protection level [A]
         # fmt: on
 
     # --------------------------------------------------------------------------
     #   __init__
     # --------------------------------------------------------------------------
 
     def __init__(
@@ -89,27 +89,29 @@
             valid_ID_specific=connect_to_serial_number,
         )
 
         # Container for the process and measurement variables
         self.state = self.State()
         self.config = self.Config()
 
-        self.idn_str = None  # Identity response of the device
-        self.serial_str = None  # Serial number of the device
-        self.model_str = None  # Model of the device
+        self.idn_str = ""  # Identity response of the device
+        self.serial_str = ""  # Serial number of the device
+        self.model_str = ""  # Model of the device
 
         # Location of the configuration file
         self.path_config = Path(path_config)
 
     # --------------------------------------------------------------------------
     #   write_and_wait_for_opc
     # --------------------------------------------------------------------------
 
     def write_and_wait_for_opc(
-        self, msg: AnyStr, raises_on_timeout: bool = False
+        self,
+        msg: Union[str, bytes],
+        raises_on_timeout: bool = False,
     ) -> bool:
         """For proper synchronization we have to wait for the Operation Complete
         status of the device for the majority of the `set` commands. Hence this
         method.
         """
         success = self.write(msg=msg, raises_on_timeout=raises_on_timeout)
         if success:
@@ -125,15 +127,15 @@
         success = self.query_IDN()
         return success, self.serial_str
 
     # --------------------------------------------------------------------------
     #   begin
     # --------------------------------------------------------------------------
 
-    def begin(self):
+    def begin(self) -> bool:
         """This function should run directly after having established a
         connection to the device.
 
         Returns: True if successful, False otherwise.
         """
         if not self.is_alive:
             print("ERROR: Device is not connected yet or already closed.")
@@ -145,31 +147,38 @@
         success &= self.query_V_source()
         success &= self.query_I_source()
         success &= self.query_LSR()
 
         return success
 
     # --------------------------------------------------------------------------
+    #   flush_serial_input_and_output
+    # --------------------------------------------------------------------------
+
+    def flush_serial_input_and_output(self):
+        # Flush the serial input and output buffers
+        self.ser.flushInput()  # type: ignore
+        self.ser.flushOutput()  # type: ignore
+
+    # --------------------------------------------------------------------------
     #   reinitialize
     # --------------------------------------------------------------------------
 
-    def reinitialize(self):
+    def reinitialize(self) -> bool:
         """Reinitialize the PSU, including clear and reset
 
         Returns: True if all messages were sent and received successfully,
             False otherwise.
         """
 
         if not self.is_alive:
             print("ERROR: Device is not connected yet or already closed.")
             return False
 
-        # Flush the serial input and output buffers
-        self.ser.flushInput()
-        self.ser.flushOutput()
+        self.flush_serial_input_and_output()
 
         success = self.clear_and_reset()
         success &= self.set_OVP_level(self.config.OVP_level)
         success &= self.set_OCP_level(self.config.OCP_level)
         success &= self.set_V_source(self.config.V_source)
         success &= self.set_I_source(self.config.I_source)
 
@@ -189,23 +198,27 @@
     def query_IDN(self) -> bool:
         """Query the identity, serial and model number and store it in the class
         members.
 
         Returns: True if successful, False otherwise.
         """
         success, reply = self.query("*idn?")
-        if success and reply[:19] == "THURLBY THANDAR, QL":
+        if (
+            success
+            and isinstance(reply, str)
+            and reply[:19] == "THURLBY THANDAR, QL"
+        ):
             self.idn_str = reply
             self.serial_str = reply.split(",")[2].strip()
             self.model_str = reply.split(",")[1].strip()
             return True
 
-        self.idn_str = None
-        self.serial_str = None
-        self.model_str = None
+        self.idn_str = ""
+        self.serial_str = ""
+        self.model_str = ""
         return False
 
     # --------------------------------------------------------------------------
     #   System status related
     # --------------------------------------------------------------------------
 
     def clear_and_reset(self) -> bool:
@@ -237,15 +250,15 @@
         """
         # Returns an ASCII "1" when all pending overlapped operations have been
         # completed.
         success, reply = self.query("*opc?")
         if success and reply == "1":
             return True
 
-        pft("Warning: *opc? timed out at device %s" % self.name)
+        pft(f"Warning: *opc? timed out at device {self.name}")
         return False
 
     def set_LSE(self, value: int, channel: int = 1) -> bool:
         """Set the value of the Limit Event Status Enable Register (LSE).
 
         Args:
             value (int): (0-255)
@@ -256,28 +269,28 @@
                 * bit 3: Over-current trip
                 * bit 2: Over-voltage trip
                 * bit 1: Constant-current mode
                 * bit 0: Constant-voltage mode
 
         Returns: True if successful, False otherwise.
         """
-        return self.write_and_wait_for_opc("LSE%d %d" % (channel, value))
+        return self.write_and_wait_for_opc(f"LSE{channel} {value}")
 
     def query_LSR(self, verbose: bool = False, channel: int = 1) -> bool:
         """Query and parse the Limit Event Status Register (LSR). This holds
         the protection trips and output modes.
 
         Returns: True if successful, False otherwise.
         """
         # We will ignore the first read-out, because it apparently always lags
         # one behind.
-        self.query("LSR%d?" % channel)
+        self.query(f"LSR{channel}?")
 
-        success, reply = self.query("LSR%d?" % channel)
-        if success:
+        success, reply = self.query(f"LSR{channel}?")
+        if success and isinstance(reply, str):
             # fmt: off
             status_code = int(reply)
             self.state.LSR_TRIP_AUX    = bool(status_code & 128)
             self.state.LSR_MODE_AUX_CC = bool(status_code & 64)
             self.state.LSR_TRIP_SENSE  = bool(status_code & 32)
             self.state.LSR_TRIP_OTP    = bool(status_code & 16)
             self.state.LSR_TRIP_OCP    = bool(status_code & 8)
@@ -319,69 +332,69 @@
 
     def set_OVP_level(self, voltage_V, channel: int = 1) -> bool:
         """Returns: True if the message was sent successfully, False otherwise."""
         try:
             voltage_V = float(voltage_V)
         except (ValueError, TypeError):
             voltage_V = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
 
-        if self.write_and_wait_for_opc("OVP%d %f" % (channel, voltage_V)):
+        if self.write_and_wait_for_opc(f"OVP{channel} {voltage_V}"):
             self.state.OVP_level = voltage_V
             return True
 
         return False
 
     def set_OCP_level(self, current_A, channel: int = 1) -> bool:
         """Returns: True if the message was sent successfully, False otherwise."""
         try:
             current_A = float(current_A)
         except (ValueError, TypeError):
             current_A = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
 
-        if self.write_and_wait_for_opc("OCP%d %f" % (channel, current_A)):
+        if self.write_and_wait_for_opc(f"OCP{channel} {current_A}"):
             self.state.OCP_level = current_A
             return True
 
         return False
 
     def query_OVP_level(self, channel: int = 1) -> bool:
         """Returns: True if successful, False otherwise."""
-        success, reply = self.query("OVP%d?" % channel)
+        success, reply = self.query(f"OVP{channel}?")
         if success:
-            if reply[:3] == "VP%d" % channel:
+            if isinstance(reply, str) and reply[:3] == f"VP{channel}":
                 self.state.OVP_level = float(reply[4:])
                 return True
             else:
-                pft("Received incorrect reply: %s" % reply)
+                pft(f"Received incorrect reply: {reply}")
 
         return False
 
     def query_OCP_level(self, channel: int = 1) -> bool:
         """Returns: True if successful, False otherwise."""
-        success, reply = self.query("OCP%d?" % channel)
+        success, reply = self.query(f"OCP{channel}?")
         if success:
-            if reply[:3] == "CP%d" % channel:
+            if isinstance(reply, str) and reply[:3] == f"CP{channel}":
                 self.state.OCP_level = float(reply[4:])
                 return True
             else:
-                pft("Received incorrect reply: %s" % reply)
+                pft(f"Received incorrect reply: {reply}")
 
         return False
 
     # --------------------------------------------------------------------------
     #   Output related
     # --------------------------------------------------------------------------
 
     def reset_trips_and_turn_on(self, channel: int = 1) -> bool:
         """Returns: True if the message was sent successfully, False otherwise."""
-        if self.write_and_wait_for_opc("triprst;*opc;OP%d 1" % channel):
+        if self.write_and_wait_for_opc(f"triprst;*opc;OP{channel} 1"):
             self.state.ENA_output = True
             return True
 
         return False
 
     def turn_on(self, channel: int = 1) -> bool:
         """Returns: True if the message was sent successfully, False otherwise."""
@@ -389,150 +402,141 @@
 
     def turn_off(self, channel: int = 1) -> bool:
         """Returns: True if the message was sent successfully, False otherwise."""
         return self.set_ENA_output(ENA=False, channel=channel)
 
     def set_ENA_output(self, ENA: bool, channel: int = 1) -> bool:
         """Returns: True if the message was sent successfully, False otherwise."""
-        if self.write_and_wait_for_opc("OP%d %d" % (channel, ENA)):
+        if self.write_and_wait_for_opc(f"OP{channel} {ENA}"):
             self.state.ENA_output = ENA
             return True
 
         return False
 
     def set_V_source(self, voltage_V, channel: int = 1) -> bool:
         """Returns: True if the message was sent successfully, False otherwise."""
         try:
             voltage_V = float(voltage_V)
         except (ValueError, TypeError):
             voltage_V = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
 
-        if self.write_and_wait_for_opc("V%d %.3f" % (channel, voltage_V)):
+        if self.write_and_wait_for_opc(f"V{channel} {voltage_V:.3f}"):
             self.state.V_source = voltage_V
             return True
 
         return False
 
     def set_I_source(self, current_A, channel: int = 1) -> bool:
         """Returns: True if the message was sent successfully, False otherwise."""
         try:
             current_A = float(current_A)
         except (ValueError, TypeError):
             current_A = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
 
-        if self.write_and_wait_for_opc("I%d %.4f" % (channel, current_A)):
+        if self.write_and_wait_for_opc(f"I{channel} {current_A:.4f}"):
             self.state.I_source = current_A
             return True
 
         return False
 
     def query_ENA_output(self, channel: int = 1) -> bool:
         """Returns: True if the query was received successfully, False otherwise."""
-        success, reply = self.query("OP%d?" % channel)
+        success, reply = self.query(f"OP{channel}?")
         if success:
-            try:
+            if isinstance(reply, str) and reply.isnumeric():
                 self.state.ENA_output = bool(int(reply))
-            except:
-                pft("Received incorrect reply: %s" % reply)
-                self.ser.flushOutput()
-                self.ser.flushInput()
+                return True
 
-        return success
+            pft(f"Received incorrect reply: {reply}")
+            self.flush_serial_input_and_output()
+
+        return False
 
     def query_V_source(self, channel: int = 1) -> bool:
         """Returns: True if the query was received successfully, False otherwise."""
-        success, reply = self.query("V%d?" % channel)
+        success, reply = self.query(f"V{channel}?")
         if success:
-            if reply[:2] == "V%d" % channel:
+            if isinstance(reply, str) and reply[:2] == f"V{channel}":
                 self.state.V_source = float(reply[3:])
                 return True
 
-            pft("Received incorrect reply: %s" % reply)
-            self.ser.flushOutput()
-            self.ser.flushInput()
+            pft(f"Received incorrect reply: {reply}")
+            self.flush_serial_input_and_output()
 
         return False
 
     def query_V_meas(self, channel: int = 1) -> bool:
         """Returns: True if the query was received successfully, False otherwise."""
-        success, reply = self.query("V%dO?" % channel)
+        success, reply = self.query(f"V{channel}O?")
         if success:
-            if reply[-1:] == "V":
+            if isinstance(reply, str) and reply[-1:] == "V":
                 self.state.V_meas = float(reply[:-1])
                 self.state.P_meas = self.state.I_meas * self.state.V_meas
                 return True
 
-            pft("Received incorrect reply: %s" % reply)
-            self.ser.flushOutput()
-            self.ser.flushInput()
+            pft(f"Received incorrect reply: {reply}")
+            self.flush_serial_input_and_output()
 
         return False
 
     def query_I_source(self, channel: int = 1) -> bool:
         """Returns: True if the query was received successfully, False otherwise."""
-        success, reply = self.query("I%d?" % channel)
+        success, reply = self.query(f"I{channel}?")
         if success:
-            if reply[:2] == "I%d" % channel:
+            if isinstance(reply, str) and reply[:2] == f"I{channel}":
                 self.state.I_source = float(reply[3:])
                 return True
 
-            pft("Received incorrect reply: %s" % reply)
-            self.ser.flushOutput()
-            self.ser.flushInput()
+            pft(f"Received incorrect reply: {reply}")
+            self.flush_serial_input_and_output()
 
         return False
 
     def query_I_meas(self, channel: int = 1) -> bool:
         """Returns: True if the query was received successfully, False otherwise."""
-        success, reply = self.query("I%dO?" % channel)
+        success, reply = self.query(f"I{channel}O?")
         if success:
-            if reply[-1:] == "A":
+            if isinstance(reply, str) and reply[-1:] == "A":
                 self.state.I_meas = float(reply[:-1])
                 self.state.P_meas = self.state.I_meas * self.state.V_meas
                 return True
 
-            pft("Received incorrect reply: %s" % reply)
-            self.ser.flushOutput()
-            self.ser.flushInput()
+            pft(f"Received incorrect reply: {reply}")
+            self.flush_serial_input_and_output()
 
         return False
 
     # --------------------------------------------------------------------------
     #   Speed tests for debugging
     # --------------------------------------------------------------------------
 
     def speed_test(self):
         """Results: Each iteration takes 80 ms to finish."""
         self.turn_off()  # Disable output for safety
 
         tic = time.perf_counter()
         for i in range(100):
-            print("%d %.3f" % (i, time.perf_counter() - tic))
+            print(f"i {time.perf_counter() - tic:.3f}")
             self.set_V_source(i % 10)
 
         print(time.perf_counter() - tic)
         self.report()
 
     def speed_test2(self):
         """Results: Each iteration takes 8 ms to finish."""
 
         tic = time.perf_counter()
         for i in range(100):
             print(
-                "%d %.3f %.3f %.3f"
-                % (
-                    i,
-                    time.perf_counter() - tic,
-                    self.state.V_meas,
-                    self.state.I_meas,
-                )
+                f"{i} {time.perf_counter() - tic:.3f} "
+                f"{self.state.V_meas:.3f} {self.state.I_meas:.3f}"
             )
             self.query_V_meas()
             self.query_I_meas()
 
         print(time.perf_counter() - tic)
         self.report()
 
@@ -549,95 +553,93 @@
         self.query_V_source(channel=channel)
         self.query_I_source(channel=channel)
         self.query_V_meas(channel=channel)
         self.query_I_meas(channel=channel)
 
         print("")
         print(
-            "  %-3s         %4.1f OVP     %4.2f OCP"
-            % (
-                ("ON" if self.state.ENA_output else "OFF"),
-                self.state.OVP_level,
-                self.state.OCP_level,
-            )
+            f"  {('ON' if self.state.ENA_output else 'OFF'):-3s}       "
+            f"  {self.state.OVP_level:4.1f} OVP   "
+            f"  {self.state.OCP_level:4.2f} OCP"
         )
         print("  " + chr(0x2014) * 46)
 
         print(
-            "  Source      %6.3f V     %6.4f A"
-            % (self.state.V_source, self.state.I_source)
+            f"  Source "
+            f"     {self.state.V_source:6.3f} V"
+            f"     {self.state.I_source:6.4f} A"
         )
         print("  " + chr(0x2014) * 46)
         print(
-            "  Measure     %6.3f V     %6.4f A     %6.3f W"
-            % (self.state.V_meas, self.state.I_meas, self.state.P_meas)
+            f"  Measure "
+            f"    {self.state.V_meas:6.3f} V "
+            f"    {self.state.I_meas:6.4f} A "
+            f"    {self.state.P_meas:6.3f} W"
         )
 
     # --------------------------------------------------------------------------
     #   read_config_file
     # --------------------------------------------------------------------------
 
-    def read_config_file(self):
+    def read_config_file(self) -> bool:
         """Try to open the config textfile containing:
             * V_source   # Voltage to be sourced         [V]
             * I_source   # Current to be sourced (limit) [A]
             * OVP_level  # Over-voltage protection level [V]
             * OCP_level  # Over-current protection level [A]
         Do not panic if the file does not exist or cannot be read.
 
         Returns: True if successful, False otherwise.
         """
         if self.path_config.is_file():
             try:
-                with self.path_config.open() as f:
+                with self.path_config.open(encoding="utf8") as f:
                     self.config.V_source = float(f.readline().strip())
                     self.config.I_source = float(f.readline().strip())
                     self.config.OVP_level = float(f.readline().strip())
                     self.config.OCP_level = float(f.readline().strip())
 
                 return True
-            except:
+            except Exception:
                 pass  # Do not panic and remain silent
 
         return False
 
     # --------------------------------------------------------------------------
     #   write_config_file
     # --------------------------------------------------------------------------
 
-    def write_config_file(self):
+    def write_config_file(self) -> bool:
         """Try to write the config textfile containing:
              * V_source   # Voltage to be sourced         [V]
              * I_source   # Current to be sourced (limit) [A]
              * OVP_level  # Over-voltage protection level [V]
              * OCP_level  # Over-current protection level [A]
         Do not panic if the file does not exist or cannot be read.
 
         Returns: True if successful, False otherwise.
         """
 
         if not self.path_config.parent.is_dir():
             # Subfolder does not exists yet. Create.
             try:
                 self.path_config.parent.mkdir()
-            except:
+            except Exception:
                 pass  # Do not panic and remain silent
 
         try:
             # Write the config file
             self.path_config.write_text(
-                "%.3f\n%.3f\n%.1f\n%.2f"
-                % (
-                    self.state.V_source,
-                    self.state.I_source,
-                    self.state.OVP_level,
-                    self.state.OCP_level,
-                )
+                f"{self.state.V_source:.3f}\n"
+                f"{self.state.I_source:.3f}\n"
+                f"{self.state.OVP_level:.1f}\n"
+                f"{self.state.OCP_level:.2f}",
+                encoding="utf8",
             )
-        except:
+        except Exception:
             pass  # Do not panic and remain silent
         else:
             return True
 
         return False
 
 
@@ -655,13 +657,13 @@
     PATH_PORT = "config/port_Aim_TTi_PSU.txt"
 
     # Create connection to Aim TTi PSU over RS232
     psu = Aim_TTi_PSU(connect_to_serial_number=SERIAL_PSU)
 
     if psu.auto_connect(PATH_PORT):
         psu.begin()  # Retrieve necessary parameters
-        print("  IDN: %s" % psu.idn_str)
+        print(f"  IDN: {psu.idn_str}")
 
         psu.report()
         psu.close()
 
     sys.exit(0)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Aim_TTi_PSU_qdev.py` & `dvg-devices-1.4.0/src/dvg_devices/Aim_TTi_PSU_qdev.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,88 +2,34 @@
 # -*- coding: utf-8 -*-
 """PyQt/Pyside module to provide multithreaded communication and periodical data
 acquisition for an Aim TTi power supply unit (PSU), QL series II.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except, broad-except, try-except-raise
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=broad-except, missing-function-docstring, multiple-statements
 
-import os
-import sys
 import time
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt5.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt6.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-    from PySide2.QtCore import Signal                      # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-    from PySide6.QtCore import Signal                      # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Signal, Slot  # type: ignore
 
 from dvg_pyqt_controls import create_Toggle_button, create_tiny_error_LED
 from dvg_debug_functions import dprint, print_fancy_traceback as pft
 
 from dvg_qdeviceio import QDeviceIO, DAQ_TRIGGER
 from dvg_devices.Aim_TTi_PSU_protocol_RS232 import Aim_TTi_PSU
 
 # Monospace font
 FONT_MONOSPACE = QtGui.QFont("Monospace", 12, weight=QtGui.QFont.Weight.Bold)
 FONT_MONOSPACE.setStyleHint(QtGui.QFont.StyleHint.TypeWriter)
 
+
 # Enumeration
 class GUI_input_fields:
     [ALL, V_source, I_source, OVP_level, OCP_level] = range(5)
 
 
 class Aim_TTi_PSU_qdev(QDeviceIO):
     """Manages multithreaded communication and periodical data acquisition for
@@ -119,14 +65,15 @@
         DAQ_interval_ms=200,
         DAQ_timer_type=QtCore.Qt.TimerType.CoarseTimer,
         critical_not_alive_count=3,
         debug=False,
         **kwargs,
     ):
         super().__init__(dev, **kwargs)  # Pass kwargs onto QtCore.QObject()
+        self.dev: Aim_TTi_PSU  # Enforce type: removes `_NoDevice()`
 
         self.create_worker_DAQ(
             DAQ_trigger=DAQ_trigger,
             DAQ_function=self.DAQ_function,
             DAQ_interval_ms=DAQ_interval_ms,
             DAQ_timer_type=DAQ_timer_type,
             critical_not_alive_count=critical_not_alive_count,
@@ -164,15 +111,15 @@
         # on a hardware level by a triggered protection or fault.
         if self.dev.state.ENA_output and self.dev.state.LSR_is_tripped:
             self.dev.state.ENA_output = False
             self.dev.set_ENA_output(False)
 
         if DEBUG_local:
             tock = time.perf_counter()
-            dprint("%s: done in %i" % (self.dev.name, tock - tick))
+            dprint(f"{self.dev.name}: done in {tock - tick}")
 
         return True
 
     # --------------------------------------------------------------------------
     #   jobs_function
     # --------------------------------------------------------------------------
 
@@ -304,15 +251,15 @@
         grid.setColumnStretch(1, 0)
         grid.setColumnStretch(2, 0)
         grid.setColumnStretch(3, 1)
         grid.setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
         # grid.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeft)
         self.grid = grid
 
-        self.grpb = QtWid.QGroupBox("%s" % self.dev.name)
+        self.grpb = QtWid.QGroupBox(f"{self.dev.name}")
         self.grpb.setLayout(self.grid)
 
     # --------------------------------------------------------------------------
     #   update_GUI
     # --------------------------------------------------------------------------
 
     @Slot()
@@ -323,32 +270,32 @@
         """
         if self.dev.is_alive:
             if self.dev.state.LSR_is_tripped:
                 self.V_meas.setText("Safety")
                 self.I_meas.setText("tripped")
                 self.P_meas.setText("")
             else:
-                self.V_meas.setText("%6.3f V" % self.dev.state.V_meas)
-                self.I_meas.setText("%6.3f A" % self.dev.state.I_meas)
-                self.P_meas.setText("%6.3f W" % self.dev.state.P_meas)
+                self.V_meas.setText(f"{self.dev.state.V_meas:6.3f} V")
+                self.I_meas.setText(f"{self.dev.state.I_meas:6.3f} A")
+                self.P_meas.setText(f"{self.dev.state.P_meas:6.3f} W")
 
             self.pbtn_ENA_output.setChecked(self.dev.state.ENA_output)
             if self.pbtn_ENA_output.isChecked():
                 self.pbtn_ENA_output.setText("Output ON")
             else:
                 self.pbtn_ENA_output.setText("Output OFF")
 
             self.status_LSR_TRIP_SENSE.setChecked(self.dev.state.LSR_TRIP_SENSE)
             self.status_LSR_TRIP_OTP.setChecked(self.dev.state.LSR_TRIP_OTP)
             self.status_LSR_TRIP_OCP.setChecked(self.dev.state.LSR_TRIP_OCP)
             self.status_LSR_TRIP_OVP.setChecked(self.dev.state.LSR_TRIP_OVP)
             self.status_LSR_MODE_CC.setChecked(self.dev.state.LSR_MODE_CC)
             self.status_LSR_MODE_CV.setChecked(self.dev.state.LSR_MODE_CV)
 
-            self.lbl_update_counter.setText("%s" % self.update_counter_DAQ)
+            self.lbl_update_counter.setText(f"{self.update_counter_DAQ}")
         else:
             self.V_meas.setText("")
             self.I_meas.setText("Offline")
             self.I_meas.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
             self.P_meas.setText("")
             self.grpb.setEnabled(False)
 
@@ -356,30 +303,30 @@
     #   update_GUI_input_field
     # --------------------------------------------------------------------------
 
     @Slot()
     @Slot(int)
     def update_GUI_input_field(self, GUI_input_field=GUI_input_fields.ALL):
         if GUI_input_field == GUI_input_fields.V_source:
-            self.V_source.setText("%.3f" % self.dev.state.V_source)
+            self.V_source.setText(f"{self.dev.state.V_source:.3f}")
 
         elif GUI_input_field == GUI_input_fields.I_source:
-            self.I_source.setText("%.3f" % self.dev.state.I_source)
+            self.I_source.setText(f"{self.dev.state.I_source:.3f}")
 
         elif GUI_input_field == GUI_input_fields.OVP_level:
-            self.OVP_level.setText("%.1f" % self.dev.state.OVP_level)
+            self.OVP_level.setText(f"{self.dev.state.OVP_level:.1f}")
 
         elif GUI_input_field == GUI_input_fields.OCP_level:
-            self.OCP_level.setText("%.2f" % self.dev.state.OCP_level)
+            self.OCP_level.setText(f"{self.dev.state.OCP_level:.2f}")
 
         else:
-            self.V_source.setText("%.3f" % self.dev.state.V_source)
-            self.I_source.setText("%.3f" % self.dev.state.I_source)
-            self.OVP_level.setText("%.1f" % self.dev.state.OVP_level)
-            self.OCP_level.setText("%.2f" % self.dev.state.OCP_level)
+            self.V_source.setText(f"{self.dev.state.V_source:.3f}")
+            self.I_source.setText(f"{self.dev.state.I_source:.3f}")
+            self.OVP_level.setText(f"{self.dev.state.OVP_level:.1f}")
+            self.OCP_level.setText(f"{self.dev.state.OCP_level:.2f}")
 
     # --------------------------------------------------------------------------
     #   GUI functions
     # --------------------------------------------------------------------------
 
     @Slot()
     def process_pbtn_ENA_output(self):
@@ -392,79 +339,85 @@
 
     @Slot()
     def process_pbtn_reset_trips(self):
         self.send(self.dev.reset_trips)
 
     @Slot()
     def process_pbtn_save_settings(self):
-        str_title = "Save settings %s" % self.dev.name
-        str_msg = (
+        title = f"Save settings {self.dev.name}"
+        msg = (
             "This will save the following settings to file:\n"
             "  - source voltage\n"
             "  - source current\n"
             "  - OVP (over-voltage protection)\n"
             "  - OCP (over-current protection)"
         )
-        reply = QtWid.QMessageBox.information(
-            None,
-            str_title,
-            str_msg,
-            QtWid.QMessageBox.Cancel | QtWid.QMessageBox.Ok,
-            QtWid.QMessageBox.Cancel,
+        msgbox = QtWid.QMessageBox()
+        msgbox.setIcon(QtWid.QMessageBox.Icon.Information)
+        msgbox.setWindowTitle(title)
+        msgbox.setText(msg)
+        msgbox.setStandardButtons(
+            QtWid.QMessageBox.StandardButton.Cancel
+            | QtWid.QMessageBox.StandardButton.Ok
         )
+        msgbox.setDefaultButton(QtWid.QMessageBox.StandardButton.Cancel)
+        reply = msgbox.exec()
 
-        if reply == QtWid.QMessageBox.Ok:
+        if reply == QtWid.QMessageBox.StandardButton.Ok:
             if self.dev.write_config_file():
-                QtWid.QMessageBox.information(
-                    None,
-                    str_title,
-                    "Successfully saved to disk:\n%s" % self.dev.path_config,
-                )
+                icon = QtWid.QMessageBox.Icon.Information
+                msg = f"Successfully saved to disk:\n{self.dev.path_config}"
             else:
-                QtWid.QMessageBox.critical(
-                    None,
-                    str_title,
-                    "Failed to save to disk:\n%s" % self.dev.path_config,
-                )
+                icon = QtWid.QMessageBox.Icon.Critical
+                msg = f"Failed to save to disk:\n{self.dev.path_config}"
+
+            msgbox = QtWid.QMessageBox()
+            msgbox.setIcon(icon)
+            msgbox.setWindowTitle(title)
+            msgbox.setText(msg)
+            msgbox.exec()
 
     @Slot()
     def process_pbtn_load_settings(self):
-        str_title = "Load settings %s" % self.dev.name
-        str_msg = (
+        title = f"Load settings {self.dev.name}"
+        msg = (
             "This will reset the power supply and\n"
             "load the following settings from file:\n"
             "  - source voltage\n"
             "  - source current\n"
             "  - OVP (over-voltage protection)\n"
             "  - OCP (over-current protection)"
         )
-        reply = QtWid.QMessageBox.question(
-            None,
-            str_title,
-            str_msg,
-            QtWid.QMessageBox.Cancel | QtWid.QMessageBox.Ok,
-            QtWid.QMessageBox.Cancel,
+        msgbox = QtWid.QMessageBox()
+        msgbox.setIcon(QtWid.QMessageBox.Icon.Question)
+        msgbox.setWindowTitle(title)
+        msgbox.setText(msg)
+        msgbox.setStandardButtons(
+            QtWid.QMessageBox.StandardButton.Cancel
+            | QtWid.QMessageBox.StandardButton.Ok
         )
+        msgbox.setDefaultButton(QtWid.QMessageBox.StandardButton.Cancel)
+        reply = msgbox.exec()
 
-        if reply == QtWid.QMessageBox.Ok:
+        if reply == QtWid.QMessageBox.StandardButton.Ok:
             self.dev.read_config_file()
             self.add_to_jobs_queue(self.dev.reinitialize)
             self.add_to_jobs_queue(
                 "signal_GUI_input_field_update", GUI_input_fields.ALL
             )
             self.process_jobs_queue()
 
     @Slot()
     def send_V_source_from_textbox(self):
         try:
             voltage = float(self.V_source.text())
         except (TypeError, ValueError):
             voltage = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
 
         if voltage < 0:
             voltage = 0
 
         self.add_to_jobs_queue(self.dev.set_V_source, voltage)
         self.add_to_jobs_queue(self.dev.query_V_source)
         self.add_to_jobs_queue(
@@ -474,16 +427,16 @@
 
     @Slot()
     def send_I_source_from_textbox(self):
         try:
             current = float(self.I_source.text())
         except (TypeError, ValueError):
             current = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
 
         if current < 0:
             current = 0
 
         self.add_to_jobs_queue(self.dev.set_I_source, current)
         self.add_to_jobs_queue(self.dev.query_I_source)
         self.add_to_jobs_queue(
@@ -493,32 +446,32 @@
 
     @Slot()
     def send_OVP_level_from_textbox(self):
         try:
             OVP_level = float(self.OVP_level.text())
         except (TypeError, ValueError):
             OVP_level = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
 
         self.add_to_jobs_queue(self.dev.set_OVP_level, OVP_level)
         self.add_to_jobs_queue(self.dev.query_OVP_level)
         self.add_to_jobs_queue(
             "signal_GUI_input_field_update", GUI_input_fields.OVP_level
         )
         self.process_jobs_queue()
 
     @Slot()
     def send_OCP_level_from_textbox(self):
         try:
             OCP_level = float(self.OCP_level.text())
         except (TypeError, ValueError):
             OCP_level = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
 
         self.add_to_jobs_queue(self.dev.set_OCP_level, OCP_level)
         self.add_to_jobs_queue(self.dev.query_OCP_level)
         self.add_to_jobs_queue(
             "signal_GUI_input_field_update", GUI_input_fields.OCP_level
         )
         self.process_jobs_queue()
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Arduino_protocol_serial.py` & `dvg-devices-1.4.0/src/dvg_devices/Arduino_protocol_serial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""Provides higher-level general I/O methods for communicating with an
+Arduino(-like) board over the serial connection."""
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "14-09-2022"
-__version__ = "1.0.0"
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring
 
 import sys
-from typing import Tuple
+from typing import Union, Tuple
 
 from dvg_devices.BaseDevice import SerialDevice
 
 
 class Arduino(SerialDevice):
     """Provides higher-level general I/O methods for communicating with an
     Arduino(-like) board over the serial connection.
@@ -67,20 +70,24 @@
             valid_ID_specific=connect_to_specific_ID,
         )
 
     # --------------------------------------------------------------------------
     #   ID_validation_query
     # --------------------------------------------------------------------------
 
-    def ID_validation_query(self) -> Tuple[str, str]:
+    def ID_validation_query(self) -> Tuple[str, Union[str, None]]:
         # Expected: reply = "Arduino, [specific ID]"
         _success, reply = self.query("id?")
-        reply = reply.split(",")
-        reply_broad = reply[0].strip()  # "Arduino"
-        reply_specific = reply[1].strip() if len(reply) > 1 else None
+        if isinstance(reply, str):
+            reply = reply.split(",")
+            reply_broad = reply[0].strip()  # "Arduino"
+            reply_specific = reply[1].strip() if len(reply) > 1 else None
+        else:
+            reply_broad = ""
+            reply_specific = None
 
         return reply_broad, reply_specific
 
 
 # ------------------------------------------------------------------------------
 #   Main: Will show a demo when run from the terminal
 # ------------------------------------------------------------------------------
@@ -94,11 +101,11 @@
 
     if not ard.is_alive:
         sys.exit(0)
 
     _success, readings = ard.query_ascii_values("?")
     print(readings)
 
-    _success, reply = ard.query("?")
-    print(reply)
+    _success, my_reply = ard.query("?")
+    print(my_reply)
 
     ard.close()
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/BaseDevice.py` & `dvg-devices-1.4.0/src/dvg_devices/BaseDevice.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 These base classes are meant to be inherited into your own specific *Device*
 class.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "23-20-2023"
-__version__ = "1.3.0"
-# pylint: disable=bare-except, broad-except, try-except-raise
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=broad-except
 
 import sys
 import time
-from typing import AnyStr, Callable, Tuple, Union
+from typing import Union, Tuple, Callable
 from pathlib import Path
 
 # Use of `ast.literal_eval` got removed in v0.2.2 because it chokes on `nan`
 # from ast import literal_eval
 
 import serial
 import serial.tools.list_ports
@@ -91,22 +91,32 @@
         long_name="Serial Device",
     ):
         self.long_name = long_name
         self.name = name
 
         # Default serial settings
         self.serial_settings = {
+            # Defaults from `serial.Serial`
+            "bytesize": 8,
+            "parity": "N",
+            "stopbits": 1,
+            "xonxoff": False,
+            "rtscts": False,
+            "dsrdtr": False,
+            "inter_byte_timeout": None,
+            "exclusive": None,
+            # Edited
             "baudrate": 9600,
             "timeout": 2,
             "write_timeout": 2,
         }
 
         # Termination characters, must always be of type `bytes`.
-        self._read_termination = "\n".encode()
-        self._write_termination = "\n".encode()
+        self._read_termination: bytes = "\n".encode()
+        self._write_termination: bytes = "\n".encode()
 
         # Wait time during :meth:`query` in case there is no read termination
         # character set. We have to wait long enough to make sure the device has
         # had ample time to send out the reply to the serial-input buffer of
         # the host PC, which we will then read completely in one go.
         self._query_wait_time = 0.1  # [s]
 
@@ -126,15 +136,15 @@
 
     # --------------------------------------------------------------------------
     #   set_read_termination
     # --------------------------------------------------------------------------
 
     def set_read_termination(
         self,
-        termination: AnyStr,
+        termination: Union[str, bytes, None],
         query_wait_time: float = 0.1,
     ):
         """Set the termination character(s) for serial read.
 
         Args:
             termination (:obj:`str` | :obj:`bytes` | :obj:`None`):
                 Termination character(s). When set to :obj:`None` or empty the
@@ -146,41 +156,38 @@
                 See above.
 
                 Default: :const:`0.1`
         """
         if termination is None:
             termination = b""
 
-        self._read_termination = (
-            termination.encode()
-            if isinstance(termination, str)
-            else termination
-        )
+        if isinstance(termination, str):
+            termination = termination.encode()
 
+        self._read_termination = bytes(termination)
         self._query_wait_time = query_wait_time
 
     # --------------------------------------------------------------------------
     #   set_write_termination
     # --------------------------------------------------------------------------
 
-    def set_write_termination(self, termination: AnyStr):
+    def set_write_termination(self, termination: Union[str, bytes, None]):
         """Set the termination character(s) for serial write.
 
         Args:
             termination (:obj:`str` | :obj:`bytes` | :obj:`None`):
                 Termination character(s).
         """
         if termination is None:
             termination = b""
 
-        self._write_termination = (
-            termination.encode()
-            if isinstance(termination, str)
-            else termination
-        )
+        if isinstance(termination, str):
+            termination = termination.encode()
+
+        self._write_termination = bytes(termination)
 
     # --------------------------------------------------------------------------
     #   set_ID_validation_query
     # --------------------------------------------------------------------------
 
     def set_ID_validation_query(
         self,
@@ -201,15 +208,15 @@
             :meth:`auto_connect` a connection to a *desired* device will be
             attempted by performing a query for a device ID over the serial
             connection. The serial connection will be accepted and be stored in
             class member :attr:`ser` whenever the following scheme returns
             succesful:
 
         Args:
-            ID_validation_query (:obj:`~typing.Callable` [[], :obj:`tuple`]):
+            ID_validation_query (:obj:`~collections.abc.Callable` [[], :obj:`tuple`]):
                 Reference to a function to perform an ID validation query
                 on the device when connecting. The function should take zero
                 arguments and return a tuple consisting of two objects, as will
                 be explained further down. Only when the outcome of the
                 validation is successful, will the connection be accepted and
                 remain open. Otherwise, the connection will be automatically
                 closed again.
@@ -304,15 +311,16 @@
 
         try:
             reply = self.ser.readline()
         except serial.SerialException as err:
             # NOTE: The Serial library does not throw an exception when it
             # times out in `read`, only when it times out in `write`! We
             # will check for zero received bytes as indication for a read
-            # timeout, later. See: https://stackoverflow.com/questions/10978224/serialtimeoutexception-in-python-not-working-as-expected
+            # timeout, later. See:
+            # https://stackoverflow.com/questions/10978224/serialtimeoutexception-in-python-not-working-as-expected
             pft(err)
             return False, None
         except Exception as err:
             pft(err)
             return False, None
 
         if len(reply) == 0:
@@ -333,15 +341,17 @@
 
         return True, reply
 
     # --------------------------------------------------------------------------
     #   write
     # --------------------------------------------------------------------------
 
-    def write(self, msg: AnyStr, raises_on_timeout: bool = False) -> bool:
+    def write(
+        self, msg: Union[str, bytes], raises_on_timeout: bool = False
+    ) -> bool:
         """Send a message to the serial device.
 
         Args:
             msg (:obj:`str` | :obj:`bytes`):
                 ASCII string or bytes to be sent to the serial device.
 
             raises_on_timeout (:obj:`bool`, optional):
@@ -356,37 +366,37 @@
             pft("Device is not connected yet or already closed.", 3)
             return False  # --> leaving
 
         if isinstance(msg, str):
             msg = msg.encode()
 
         try:
-            self.ser.write(msg + self._write_termination)
+            self.ser.write(bytes(msg) + self._write_termination)
         except (
             serial.SerialTimeoutException,
             serial.SerialException,
         ) as err:
             if raises_on_timeout:
                 raise err  # --> leaving
-            else:
-                pft(err, 3)
-                return False  # --> leaving
+
+            pft(err, 3)
+            return False  # --> leaving
         except Exception as err:
             pft(err, 3)
             sys.exit(0)  # --> leaving
 
         return True
 
     # --------------------------------------------------------------------------
     #   query
     # --------------------------------------------------------------------------
 
     def query(
         self,
-        msg: AnyStr,
+        msg: Union[str, bytes],
         raises_on_timeout: bool = False,
         returns_ascii: bool = True,
     ) -> Tuple[bool, Union[str, bytes, None]]:
         """Send a message to the serial device and subsequently read the reply.
 
         Args:
             msg (:obj:`str` | :obj:`bytes`):
@@ -398,14 +408,18 @@
 
                 Default: :const:`False`
 
             returns_ascii (:obj:`bool`, optional):
                 When set to :const:`True` the device's reply will be returned as
                 an ASCII string. Otherwise, it will return as bytes.
 
+                TODO & NOTE: ASCII is a misnomer. The returned reply will be
+                UTF-8 encoded, not ASCII. Need to fix the argument name somehow,
+                without breaking code elsewhere.
+
                 Default: :const:`True`
 
         Returns:
             :obj:`tuple`:
                 success (:obj:`bool`):
                     True if successful, False otherwise.
 
@@ -432,29 +446,30 @@
                 reply = self.ser.read(self.ser.in_waiting)
             else:
                 reply = self.ser.read_until(self._read_termination)
         except serial.SerialException as err:
             # Note: The Serial library does not throw an exception when it
             # times out in `read`, only when it times out in `write`! We
             # will check for zero received bytes as indication for a read
-            # timeout, later. See: https://stackoverflow.com/questions/10978224/serialtimeoutexception-in-python-not-working-as-expected
+            # timeout, later. See:
+            # https://stackoverflow.com/questions/10978224/serialtimeoutexception-in-python-not-working-as-expected
             pft(err, 3)
             return (False, None)  # --> leaving
         except Exception as err:
             pft(err, 3)
             sys.exit(0)  # --> leaving
 
         if len(reply) == 0:
             if raises_on_timeout:
                 raise serial.SerialException(
                     "Received 0 bytes. Read probably timed out."
                 )  # --> leaving
-            else:
-                pft("Received 0 bytes. Read probably timed out.", 3)
-                return (False, None)  # --> leaving
+
+            pft("Received 0 bytes. Read probably timed out.", 3)
+            return (False, None)  # --> leaving
 
         if returns_ascii:
             try:
                 reply = reply.decode("utf8").strip()
             except UnicodeDecodeError as err:
                 pft(err, 3)
                 return (False, None)  # --> leaving
@@ -523,38 +538,39 @@
             else:
                 reply = b""
                 self.ser.flush()
         except serial.SerialException as err:
             # Note: The Serial library does not throw an exception when it
             # times out in `read`, only when it times out in `write`! We
             # will check for zero received bytes as indication for a read
-            # timeout, later. See: https://stackoverflow.com/questions/10978224/serialtimeoutexception-in-python-not-working-as-expected
+            # timeout, later. See:
+            # https://stackoverflow.com/questions/10978224/serialtimeoutexception-in-python-not-working-as-expected
             pft(err, 3)
             return (False, None)  # --> leaving
         except Exception as err:
             pft(err, 3)
             sys.exit(0)  # --> leaving
 
         if (N_bytes_to_read > 0) and (len(reply) == 0):
             if raises_on_timeout:
                 raise serial.SerialException(
                     "Received 0 bytes. Read probably timed out."
                 )  # --> leaving
-            else:
-                pft("Received 0 bytes. Read probably timed out.", 3)
-                return (False, None)  # --> leaving
+
+            pft("Received 0 bytes. Read probably timed out.", 3)
+            return (False, None)  # --> leaving
 
         if N_bytes_to_read != len(reply):
             if raises_on_timeout:
                 raise serial.SerialException(
                     "Received too few bytes. Read probably timed out."
                 )  # --> leaving
-            else:
-                pft("Received too few bytes. Read probably timed out.", 3)
-                return (False, reply)  # --> leaving
+
+            pft("Received too few bytes. Read probably timed out.", 3)
+            return (False, reply)  # --> leaving
 
         return (True, reply)
 
     # --------------------------------------------------------------------------
     #   query_ascii_values
     # --------------------------------------------------------------------------
 
@@ -593,25 +609,27 @@
                     Reply received from the device and parsed into a list of
                     separate values. The list is empty if unsuccessful.
         """
         success, reply = self.query(
             msg, raises_on_timeout=raises_on_timeout, returns_ascii=True
         )
 
-        if not success:
-            return (False, list())  # --> leaving
+        if not success or not isinstance(reply, str):
+            return (False, [])  # --> leaving
 
         try:
             # NOTE: `ast.literal_eval` chokes when it receives 'nan' so we ditch
             # it and just interpret everything as `float` instead.
             # reply_list = list(map(literal_eval, reply.split(delimiter)))
             reply_list = list(map(float, reply.split(delimiter)))
+
         except ValueError as err:
             pft(err, 3)
-            return (False, list())  # --> leaving
+            return (False, [])  # --> leaving
+
         except Exception as err:
             pft(err, 3)
             sys.exit(0)  # --> leaving
 
         return (True, reply_list)
 
     # --------------------------------------------------------------------------
@@ -619,19 +637,19 @@
     # --------------------------------------------------------------------------
 
     def close(self, ignore_exceptions=False):
         """Cancel all pending serial operations and close the serial port."""
         if self.ser is not None:
             try:
                 self.ser.cancel_read()
-            except:
+            except Exception:
                 pass
             try:
                 self.ser.cancel_write()
-            except:
+            except Exception:
                 pass
 
             try:
                 self.ser.close()
             except Exception as err:
                 if ignore_exceptions:
                     pass
@@ -667,32 +685,33 @@
 
         Returns:
             True if successful, False otherwise.
         """
 
         def print_success(success_str: str):
             dprint(success_str, ANSI.GREEN)
-            dprint(" " * 16 + "--> %s\n" % self.name, ANSI.GREEN)
+            dprint((" " * 16 + f"--> {self.name}\n"), ANSI.GREEN)
 
         if verbose:
             _print_hrule(True)
             if (
                 self._ID_validation_query is None
                 or self._valid_ID_specific is None
             ):
-                dprint("  Connecting to: %s" % self.long_name, ANSI.YELLOW)
+                msg = f"  Connecting to: {self.long_name}"
             else:
-                dprint(
-                    "  Connecting to: %s `%s`"
-                    % (self.long_name, self._valid_ID_specific),
-                    ANSI.YELLOW,
+                msg = (
+                    f"  Connecting to: {self.long_name} "
+                    f"`{self._valid_ID_specific}`"
                 )
+
+            dprint(msg, ANSI.YELLOW)
             _print_hrule()
 
-        print("  @ %-11s " % port, end="")
+        print(f"  @ {port:<11s} ", end="")
         try:
             # Open the serial port
             self.ser = serial.Serial(port=port, **self.serial_settings)
         except serial.SerialException:
             print("Could not open port.")
             return False  # --> leaving
         except Exception as err:
@@ -706,32 +725,32 @@
             return True  # --> leaving
 
         # Optional validation query
         try:
             self._force_query_to_raise_on_timeout = True
             self.is_alive = True  # We must assume communication is possible
             reply_broad, reply_specific = self._ID_validation_query()
-        except:
+        except Exception:
             print("Wrong or no device.")
             self.close(ignore_exceptions=True)
             return False  # --> leaving
         finally:
             self._force_query_to_raise_on_timeout = False
 
         if reply_broad == self._valid_ID_broad:
             if reply_specific is not None:
-                print("Found `%s`: " % reply_specific, end="")
+                print(f"Found `{reply_specific}`: ", end="")
 
             if self._valid_ID_specific is None:
                 # Found a matching device in a broad sense
                 print_success("Broad Success!")
                 self.is_alive = True
                 return True  # --> leaving
 
-            elif reply_specific == self._valid_ID_specific:
+            if reply_specific == self._valid_ID_specific:
                 # Found a matching device in a specific sense
                 print_success("Specific Success!")
                 self.is_alive = True
                 return True  # --> leaving
 
         print("Wrong device.")
         self.close(ignore_exceptions=True)
@@ -757,21 +776,21 @@
 
         if verbose:
             _print_hrule(True)
             if (
                 self._ID_validation_query is None
                 or self._valid_ID_specific is None
             ):
-                dprint("  Scanning ports for: %s" % self.long_name, ANSI.YELLOW)
+                msg = f"  Scanning ports for: {self.long_name}"
             else:
-                dprint(
-                    "  Scanning ports for: %s `%s`"
-                    % (self.long_name, self._valid_ID_specific),
-                    ANSI.YELLOW,
+                msg = (
+                    f"  Scanning ports for: {self.long_name} "
+                    f"`{self._valid_ID_specific}`"
                 )
+            dprint(msg, ANSI.YELLOW)
             _print_hrule()
 
         # Ports is a list of tuples
         ports = list(serial.tools.list_ports.comports())
         for p in ports:
             port = p[0]
             if self.connect_at_port(port, verbose=False):
@@ -808,26 +827,26 @@
         path = Path(filepath_last_known_port)
         port = self._get_last_known_port(path)
 
         if port is None:
             if self.scan_ports():
                 self._store_last_known_port(path, self.ser.portstr)
                 return True
-            else:
-                return False
-        else:
-            if self.connect_at_port(port):
-                self._store_last_known_port(path, self.ser.portstr)
-                return True
-            else:
-                if self.scan_ports(verbose=False):
-                    self._store_last_known_port(path, self.ser.portstr)
-                    return True
-                else:
-                    return False
+
+            return False
+
+        if self.connect_at_port(port):
+            self._store_last_known_port(path, self.ser.portstr)
+            return True
+
+        if self.scan_ports(verbose=False):
+            self._store_last_known_port(path, self.ser.portstr)
+            return True
+
+        return False
 
     # -----------------------------------------------------------------------------
     #   _get_last_known_port
     # -----------------------------------------------------------------------------
 
     def _get_last_known_port(self, path: Path):
         """Try to open the textfile pointed to by ``path``, containing the port
@@ -843,15 +862,15 @@
         """
         if isinstance(path, Path):
             if path.is_file():
                 try:
                     with path.open() as f:
                         port = f.readline().strip()
                     return port
-                except:
+                except Exception:
                     pass  # Do not panic and remain silent
 
         return None
 
     # -----------------------------------------------------------------------------
     #   _store_last_known_port
     # -----------------------------------------------------------------------------
@@ -872,21 +891,21 @@
             True if successful, False otherwise.
         """
         if isinstance(path, Path):
             if not path.parent.is_dir():
                 # Subfolder does not exists yet. Create.
                 try:
                     path.parent.mkdir()
-                except:
+                except Exception:
                     pass  # Do not panic and remain silent
 
             try:
                 # Write the config file
                 path.write_text(port_str)
-            except:
+            except Exception:
                 pass  # Do not panic and remain silent
             else:
                 return True
 
         return False
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Bronkhorst_MFC_demo.py` & `dvg-devices-1.4.0/src/dvg_devices/Keysight_N8700_demo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,174 +1,197 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""Multithreaded PyQt/PySide GUI to interface with a Bronkhorst mass flow
-controller (MFC).
+"""Multithreaded PyQt/PySide GUI to interface with a Keysight N8700 power supply
+(PSU).
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+print(__url__)
+# pylint: disable=wrong-import-position, missing-function-docstring, bare-except
 
 import os
 import sys
+from pathlib import Path
+from typing import List
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-# Parse optional cli argument to enfore a QT_LIB
-# cli example: python benchmark.py pyside6
-if len(sys.argv) > 1:
-    arg1 = str(sys.argv[1]).upper()
-    for i, lib in enumerate(QT_LIB_ORDER):
-        if arg1 == lib.upper():
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
-from dvg_devices.Bronkhorst_MFC_protocol_RS232 import Bronkhorst_MFC
-from dvg_devices.Bronkhorst_MFC_qdev import Bronkhorst_MFC_qdev
+import qtpy
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+import pyvisa
+
+import dvg_pyqt_controls as controls
+from dvg_debug_functions import ANSI, dprint
+from dvg_qdeviceio import DAQ_TRIGGER
+from dvg_devices.Keysight_N8700_protocol_SCPI import Keysight_N8700
+from dvg_devices.Keysight_N8700_qdev import Keysight_N8700_qdev
 
+# Show debug info in terminal? Warning: Slow! Do not leave on unintentionally.
+DEBUG = False
 
 # ------------------------------------------------------------------------------
 #   MainWindow
 # ------------------------------------------------------------------------------
 
 
 class MainWindow(QtWid.QWidget):
-    def __init__(self, parent=None, **kwargs):
+    def __init__(
+        self,
+        qdevs: List[Keysight_N8700_qdev],
+        parent=None,
+        **kwargs,
+    ):
         super().__init__(parent, **kwargs)
 
+        self.setWindowTitle("Keysight N8700 power supply control")
         self.setGeometry(40, 60, 0, 0)
-        self.setWindowTitle("Bronkhorst mass flow controller")
+        self.setStyleSheet(
+            controls.SS_TEXTBOX_READ_ONLY
+            + controls.SS_GROUP
+            + controls.SS_HOVER
+        )
 
         # Top grid
-        self.qlbl_title = QtWid.QLabel(
-            "Bronkhorst MFC",
-            font=QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold),
+        self.lbl_title = QtWid.QLabel("Keysight N8700 power supply control")
+        self.lbl_title.setFont(
+            QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold)
         )
-        self.qpbt_exit = QtWid.QPushButton("Exit")
-        self.qpbt_exit.clicked.connect(self.close)
-        self.qpbt_exit.setMinimumHeight(30)
+        self.pbtn_exit = QtWid.QPushButton("Exit")
+        self.pbtn_exit.clicked.connect(self.close)
+        self.pbtn_exit.setMinimumHeight(30)
 
         grid_top = QtWid.QGridLayout()
-        grid_top.addWidget(self.qlbl_title, 0, 0)
+        grid_top.addWidget(self.lbl_title, 0, 0)
         grid_top.addWidget(
-            self.qpbt_exit, 0, 1, QtCore.Qt.AlignmentFlag.AlignRight
+            self.pbtn_exit, 0, 1, QtCore.Qt.AlignmentFlag.AlignRight
         )
 
+        # PSU groups
+        hbox1 = QtWid.QHBoxLayout()
+        for qdev in qdevs:
+            hbox1.addWidget(qdev.grpb)
+        hbox1.addStretch(1)
+
         # Round up full window
         vbox = QtWid.QVBoxLayout(self)
         vbox.addLayout(grid_top)
-        vbox.addWidget(mfc_qdev.qgrp)
+        vbox.addLayout(hbox1)
         vbox.addStretch(1)
-        vbox.setAlignment(mfc_qdev.qgrp, QtCore.Qt.AlignmentFlag.AlignLeft)
-        mfc_qdev.qgrp.setTitle("")
-
-
-# ------------------------------------------------------------------------------
-#   about_to_quit
-# ------------------------------------------------------------------------------
-
-
-def about_to_quit():
-    print("About to quit")
-    app.processEvents()
-    mfc_qdev.quit()
-    mfc.close()
 
 
 # ------------------------------------------------------------------------------
 #   Main
 # ------------------------------------------------------------------------------
 
 if __name__ == "__main__":
-    # Config file containing COM port address
-    PATH_CONFIG = "config/port_Bronkhorst_MFC_1.txt"
-
-    # Serial number of Bronkhorst mass flow controller to connect to.
-    # SERIAL_MFC = "M16216843A"
-    SERIAL_MFC = None
+    # VISA addresses of the Keysight PSUs
+    VISA_ADDRESS_PSU_1 = "USB0::0x0957::0x8707::US15M3727P::INSTR"
+    VISA_ADDRESS_PSU_2 = "USB0::0x0957::0x8707::US15M3728P::INSTR"
+    VISA_ADDRESS_PSU_3 = "USB0::0x0957::0x8707::US15M3726P::INSTR"
+
+    # Config files
+    PATH_CONFIG_PSU_1 = Path(
+        os.getcwd() + "/config/settings_Keysight_PSU_1.txt"
+    )
+    PATH_CONFIG_PSU_2 = Path(
+        os.getcwd() + "/config/settings_Keysight_PSU_2.txt"
+    )
+    PATH_CONFIG_PSU_3 = Path(
+        os.getcwd() + "/config/settings_Keysight_PSU_3.txt"
+    )
 
-    # The state of the MFC is polled with this time interval
-    DAQ_INTERVAL_MS = 200  # [ms]
+    # The state of the PSUs is polled with this time interval
+    UPDATE_INTERVAL_MS = 1000  # [ms]
 
     # --------------------------------------------------------------------------
-    #   Connect to Bronkhorst mass flow controller (MFC)
+    #   Connect to and set up Keysight power supplies (PSU)
     # --------------------------------------------------------------------------
 
-    mfc = Bronkhorst_MFC(connect_to_serial_number=SERIAL_MFC)
-    if mfc.auto_connect(filepath_last_known_port=PATH_CONFIG):
-        mfc.begin()
+    rm = pyvisa.ResourceManager()
+
+    psu1 = Keysight_N8700(VISA_ADDRESS_PSU_1, PATH_CONFIG_PSU_1, "PSU 1")
+    psu2 = Keysight_N8700(VISA_ADDRESS_PSU_2, PATH_CONFIG_PSU_2, "PSU 2")
+    psu3 = Keysight_N8700(VISA_ADDRESS_PSU_3, PATH_CONFIG_PSU_3, "PSU 3")
+    psus = [psu1, psu2, psu3]
+
+    for psu in psus:
+        if psu.connect(rm):
+            psu.read_config_file()
+            psu.begin()
 
     # --------------------------------------------------------------------------
     #   Create application
     # --------------------------------------------------------------------------
-    QtCore.QThread.currentThread().setObjectName("MAIN")  # For DEBUG info
 
-    app = 0  # Work-around for kernel crash when using Spyder IDE
+    main_thread = QtCore.QThread.currentThread()
+    if isinstance(main_thread, QtCore.QThread):
+        main_thread.setObjectName("MAIN")  # For DEBUG info
+
+    if qtpy.PYQT6 or qtpy.PYSIDE6:
+        sys.argv += ["-platform", "windows:darkmode=0"]
     app = QtWid.QApplication(sys.argv)
-    app.setFont(QtGui.QFont("Arial", 9))
-    app.aboutToQuit.connect(about_to_quit)
+    app.setStyle("Fusion")
 
     # --------------------------------------------------------------------------
-    #   Set up communication threads for the MFC
+    #   Set up communication threads for the PSUs
     # --------------------------------------------------------------------------
 
-    mfc_qdev = Bronkhorst_MFC_qdev(dev=mfc, DAQ_interval_ms=DAQ_INTERVAL_MS)
-    mfc_qdev.start()
+    psu_qdevs: List[Keysight_N8700_qdev] = []
+    for psu in psus:
+        psu_qdevs.append(
+            Keysight_N8700_qdev(
+                dev=psu,
+                DAQ_trigger=DAQ_TRIGGER.SINGLE_SHOT_WAKE_UP,
+                debug=DEBUG,
+            )
+        )
+
+    # DEBUG information
+    psu_qdevs[0].worker_DAQ.debug_color = ANSI.YELLOW  # type: ignore
+    psu_qdevs[0].worker_jobs.debug_color = ANSI.CYAN  # type: ignore
+    psu_qdevs[1].worker_DAQ.debug_color = ANSI.GREEN  # type: ignore
+    psu_qdevs[1].worker_jobs.debug_color = ANSI.RED  # type: ignore
+
+    for psu_qdev in psu_qdevs:
+        psu_qdev.start()
+
+    # --------------------------------------------------------------------------
+    #   Set up PSU update timer
+    # --------------------------------------------------------------------------
+
+    def trigger_update_psus():
+        if DEBUG:
+            dprint("timer_psus: wake up all DAQ")
+
+        for psu_qdev_ in psu_qdevs:
+            if psu_qdev_.worker_DAQ is not None:
+                psu_qdev_.worker_DAQ.wake_up()
+
+    timer_psus = QtCore.QTimer()
+    timer_psus.timeout.connect(trigger_update_psus)
+    timer_psus.start(UPDATE_INTERVAL_MS)
 
     # --------------------------------------------------------------------------
     #   Start the main GUI event loop
     # --------------------------------------------------------------------------
 
-    window = MainWindow()
+    def about_to_quit():
+        print("About to quit")
+        app.processEvents()
+        for psu_qdev_ in psu_qdevs:
+            psu_qdev_.quit()
+        for psu_ in psus:
+            try:
+                psu_.close()
+            except:
+                pass
+        try:
+            rm.close()
+        except:
+            pass
+
+    app.aboutToQuit.connect(about_to_quit)
+    window = MainWindow(qdevs=psu_qdevs)
     window.show()
-    if QT_LIB in (PYQT5, PYSIDE2):
-        sys.exit(app.exec_())
-    else:
-        sys.exit(app.exec())
+
+    sys.exit(app.exec())
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Bronkhorst_MFC_protocol_RS232.py` & `dvg-devices-1.4.0/src/dvg_devices/Bronkhorst_MFC_protocol_RS232.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,35 @@
 MFC is assumed per port.
 
 When this module is directly run from the terminal a demo will be shown.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except, broad-except, try-except-raise
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring
 
 import sys
 import struct
-from typing import Tuple
+from typing import Union, Tuple
+
+import numpy as np
 
 from dvg_devices.BaseDevice import SerialDevice
 
 
 class Bronkhorst_MFC(SerialDevice):
     class State:
-        # Container for the process and measurement variables
-        setpoint = None  # Setpoint read out of the MFC   [ln/min]
-        flow_rate = None  # Flow rate measured by the MFC [ln/min]
+        """Container for the process and measurement variables"""
+
+        setpoint: float = np.nan
+        """Setpoint read out of the MFC  [ln/min]"""
+        flow_rate: float = np.nan
+        """Flow rate measured by the MFC [ln/min]"""
 
     def __init__(
         self,
         name="MFC",
         long_name="Bronkhorst MFC",
         connect_to_serial_number=None,
     ):
@@ -51,29 +56,33 @@
             valid_ID_broad="8002716300",
             valid_ID_specific=connect_to_serial_number,
         )
 
         # Container for the process and measurement variables
         self.state = self.State()
 
-        self.serial_str = None  # Serial number of the MFC
-        self.model_str = None  # Model of the MFC
-        self.fluid_name = None  # Fluid for which the MFC is calibrated
-        self.max_flow_rate = None  # Max. capacity [ln/min]
+        # fmt: off
+        self.serial_str: str = ""  # Serial number of the MFC
+        self.model_str : str = ""  # Model of the MFC
+        self.fluid_name: str = ""  # Fluid for which the MFC is calibrated
+        self.max_flow_rate: float = np.nan  # Max. capacity [ln/min]
+        # fmt: on
 
     # --------------------------------------------------------------------------
     #   ID_validation_query
     # --------------------------------------------------------------------------
 
-    def ID_validation_query(self) -> Tuple[str, str]:
+    def ID_validation_query(self) -> Tuple[str, Union[str, None]]:
         _success, reply = self.query(":0780047163716300")
-        broad_reply = reply[3:13]  # Expected: "8002716300"
-        specific_reply = bytearray.fromhex(
-            reply[13:-2]
-        ).decode()  # Serial number
+        if isinstance(reply, str):
+            broad_reply = reply[3:13]  # Expected: "8002716300"
+            specific_reply = bytearray.fromhex(reply[13:-2]).decode()  # Serial
+        else:
+            broad_reply = ""
+            specific_reply = None
 
         return broad_reply, specific_reply
 
     # --------------------------------------------------------------------------
     #   begin
     # --------------------------------------------------------------------------
 
@@ -101,148 +110,144 @@
     # --------------------------------------------------------------------------
 
     def query_serial_str(self) -> bool:
         """Query the serial number and store it in the class member 'serial_str'
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query(":0780047163716300")
-        if success and reply[3:13] == "8002716300":
+        _success, reply = self.query(":0780047163716300")
+        if isinstance(reply, str) and reply[3:13] == "8002716300":
             self.serial_str = bytearray.fromhex(reply[13:-2]).decode()
             return True
 
-        self.serial_str = None
+        self.serial_str = ""
         return False
 
     # --------------------------------------------------------------------------
     #   query_model_str
     # --------------------------------------------------------------------------
 
     def query_model_str(self) -> bool:
-        """Query the model name of the MFC and store it in the class member 'state'.
+        """Query the model name of the MFC and store it in the class member
+        'state'.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query(":0780047162716200")
-        if success:
+        _success, reply = self.query(":0780047162716200")
+        if isinstance(reply, str):
             self.model_str = bytearray.fromhex(reply[13:-2]).decode()
             return True
 
-        self.model_str = None
+        self.model_str = ""
         return False
 
     # --------------------------------------------------------------------------
     #   query_fluid_name
     # --------------------------------------------------------------------------
 
     def query_fluid_name(self) -> bool:
         """Query the fluid name that the MFC is calibrated for and store it in
         the class member 'state'.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query(":078004017101710A")
-        if success:
+        _success, reply = self.query(":078004017101710A")
+        if isinstance(reply, str):
             self.fluid_name = bytearray.fromhex(reply[13:-2]).decode()
             return True
 
-        self.fluid_name = None
+        self.fluid_name = ""
         return False
 
     # --------------------------------------------------------------------------
     #   query_max_flow_rate
     # --------------------------------------------------------------------------
 
     def query_max_flow_rate(self) -> bool:
         """Query the maximum mass flow rate in [ln/min] of the MFC and store it
         in the class member 'state'. This value is mandatory to be known, because it is
         used to set and read the setpoint, and to read the flow rate.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query(":068004014D014D")
-        if success:
+        _success, reply = self.query(":068004014D014D")
+        if isinstance(reply, str):
             self.max_flow_rate = hex_to_32bit_IEEE754_float(reply[11:])
             return True
 
-        self.max_flow_rate = None
+        self.max_flow_rate = np.nan
         return False
 
     # --------------------------------------------------------------------------
     #   query_setpoint
     # --------------------------------------------------------------------------
 
     def query_setpoint(self) -> bool:
         """Query the mass flow rate setpoint in [ln/min] set at the MFC and
         store it in the class member 'state' 'state'. Will be set to None if
         unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query(":06800401210121")
-        if success:
+        _success, reply = self.query(":06800401210121")
+        if isinstance(reply, str):
             try:
                 num = int(reply[-4:], 16)
             except ValueError:
                 pass
             else:
                 self.state.setpoint = num / 32000.0 * self.max_flow_rate
                 return True
 
-        self.state.setpoint = None
+        self.state.setpoint = np.nan
         return False
 
     # --------------------------------------------------------------------------
     #   query_flow_rate
     # --------------------------------------------------------------------------
 
     def query_flow_rate(self) -> bool:
         """Query the mass flow rate in [ln/min] measured by the MFC and
         store it in the class member 'state'. Will be set to None if
         unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query(":06800401210120")
-        if success:
+        _success, reply = self.query(":06800401210120")
+        if isinstance(reply, str):
             try:
                 num = int(reply[-4:], 16)
             except ValueError:
                 pass
             else:
                 self.state.flow_rate = num / 32000.0 * self.max_flow_rate
                 return True
 
-        self.state.flow_rate = None
+        self.state.flow_rate = np.nan
         return False
 
     # --------------------------------------------------------------------------
     #   send_setpoint
     # --------------------------------------------------------------------------
 
-    def send_setpoint(self, setpoint) -> bool:
+    def send_setpoint(self, setpoint: float) -> bool:
         """Send a new mass flow rate setpoint in [ln/min] to the MFC.
 
         Args:
             setpoint (float): mass flow rate in [ln/min].
 
         Returns: True if successful, False otherwise.
         """
-        try:
-            setpoint = float(setpoint)
-        except (TypeError, ValueError):
-            setpoint = 0.0
-
         # Transform setpoint and limit
         setpoint = int(setpoint / self.max_flow_rate * 32000)
         setpoint = max(0, min(setpoint, 32000))
 
-        success, reply = self.query(":0680010121%04x" % setpoint)
-        if success and reply[5:].strip() == "000005":  # Also check status reply
-            return True
+        _success, reply = self.query(f":0680010121{setpoint:04x}")
+        if isinstance(reply, str) and reply[5:].strip() == "000005":
+            return True  # Also checked status reply
 
         return False
 
 
 # ------------------------------------------------------------------------------
 #   hex_to_32bit_IEEE754_float
 # ------------------------------------------------------------------------------
@@ -271,18 +276,18 @@
     # SERIAL_MFC = "M16216843A"
     SERIAL_MFC = None
 
     # Create connection to Bronkhorst MFC over RS232
     mfc = Bronkhorst_MFC(connect_to_serial_number=SERIAL_MFC)
     if mfc.auto_connect(filepath_last_known_port=PATH_CONFIG):
         mfc.begin()  # Retrieve necessary parameters
-        print("  Serial  : %s" % mfc.serial_str)
-        print("  Model   : %s" % mfc.model_str)
-        print("  Fluid   : %s" % mfc.fluid_name)
-        print("  Capacity: %.2f ln/min" % mfc.max_flow_rate)
+        print(f"  Serial  : {mfc.serial_str}")
+        print(f"  Model   : {mfc.model_str}")
+        print(f"  Fluid   : {mfc.fluid_name}")
+        print(f"  Capacity: {mfc.max_flow_rate:.2f} ln/min")
     else:
         time.sleep(1)
         sys.exit(0)
 
     if os.name == "nt":
         import msvcrt
 
@@ -295,44 +300,49 @@
         print("No other keyboard input possible because OS is not Windows.")
 
     # Prepare
     send_setpoint = 0.0
     do_send_setpoint = False
 
     mfc.query_setpoint()
-    print("\nSetpoint       : %6.2f ln/min" % mfc.state.setpoint)
+    print(f"\nSetpoint       : {mfc.state.setpoint:6.2f} ln/min")
 
     # Loop
     done = False
     while not done:
         # Check if a new setpoint has to be send
         if do_send_setpoint:
             mfc.send_setpoint(send_setpoint)
             mfc.query_setpoint()
-            print("\nSetpoint       : %6.2f ln/min" % mfc.state.setpoint)
+            print(f"\nSetpoint       : {mfc.state.setpoint:6.2f} ln/min")
             do_send_setpoint = False
 
         # Measure and report the flow rate
         mfc.query_flow_rate()
-        print("\rMeas. flow rate: %6.2f ln/min" % mfc.state.flow_rate, end="")
+        print(f"\rMeas. flow rate: {mfc.state.flow_rate:6.2f} ln/min", end="")
         sys.stdout.flush()
 
         # Process keyboard input
         if running_Windows:
             if msvcrt.kbhit():
                 key = msvcrt.getch()
                 if key == b"q":
                     print("\nAre you sure you want to quit [y/n]?")
                     if msvcrt.getch() == b"y":
                         print("Quitting.")
                         done = True
                     else:
                         do_send_setpoint = True  # Esthestics
                 elif key == b"s":
-                    send_setpoint = input("\nEnter new setpoint [ln/min]: ")
+                    input_str = input("\nEnter new setpoint [ln/min]: ")
+                    try:
+                        input_float = float(input_str)
+                    except ValueError:
+                        input_float = 0.0
+                    send_setpoint = input_float
                     do_send_setpoint = True
 
         # Slow down update period
         time.sleep(0.02)
 
     mfc.close()
     time.sleep(1)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Bronkhorst_MFC_qdev.py` & `dvg-devices-1.4.0/src/dvg_devices/Julabo_circulator_qdev.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,316 +1,316 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """PyQt/PySide module to provide multithreaded communication and periodical data
-acquisition for a Bronkhorst mass flow controller (MFC).
+acquisition for a Julabo circulating bath.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=broad-except, missing-function-docstring, multiple-statements
 
-import os
-import sys
+from qtpy import QtCore, QtWidgets as QtWid
+from qtpy.QtCore import Signal, Slot  # type: ignore
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt5.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt6.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-    from PySide2.QtCore import Signal                      # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-    from PySide6.QtCore import Signal                      # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
-from dvg_pyqt_controls import SS_GROUP, SS_TEXTBOX_READ_ONLY
+import dvg_pyqt_controls as controls
 from dvg_debug_functions import print_fancy_traceback as pft
-
 from dvg_qdeviceio import QDeviceIO, DAQ_TRIGGER
-from dvg_devices.Bronkhorst_MFC_protocol_RS232 import Bronkhorst_MFC
+from dvg_devices.Julabo_circulator_protocol_RS232 import Julabo_circulator
+
 
+# Enumeration
+class GUI_input_fields:
+    [ALL, setpoint, sub_temp, over_temp] = range(4)
 
-class Bronkhorst_MFC_qdev(QDeviceIO):
-    """Manages multithreaded communication and data acquisition for a
-    Bronkhorst mass flow controller (MFC), referred to as the 'device'.
+
+class Julabo_circulator_qdev(QDeviceIO):
+    """Manages multithreaded communication and periodical data acquisition for
+    a Julabo circulator, referred to as the 'device'.
 
     In addition, it also provides PyQt/PySide GUI objects for control of the
     device. These can be incorporated into your application.
 
-    Extra functionality is provided to allow for automatic closing and opening
-    of a peripheral valve that could be in line with the mass flow controller.
-    This can be used to e.g. prevent liquid from entering the mass flow
-    controller from the upstream side when the flow rate has dropped to 0 for
-    some reason. Signals 'signal_valve_auto_close' and 'signal_valve_auto_open'
-    are emitted from within this class and the user can connect to these to
-    automate opening and closing of such a valve. There is a deadtime where the
-    auto close signal will not be emitted after a setpoint > 0 has been send,
-    because time might have to be given to the mass flow controller to get the
-    flow going.
-
     All device I/O operations will be offloaded to 'workers', each running in
     a newly created thread.
 
     (*): See 'dvg_qdeviceio.QDeviceIO()' for details.
 
     Args:
         dev:
             Reference to a
-            'dvg_devices.Bronkhorst_MFC_protocol_RS232.Bronkhorst_MFC'
+            'dvg_devices.Julabo_circulator_protocol_RS232.Julabo_circulator'
             instance.
 
-        valve_auto_close_deadtime_period_ms (optional, default=3000):
-            Deadtime period in milliseconds of the auto close signal after a
-            setpoint > 0 has been send.
-
         debug:
             Show debug info in terminal? Warning: Slow! Do not leave on
             unintentionally.
 
     Main GUI objects:
         qgrp (PyQt5.QtWidgets.QGroupBox)
-
-    Signals:
-        signal_valve_auto_close()
-        signal_valve_auto_open()
     """
 
-    signal_valve_auto_close = Signal()
-    signal_valve_auto_open = Signal()
+    signal_GUI_input_field_update = Signal(int)
 
     def __init__(
         self,
-        dev: Bronkhorst_MFC,
-        DAQ_interval_ms=200,
+        dev: Julabo_circulator,
+        DAQ_trigger=DAQ_TRIGGER.INTERNAL_TIMER,
+        DAQ_interval_ms=500,
         DAQ_timer_type=QtCore.Qt.TimerType.CoarseTimer,
-        critical_not_alive_count=1,
-        valve_auto_close_deadtime_period_ms=3000,
+        critical_not_alive_count=3,
         debug=False,
         **kwargs,
     ):
         super().__init__(dev, **kwargs)  # Pass kwargs onto QtCore.QObject()
+        self.dev: Julabo_circulator  # Enforce type: removes `_NoDevice()`
 
         self.create_worker_DAQ(
-            DAQ_trigger=DAQ_TRIGGER.INTERNAL_TIMER,
-            DAQ_function=self._DAQ_function,
+            DAQ_trigger=DAQ_trigger,
+            DAQ_function=self.DAQ_function,
             DAQ_interval_ms=DAQ_interval_ms,
             DAQ_timer_type=DAQ_timer_type,
             critical_not_alive_count=critical_not_alive_count,
             debug=debug,
         )
+        self.create_worker_jobs(jobs_function=self.jobs_function, debug=debug)
 
-        self.create_worker_jobs(jobs_function=self._jobs_function, debug=debug)
+        self.create_GUI()
+        self.signal_DAQ_updated.connect(self.update_GUI)
+        self.signal_connection_lost.connect(self.update_GUI)
+        self.signal_GUI_input_field_update.connect(self.update_GUI_input_field)
 
-        self._create_GUI()
-        self.signal_DAQ_updated.connect(self._update_GUI)
-        if not self.dev.is_alive:
-            self._update_GUI()  # Correctly reflect an offline device
-
-        # Auto open or close of an optional peripheral valve
-        self.dev.state.prev_flow_rate = self.dev.state.flow_rate
-        self.dev.valve_auto_close_briefly_prevent = False
-        self.dev.valve_auto_close_deadtime_period_ms = (
-            valve_auto_close_deadtime_period_ms
-        )
-        self.dev.valve_auto_close_start_deadtime = 0
+        self.safe_temp.setText(f"{self.dev.state.safe_temp:.2f}")
+
+        self.update_GUI()
+        self.update_GUI_input_field()
 
     # --------------------------------------------------------------------------
-    #   _DAQ_function
+    #   DAQ_function
     # --------------------------------------------------------------------------
 
-    def _DAQ_function(self) -> bool:
-        success = self.dev.query_setpoint()
-        success &= self.dev.query_flow_rate()
-
-        if success:
-            # Check to signal auto open or close of an optional peripheral valve
-            if (
-                self.dev.state.flow_rate == 0
-                and not self.dev.state.prev_flow_rate
-                == self.dev.state.flow_rate
-            ):
-                # The flow rate has just dropped to 0
-                if (
-                    self.dev.valve_auto_close_briefly_prevent
-                    and self.dev.valve_auto_close_start_deadtime.msecsTo(
-                        QtCore.QDateTime.currentDateTime()
-                    )
-                    < self.dev.valve_auto_close_deadtime_period_ms
-                ):
-                    # We are still in deadtime
-                    pass
-                else:
-                    # Signal auto close and force setpoint = 0
-                    self.signal_valve_auto_close.emit()
-                    self.dev.send_setpoint(0)
-                    self.dev.valve_auto_close_briefly_prevent = False
-                    self.dev.state.prev_flow_rate = self.dev.state.flow_rate
-            else:
-                self.dev.state.prev_flow_rate = self.dev.state.flow_rate
-
-        return success
+    def DAQ_function(self) -> bool:
+        return self.dev.query_common_readings()
 
     # --------------------------------------------------------------------------
-    #   _jobs_function
+    #   jobs_function
     # --------------------------------------------------------------------------
 
-    def _jobs_function(self, func, args):
-        # Send I/O operation to the device
-        try:
-            func(*args)
-        except Exception as err:  # pylint: disable=broad-except
-            pft(err)
-
-        # Check to signal auto open or close of an optional peripheral valve
-        if func == self.dev.send_setpoint:
-            if args[0] == 0:
-                # Setpoint was set to 0 --> signal auto close
-                self.dev.valve_auto_close_briefly_prevent = False
-                self.signal_valve_auto_close.emit()
-            else:
-                # Flow enabled --> start deadtime on auto close
-                #              --> signal auto open
-                self.dev.valve_auto_close_briefly_prevent = True
-                self.dev.valve_auto_close_start_deadtime = (
-                    QtCore.QDateTime.currentDateTime()
-                )
-                self.dev.state.prev_flow_rate = -1  # Necessary reset
-                self.signal_valve_auto_open.emit()
-
-    # --------------------------------------------------------------------------
-    #   _create_GUI
-    # --------------------------------------------------------------------------
-
-    def _create_GUI(self):
-        self.qlbl_offline = QtWid.QLabel(
-            "MFC OFFLINE",
-            visible=False,
-            font=QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold),
-            alignment=QtCore.Qt.AlignmentFlag.AlignCenter,
-        )
+    def jobs_function(self, func, args):
+        if func == "signal_GUI_input_field_update":
+            # Special instruction
+            self.signal_GUI_input_field_update.emit(*args)
+        else:
+            # Default job processing:
+            # Send I/O operation to the device
+            try:
+                func(*args)
+            except Exception as err:
+                pft(err)
 
+    # --------------------------------------------------------------------------
+    #   create GUI
+    # --------------------------------------------------------------------------
+
+    def create_GUI(self):
+        # Safety
         p = {
             "alignment": QtCore.Qt.AlignmentFlag.AlignRight,
-            "minimumWidth": 50,
+            "minimumWidth": 60,
             "maximumWidth": 30,
-            "styleSheet": SS_TEXTBOX_READ_ONLY,
         }
-        # fmt: off
-        self.qled_send_setpoint  = QtWid.QLineEdit(**p)
-        self.qled_read_setpoint  = QtWid.QLineEdit(**p, readOnly=True)
-        self.qled_flow_rate      = QtWid.QLineEdit(**p, readOnly=True)
-        self.qlbl_update_counter = QtWid.QLabel("0")
-        # fmt: on
-
-        self.qled_send_setpoint.editingFinished.connect(
-            self._send_setpoint_from_textbox
+        p2 = {**p, "readOnly": True}
+        self.safe_sens = QtWid.QLineEdit("nan", **p2)
+        self.safe_temp = QtWid.QLineEdit("nan", **p2)
+        self.sub_temp = QtWid.QLineEdit("nan", **p)
+        self.sub_temp.editingFinished.connect(self.send_sub_temp_from_textbox)
+        self.over_temp = QtWid.QLineEdit("nan", **p)
+        self.over_temp.editingFinished.connect(self.send_over_temp_from_textbox)
+
+        # Control
+        self.pbtn_running = controls.create_Toggle_button("OFFLINE")
+        self.pbtn_running.clicked.connect(self.process_pbtn_running)
+        self.send_setpoint = QtWid.QLineEdit("nan", **p)
+        self.send_setpoint.editingFinished.connect(
+            self.send_setpoint_from_textbox
         )
+        self.read_setpoint = QtWid.QLineEdit("nan", **p2)
+        self.bath_temp = QtWid.QLineEdit("nan", **p2)
+        self.pt100_temp = QtWid.QLineEdit("nan", **p2)
+        self.status = QtWid.QPlainTextEdit()
+        self.status.setReadOnly(True)
+        self.status.setMaximumWidth(180)
+        self.status.setStyleSheet(controls.SS_TEXTBOX_ERRORS)
+        self.update_counter = QtWid.QLabel("0")
+
+        i = 0
+        p = {"alignment": QtCore.Qt.AlignmentFlag.AlignLeft}
+        lbl_temp_unit = f"\u00b0{self.dev.state.temp_unit}"
 
         # fmt: off
-        self.grid = QtWid.QGridLayout()
-        self.grid.setVerticalSpacing(4)
-        self.grid.addWidget(self.qlbl_offline             , 0, 0, 1, 3)
-        self.grid.addWidget(QtWid.QLabel("Send setpoint") , 1, 0)
-        self.grid.addWidget(self.qled_send_setpoint       , 1, 1)
-        self.grid.addWidget(QtWid.QLabel("ln/min")        , 1, 2)
-        self.grid.addWidget(QtWid.QLabel("Read setpoint") , 2, 0)
-        self.grid.addWidget(self.qled_read_setpoint       , 2, 1)
-        self.grid.addWidget(QtWid.QLabel("ln/min")        , 2, 2)
-        self.grid.addItem(QtWid.QSpacerItem(1, 12)        , 3, 0)
-        self.grid.addWidget(QtWid.QLabel("Read flow rate"), 4, 0)
-        self.grid.addWidget(self.qled_flow_rate           , 4, 1)
-        self.grid.addWidget(QtWid.QLabel("ln/min")        , 4, 2)
-        self.grid.addWidget(self.qlbl_update_counter      , 5, 0, 1, 3)
+        grid = QtWid.QGridLayout()
+        grid.setVerticalSpacing(4)
+
+        grid.addWidget(QtWid.QLabel("<b>Safety</b>")        , i, 0, 1, 3); i+=1
+        grid.addItem(QtWid.QSpacerItem(1, 6)                , i, 0)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Safe sensor")          , i, 0)
+        grid.addWidget(self.safe_sens                       , i, 1)
+        grid.addWidget(QtWid.QLabel(lbl_temp_unit)          , i, 2)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Safe temp.")           , i, 0)
+        grid.addWidget(self.safe_temp                       , i, 1)
+        grid.addWidget(QtWid.QLabel(lbl_temp_unit)          , i, 2)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Sub temp.")            , i, 0)
+        grid.addWidget(self.sub_temp                        , i, 1)
+        grid.addWidget(QtWid.QLabel(lbl_temp_unit)          , i, 2)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Over temp.")           , i, 0)
+        grid.addWidget(self.over_temp                       , i, 1)
+        grid.addWidget(QtWid.QLabel(lbl_temp_unit)          , i, 2)      ; i+=1
+
+        grid.addItem(QtWid.QSpacerItem(1, 10)               , i, 0)      ; i+=1
+        grid.addWidget(QtWid.QLabel("<b>Control</b>")       , i, 0, 1, 3); i+=1
+        grid.addItem(QtWid.QSpacerItem(1, 6)                , i, 0)      ; i+=1
+        grid.addWidget(self.pbtn_running                    , i, 0, 1, 3); i+=1
+        grid.addItem(QtWid.QSpacerItem(1, 8)                , i, 0)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Send setpoint")        , i, 0)
+        grid.addWidget(self.send_setpoint                   , i, 1)
+        grid.addWidget(QtWid.QLabel(lbl_temp_unit)          , i, 2)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Read setpoint")        , i, 0)
+        grid.addWidget(self.read_setpoint                   , i, 1)
+        grid.addWidget(QtWid.QLabel(lbl_temp_unit)          , i, 2)      ; i+=1
+        grid.addItem(QtWid.QSpacerItem(1, 8)                , i, 0)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Bath temp.")           , i, 0)
+        grid.addWidget(self.bath_temp                       , i, 1)
+        grid.addWidget(QtWid.QLabel(lbl_temp_unit)          , i, 2)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Pt100 temp.")          , i, 0)
+        grid.addWidget(self.pt100_temp                      , i, 1)
+        grid.addWidget(QtWid.QLabel(lbl_temp_unit)          , i, 2)      ; i+=1
+        grid.addItem(QtWid.QSpacerItem(1, 8)                , i, 0)      ; i+=1
+        grid.addWidget(QtWid.QLabel("Status")               , i, 0, 1, 3); i+=1
+        grid.addWidget(self.status                          , i, 0, 1, 3); i+=1
+        grid.addItem(QtWid.QSpacerItem(1, 4)                , i, 0)      ; i+=1
+        grid.addWidget(self.update_counter                  , i, 0, 1, 3); i+=1
         # fmt: on
 
-        self.qgrp = QtWid.QGroupBox("%s" % self.dev.name)
-        self.qgrp.setStyleSheet(SS_GROUP)
-        self.qgrp.setLayout(self.grid)
+        grid.setColumnStretch(0, 0)
+        grid.setColumnStretch(1, 0)
+        grid.setColumnStretch(2, 1)
+        grid.setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
+        self.grid = grid
+
+        self.grpb = QtWid.QGroupBox(self.dev.name)
+        self.grpb.setLayout(self.grid)
 
     # --------------------------------------------------------------------------
-    #   _update_GUI
+    #   update_GUI
     # --------------------------------------------------------------------------
 
     @Slot()
-    def _update_GUI(self):
+    def update_GUI(self):
         """NOTE: 'self.dev.mutex' is not being locked, because we are only
         reading 'state' for displaying purposes. We can do this because 'state'
         members are written and read atomicly.
-        Not locking the mutex might speed up the program.
         """
         if self.dev.is_alive:
-            # At startup
-            if self.update_counter_DAQ == 1:
-                self.qled_send_setpoint.setText(
-                    "%.2f" % self.dev.state.setpoint
-                )
-            self.qled_flow_rate.setText("%.2f" % self.dev.state.flow_rate)
-            self.qled_read_setpoint.setText("%.2f" % self.dev.state.setpoint)
-            self.qlbl_update_counter.setText("%s" % self.update_counter_DAQ)
+            self.pbtn_running.setChecked(bool(self.dev.state.running))
+            if self.dev.state.running:
+                self.pbtn_running.setText("RUNNING")
+            else:
+                self.pbtn_running.setText("OFF")
+
+            self.safe_sens.setText(f"{self.dev.state.safe_sens:.2f}")
+            self.read_setpoint.setText(f"{self.dev.state.setpoint:.2f}")
+            self.bath_temp.setText(f"{self.dev.state.bath_temp:.2f}")
+            self.pt100_temp.setText(f"{self.dev.state.pt100_temp:.2f}")
+
+            # Check status
+            self.status.setReadOnly(bool(self.dev.state.has_error))
+            self.status.setStyleSheet(controls.SS_TEXTBOX_ERRORS)
+            self.status.setPlainText(f"{self.dev.state.status}")
+
+            self.update_counter.setText(f"{self.update_counter_DAQ}")
         else:
-            self.qgrp.setEnabled(False)
-            self.qlbl_offline.setVisible(True)
+            self.pbtn_running.setText("OFFLINE")
+            self.grpb.setEnabled(False)
+
+    # --------------------------------------------------------------------------
+    #   update_GUI_input_field
+    # --------------------------------------------------------------------------
+
+    @Slot()
+    @Slot(int)
+    def update_GUI_input_field(self, GUI_input_field=GUI_input_fields.ALL):
+        if GUI_input_field == GUI_input_fields.setpoint:
+            self.send_setpoint.setText(f"{self.dev.state.setpoint:.2f}")
+
+        elif GUI_input_field == GUI_input_fields.sub_temp:
+            self.sub_temp.setText(f"{self.dev.state.sub_temp:.2f}")
+
+        elif GUI_input_field == GUI_input_fields.over_temp:
+            self.over_temp.setText(f"{self.dev.state.over_temp:.2f}")
+
+        else:
+            self.send_setpoint.setText(f"{self.dev.state.setpoint:.2f}")
+            self.sub_temp.setText(f"{self.dev.state.sub_temp:.2f}")
+            self.over_temp.setText(f"{self.dev.state.over_temp:.2f}")
 
     # --------------------------------------------------------------------------
     #   GUI functions
     # --------------------------------------------------------------------------
 
     @Slot()
-    def _send_setpoint_from_textbox(self):
+    def process_pbtn_running(self):
+        if self.dev.state.running:
+            self.send(self.dev.turn_off)
+        else:
+            self.send(self.dev.turn_on)
+
+        # React as fast as possible by manually triggering processEvents()
+        QtWid.QApplication.processEvents()
+
+    @Slot()
+    def send_setpoint_from_textbox(self):
         try:
-            setpoint = float(self.qled_send_setpoint.text())
+            value = float(self.send_setpoint.text())
         except (TypeError, ValueError):
-            setpoint = 0.0
-        except:  # pylint: disable=try-except-raise
-            raise
-
-        setpoint = max(setpoint, 0)
-        setpoint = min(setpoint, self.dev.max_flow_rate)
-        self.qled_send_setpoint.setText("%.2f" % setpoint)
+            # Revert to previously set value
+            value = self.dev.state.setpoint
+        except Exception as e:
+            raise e
+
+        self.add_to_jobs_queue(self.dev.set_setpoint, value)
+        self.add_to_jobs_queue(
+            "signal_GUI_input_field_update", GUI_input_fields.setpoint
+        )
+        self.process_jobs_queue()
 
-        self.send(self.dev.send_setpoint, setpoint)
+    @Slot()
+    def send_sub_temp_from_textbox(self):
+        try:
+            value = float(self.sub_temp.text())
+        except (TypeError, ValueError):
+            # Revert to previously set value
+            value = self.dev.state.sub_temp
+        except Exception as e:
+            raise e
+
+        self.add_to_jobs_queue(self.dev.set_sub_temp, value)
+        self.add_to_jobs_queue(
+            "signal_GUI_input_field_update", GUI_input_fields.sub_temp
+        )
+        self.process_jobs_queue()
+
+    @Slot()
+    def send_over_temp_from_textbox(self):
+        try:
+            value = float(self.over_temp.text())
+        except (TypeError, ValueError):
+            # Revert to previously set value
+            value = self.dev.state.over_temp
+        except Exception as e:
+            raise e
+
+        self.add_to_jobs_queue(self.dev.set_over_temp, value)
+        self.add_to_jobs_queue(
+            "signal_GUI_input_field_update", GUI_input_fields.over_temp
+        )
+        self.process_jobs_queue()
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Compax3_servo_demo.py` & `dvg-devices-1.4.0/src/dvg_devices/Compax3_servo_demo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,63 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """Multithreaded PyQt/PySide GUI to interface with a Compax3 servo controller.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+print(__url__)
+# pylint: disable=wrong-import-position, missing-function-docstring
 
-import os
 import sys
 from pathlib import Path
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-# Parse optional cli argument to enfore a QT_LIB
-# cli example: python benchmark.py pyside6
-if len(sys.argv) > 1:
-    arg1 = str(sys.argv[1]).upper()
-    for i, lib in enumerate(QT_LIB_ORDER):
-        if arg1 == lib.upper():
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
-from dvg_pyqt_controls import SS_TEXTBOX_READ_ONLY, SS_GROUP
+import qtpy
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Slot  # type: ignore
 
+import dvg_pyqt_controls as controls
 from dvg_devices.Compax3_servo_protocol_RS232 import Compax3_servo
 from dvg_devices.Compax3_servo_qdev import Compax3_servo_qdev
 from dvg_devices.Compax3_servo_step_navigator_GUI import Compax3_step_navigator
 
+# Show debug info in terminal? Warning: Slow! Do not leave on unintentionally.
+DEBUG = False
+
 # ------------------------------------------------------------------------------
 #   MainWindow
 # ------------------------------------------------------------------------------
 
 
 class MainWindow(QtWid.QWidget):
-    def __init__(self, parent=None, **kwargs):
+    def __init__(
+        self,
+        qdev_horz: Compax3_servo_qdev,
+        qdev_vert: Compax3_servo_qdev,
+        step_nav: Compax3_step_navigator,
+        parent=None,
+        **kwargs,
+    ):
         super().__init__(parent, **kwargs)
 
-        self.setGeometry(40, 60, 0, 0)
         self.setWindowTitle("Compax3 traverse controller")
+        self.setGeometry(40, 60, 0, 0)
+        self.setFont(QtGui.QFont("Arial", 9))
+        self.setStyleSheet(
+            controls.SS_TEXTBOX_READ_ONLY
+            + controls.SS_GROUP
+            + controls.SS_HOVER
+        )
 
         # Top grid
-        self.lbl_title = QtWid.QLabel(
-            "Compax3 traverse controller",
-            font=QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold),
+        self.lbl_title = QtWid.QLabel("Compax3 traverse controller")
+        self.lbl_title.setFont(
+            QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold)
         )
         self.pbtn_exit = QtWid.QPushButton("Exit")
         self.pbtn_exit.clicked.connect(self.close)
         self.pbtn_exit.setMinimumHeight(30)
 
         grid_top = QtWid.QGridLayout()
         grid_top.addWidget(self.lbl_title, 0, 0)
@@ -107,103 +65,56 @@
             self.pbtn_exit, 0, 1, QtCore.Qt.AlignmentFlag.AlignRight
         )
 
         # Traverse schematic image
         lbl_trav_img = QtWid.QLabel()
         lbl_trav_img.setPixmap(
             QtGui.QPixmap(
-                str(Path(sys.modules[__name__].__file__).parent)
+                str(Path(sys.modules[__name__].__file__).parent)  # type: ignore
                 + "/Traverse_layout.png"
             )
         )
         lbl_trav_img.setFixedSize(244, 240)
 
         grid = QtWid.QGridLayout()
         grid.addWidget(lbl_trav_img, 0, 0, QtCore.Qt.AlignmentFlag.AlignTop)
 
         grpb_trav_img = QtWid.QGroupBox("Traverse schematic")
-        grpb_trav_img.setStyleSheet(SS_GROUP)
         grpb_trav_img.setLayout(grid)
 
         # Round up full window
         vbox = QtWid.QVBoxLayout()
         vbox.addWidget(grpb_trav_img)
-        vbox.addWidget(trav_step_nav.grpb)
+        vbox.addWidget(step_nav.grpb)
         vbox.addStretch(1)
-        vbox.setAlignment(trav_step_nav.grpb, QtCore.Qt.AlignmentFlag.AlignLeft)
+        vbox.setAlignment(step_nav.grpb, QtCore.Qt.AlignmentFlag.AlignLeft)
 
         hbox = QtWid.QHBoxLayout()
-        hbox.addWidget(trav_vert_qdev.qgrp)
-        hbox.addWidget(trav_horz_qdev.qgrp)
+        hbox.addWidget(qdev_vert.qgrp)
+        hbox.addWidget(qdev_horz.qgrp)
         hbox.addLayout(vbox)
         hbox.addStretch(1)
-        hbox.setAlignment(trav_horz_qdev.qgrp, QtCore.Qt.AlignmentFlag.AlignTop)
-        hbox.setAlignment(trav_vert_qdev.qgrp, QtCore.Qt.AlignmentFlag.AlignTop)
+        hbox.setAlignment(qdev_horz.qgrp, QtCore.Qt.AlignmentFlag.AlignTop)
+        hbox.setAlignment(qdev_vert.qgrp, QtCore.Qt.AlignmentFlag.AlignTop)
 
         vbox = QtWid.QVBoxLayout(self)
         vbox.addLayout(grid_top)
         vbox.addLayout(hbox)
 
 
 # ------------------------------------------------------------------------------
-#   Act on step signals
-# ------------------------------------------------------------------------------
-
-
-@Slot()
-def act_upon_signal_step_up(new_pos: float):
-    trav_vert_qdev.qled_new_pos.setText("%.2f" % new_pos)
-    trav_vert_qdev.process_pbtn_move_to_new_pos()
-
-
-@Slot()
-def act_upon_signal_step_down(new_pos: float):
-    trav_vert_qdev.qled_new_pos.setText("%.2f" % new_pos)
-    trav_vert_qdev.process_pbtn_move_to_new_pos()
-
-
-@Slot()
-def act_upon_signal_step_left(new_pos: float):
-    trav_horz_qdev.qled_new_pos.setText("%.2f" % new_pos)
-    trav_horz_qdev.process_pbtn_move_to_new_pos()
-
-
-@Slot()
-def act_upon_signal_step_right(new_pos: float):
-    trav_horz_qdev.qled_new_pos.setText("%.2f" % new_pos)
-    trav_horz_qdev.process_pbtn_move_to_new_pos()
-
-
-# ------------------------------------------------------------------------------
-#   about_to_quit
-# ------------------------------------------------------------------------------
-
-
-def about_to_quit():
-    print("About to quit")
-    app.processEvents()
-
-    for trav_qdev in travs_qdev:
-        trav_qdev.quit()
-
-    for trav in travs:
-        trav.close()
-
-
-# ------------------------------------------------------------------------------
 #   Main
 # ------------------------------------------------------------------------------
 
 if __name__ == "__main__":
-
     # Specific connection settings of each traverse axis of our setup
     class Trav_connection_params:
         # Serial number of the Compax3 traverse controller to connect to.
-        # Set to '' or None to connect to any Compax3.
-        serial = None
+        # Set to "" to connect to any Compax3.
+        serial = ""
         # Display name
         name = "TRAV"
         # Path to the config textfile containing the (last used) RS232 port
         path_config = "config/port_Compax3_trav.txt"
 
     # Horizontal axis
     trav_conn_horz = Trav_connection_params()
@@ -217,15 +128,15 @@
     trav_conn_vert.name = "TRAV VERT"
     trav_conn_vert.path_config = "config/port_Compax3_trav_vert.txt"
 
     # The state of the traverse controllers is polled with this time interval
     UPDATE_INTERVAL_MS = 250  # [ms]
 
     # --------------------------------------------------------------------------
-    #   Connect to and set up Compax3 traverse controllers
+    #   Connect to Compax3 traverse controllers
     # --------------------------------------------------------------------------
 
     trav_horz = Compax3_servo(
         name=trav_conn_horz.name,
         connect_to_serial_number=trav_conn_horz.serial,
     )
     trav_vert = Compax3_servo(
@@ -266,52 +177,88 @@
         )
 
     travs = [trav_horz, trav_vert]
 
     # --------------------------------------------------------------------------
     #   Create application
     # --------------------------------------------------------------------------
-    QtCore.QThread.currentThread().setObjectName("MAIN")  # For DEBUG info
 
-    app = 0  # Work-around for kernel crash when using Spyder IDE
+    main_thread = QtCore.QThread.currentThread()
+    if isinstance(main_thread, QtCore.QThread):
+        main_thread.setObjectName("MAIN")  # For DEBUG info
+
+    if qtpy.PYQT6 or qtpy.PYSIDE6:
+        sys.argv += ["-platform", "windows:darkmode=0"]
     app = QtWid.QApplication(sys.argv)
-    app.setFont(QtGui.QFont("Arial", 9))
-    app.setStyleSheet(SS_TEXTBOX_READ_ONLY)
-    app.aboutToQuit.connect(about_to_quit)
+    app.setStyle("Fusion")
+
+    # --------------------------------------------------------------------------
+    #   Set up communication threads for the Compax3 traverse controllers
+    # --------------------------------------------------------------------------
 
-    # Create PyQt GUI interfaces and communication threads for the device
     trav_horz_qdev = Compax3_servo_qdev(
-        dev=trav_horz, DAQ_interval_ms=UPDATE_INTERVAL_MS
+        dev=trav_horz,
+        DAQ_interval_ms=UPDATE_INTERVAL_MS,
+        debug=DEBUG,
     )
     trav_vert_qdev = Compax3_servo_qdev(
-        dev=trav_vert, DAQ_interval_ms=UPDATE_INTERVAL_MS
+        dev=trav_vert,
+        DAQ_interval_ms=UPDATE_INTERVAL_MS,
+        debug=DEBUG,
     )
     travs_qdev = [trav_horz_qdev, trav_vert_qdev]
 
     # Create Compax3 single step navigator
     trav_step_nav = Compax3_step_navigator(
         trav_horz=trav_horz, trav_vert=trav_vert
     )
+
+    # Act on step signals
+    @Slot()
+    def act_upon_signal_step_up(new_pos: float):
+        trav_vert_qdev.qlin_new_pos.setText(f"{new_pos:.2f}")
+        trav_vert_qdev.process_pbtn_move_to_new_pos()
+
+    @Slot()
+    def act_upon_signal_step_down(new_pos: float):
+        trav_vert_qdev.qlin_new_pos.setText(f"{new_pos:.2f}")
+        trav_vert_qdev.process_pbtn_move_to_new_pos()
+
+    @Slot()
+    def act_upon_signal_step_left(new_pos: float):
+        trav_horz_qdev.qlin_new_pos.setText(f"{new_pos:.2f}")
+        trav_horz_qdev.process_pbtn_move_to_new_pos()
+
+    @Slot()
+    def act_upon_signal_step_right(new_pos: float):
+        trav_horz_qdev.qlin_new_pos.setText(f"{new_pos:.2f}")
+        trav_horz_qdev.process_pbtn_move_to_new_pos()
+
     trav_step_nav.step_up.connect(act_upon_signal_step_up)
     trav_step_nav.step_down.connect(act_upon_signal_step_down)
     trav_step_nav.step_left.connect(act_upon_signal_step_left)
     trav_step_nav.step_right.connect(act_upon_signal_step_right)
 
-    # Create window
-    window = MainWindow()
-
-    # --------------------------------------------------------------------------
-    #   Start threads
-    # --------------------------------------------------------------------------
-
     trav_horz_qdev.start()
     trav_vert_qdev.start()
 
     # --------------------------------------------------------------------------
     #   Start the main GUI event loop
     # --------------------------------------------------------------------------
 
+    def about_to_quit():
+        print("About to quit")
+        app.processEvents()
+        for trav_qdev in travs_qdev:
+            trav_qdev.quit()
+        for trav in travs:
+            trav.close()
+
+    app.aboutToQuit.connect(about_to_quit)
+    window = MainWindow(
+        qdev_horz=trav_horz_qdev,
+        qdev_vert=trav_vert_qdev,
+        step_nav=trav_step_nav,
+    )
     window.show()
-    if QT_LIB in (PYQT5, PYSIDE2):
-        sys.exit(app.exec_())
-    else:
-        sys.exit(app.exec())
+
+    sys.exit(app.exec())
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Compax3_servo_protocol_RS232.py` & `dvg-devices-1.4.0/src/dvg_devices/Compax3_servo_protocol_RS232.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,57 +11,57 @@
 the previous query resulted in a communication error.
 
 When this module is directly run from the terminal a demo will be shown.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except, broad-except, try-except-raise, pointless-string-statement
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, pointless-string-statement
 
 import sys
 from typing import Union, Tuple
+
 import numpy as np
 
 from dvg_devices.BaseDevice import SerialDevice
 
 
 class Compax3_servo(SerialDevice):
-    """Containers for the process and measurement variables
-    [numpy.nan] values indicate that the parameter is not initialized or that
-    the last query was unsuccessful in communication.
-    """
-
     class Status_word_1:
-        # Container for Status word 1
+        """[numpy.nan] values indicate that the parameter is not initialized or
+        that the last query was unsuccessful in communication."""
+
         # fmt: off
-        I0 = np.nan                 # bit 0
-        I1 = np.nan                 # bit 1
-        I2 = np.nan                 # bit 2
-        I3 = np.nan                 # bit 3
-        I4 = np.nan                 # bit 4
-        I5 = np.nan                 # bit 5
-        I6 = np.nan                 # bit 6
-        I7 = np.nan                 # bit 7 'open motor holding brake'
-        no_error           = np.nan # bit 8
-        pos_reached        = np.nan # bit 9
-        powerless          = np.nan # bit 10
-        powered_stationary = np.nan # bit 11 'standstill'
-        zero_pos_known     = np.nan # bit 12
-        PSB0 = np.nan               # bit 13
-        PSB1 = np.nan               # bit 14
-        PSB2 = np.nan               # bit 15
+        I0                : Union[float, bool] = np.nan  # bit 0
+        I1                : Union[float, bool] = np.nan  # bit 1
+        I2                : Union[float, bool] = np.nan  # bit 2
+        I3                : Union[float, bool] = np.nan  # bit 3
+        I4                : Union[float, bool] = np.nan  # bit 4
+        I5                : Union[float, bool] = np.nan  # bit 5
+        I6                : Union[float, bool] = np.nan  # bit 6
+        I7                : Union[float, bool] = np.nan  # bit 7 'open motor holding brake'
+        no_error          : Union[float, bool] = np.nan  # bit 8
+        pos_reached       : Union[float, bool] = np.nan  # bit 9
+        powerless         : Union[float, bool] = np.nan  # bit 10
+        powered_stationary: Union[float, bool] = np.nan  # bit 11 'standstill'
+        zero_pos_known    : Union[float, bool] = np.nan  # bit 12
+        PSB0              : Union[float, bool] = np.nan  # bit 13
+        PSB1              : Union[float, bool] = np.nan  # bit 14
+        PSB2              : Union[float, bool] = np.nan  # bit 15
         # fmt: on
 
     class State:
-        # Container for the process and measurement variables
+        """[numpy.nan] values indicate that the parameter is not initialized or
+        that the last query was unsuccessful in communication."""
+
         # fmt: off
-        cur_pos = np.nan            # position [mm]
-        error_msg = np.nan          # error string message
+        cur_pos: float = np.nan  # position [mm]
+        error_msg: str = ""      # error string message
         # fmt: on
 
     def __init__(
         self,
         name="trav",
         long_name="Compax3 servo",
         connect_to_serial_number=None,
@@ -84,15 +84,15 @@
             valid_ID_specific=connect_to_serial_number,
         )
 
         # Containers for the status, process and measurement variables
         self.status_word_1 = self.Status_word_1()
         self.state = self.State()
 
-        self.serial_str = None  # Serial number of the Compax3
+        self.serial_str = ""  # Serial number of the Compax3
 
     # --------------------------------------------------------------------------
     #   OVERRIDE: query
     # --------------------------------------------------------------------------
 
     def query(
         self,
@@ -100,15 +100,15 @@
         raises_on_timeout: bool = False,
         returns_ascii: bool = True,
     ) -> Tuple[bool, Union[str, bytes, None]]:
         success, reply = super().query(msg, raises_on_timeout, returns_ascii)
 
         # The Compax3 is more complex in its replies than the average device.
         # Hence:
-        if success:
+        if isinstance(reply, str):
             if reply[0] == ">":
                 # Successful operation without meaningful reply
                 pass
             elif reply[0] == "!":
                 # Error reply
                 print("COMPAX3 COMMUNICATION ERROR: " + reply)
                 success = False
@@ -118,19 +118,26 @@
 
         return success, reply
 
     # --------------------------------------------------------------------------
     #   ID_validation_query
     # --------------------------------------------------------------------------
 
-    def ID_validation_query(self) -> Tuple[str, str]:
+    def ID_validation_query(self) -> Tuple[str, Union[str, None]]:
+        broad_reply = ""
+        specific_reply = None
+
         _success, reply = self.query("_?")
-        broad_reply = reply[:7]  # Expected: "Compax3"
+        if isinstance(reply, str):
+            broad_reply = reply[:7]  # Expected: "Compax3"
+
         _success, reply = self.query("o1.4")
-        specific_reply = reply  # Serial number
+        if isinstance(reply, str):
+            specific_reply = reply  # Serial number
+
         return broad_reply, specific_reply
 
     # --------------------------------------------------------------------------
     #   begin
     # --------------------------------------------------------------------------
 
     def begin(self):
@@ -154,76 +161,76 @@
 
         Returns: True if successful, False otherwise.
         """
         # First make sure we're dealing with a Compax3 controller, because we
         # have to exclude the possibility that another device will reply with
         # an error message to the serial number request, which then could be
         # mistaken for /the/ serial number.
-        success, reply = self.query("_?")
-        if success and reply.startswith("Compax3"):
+        _success, reply = self.query("_?")
+        if isinstance(reply, str) and reply.startswith("Compax3"):
             # Now we can query the serial number
-            success, reply = self.query("o1.4")
-            if success:
+            _success, reply = self.query("o1.4")
+            if isinstance(reply, str):
                 self.serial_str = reply
                 return True
 
-        self.serial_str = None
+        self.serial_str = ""
         return False
 
     def query_position(self) -> bool:
         """Query the position and store in the class member 'state.cur_pos'
         when successful. When the communication fails the class member will be
         set to [numpy.nan].
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query("o680.5")
-        if success:
+        _success, reply = self.query("o680.5")
+        if isinstance(reply, str):
             self.state.cur_pos = float(reply)
-        else:
-            self.state.cur_pos = np.nan
+            return True
 
-        return success
+        self.state.cur_pos = np.nan
+        return False
 
     def query_error(self) -> bool:
         """Query the last error and store in the class member 'state.error_msg'
         when successful. When the communication fails the class member will be
         set to [numpy.nan].
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query("o550.1")
-        if success:
+        _success, reply = self.query("o550.1")
+        if isinstance(reply, str):
             # Translate error codes to more meaningful messages
             if reply == "1":
                 self.state.error_msg = ""
             elif reply == "17168":
-                self.state.error_msg = "%s: Motor temperature" % reply
+                self.state.error_msg = f"{reply}: Motor temperature"
             elif reply == "29472":
-                self.state.error_msg = "%s: Following error" % reply
+                self.state.error_msg = f"{reply}: Following error"
             elif reply == "29475":
                 self.state.error_msg = (
-                    "%s: Target or actual position "
-                    "exceeds positive end limit" % reply
+                    f"{reply}: Target or actual position "
+                    "exceeds positive end limit"
                 )
             elif reply == "29476":
                 self.state.error_msg = (
-                    "%s: Target or actual position "
-                    "exceeds negative end limit" % reply
+                    f"{reply}: Target or actual position "
+                    "exceeds negative end limit"
                 )
             elif reply == "29479":
                 self.state.error_msg = (
-                    "%s: Change of direction during " "movement" % reply
+                    f"{reply}: Change of direction during " "movement"
                 )
             else:
                 self.state.error_msg = reply
-        else:
-            self.state.error_msg = np.nan
+            return True
 
-        return success
+        self.state.error_msg = ""
+        return False
 
     def query_status_word_1(self) -> bool:
         """Query the status word 1 and store in the class member 'status_word_1'
         when successful. When the communication fails the class member
         'status_word_1' will be populated with [numpy.nan].
 
         Returns: True if successful, False otherwise.
@@ -292,117 +299,101 @@
     ) -> bool:
         """
         Note:
             Profile_number 0 is reserved for homing.
             Movement mode is fixed to absolute, not relative.
         """
         mode = 1  # Overrule, set movement mode to absolute position
+        p = profile_number  # Shorthand
 
-        print("  Profile number: %d" % profile_number)
-        print("    pos   = %.2f" % target_position)
-        print("    vel   = %.2f" % velocity)
-        print("    mode  = %d (fixed to absolute)" % mode)
-        print("    accel = %.2f" % accel)
-        print("    decel = %.2f" % decel)
-        print("    jerk  = %.2f\n" % jerk)
+        print(f"  Profile number: {p}")
+        print(f"    pos   = {target_position:.2f}")
+        print(f"    vel   = {velocity:.2f}")
+        print(f"    mode  = {mode:d} (fixed to absolute)")
+        print(f"    accel = {accel:.2f}")
+        print(f"    decel = {decel:.2f}")
+        print(f"    jerk  = {jerk:.2f}\n")
 
-        success, _reply = self.query(
-            "o1901.%d=%.2f" % (profile_number, target_position)
-        )
+        success, _reply = self.query(f"o1901.{p:d}={target_position:.2f}")
+        if success:
+            success, _reply = self.query(f"o1902.{p:d}={velocity:.2f}")
+        if success:
+            success, _reply = self.query(f"o1905.{p:d}={mode:d}")
+        if success:
+            success, _reply = self.query(f"o1906.{p:d}={accel:.2f}")
+        if success:
+            success, _reply = self.query(f"o1907.{p:d}={decel:.2f}")
+        if success:
+            success, _reply = self.query(f"o1908.{p:d}={jerk:.2f}")
         if success:
-            success, _reply = self.query(
-                "o1902.%d=%.2f" % (profile_number, velocity)
-            )
-        if success:
-            success, _reply = self.query("o1905.%d=%d" % (profile_number, mode))
-        if success:
-            success, _reply = self.query(
-                "o1906.%d=%.2f" % (profile_number, accel)
-            )
-        if success:
-            success, _reply = self.query(
-                "o1907.%d=%.2f" % (profile_number, decel)
-            )
-        if success:
-            success, _reply = self.query(
-                "o1908.%d=%.2f" % (profile_number, jerk)
-            )
-        if success:
-            success, _reply = self.query(
-                "o1904.%d=$32" % (profile_number)
-            )  # Store profile
+            success, _reply = self.query(f"o1904.{p:d}=$32")  # Store profile
 
         return success
 
     def activate_motion_profile(self, profile_number=2) -> bool:
-        """ """
         # Control word (CW) for activating the passed profile number
         # First send: quit/motor bit (bit 0) high
         #             stop bits (bits 1, 14) high
         #             start bit (bit 13) low
         CW_LO = 0b0100000000000011
         CW_LO = CW_LO + (profile_number << 8)
-        success, _reply = self.query("o1100.3=%d" % CW_LO)
+        success, _reply = self.query(f"o1100.3={CW_LO:d}")
         if success:
             # Then send start bit (bit 13) high
             CW_HI = CW_LO + (1 << 13)
-            success, _reply = self.query("o1100.3=%d" % CW_HI)
+            success, _reply = self.query(f"o1100.3={CW_HI:d}")
 
         return success
 
     def move_to_target_position(
         self, target_position, profile_number=2
     ) -> bool:
         """
         Note: Make sure a motion profile with number 'profile_number' is stored
         at least once with 'self.store_motion_profile' before moving.
         """
         # Send new target position
         success, _reply = self.query(
-            "o1901.%d=%.2f" % (profile_number, target_position)
+            f"o1901.{profile_number:d}={target_position:.2f}"
         )
 
         if success:
             self.activate_motion_profile(profile_number=2)
 
         return success
 
     def jog_plus(self) -> bool:
-        """ """
         # Control word (CW) for activating the jog+
         CW_LO = 0b0100000000000011
-        success, _reply = self.query("o1100.3=%d" % CW_LO)
+        success, _reply = self.query(f"o1100.3={CW_LO:d}")
         if success:
             # Then send jog+ bit (bit 2) high
             CW_HI = CW_LO + (1 << 2)
-            success, _reply = self.query("o1100.3=%d" % CW_HI)
+            success, _reply = self.query(f"o1100.3={CW_HI:d}")
 
         return success
 
     def jog_minus(self) -> bool:
-        """ """
         # Control word (CW) for activating the jog-
         CW_LO = 0b0100000000000011
-        success, _reply = self.query("o1100.3=%d" % CW_LO)
+        success, _reply = self.query(f"o1100.3={CW_LO:d}")
         if success:
             # Then send jog- bit (bit 3) high
             CW_HI = CW_LO + (1 << 3)
-            success, _reply = self.query("o1100.3=%d" % CW_HI)
+            success, _reply = self.query(f"o1100.3={CW_HI:d}")
 
         return success
 
     def stop_motion_but_keep_power(self) -> bool:
-        """ """
         CW_LO = 0b0100000000000011
-        success, _reply = self.query("o1100.3=%d" % CW_LO)
+        success, _reply = self.query(f"o1100.3={CW_LO:d}")
 
         return success
 
     def stop_motion_and_remove_power(self) -> bool:
-        """ """
         success, _reply = self.query("o1100.3=0")
 
         return success
 
     def acknowledge_error(self) -> bool:
         """If the cause of an error is eliminated, the error can be
         acknowledged. This is necessary for the axis to be able to get powered
@@ -416,50 +407,48 @@
         success, _reply = self.query("o1100.3=0")
         if success:
             success, _reply = self.query("o1100.3=1")
 
         return success
 
     def report_status_word_1(self, compact=False):
-        """ """
+        SW = self.status_word_1  # Shorthand
         if not compact:
             print("Status word 1:")
-            print("  %-6s: I0" % self.status_word_1.I0)
-            print("  %-6s: I1" % self.status_word_1.I1)
-            print("  %-6s: I2" % self.status_word_1.I2)
-            print("  %-6s: I3" % self.status_word_1.I3)
-            print("  %-6s: I4" % self.status_word_1.I4)
-            print("  %-6s: I5" % self.status_word_1.I5)
-            print("  %-6s: I6" % self.status_word_1.I6)
-            print("  %-6s: I7" % self.status_word_1.I7)
-            print("  %-6s: no_error" % self.status_word_1.no_error)
-            print("  %-6s: pos_reached" % self.status_word_1.pos_reached)
-            print("  %-6s: powerless" % self.status_word_1.powerless)
-            print(
-                "  %-6s: powered_stat" % self.status_word_1.powered_stationary
-            )
-            print("  %-6s: zero_pos_known" % self.status_word_1.zero_pos_known)
-            print("  %-6s: PSB0" % self.status_word_1.PSB1)
-            print("  %-6s: PSB1" % self.status_word_1.PSB1)
-            print("  %-6s: PSB2" % self.status_word_1.PSB2)
+            print(f"  {SW.I0:-6s}: I0")
+            print(f"  {SW.I1:-6s}: I1")
+            print(f"  {SW.I2:-6s}: I2")
+            print(f"  {SW.I3:-6s}: I3")
+            print(f"  {SW.I4:-6s}: I4")
+            print(f"  {SW.I5:-6s}: I5")
+            print(f"  {SW.I6:-6s}: I6")
+            print(f"  {SW.I7:-6s}: I7")
+            print(f"  {SW.no_error:-6s}: no_error")
+            print(f"  {SW.pos_reached:-6s}: pos_reached")
+            print(f"  {SW.powerless:-6s}: powerless")
+            print(f"  {SW.powered_stationary:-6s}: powered_stat")
+            print(f"  {SW.zero_pos_known:-6s}: zero_pos_known")
+            print(f"  {SW.PSB0:-6s}: PSB0")
+            print(f"  {SW.PSB1:-6s}: PSB1")
+            print(f"  {SW.PSB2:-6s}: PSB2")
         else:
-            if not self.status_word_1.no_error:
+            if not SW.no_error:
                 print("  ERROR!")
-            if self.status_word_1.powerless:
+            if SW.powerless:
                 print("  Axis    : unpowered")
             else:
-                if self.status_word_1.powered_stationary:
+                if SW.powered_stationary:
                     print("  Axis    : POWERED STANDSTILL")
                 else:
                     print("  Axis    : POWERED")
-            if self.status_word_1.zero_pos_known:
+            if SW.zero_pos_known:
                 print("  Zero pos: known")
             else:
                 print("  Zero pos: UNKNOWN")
-            if self.status_word_1.pos_reached:
+            if SW.pos_reached:
                 print("  Position: REACHED")
             else:
                 print("  Position: unreached")
         print("")
 
 
 # ------------------------------------------------------------------------------
@@ -468,16 +457,16 @@
 
 if __name__ == "__main__":
     import time
 
     # Specific connection settings of each traverse axis of our setup
     class Trav_connection_params:
         # Serial number of the Compax3 servo controller to connect to.
-        # Set to '' or None to connect to any Compax3.
-        serial = None
+        # Set to "" to connect to any Compax3.
+        serial = ""
         # Display name
         name = "TRAV"
         # Path to the config textfile containing the (last used) RS232 port
         path_config = "config/port_Compax3_servo.txt"
 
     # Horizontal axis
     trav_conn_horz = Trav_connection_params()
@@ -497,25 +486,26 @@
     trav_conn = trav_conn_vert
 
     # --------------------------------------------------------------------------
     # --------------------------------------------------------------------------
 
     # Create connection to Compax3 servo controller over RS232
     trav = Compax3_servo(
-        name=trav_conn.name, connect_to_serial_number=trav_conn.serial
+        name=trav_conn.name,
+        connect_to_serial_number=trav_conn.serial,
     )
 
     if trav.auto_connect(filepath_last_known_port=trav_conn.path_config):
         trav.begin()  # Retrieve necessary parameters
     else:
         time.sleep(1)
         sys.exit(0)
 
-    print("Error msg: %s" % trav.state.error_msg)
-    print("Current position: %.2f" % trav.state.cur_pos)
+    print(f"Error msg: {trav.state.error_msg}")
+    print(f"Current position: {trav.state.cur_pos:.2f}")
     trav.report_status_word_1(compact=True)
 
     trav.acknowledge_error()
 
     print("ERRORS RESET")
     print("ACTIVATE\n")
     time.sleep(0.1)
@@ -542,41 +532,41 @@
     """
 
     """
     trav.query("o1100.3=$4007")      # jog+
     time.sleep(2);
 
     trav.query_position()
-    print("Current position: %.2f" % trav.state.cur_pos)
+    print(f"Current position: {trav.state.cur_pos:.2f}")
 
     trav.query("o1100.3=$400b")      # jog-
     time.sleep(2);
     """
     # fmt: on
 
     print("MOVING\n")
 
     for i in range(14):
         trav.query_position()
-        print("Current position: %.2f" % trav.state.cur_pos)
+        print(f"Current position: {trav.state.cur_pos:.2f}")
         trav.query_status_word_1()
         trav.report_status_word_1(compact=True)
         time.sleep(0.2)
 
     trav.query("o1100.3=0")  # disable axis
     # trav.query("o1000.4")   # last executed set #
 
     print("DEACTIVATE\n")
     time.sleep(1)
 
     trav.query_error()
     trav.query_position()
     trav.query_status_word_1()
 
-    print("Error msg: %s" % trav.state.error_msg)
-    print("Current position: %.2f" % trav.state.cur_pos)
+    print(f"Error msg: {trav.state.error_msg}")
+    print(f"Current position: {trav.state.cur_pos:.2f}")
     trav.report_status_word_1(compact=True)
 
     # Close
     print("")
     trav.close()
     sys.exit(0)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Compax3_servo_qdev.py` & `dvg-devices-1.4.0/src/dvg_devices/Compax3_servo_qdev.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,80 +2,22 @@
 # -*- coding: utf-8 -*-
 """PyQt/PySide module to provide multithreaded communication and periodical data
 acquisition for a Compax3 traverse controller.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "0.2.1"
-# pylint: disable=try-except-raise
-
-import os
-import sys
-
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, multiple-statements
 
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
-from dvg_pyqt_controls import (
-    SS_GROUP,
-    SS_TEXTBOX_ERRORS,
-    create_error_LED,
-    create_tiny_LED,
-)
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Slot  # type: ignore
 
+import dvg_pyqt_controls as controls
 from dvg_qdeviceio import QDeviceIO, DAQ_TRIGGER
 from dvg_devices.Compax3_servo_protocol_RS232 import Compax3_servo
 
 
 class Compax3_servo_qdev(QDeviceIO):
     """Manages multithreaded communication and periodical data acquisition for
     a Compax3 traverse controller, referred to as the 'device'.
@@ -108,14 +50,15 @@
         DAQ_interval_ms=250,
         critical_not_alive_count=1,
         DAQ_timer_type=QtCore.Qt.TimerType.CoarseTimer,
         debug=False,
         **kwargs,
     ):
         super().__init__(dev, **kwargs)  # Pass kwargs onto QtCore.QObject()
+        self.dev: Compax3_servo  # Enforce type: removes `_NoDevice()`
 
         self.create_worker_DAQ(
             DAQ_trigger=DAQ_TRIGGER.INTERNAL_TIMER,
             DAQ_function=self._DAQ_function,
             DAQ_interval_ms=DAQ_interval_ms,
             DAQ_timer_type=DAQ_timer_type,
             critical_not_alive_count=critical_not_alive_count,
@@ -153,21 +96,21 @@
     # --------------------------------------------------------------------------
 
     def _create_GUI(self):
         default_font_height = 17
         default_font_width = 8
 
         # Sub-groupbox: Status word 1 bits
-        self.sw1_powerless = create_tiny_LED()
-        self.sw1_powered_stationary = create_tiny_LED()
-        self.sw1_zero_pos_known = create_tiny_LED()
-        self.sw1_pos_reached = create_tiny_LED()
+        self.sw1_powerless = controls.create_tiny_LED()
+        self.sw1_powered_stationary = controls.create_tiny_LED()
+        self.sw1_zero_pos_known = controls.create_tiny_LED()
+        self.sw1_pos_reached = controls.create_tiny_LED()
 
         i = 0
-        p = {"alignment": QtCore.Qt.AlignmentFlag.AlignRight}
+        p = {"parent": None, "alignment": QtCore.Qt.AlignmentFlag.AlignRight}
         grid = QtWid.QGridLayout()
         grid.setVerticalSpacing(4)
         # fmt: off
         grid.addWidget(QtWid.QLabel("powerless", **p)         , i, 0)
         grid.addWidget(self.sw1_powerless                     , i, 1); i+=1
         grid.addWidget(QtWid.QLabel("powered stationary", **p), i, 0)
         grid.addWidget(self.sw1_powered_stationary            , i, 1); i+=1
@@ -182,159 +125,149 @@
         self.qgrp_sw1 = QtWid.QGroupBox("Status word 1")
         self.qgrp_sw1.setLayout(grid)
 
         # Main groupbox
         font_lbl_status = QtGui.QFont(
             "Palatino", 14, weight=QtGui.QFont.Weight.Bold
         )
-        self.lbl_status = QtWid.QLabel(
-            "OFFLINE",
-            font=font_lbl_status,
-            alignment=QtCore.Qt.AlignmentFlag.AlignCenter,
-        )
+        self.lbl_status = QtWid.QLabel("OFFLINE")
+        self.lbl_status.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.lbl_status.setFont(font_lbl_status)
         self.lbl_status.setFixedHeight(
             3 * QtGui.QFontMetrics(font_lbl_status).height()
         )
 
-        self.sw1_error_tripped = create_error_LED(text="No error")
+        self.sw1_error_tripped = controls.create_error_LED(text="No error")
         self.error_msg = QtWid.QPlainTextEdit("")
         self.error_msg.setLineWrapMode(
             QtWid.QPlainTextEdit.LineWrapMode.WidgetWidth
         )
-        self.error_msg.setStyleSheet(SS_TEXTBOX_ERRORS)
+        self.error_msg.setStyleSheet(controls.SS_TEXTBOX_ERRORS)
         self.error_msg.setMinimumWidth(22 * default_font_width)
         self.error_msg.setFixedHeight(4 * default_font_height)
         self.pbtn_ackn_error = QtWid.QPushButton("Acknowledge error")
-        self.qled_cur_pos = QtWid.QLineEdit(
-            "nan", readOnly=True, alignment=QtCore.Qt.AlignmentFlag.AlignRight
-        )
-        self.qled_new_pos = QtWid.QLineEdit(
-            "nan", readOnly=False, alignment=QtCore.Qt.AlignmentFlag.AlignRight
-        )
+        p = {"parent": None, "alignment": QtCore.Qt.AlignmentFlag.AlignRight}
+        p2 = {**p, "readOnly": True}
+        self.qlin_cur_pos = QtWid.QLineEdit("nan", **p2)
+        self.qlin_new_pos = QtWid.QLineEdit("nan", **p)
         self.pbtn_move_to_new_pos = QtWid.QPushButton("Move to new position")
         self.pbtn_move_to_new_pos.setFixedHeight(3 * default_font_height)
         self.pbtn_jog_plus = QtWid.QPushButton("Jog +")
         self.pbtn_jog_minus = QtWid.QPushButton("Jog -")
         self.pbtn_stop = QtWid.QPushButton("\nSTOP &&\nREMOVE POWER\n")
         self.lbl_update_counter = QtWid.QLabel("0")
 
         i = 0
-        p = {"alignment": QtCore.Qt.AlignmentFlag.AlignRight}
         grid = QtWid.QGridLayout()
         grid.setVerticalSpacing(4)
         # fmt: off
         grid.addWidget(self.lbl_status             , i, 0, 1, 3); i+=1
         grid.addItem(QtWid.QSpacerItem(1, 12)      , i, 0)      ; i+=1
         grid.addWidget(self.sw1_error_tripped      , i, 0, 1, 3); i+=1
         grid.addWidget(self.error_msg              , i, 0, 1, 3); i+=1
         grid.addWidget(self.pbtn_ackn_error        , i, 0, 1, 3); i+=1
         grid.addItem(QtWid.QSpacerItem(1, 12)      , i, 0)      ; i+=1
         grid.addWidget(self.qgrp_sw1               , i, 0, 1, 3); i+=1
         grid.addItem(QtWid.QSpacerItem(1, 12)      , i, 0)      ; i+=1
 
         grid.addWidget(QtWid.QLabel("Position:")   , i, 0, 1, 3); i+=1
         grid.addWidget(QtWid.QLabel("Current")     , i, 0)
-        grid.addWidget(self.qled_cur_pos           , i, 1)
+        grid.addWidget(self.qlin_cur_pos           , i, 1)
         grid.addWidget(QtWid.QLabel("mm")          , i, 2)      ; i+=1
         grid.addWidget(QtWid.QLabel("New")         , i, 0)
-        grid.addWidget(self.qled_new_pos           , i, 1)
+        grid.addWidget(self.qlin_new_pos           , i, 1)
         grid.addWidget(QtWid.QLabel("mm")          , i, 2)      ; i+=1
 
         grid.addItem(QtWid.QSpacerItem(1, 12)      , i, 0)      ; i+=1
         grid.addWidget(self.pbtn_move_to_new_pos   , i, 0, 1, 3); i+=1
         grid.addWidget(self.pbtn_jog_plus          , i, 0, 1, 3); i+=1
         grid.addWidget(self.pbtn_jog_minus         , i, 0, 1, 3); i+=1
         grid.addWidget(self.pbtn_stop              , i, 0, 1, 3); i+=1
         grid.addWidget(self.lbl_update_counter     , i, 0, 1, 3); i+=1
         # fmt: on
         # grid.setColumnStretch(0, 0)
         # grid.setColumnStretch(1, 0)
         # grid.setColumnStretch(2, 0)
 
-        self.qgrp = QtWid.QGroupBox("%s" % self.dev.name)
-        self.qgrp.setStyleSheet(SS_GROUP)
+        self.qgrp = QtWid.QGroupBox(f"{self.dev.name}")
+        self.qgrp.setStyleSheet(controls.SS_GROUP)
         self.qgrp.setLayout(grid)
-        self.qgrp.setMaximumWidth(200)  # Work=around, hard limit width
+        self.qgrp.setMaximumWidth(200)  # Work-around, hard limit width
 
     # --------------------------------------------------------------------------
     #   _update_GUI
     # --------------------------------------------------------------------------
 
     @Slot()
     def _update_GUI(self):
         """NOTE: 'self.dev.mutex' is not being locked, because we are only
         reading 'state' for displaying purposes. We can do this because 'state'
         members are written and read atomicly.
         Not locking the mutex might speed up the program.
         """
+        SW = self.dev.status_word_1  # Shorthand
         if self.dev.is_alive:
             # At startup
             if self.update_counter_DAQ == 1:
-                self.qled_new_pos.setText("%.2f" % self.dev.state.cur_pos)
+                self.qlin_new_pos.setText(f"{self.dev.state.cur_pos:.2f}")
 
-            if self.dev.status_word_1.powerless:
+            if SW.powerless:
                 self.lbl_status.setText("powerless")
             else:
-                if self.dev.status_word_1.powered_stationary:
+                if SW.powered_stationary:
                     self.lbl_status.setText("POWERED\nstationary")
                 else:
                     self.lbl_status.setText("POWERED")
 
-            self.sw1_error_tripped.setChecked(
-                not (self.dev.status_word_1.no_error)
-            )
-            if self.dev.status_word_1.no_error:
+            self.sw1_error_tripped.setChecked(not SW.no_error)
+            if SW.no_error:
                 self.sw1_error_tripped.setText("No error")
                 self.error_msg.setPlainText("")
                 self.error_msg.setReadOnly(False)
-                self.error_msg.setStyleSheet(SS_TEXTBOX_ERRORS)
+                self.error_msg.setStyleSheet(controls.SS_TEXTBOX_ERRORS)
             else:
                 self.sw1_error_tripped.setText("ERROR TRIPPED")
                 self.error_msg.setPlainText(self.dev.state.error_msg)
                 self.error_msg.setReadOnly(True)
-                self.error_msg.setStyleSheet(SS_TEXTBOX_ERRORS)
-            self.sw1_powerless.setChecked(self.dev.status_word_1.powerless)
-            self.sw1_powered_stationary.setChecked(
-                self.dev.status_word_1.powered_stationary
-            )
-            self.sw1_zero_pos_known.setChecked(
-                self.dev.status_word_1.zero_pos_known
-            )
-            self.sw1_pos_reached.setChecked(self.dev.status_word_1.pos_reached)
-            self.qled_cur_pos.setText("%.2f" % self.dev.state.cur_pos)
+                self.error_msg.setStyleSheet(controls.SS_TEXTBOX_ERRORS)
+            self.sw1_powerless.setChecked(bool(SW.powerless))
+            self.sw1_powered_stationary.setChecked(bool(SW.powered_stationary))
+            self.sw1_zero_pos_known.setChecked(bool(SW.zero_pos_known))
+            self.sw1_pos_reached.setChecked(bool(SW.pos_reached))
+            self.qlin_cur_pos.setText(f"{self.dev.state.cur_pos:.2f}")
 
-            self.lbl_update_counter.setText("%s" % self.update_counter_DAQ)
+            self.lbl_update_counter.setText(f"{self.update_counter_DAQ}")
         else:
             self.qgrp.setEnabled(False)
 
     # --------------------------------------------------------------------------
     #   GUI functions
     # --------------------------------------------------------------------------
 
     @Slot()
     def process_pbtn_ackn_error(self):
         self.send(self.dev.acknowledge_error)
 
     @Slot()
-    def process_editingFinished_qled_new_pos(self):
+    def process_editingFinished_qlin_new_pos(self):
         try:
-            new_pos = float(self.qled_new_pos.text())
+            new_pos = float(self.qlin_new_pos.text())
         except (TypeError, ValueError):
             new_pos = 0.0
-        except:
-            raise
-        self.qled_new_pos.setText("%.2f" % new_pos)
+        except Exception as e:
+            raise e
+        self.qlin_new_pos.setText(f"{new_pos:.2f}")
 
     @Slot()
     def process_pbtn_move_to_new_pos(self):
         # Double check if the value in the QLineEdit is actually numeric
         try:
-            new_pos = float(self.qled_new_pos.text())
-        except:
-            raise
+            new_pos = float(self.qlin_new_pos.text())
+        except Exception as e:
+            raise e
         self.send(self.dev.move_to_target_position, (new_pos, 2))
 
     @Slot()
     def process_pbtn_jog_plus_pressed(self):
         if not self._jog_plus_is_active:
             self._jog_plus_is_active = True
             self.send(self.dev.jog_plus)
@@ -364,16 +297,16 @@
     # --------------------------------------------------------------------------
 
     def _connect_signals_to_slots(self):
         # self.send_setpoint.editingFinished.connect(
         #        self.send_setpoint_from_textbox)
 
         self.pbtn_ackn_error.clicked.connect(self.process_pbtn_ackn_error)
-        self.qled_new_pos.editingFinished.connect(
-            self.process_editingFinished_qled_new_pos
+        self.qlin_new_pos.editingFinished.connect(
+            self.process_editingFinished_qlin_new_pos
         )
         self.pbtn_move_to_new_pos.clicked.connect(
             self.process_pbtn_move_to_new_pos
         )
         # self.pbtn_debug.clicked.connect(self.process_pbtn_debug)
         self.pbtn_jog_plus.pressed.connect(self.process_pbtn_jog_plus_pressed)
         self.pbtn_jog_plus.released.connect(self.process_pbtn_jog_plus_released)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Compax3_servo_step_navigator_GUI.py` & `dvg-devices-1.4.0/src/dvg_devices/Compax3_servo_step_navigator_GUI.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,97 +10,42 @@
 
 No communication with a Compax3 servo controller will take place inside this
 module. It will only read out the software state. Pure GUI.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=try-except-raise
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring
 
-import os
 import sys
+from typing import Union
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt5.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt6.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-    from PySide2.QtCore import Signal                      # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-    from PySide6.QtCore import Signal                      # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Signal, Slot  # type: ignore
 import numpy as np
 
+import dvg_pyqt_controls as controls
 from dvg_debug_functions import print_fancy_traceback as pft
-from dvg_pyqt_controls import create_Toggle_button, SS_GROUP
-
 from dvg_devices.Compax3_servo_protocol_RS232 import Compax3_servo
 
 
 class Compax3_step_navigator(QtWid.QWidget):
     # fmt: off
     step_up    = Signal(float)
     step_down  = Signal(float)
     step_left  = Signal(float)
     step_right = Signal(float)
     # fmt: on
 
     def __init__(
         self,
-        trav_horz: Compax3_servo = None,
-        trav_vert: Compax3_servo = None,
+        trav_horz: Union[Compax3_servo, None] = None,
+        trav_vert: Union[Compax3_servo, None] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         if not (isinstance(trav_horz, Compax3_servo) or trav_horz is None):
             pft("Argument 'trav_horz' is of a wrong type.", 3)
             sys.exit(1)
@@ -113,27 +58,26 @@
         self.trav_vert = trav_vert
         self.horz_pos = np.nan  # [mm]
         self.vert_pos = np.nan  # [mm]
         self.step_size = np.nan  # [mm]
 
         self.create_GUI()
         self.connect_signals_to_slots()
-        self.process_editingFinished_qled_step_size()
+        self.process_editingFinished_qlin_step_size()
 
     def create_GUI(self):
-        self.pbtn_step_activate = create_Toggle_button("Disabled")
-        self.qled_step_size = QtWid.QLineEdit(
-            "1.0", alignment=QtCore.Qt.AlignmentFlag.AlignRight
-        )
-        self.qled_step_size.setFixedWidth(70)
+        self.pbtn_step_activate = controls.create_Toggle_button("Disabled")
+        self.qlin_step_size = QtWid.QLineEdit("1.0")
+        self.qlin_step_size.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
+        self.qlin_step_size.setFixedWidth(70)
 
         grid_sub = QtWid.QGridLayout()
         grid_sub.addWidget(self.pbtn_step_activate, 0, 0, 1, 3)
         grid_sub.addWidget(QtWid.QLabel("Step size"), 1, 0)
-        grid_sub.addWidget(self.qled_step_size, 1, 1)
+        grid_sub.addWidget(self.qlin_step_size, 1, 1)
         grid_sub.addWidget(QtWid.QLabel("mm"), 1, 2)
 
         font_1 = QtGui.QFont("Arial", 20)
         font_2 = QtGui.QFont("Arial", 30)
         p1 = {"font": font_1, "enabled": False}
         p2 = {"font": font_2, "enabled": False}
         self.pbtn_step_up = QtWid.QPushButton(chr(0x25B2), **p1)
@@ -141,15 +85,16 @@
         self.pbtn_step_down = QtWid.QPushButton(chr(0x25BC), **p1)
         self.pbtn_step_down.setFixedSize(50, 50)
         self.pbtn_step_left = QtWid.QPushButton(chr(0x25C0), **p2)
         self.pbtn_step_left.setFixedSize(50, 50)
         self.pbtn_step_right = QtWid.QPushButton(chr(0x25B6), **p2)
         self.pbtn_step_right.setFixedSize(50, 50)
 
-        self.pted_focus_trap = QtWid.QPlainTextEdit("", enabled=False)
+        self.pted_focus_trap = QtWid.QPlainTextEdit("")
+        self.pted_focus_trap.setEnabled(False)
         self.pted_focus_trap.setFixedSize(0, 0)
 
         # fmt: off
         grid = QtWid.QGridLayout()
         grid.addLayout(grid_sub               , 0, 0, 1, 4)
         grid.addItem(QtWid.QSpacerItem(1, 12) , 1, 0)
         grid.addWidget(self.pbtn_step_up      , 2, 1, QtCore.Qt.AlignmentFlag.AlignHCenter)
@@ -158,96 +103,98 @@
         grid.addWidget(self.pbtn_step_down    , 4, 1, QtCore.Qt.AlignmentFlag.AlignHCenter)
         grid.addWidget(self.pted_focus_trap   , 5, 1, QtCore.Qt.AlignmentFlag.AlignHCenter)
         # fmt: on
 
         self.grpb = QtWid.QGroupBox("Move single step")
         self.grpb.eventFilter = self.eventFilter
         self.grpb.installEventFilter(self.grpb)
-        self.grpb.setStyleSheet(SS_GROUP)
+        self.grpb.setStyleSheet(controls.SS_GROUP)
         self.grpb.setLayout(grid)
 
-    def eventFilter(self, obj, event):
+    def eventFilter(
+        self, watched: QtCore.QObject, event: QtCore.QEvent
+    ) -> bool:
         if self.listening_to_arrow_keys:
             if (
                 event.type() == QtCore.QEvent.Type.KeyRelease
-            ) and not event.isAutoRepeat():
-                if event.key() == QtCore.Qt.Key.Key_Up:
+            ) and not event.isAutoRepeat():  # type: ignore
+                if event.key() == QtCore.Qt.Key.Key_Up:  # type: ignore
                     print("up")
                     self.process_step_up()
                     self.pted_focus_trap.setFocus()
                     event.ignore()
                     return True
 
-                if event.key() == QtCore.Qt.Key.Key_Down:
+                if event.key() == QtCore.Qt.Key.Key_Down:  # type: ignore
                     print("down")
                     self.process_step_down()
                     self.pted_focus_trap.setFocus()
                     event.ignore()
                     return True
 
-                if event.key() == QtCore.Qt.Key.Key_Left:
+                if event.key() == QtCore.Qt.Key.Key_Left:  # type: ignore
                     print("left")
                     self.process_step_left()
                     self.pted_focus_trap.setFocus()
                     event.ignore()
                     return True
 
-                if event.key() == QtCore.Qt.Key.Key_Right:
+                if event.key() == QtCore.Qt.Key.Key_Right:  # type: ignore
                     print("right")
                     self.process_step_right()
                     self.pted_focus_trap.setFocus()
                     event.ignore()
                     return True
 
-        return super().eventFilter(obj, event)
+        return super().eventFilter(watched, event)
 
     @Slot()
     def process_pbtn_step_activate(self):
         if self.pbtn_step_activate.isChecked():
             self.listening_to_arrow_keys = True
             self.pbtn_step_activate.setText("Enabled")
             self.pbtn_step_up.setEnabled(True)
             self.pbtn_step_down.setEnabled(True)
             self.pbtn_step_left.setEnabled(True)
             self.pbtn_step_right.setEnabled(True)
             self.pted_focus_trap.setEnabled(True)
-            self.qled_step_size.setReadOnly(True)
+            self.qlin_step_size.setReadOnly(True)
 
             self.pted_focus_trap.setFocus()
 
             if self.trav_horz is not None:
-                self.horz_pos = float("%.2f" % self.trav_horz.state.cur_pos)
+                self.horz_pos = float(f"{self.trav_horz.state.cur_pos:.2f}")
             if self.trav_vert is not None:
-                self.vert_pos = float("%.2f" % self.trav_vert.state.cur_pos)
+                self.vert_pos = float(f"{self.trav_vert.state.cur_pos:.2f}")
         else:
             self.pbtn_step_activate.setText("Disabled")
             self.listening_to_arrow_keys = False
             self.pbtn_step_up.setEnabled(False)
             self.pbtn_step_down.setEnabled(False)
             self.pbtn_step_left.setEnabled(False)
             self.pbtn_step_right.setEnabled(False)
             self.pted_focus_trap.setEnabled(False)
-            self.qled_step_size.setReadOnly(False)
+            self.qlin_step_size.setReadOnly(False)
 
     @Slot()
-    def process_editingFinished_qled_step_size(self):
+    def process_editingFinished_qlin_step_size(self):
         try:
-            val = float(self.qled_step_size.text())
+            val = float(self.qlin_step_size.text())
         except (TypeError, ValueError):
             val = 0.0
-        except:
-            raise
+        except Exception as e:
+            raise e
         val = max(0.0, val)
-        self.qled_step_size.setText("%.2f" % val)
+        self.qlin_step_size.setText(f"{val:.2f}")
         self.step_size = val
 
     def connect_signals_to_slots(self):
         self.pbtn_step_activate.clicked.connect(self.process_pbtn_step_activate)
-        self.qled_step_size.editingFinished.connect(
-            self.process_editingFinished_qled_step_size
+        self.qlin_step_size.editingFinished.connect(
+            self.process_editingFinished_qlin_step_size
         )
         self.pbtn_step_up.clicked.connect(self.process_step_up)
         self.pbtn_step_down.clicked.connect(self.process_step_down)
         self.pbtn_step_left.clicked.connect(self.process_step_left)
         self.pbtn_step_right.clicked.connect(self.process_step_right)
 
     def process_step_up(self):
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Julabo_circulator_protocol_RS232.py` & `dvg-devices-1.4.0/src/dvg_devices/Julabo_circulator_protocol_RS232.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 # -*- coding: utf-8 -*-
 """RS232 function library for Julabo circulators.
 Tested on model FP51-SL.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except, broad-except, bad-string-format-type
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=broad-except, missing-function-docstring, multiple-statements
 
 import time
+import serial
 from typing import Union, Tuple
+
 import numpy as np
-import serial
 
 from dvg_debug_functions import print_fancy_traceback as pft
 from dvg_devices.BaseDevice import SerialDevice
 
 
 # The manual states that
 # - OUT commands should have a time gap > 250 ms. These are 'send' operations.
@@ -25,22 +26,23 @@
 # This module will enforce these time gaps.
 DELAY_COMMAND_IN = 0.02  # [s] 0.02 tested stable
 DELAY_COMMAND_OUT = 0.3  # [s] 0.3 tested stable
 
 
 class Julabo_circulator(SerialDevice):
     class State:
-        # Container for the process and measurement variables
+        """Container for the process and measurement variables."""
+
         # fmt: off
-        version = ""         # Version of the Julabo firmware         (string)
+        version: str = ""    # Version of the Julabo firmware
                              # FP51-SL: "JULABO HIGHTECH FL HL/SL VERSION 4.0"
-        status = np.nan      # Status or error message of the Julabo  (string)
-        has_error = np.nan   # True when status is a negative number    (bool)
-        temp_unit = np.nan   # Temperature unit used by the Julabo  ("C"; "F")
-        running = np.nan     # Is the circulator running?               (bool)
+        temp_unit: str = ""  # Temperature unit used by the Julabo  ("C"; "F")
+        status   : Union[float, str] = np.nan  # Status or error message of the Julabo
+        has_error: Union[float, bool] = np.nan  # True when status is a negative number
+        running  : Union[float, bool] = np.nan  # Is the circulator running?
 
         setpoint_preset = np.nan # Active setpoint preset in the Julabo (1; 2; 3)
         setpoint = np.nan    # Read-out temp. setpoint of active preset [C; F]
         setpoint_1 = np.nan  # Read-out temp. setpoint preset #1        [C; F]
         setpoint_2 = np.nan  # Read-out temp. setpoint preset #2        [C; F]
         setpoint_3 = np.nan  # Read-out temp. setpoint preset #3        [C; F]
         bath_temp = np.nan   # Current bath temperature                 [C; F]
@@ -83,24 +85,28 @@
         # Container for the process and measurement variables
         self.state = self.State()
 
     # --------------------------------------------------------------------------
     #   ID_validation_query
     # --------------------------------------------------------------------------
 
-    def ID_validation_query(self) -> Tuple[str, str]:
+    def ID_validation_query(self) -> Tuple[str, Union[str, None]]:
         # Strange Julabo quirk: The first query always times out
         try:
             self.query("VERSION")
-        except:
+        except Exception:
             pass  # Ignore the first time-out
 
         _success, reply = self.query("VERSION")
-        broad_reply = reply[:6]  # Expected: "JULABO"
-        reply_specific = reply[7:]
+        if isinstance(reply, str):
+            broad_reply = reply[:6]  # Expected: "JULABO"
+            reply_specific = reply[7:]
+        else:
+            broad_reply = ""
+            reply_specific = None
 
         return broad_reply, reply_specific
 
     # --------------------------------------------------------------------------
     #   begin
     # --------------------------------------------------------------------------
 
@@ -176,15 +182,15 @@
 
         try:
             value = float(value)
         except (TypeError, ValueError) as err:
             pft(err)
             return False
 
-        if self.write_("OUT_SP_04 %.2f" % value):
+        if self.write_(f"OUT_SP_04 {value:.2f}"):
             return self.query_sub_temp()
 
         return False
 
     # --------------------------------------------------------------------------
     #   set_over_temp
     # --------------------------------------------------------------------------
@@ -199,15 +205,15 @@
 
         try:
             value = float(value)
         except (TypeError, ValueError) as err:
             pft(err)
             return False
 
-        if self.write_("OUT_SP_03 %.2f" % value):
+        if self.write_(f"OUT_SP_03 {value:.2f}"):
             return self.query_over_temp()
 
         return False
 
     # --------------------------------------------------------------------------
     #   set_setpoint_preset
     # --------------------------------------------------------------------------
@@ -224,15 +230,15 @@
         if not n in (1, 2, 3):
             pft(
                 "WARNING: Received illegal setpoint preset.\n"
                 "Must be either 1, 2 or 3."
             )
             return False
 
-        if self.write_("OUT_MODE_01 %i" % (n - 1)):
+        if self.write_(f"OUT_MODE_01 {(n - 1):d}"):
             self.state.setpoint_preset = n
             return True
 
         return False
 
     # --------------------------------------------------------------------------
     #   set_sendpoint
@@ -273,15 +279,15 @@
 
         try:
             value = float(value)
         except (TypeError, ValueError) as err:
             pft(err)
             return False
 
-        if self.write_("OUT_SP_00 %.2f" % value):
+        if self.write_(f"OUT_SP_00 {value:.2f}"):
             return self.query_setpoint_1()
 
         return False
 
     # --------------------------------------------------------------------------
     #   set_sendpoint_2
     # --------------------------------------------------------------------------
@@ -295,15 +301,15 @@
 
         try:
             value = float(value)
         except (TypeError, ValueError) as err:
             pft(err)
             return False
 
-        if self.write_("OUT_SP_01 %.2f" % value):
+        if self.write_(f"OUT_SP_01 {value:.2f}"):
             return self.query_setpoint_2()
 
         return False
 
     # --------------------------------------------------------------------------
     #   set_sendpoint_3
     # --------------------------------------------------------------------------
@@ -317,49 +323,49 @@
 
         try:
             value = float(value)
         except (TypeError, ValueError) as err:
             pft(err)
             return False
 
-        if self.write_("OUT_SP_02 %.2f" % value):
+        if self.write_(f"OUT_SP_02 {value:.2f}"):
             return self.query_setpoint_3()
 
         return False
 
     # --------------------------------------------------------------------------
     #   query_version
     # --------------------------------------------------------------------------
 
     def query_version(self) -> bool:
         """Query the version of the Julabo firmware and store it in the class
         member 'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("VERSION")
-        if success:
+        _success, reply = self.query_("VERSION")
+        if isinstance(reply, str):
             self.state.version = reply
             return True
 
-        self.state.version = np.nan
+        self.state.version = ""
         return False
 
     # --------------------------------------------------------------------------
     #   query_status
     # --------------------------------------------------------------------------
 
     def query_status(self) -> bool:
         """Query the status or error message of the Julabo and store it in the
         class member 'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("STATUS")
-        if success:
+        _success, reply = self.query_("STATUS")
+        if isinstance(reply, str):
             self.state.status = reply
 
             try:
                 status_number = int(self.state.status[:3])
             except (TypeError, ValueError) as err:
                 self.state.has_error = np.nan
                 pft(err)
@@ -377,44 +383,44 @@
 
     # --------------------------------------------------------------------------
     #   query_temp_unit
     # --------------------------------------------------------------------------
 
     def query_temp_unit(self) -> bool:
         """Query the temperature unit used by the Julabo and store it in the
-        class member 'state'. Will be set to numpy.nan if unsuccessful, else
-        either "C" or "F".
+        class member 'state'. Will be set to "" if unsuccessful, else either "C"
+        or "F".
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_SP_06")
-        if success:
+        _success, reply = self.query_("IN_SP_06")
+        if isinstance(reply, str):
             try:
                 num = int(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.temp_unit = "C" if num == 0 else "F"
                 return True
 
-        self.state.temp_unit = np.nan
+        self.state.temp_unit = ""
         return False
 
     # --------------------------------------------------------------------------
     #   query_running
     # --------------------------------------------------------------------------
 
     def query_running(self) -> bool:
         """Query if the Julabo is running and store it in the class member
         'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_MODE_05")
-        if success:
+        _success, reply = self.query_("IN_MODE_05")
+        if isinstance(reply, str):
             try:
                 ans = bool(int(reply))
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.running = ans
                 return True
@@ -428,16 +434,16 @@
 
     def query_sub_temp(self) -> bool:
         """Query the low-temperature warning limit and store it in the class
         member 'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_SP_04")
-        if success:
+        _success, reply = self.query_("IN_SP_04")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.sub_temp = num
                 return True
@@ -451,16 +457,16 @@
 
     def query_over_temp(self) -> bool:
         """Query the high-temperature warning limit and store it in the class
         member 'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_SP_03")
-        if success:
+        _success, reply = self.query_("IN_SP_03")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.over_temp = num
                 return True
@@ -474,16 +480,16 @@
 
     def query_safe_temp(self) -> bool:
         """Query the screw-set excess temperature protection and store it in the
         class member 'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_PV_04")
-        if success:
+        _success, reply = self.query_("IN_PV_04")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.safe_temp = num
                 return True
@@ -497,16 +503,16 @@
 
     def query_safe_sens(self) -> bool:
         """Query the safety sensor temperature and store it in the class member
         'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_PV_03")
-        if success:
+        _success, reply = self.query_("IN_PV_03")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.safe_sens = num
                 return True
@@ -521,16 +527,16 @@
     def query_setpoint_preset(self) -> bool:
         """Query the setpoint preset currently used by the Julabo (#1, #2 or #3)
         and store it in the class member 'state'. Will be set to numpy.nan
         if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_MODE_01")
-        if success:
+        _success, reply = self.query_("IN_MODE_01")
+        if isinstance(reply, str):
             try:
                 num = int(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.setpoint_preset = num + 1
                 return True
@@ -569,16 +575,16 @@
 
     def query_setpoint_1(self) -> bool:
         """Query the temperature setpoint #1 and store it in the class member
         'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_SP_00")
-        if success:
+        _success, reply = self.query_("IN_SP_00")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.setpoint_1 = num
                 return True
@@ -592,16 +598,16 @@
 
     def query_setpoint_2(self) -> bool:
         """Query the temperature setpoint #2 and store it in the class member
         'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_SP_01")
-        if success:
+        _success, reply = self.query_("IN_SP_01")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.setpoint_2 = num
                 return True
@@ -615,16 +621,16 @@
 
     def query_setpoint_3(self) -> bool:
         """Query the temperature setpoint #3 and store it in the class member
         'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_SP_02")
-        if success:
+        _success, reply = self.query_("IN_SP_02")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.setpoint_3 = num
                 return True
@@ -638,16 +644,16 @@
 
     def query_bath_temp(self) -> bool:
         """Query the current bath temperature and store it in the class member
         'state'. Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_PV_00")
-        if success:
+        _success, reply = self.query_("IN_PV_00")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
             else:
                 self.state.bath_temp = num
                 return True
@@ -662,16 +668,16 @@
     def query_pt100_temp(self) -> bool:
         """Query the current external Pt100 temperature sensor and store it in
         the class member 'state'. Will be set to numpy.nan if no external sensor
         is connected or when communication is unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query_("IN_PV_02")
-        if success:
+        _success, reply = self.query_("IN_PV_02")
+        if isinstance(reply, str):
             if reply == "---.--":  # Not connected
                 self.state.pt100_temp = np.nan
                 return True
 
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
@@ -722,28 +728,31 @@
 
         # Update readings
         if update_readings:
             self.query_common_readings()
 
         # Print to terminal
         print(self.state.version)
-        print("%-*s: %-*s" % (w1, "Temp. unit", w2, C.temp_unit), end="")
-        print("%-*s: #%-*s" % (w1, "Sel. setp.", w2, C.setpoint_preset))
-        print("%-*s: %-*.2f" % (w1, "Sub temp.", w2, C.sub_temp), end="")
-        print("%-*s: %-*.2f" % (w1, "Over temp.", w2, C.over_temp))
-        print("%-*s  %-*s" % (w1, "", w2, ""), end="")
-        print("%-*s: %-*.2f" % (w1, "Safe temp.", w2, C.safe_temp))
+        print(f"{'Temp. unit':<{w1}s}: {C.temp_unit:<{w2}s}", end="")
+        print(f"{'Sel. setp.':<{w1}s}: {C.setpoint_preset:<{w2}.0f}")
+        print(f"{'Sub temp.':<{w1}s}: {C.sub_temp:<{w2}.2f}", end="")
+        print(f"{'Over temp.':<{w1}s}: {C.over_temp:<{w2}.2f}")
+        print(f"{'':<{w1}s}  {'':<{w2}s}", end="")
+        print(f"{'Safe temp.':<{w1}s}: {C.safe_temp:<{w2}.2f}")
         print()
-        print("%s" % ("--> RUNNING <--" if C.running else "IDLE"))
-        print("%-*s: %-*.2f" % (w1, "Setpoint", w2, C.setpoint), end="")
-        print("%-*s: %-*.2f" % (w1, "Bath temp.", w2, C.bath_temp))
-        print("%-*s: %-*.2f" % (w1, "Safe sens", w2, C.safe_sens), end="")
-        print("%-*s: %-*.2f" % (w1, "Pt100", w2, C.pt100_temp))
+        if not isinstance(C.running, bool):
+            print("COMMUNICATION ERROR")
+        else:
+            print("--> RUNNING <--" if C.running else "IDLE")
+        print(f"{'Setpoint':<{w1}s}: {C.setpoint:<{w2}.2f}", end="")
+        print(f"{'Bath temp.':<{w1}s}: { C.bath_temp:<{w2}.2f}")
+        print(f"{'Safe sens':<{w1}s}: {C.safe_sens:<{w2}.2f}", end="")
+        print(f"{'Pt100':<{w1}s}: {C.pt100_temp:<{w2}.2f}")
         print()
-        print("Status msg: %s" % C.status)
+        print(f"Status msg: {C.status}")
 
     # --------------------------------------------------------------------------
     #   query_
     # --------------------------------------------------------------------------
 
     def query_(self, *args, **kwargs) -> Tuple[bool, Union[str, bytes, None]]:
         """Wrapper for :meth:`dvg_qdevices.query` to add enforcing of time gaps
@@ -856,31 +865,31 @@
         sys.stdout.flush()
 
         # Process keyboard input
         if running_Windows:
             if msvcrt.kbhit():
                 key = msvcrt.getch()
 
-                if key == b"q" or key == b"Q":
+                if key in (b"q", b"Q"):
                     print("\nAre you sure you want to quit [y/n]?")
                     if msvcrt.getch() == b"y":
                         print("Switching off Julabo and quitting.")
                         done = True
 
-                elif key == b"s" or key == b"S":
-                    send_setpoint = input("\nEnter new setpoint: ")
+                elif key in (b"s", b"S"):
+                    user_input = input("\nEnter new setpoint: ")
 
                     try:
-                        send_setpoint = float(send_setpoint)
-                    except:
+                        send_setpoint = float(user_input)
+                    except Exception:
                         print("Error: Could not parse float value.")
                     else:
                         do_send_setpoint = True
 
-                elif key == b"o" or key == b"O":
+                elif key in (b"o", b"O"):
                     if julabo.state.running:
                         julabo.turn_off()
                     else:
                         julabo.turn_on()
 
         # Slow down update period
         time.sleep(0.5)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Keysight_3497xA_demo_logger.py` & `dvg-devices-1.4.0/src/dvg_devices/Keysight_3497xA_demo_logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,100 +2,39 @@
 # -*- coding: utf-8 -*-
 """Multithreaded PyQt/PySide GUI to interface with a Keysight (former HP or
 Agilent) 34970A/34972A data acquisition/switch unit.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+print(__url__)
+# pylint: disable=wrong-import-position, missing-function-docstring, bare-except
 
-import os
 import sys
 import time
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-# Parse optional cli argument to enfore a QT_LIB
-# cli example: python benchmark.py pyside6
-if len(sys.argv) > 1:
-    arg1 = str(sys.argv[1]).upper()
-    for i, lib in enumerate(QT_LIB_ORDER):
-        if arg1 == lib.upper():
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
+import qtpy
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Slot  # type: ignore
 
 import pyvisa
 import matplotlib.pyplot as plt
 import numpy as np
 import pyqtgraph as pg
 
 from dvg_pyqtgraph_threadsafe import (
+    ThreadSafeCurve,
     HistoryChartCurve,
     LegendSelect,
     PlotManager,
 )
-from dvg_pyqt_controls import (
-    create_Toggle_button,
-    SS_TEXTBOX_READ_ONLY,
-    SS_GROUP,
-)
+import dvg_pyqt_controls as controls
 from dvg_pyqt_filelogger import FileLogger
-
 from dvg_devices.Keysight_3497xA_protocol_SCPI import Keysight_3497xA
 from dvg_devices.Keysight_3497xA_qdev import Keysight_3497xA_qdev, INFINITY_CAP
 
 TRY_USING_OPENGL = True
 if TRY_USING_OPENGL:
     try:
         import OpenGL.GL as gl  # pylint: disable=unused-import
@@ -108,43 +47,95 @@
         pg.setConfigOptions(antialias=True)
         pg.setConfigOptions(enableExperimental=True)
 
 # Global pyqtgraph configuration
 # pg.setConfigOptions(leftButtonPan=False)
 pg.setConfigOption("foreground", "#EEE")
 
+# VISA address of the Keysight 3497xA data acquisition/switch unit containing a
+# multiplexer plug-in module. Hence, we simply call this device a 'mux'.
+# MUX_VISA_ADDRESS = "USB0::0x0957::0x2007::MY49018071::INSTR"
+MUX_VISA_ADDRESS = "GPIB0::9::INSTR"
+
+# SCPI commands to be send to the mux to set up the scan cycle.
+"""
+scan_list = "(@101:110)"
+MUX_SCPI_COMMANDS = [
+            f"rout:open {scan_list}",
+            f"conf:temp TC,J,{scan_list}",
+            f"unit:temp C,{scan_list}",
+            f"sens:temp:tran:tc:rjun:type INT,{scan_list}",
+            f"sens:temp:tran:tc:check ON,{scan_list}",
+            f"sens:temp:nplc 1,{scan_list}",
+            f"rout:scan {scan_list}",
+]
+"""
+
+scan_list = "(@101:110)"
+MUX_SCPI_COMMANDS = [
+    f"rout:open {scan_list}",
+    f"conf:res 1e6,{scan_list}",
+    f"sens:res:nplc 1,{scan_list}",
+    f"rout:scan {scan_list}",
+]
+
+# fmt: off
+DAQ_INTERVAL_MS   = 1000  # [ms] Update interval for the mux to perform a scan
+CHART_INTERVAL_MS = 1000  # [ms] Update interval for all charts
+CHART_CAPACITY    = 1800  # [samples]
+# fmt: on
+
+# Show debug info in terminal? Warning: Slow! Do not leave on unintentionally.
+DEBUG = False
 
 # ------------------------------------------------------------------------------
 #   MainWindow
 # ------------------------------------------------------------------------------
 
 
 class MainWindow(QtWid.QWidget):
-    def __init__(self, parent=None, **kwargs):
+    def __init__(
+        self,
+        qdev: Keysight_3497xA_qdev,
+        qlog: FileLogger,
+        parent=None,
+        **kwargs,
+    ):
         super().__init__(parent, **kwargs)
 
+        self.qdev = qdev
+        self.qlog = qlog
+
         self.setWindowTitle("Keysight 3497xA control")
-        self.setGeometry(600, 120, 1200, 600)
-        self.setStyleSheet(SS_TEXTBOX_READ_ONLY + SS_GROUP)
+        self.setGeometry(40, 60, 1200, 0)
+        self.setFont(QtGui.QFont("Arial", 9))
+        self.setStyleSheet(
+            controls.SS_TEXTBOX_READ_ONLY
+            + controls.SS_GROUP
+            + controls.SS_HOVER
+        )
+
+        self.timer_GUI = QtCore.QTimer()
+        self.timer_GUI.timeout.connect(self.update_GUI)
 
         # ----------------------------------------------------------------------
         #   Top grid
         # ----------------------------------------------------------------------
 
-        self.qlbl_title = QtWid.QLabel(
-            "Keysight 3497xA control",
-            font=QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold),
+        self.qlbl_title = QtWid.QLabel("Keysight 3497xA control")
+        self.qlbl_title.setFont(
+            QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold)
         )
         self.qlbl_cur_date_time = QtWid.QLabel("00-00-0000    00:00:00")
-        self.qpbt_record = create_Toggle_button(
+        self.qpbt_record = controls.create_Toggle_button(
             "Click to start recording to file", minimumHeight=40
         )
         self.qpbt_record.setMinimumWidth(400)
         # fmt: off
-        self.qpbt_record.clicked.connect(lambda state: log.record(state))  # pylint: disable=unnecessary-lambda
+        self.qpbt_record.clicked.connect(lambda state: qlog.record(state))  # pylint: disable=unnecessary-lambda
         # fmt: on
 
         self.qpbt_exit = QtWid.QPushButton("Exit")
         self.qpbt_exit.clicked.connect(self.close)
         self.qpbt_exit.setMinimumHeight(30)
 
         grid_top = QtWid.QGridLayout()
@@ -172,22 +163,42 @@
         self.pi_mux.setLabel("bottom", "history (min)", **p)
         self.pi_mux.setLabel("left", "misc. units", **p)
         self.pi_mux.setMenuEnabled(True)
         self.pi_mux.enableAutoRange(axis=pg.ViewBox.XAxis, enable=False)
         self.pi_mux.enableAutoRange(axis=pg.ViewBox.YAxis, enable=True)
         self.pi_mux.setAutoVisible(y=True)
 
-        # Placeholder to be populated depending on the number of scan channels
-        self.tscurves_mux = list()  # List of `HistoryChartCurve`
+        # ----------------------------------------------------------------------
+        #   Create history charts depending on the number of scan channels
+        # ----------------------------------------------------------------------
+
+        self.tscurves_mux: list[ThreadSafeCurve] = []
+
+        cm = plt.get_cmap("gist_rainbow")
+        for idx, channel in enumerate(qdev.dev.state.all_scan_list_channels):
+            color = cm(1.0 * idx / qdev.dev.state.N_channels)  # RGBA tuple
+            color = np.array(color) * 255
+            pen = pg.mkPen(color=color, width=2)
+
+            self.tscurves_mux.append(
+                HistoryChartCurve(
+                    capacity=CHART_CAPACITY,
+                    linked_curve=self.pi_mux.plot(pen=pen, name=channel),
+                )
+            )
 
         # ----------------------------------------------------------------------
         #   Legend
         # ----------------------------------------------------------------------
 
+        legend = LegendSelect(linked_curves=self.tscurves_mux)
+        legend.grid.setVerticalSpacing(0)
+
         self.qgrp_legend = QtWid.QGroupBox("Legend")
+        self.qgrp_legend.setLayout(legend.grid)
 
         # ----------------------------------------------------------------------
         #   PlotManager
         # ----------------------------------------------------------------------
 
         self.plot_manager = PlotManager(parent=self)
         self.plot_manager.add_autorange_buttons(linked_plots=self.pi_mux)
@@ -245,25 +256,29 @@
         vbox1 = QtWid.QVBoxLayout()
         vbox1.addWidget(
             self.qgrp_legend,
             stretch=0,
             alignment=QtCore.Qt.AlignmentFlag.AlignTop,
         )
         vbox1.addWidget(
-            qgrp_history, stretch=0, alignment=QtCore.Qt.AlignmentFlag.AlignTop
+            qgrp_history,
+            stretch=0,
+            alignment=QtCore.Qt.AlignmentFlag.AlignTop,
         )
         vbox1.addStretch(1)
 
         # ----------------------------------------------------------------------
         #   Round up full window
         # ----------------------------------------------------------------------
 
         hbox1 = QtWid.QHBoxLayout()
         hbox1.addWidget(
-            mux_qdev.qgrp, stretch=0, alignment=QtCore.Qt.AlignmentFlag.AlignTop
+            qdev.qgrp,
+            stretch=0,
+            alignment=QtCore.Qt.AlignmentFlag.AlignTop,
         )
         hbox1.addWidget(self.gw_mux, stretch=1)
         hbox1.addLayout(vbox1)
 
         vbox = QtWid.QVBoxLayout(self)
         vbox.addLayout(grid_top)
         vbox.addLayout(hbox1)
@@ -284,228 +299,141 @@
 
         # Update curves
         for tscurve in self.tscurves_mux:
             tscurve.update()
 
 
 # ------------------------------------------------------------------------------
-#   about_to_quit
-# ------------------------------------------------------------------------------
-
-
-def about_to_quit():
-    print("About to quit")
-    app.processEvents()
-    mux_qdev.quit()
-    log.close()
-
-    try:
-        mux.close()
-    except:
-        pass
-    try:
-        rm.close()
-    except:
-        pass
-
-
-# ------------------------------------------------------------------------------
-#   DAQ_postprocess_MUX_scan_function
-# ------------------------------------------------------------------------------
-
-
-def DAQ_postprocess_MUX_scan_function():
-    """Will be called during an 'worker_DAQ' update, after a mux scan has been
-    performed. We use it to parse out the scan readings into separate variables
-    and log it to file.
-    """
-    cur_date_time = QtCore.QDateTime.currentDateTime()
-    now = time.perf_counter()
-
-    # DEBUG info
-    # dprint("thread: %s" % QtCore.QThread.currentThread().objectName())
-
-    if mux_qdev.is_MUX_scanning:
-        readings = mux.state.readings
-        for idx in range(N_channels):
-            if readings[idx] > INFINITY_CAP:
-                readings[idx] = np.nan
-    else:
-        readings = [np.nan] * N_channels
-        mux.state.readings = readings
-
-    # Add readings to charts
-    for idx, tscurve in enumerate(window.tscurves_mux):
-        tscurve.appendData(now, readings[idx])
-
-    # Log data to file
-    log.update(
-        filepath="d:/data/mux_%s.txt" % cur_date_time.toString("yyMMdd_HHmmss"),
-        mode="w",
-    )
-
-
-# ------------------------------------------------------------------------------
-#   File logging
-# ------------------------------------------------------------------------------
-
-
-def write_header_to_log():
-    log.write("time [s]\t")
-    for i_ in range(N_channels - 1):
-        log.write("CH%s\t" % mux.state.all_scan_list_channels[i_])
-    log.write("CH%s\n" % mux.state.all_scan_list_channels[-1])
-
-
-def write_data_to_log():
-    log.write("%.3f" % log.elapsed())
-    for i_ in range(N_channels):
-        if len(mux.state.readings) <= i_:
-            log.write("\t%.5e" % np.nan)
-        else:
-            log.write("\t%.5e" % mux.state.readings[i_])
-    log.write("\n")
-
-
-# ------------------------------------------------------------------------------
 #   Main
 # ------------------------------------------------------------------------------
 
 if __name__ == "__main__":
-    # VISA address of the Keysight 3497xA data acquisition/switch unit
-    # containing a multiplexer plug-in module. Hence, we simply call this device
-    # a 'mux'.
-    MUX_VISA_ADDRESS = "USB0::0x0957::0x2007::MY49018071::INSTR"
-    # MUX_VISA_ADDRESS = "GPIB0::9::INSTR"
-
-    # A scan will be performed by the mux every N milliseconds
-    MUX_SCANNING_INTERVAL_MS = 1000  # [ms]
-
-    # Chart history (CH) buffer sizes in [samples].
-    # Multiply this with the corresponding SCANNING_INTERVAL constants to get
-    # the history size in time.
-    CH_SAMPLES_MUX = 1800
-
-    # The chart will be updated at this interval
-    UPDATE_INTERVAL_GUI = 1000  # [ms]
-
-    # SCPI commands to be send to the 3497xA to set up the scan cycle.
-    # """
-    scan_list = "(@301:310)"
-    MUX_SCPI_COMMANDS = [
-        "rout:open %s" % scan_list,
-        "conf:temp TC,J,%s" % scan_list,
-        "unit:temp C,%s" % scan_list,
-        "sens:temp:tran:tc:rjun:type INT,%s" % scan_list,
-        "sens:temp:tran:tc:check ON,%s" % scan_list,
-        "sens:temp:nplc 1,%s" % scan_list,
-        "rout:scan %s" % scan_list,
-    ]
-    # """
-    """
-    scan_list = "(@101)"
-    MUX_SCPI_COMMANDS = [
-        "rout:open %s" % scan_list,
-        "conf:res 1e5,%s" % scan_list,
-        "sens:res:nplc 1,%s" % scan_list,
-        "rout:scan %s" % scan_list,
-    ]
-    """
 
     # --------------------------------------------------------------------------
     #   Connect to Keysight 3497xA (mux)
     # --------------------------------------------------------------------------
 
     rm = pyvisa.ResourceManager()
-
     mux = Keysight_3497xA(MUX_VISA_ADDRESS, "MUX")
-    if mux.connect(rm):
-        mux.begin(MUX_SCPI_COMMANDS)
+
+    try:
+        if mux.connect(rm):
+            mux.begin(MUX_SCPI_COMMANDS)
+    except ValueError as e:
+        # No connection could be made to the VISA device because module
+        # dependencies are missing. Print error, not raise and continue to
+        # show the GUI.
+        print(e)
 
     # --------------------------------------------------------------------------
     #   Create application
     # --------------------------------------------------------------------------
-    QtCore.QThread.currentThread().setObjectName("MAIN")  # For DEBUG info
-
-    app = QtWid.QApplication(sys.argv)
-    app.setFont(QtGui.QFont("Arial", 9))
-    app.aboutToQuit.connect(about_to_quit)
 
-    # Create PyQt GUI interfaces and communication threads per 3497xA
-    mux_qdev = Keysight_3497xA_qdev(
-        dev=mux,
-        DAQ_interval_ms=MUX_SCANNING_INTERVAL_MS,
-        DAQ_postprocess_MUX_scan_function=DAQ_postprocess_MUX_scan_function,
-    )
-    mux_qdev.set_table_readings_format("%.5e")
-    mux_qdev.qgrp.setFixedWidth(420)
+    main_thread = QtCore.QThread.currentThread()
+    if isinstance(main_thread, QtCore.QThread):
+        main_thread.setObjectName("MAIN")  # For DEBUG info
 
-    # Create window
-    window = MainWindow()
+    if qtpy.PYQT6 or qtpy.PYSIDE6:
+        sys.argv += ["-platform", "windows:darkmode=0"]
+    app = QtWid.QApplication(sys.argv)
+    app.setStyle("Fusion")
 
     # --------------------------------------------------------------------------
-    #   Create history charts depending on the number of scan channels
+    #   Set up communication threads for the mux
     # --------------------------------------------------------------------------
 
-    N_channels = len(mux.state.all_scan_list_channels)
+    def postprocess_mux_fun():
+        """Will be called during an 'worker_DAQ' update, after a mux scan has
+        been performed. We use it to parse out the scan readings into separate
+        variables and log it to file.
+        """
+        cur_date_time = QtCore.QDateTime.currentDateTime()
+        now = time.perf_counter()
 
-    # Create thread-safe `HistoryChartCurve`s, aka `tscurves`
-    cm = plt.get_cmap("gist_rainbow")
-    for i in range(N_channels):
-        color = cm(1.0 * i / N_channels)  # Color will now be an RGBA tuple
-        color = np.array(color) * 255
-        pen = pg.mkPen(color=color, width=2)
+        # DEBUG info
+        # dprint(f"thread: {QtCore.QThread.currentThread().objectName()}")
 
-        window.tscurves_mux.append(
-            HistoryChartCurve(
-                capacity=CH_SAMPLES_MUX,
-                linked_curve=window.pi_mux.plot(
-                    pen=pen, name=mux.state.all_scan_list_channels[i]
-                ),
-            )
+        if mux_qdev.is_MUX_scanning:
+            readings = mux.state.readings
+            for idx in range(mux.state.N_channels):
+                if readings[idx] > INFINITY_CAP:
+                    readings[idx] = np.nan
+        else:
+            readings = [np.nan] * mux.state.N_channels
+            mux.state.readings = readings
+
+        # Add readings to charts
+        for idx, tscurve in enumerate(window.tscurves_mux):
+            tscurve.appendData(now, readings[idx])
+
+        # Log data to file
+        log.update(
+            filepath=f"data_mux_{cur_date_time.toString('yyMMdd_HHmmss')}.txt",
+            mode="w",
         )
 
-    legend = LegendSelect(linked_curves=window.tscurves_mux)
-    legend.grid.setVerticalSpacing(0)
-    window.qgrp_legend.setLayout(legend.grid)
+    mux_qdev = Keysight_3497xA_qdev(
+        dev=mux,
+        DAQ_interval_ms=DAQ_INTERVAL_MS,
+        DAQ_postprocess_MUX_scan_function=postprocess_mux_fun,
+        debug=DEBUG,
+    )
+    # mux_qdev.set_table_readings_format(".5e")
+    mux_qdev.start()
 
     # --------------------------------------------------------------------------
     #   File logger
     # --------------------------------------------------------------------------
 
+    def write_header_to_log():
+        ch_labels = [f"CH{ch}" for ch in mux.state.all_scan_list_channels]
+        log.write("time [s]\t")
+        log.write(f"{chr(9).join(ch_labels)}")  # [TAB]-delimited
+        log.write("\n")
+
+    def write_data_to_log():
+        log.write(f"{log.elapsed():.3f}")
+        for idx, _ch in enumerate(mux.state.all_scan_list_channels):
+            if len(mux.state.readings) <= idx:
+                log.write(f"\t{np.nan:.5e}")
+            else:
+                log.write(f"\t{mux.state.readings[idx]:.5e}")
+        log.write("\n")
+
     log = FileLogger(
         write_header_function=write_header_to_log,
         write_data_function=write_data_to_log,
     )
     log.signal_recording_started.connect(
         lambda filepath: window.qpbt_record.setText(
-            "Recording to file: %s" % filepath
+            f"Recording to file: {filepath}"
         )
     )
     log.signal_recording_stopped.connect(
         lambda: window.qpbt_record.setText("Click to start recording to file")
     )
 
     # --------------------------------------------------------------------------
-    #   Start threads
-    # --------------------------------------------------------------------------
-
-    mux_qdev.start()
-
-    # --------------------------------------------------------------------------
-    #   Set up timers
+    #   Start the main GUI event loop
     # --------------------------------------------------------------------------
 
-    timer_GUI = QtCore.QTimer()
-    timer_GUI.timeout.connect(window.update_GUI)
-    timer_GUI.start(UPDATE_INTERVAL_GUI)
+    def about_to_quit():
+        print("About to quit")
+        app.processEvents()
+        mux_qdev.quit()
+        try:
+            mux.close()
+        except:
+            pass
+        try:
+            rm.close()
+        except:
+            pass
 
-    # --------------------------------------------------------------------------
-    #   Start the main GUI event loop
-    # --------------------------------------------------------------------------
+    app.aboutToQuit.connect(about_to_quit)
 
+    window = MainWindow(qdev=mux_qdev, qlog=log)
     window.plot_manager.perform_preset(2)  # Init time axis of the history chart
+    window.timer_GUI.start(CHART_INTERVAL_MS)
     window.show()
-    if QT_LIB in (PYQT5, PYSIDE2):
-        sys.exit(app.exec_())
-    else:
-        sys.exit(app.exec())
+
+    sys.exit(app.exec())
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Keysight_3497xA_protocol_SCPI.py` & `dvg-devices-1.4.0/src/dvg_devices/Keysight_3497xA_protocol_SCPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 
 State variables that are an empty list [] indicate that they are uninitialized
 or that the previous query resulted in a communication error.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "14-09-2022"
-__version__ = "1.0.0"
-# pylint: disable=try-except-raise
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, multiple-statements
 
 import time
+from typing import Union, Tuple, List
 
-# TODO: Current demanded requirement pyvisa~=1.11 was ~=1.9 before. 1.11 has
-# broken backwards comp. Still need to test if all is still fine. Delete this
-# comment if tested okay.
 import pyvisa
 import numpy as np
 
 from dvg_debug_functions import print_fancy_traceback
 
 WRITE_TERMINATION = "\n"
 READ_TERMINATION = "\n"
@@ -79,80 +77,84 @@
         An empty list [] indicates that the parameter is not initialized or
         that the last query was unsuccessful in communication.
         """
 
         # All the channels in the scan list retreived from the 3497xA [list of
         # strings]. This can be used to e.g. populate a table view with correct
         # labels.
-        all_scan_list_channels = []
+        all_scan_list_channels: List[str] = []
+
+        # Number of channels making up the scan list
+        N_channels: int = 0
 
         # List of readings returned by the device after a full scan cycle
         readings = []
 
         # The single error string retreived from the error queue of the device.
         # None indicates no error is left in the queue.
-        error = None
+        error: Union[str, None] = None
 
         # This list of strings is provided to be able to store all errors from
         # the device queue. This list is populated by calling 'query_error'
         # until no error is left in the queue. This list can then be printed to
         # screen or GUI and the user should 'acknowledge' the list, after which
         # the list can be emptied (=[]) again.
-        all_errors = []
+        all_errors: List[str] = []
 
     class Diag:
         """Container for the diagnostic information.
         [numpy.nan] values indicate that the parameter is not initialized or
         that the last query was unsuccessful in communication.
         """
 
         # Cycle count of the three backplane relays on the internal DMM.
         # diag:dmm:cycl?
-        slot_1_DMM_cycles = np.nan
-        slot_2_DMM_cycles = np.nan
-        slot_3_DMM_cycles = np.nan
+        slot_1_DMM_cycles: Union[float, int] = np.nan
+        slot_2_DMM_cycles: Union[float, int] = np.nan
+        slot_3_DMM_cycles: Union[float, int] = np.nan
 
         # Identity of the three plug-in modules in the specified slot.
         # syst:ctyp?
-        slot_1_ctype = "none"
-        slot_2_ctype = "none"
-        slot_3_ctype = "none"
+        slot_1_ctype: str = "none"
+        slot_2_ctype: str = "none"
+        slot_3_ctype: str = "none"
 
         # Custom label of up to 10 characters stored in non-volatile memory
         # of the module in the specified slot. We have used it to store the
         # serial number of the module as printed on its back.
         # diag:peek:slot:data?
-        slot_1_label = np.nan
-        slot_2_label = np.nan
-        slot_3_label = np.nan
+        slot_1_label: str = ""
+        slot_2_label: str = ""
+        slot_3_label: str = ""
 
         # Cycle count on all available channels of the specified slot.
         # diag:rel:cycl?
         slot_1_relay_cycles = []
         slot_2_relay_cycles = []
         slot_3_relay_cycles = []
 
     # --------------------------------------------------------------------------
     #   __init__
     # --------------------------------------------------------------------------
 
-    def __init__(self, visa_address=None, name="MUX"):
+    def __init__(self, visa_address: str = "", name: str = "MUX"):
         """
         Args:
-            visa_address (str): VISA device address
+            visa_address (`str`):
+                VISA device address
         """
         self._visa_address = visa_address
         self.name = name
-        self._idn = None  # The identity of the device ("*IDN?")
+        self._idn: str = ""  # The identity of the device ("*IDN?")
 
         # Placeholder for the VISA device instance
-        self.device = None
+        self.device: Union[pyvisa.resources.MessageBasedResource, None] = None
 
         # Is the connection to the device alive?
-        self.is_alive = False
+        self.is_alive: bool = False
 
         # Container for the process and measurement variables
         self.state = self.State()
 
         # Container for the diagnostic relay cycle counts.
         self.diag = self.Diag()
 
@@ -168,89 +170,98 @@
             self.device.close()
             self.is_alive = False
 
     # --------------------------------------------------------------------------
     #   connect
     # --------------------------------------------------------------------------
 
-    def connect(self, rm):
+    def connect(self, rm: pyvisa.ResourceManager) -> bool:
         """Try to connect to the device over VISA at the given address. When
         succesful the VISA device instance will be stored in member 'device'
         and its identity is queried and stored in '_idn'.
 
         Args:
-            rm: Instance of pyvisa.ResourceManager
+            rm `(pyvisa.ResourceManager)`:
+                Instance of VISA ResourceManager.
 
         Returns: True if successful, False otherwise.
         """
         self.is_alive = False
 
         print("Connect to: Keysight 3497xA")
-        print("  @ %s : " % self._visa_address, end="")
+        print(f"  @ {self._visa_address} : ", end="")
+
         try:
-            self.device = rm.open_resource(
-                self._visa_address, timeout=VISA_TIMEOUT
-            )
-            self.device.clear()
+            device = rm.open_resource(self._visa_address, timeout=VISA_TIMEOUT)
+            device.clear()
         except pyvisa.VisaIOError:
             print("Could not open resource.\n")
             return False
-        except:
-            raise
+        except Exception as err:
+            raise err
+
+        if not isinstance(device, pyvisa.resources.MessageBasedResource):
+            print("ERROR: Device is not a `MessageBasedResource`.")
+            return False
+
         print("Success!")
+        self.device = device
         self.is_alive = True
         self.device.write_termination = WRITE_TERMINATION
         self.device.read_termination = READ_TERMINATION
 
-        success, self._idn = self.query("*idn?")
+        _success, reply = self.query("*idn?")
         self.wait_for_OPC()
 
-        if success:
-            print("  %s\n" % self._idn)
-            return True
+        if not isinstance(reply, str):
+            return False
 
-        return False
+        self._idn = reply
+        print(f"  {self._idn}\n")
+        return True
 
     # --------------------------------------------------------------------------
     #   begin
     # --------------------------------------------------------------------------
 
-    def begin(self, SCPI_setup_commands=None):
+    def begin(self, SCPI_setup_commands: Union[List[str], None] = None) -> bool:
         """This function should run directly after having established a
         connection to a 3497xA.
 
         Args:
-            SCPI_setup_commands (list of strings): List of SCPI commands to be
-            send to the 3497xA to set up the scan cycle. [None]: The previously
-            passed set of commands remain valid. []: All commands will be
-            cleared.
+            SCPI_setup_commands (`list[str]` | `None`):
+                List of SCPI commands to be send to the 3497xA to set up the
+                scan cycle. [None]: The previously passed set of commands remain
+                valid. []: All commands will be cleared.
 
         Returns: True if all messages were sent and received successfully,
             False otherwise.
         """
         # Clear errors
         self.state.error = None
         self.state.all_errors = []
 
         # Store SCPI setup commands
         if SCPI_setup_commands is not None:
             self.SCPI_setup_commands = SCPI_setup_commands
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return False
 
         # Flag to determine if the status byte register of the device
         # (device.stb) can be used to poll for any errors in the device queue.
         if self._idn.lower().find("hewlett") >= 0:
             # E.g. 'HEWLETT-PACKARD,34970A,0,13-2-2'
             self.can_check_error_queue_by_polling_stb = False
         elif self._idn.lower().find("agilent") >= 0:
             # E.g. 'Agilent Technologies,34972A,MY49018071,1.16-1.12-02-02'
-            self.can_check_error_queue_by_polling_stb = False  # Is actually True, but .stb malfunctions and causes locked up device
+            self.can_check_error_queue_by_polling_stb = False
+            # Above is actually True, but .stb malfunctions and causes locked up
+            # device, hence set to False.
         else:
             self.can_check_error_queue_by_polling_stb = False
 
         # fmt: off
         success = self.abort_reset_clear()
         success &= self.query_diagnostics()             ; self.wait_for_OPC()
         success &= self.perform_SCPI_setup_commands()   ; self.wait_for_OPC()
@@ -261,176 +272,181 @@
 
         return success
 
     # --------------------------------------------------------------------------
     #   write
     # --------------------------------------------------------------------------
 
-    def write(self, msg_str):
+    def write(self, msg_str: str) -> bool:
         """Try to write a command to the device.
 
         Args:
-            msg_str (string): Message to be sent.
+            msg_str (`str`):
+                Message to be sent.
 
         Returns: True if the message was sent successfully, False otherwise.
             NOTE: It does not indicate whether the message made sense to the
             device.
         """
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return False
 
         try:
             self.device.write(msg_str)
         except pyvisa.VisaIOError as err:
             # Print error and struggle on
-            print_fancy_traceback(err, 3)
+            print_fancy_traceback(err)
             return False
-        except:
-            raise
+        except Exception as err:
+            raise err
 
         return True
 
     # --------------------------------------------------------------------------
     #   query
     # --------------------------------------------------------------------------
 
-    def query(self, msg_str):
+    def query(self, msg_str: str) -> Tuple[bool, Union[str, None]]:
         """Try to query the device.
 
         Args:
-            msg_str (string): Message to be sent.
+            msg_str (`str`):
+                Message to be sent.
 
         Returns:
-            success (bool): True if the message was sent and a reply was
-                received successfully, False otherwise.
-            ans_str (string): Reply received from the device. [numpy.nan] if
-                unsuccessful.
+            success (`bool`):
+                True if the message was sent and a reply was received
+                successfully, False otherwise.
+
+            reply (`str` | `None`):
+                Reply received from the device. None if unsuccessful.
         """
         success = False
-        ans_str = np.nan
+        reply = None
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
+            return success, reply
+
+        try:
+            reply = self.device.query(msg_str)
+        except pyvisa.VisaIOError as err:
+            # Print error and struggle on
+            print_fancy_traceback(err)
+        except Exception as err:
+            raise err
         else:
-            try:
-                ans_str = self.device.query(msg_str)
-            except pyvisa.VisaIOError as err:
-                # Print error and struggle on
-                print_fancy_traceback(err, 3)
-            except:
-                raise
-            else:
-                ans_str = ans_str.strip()
-                success = True
+            reply = reply.strip()
+            success = True
 
-        return success, ans_str
+        return success, reply
 
     # --------------------------------------------------------------------------
     #   query_ascii_values
     # --------------------------------------------------------------------------
 
-    def query_ascii_values(self, msg_str):
+    def query_ascii_values(self, msg_str: str) -> Tuple[bool, list]:
         """Try to query the device.
 
         Args:
-            msg_str (string): Message to be sent.
+            msg_str (`str`):
+                Message to be sent.
 
         Returns:
-            success (bool): True if the message was sent and a reply was
-                received successfully, False otherwise.
-            ans_list (list): Reply received from the device. Empty list [] if
-                unsuccessful.
+            success (`bool`):
+                True if the message was sent and a reply was received
+                successfully, False otherwise.
+
+            ans_list (`list`):
+                Reply received from the device. Empty list [] if unsuccessful.
         """
         success = False
         ans_list = []
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
+            return success, ans_list
+
+        try:
+            ans_list = list(self.device.query_ascii_values(msg_str))
+        except pyvisa.VisaIOError as err:
+            # Print error and struggle on
+            print_fancy_traceback(err)
+        except Exception as err:
+            raise err
         else:
-            try:
-                ans_list = self.device.query_ascii_values(msg_str)
-            except pyvisa.VisaIOError as err:
-                # Print error and struggle on
-                print_fancy_traceback(err, 3)
-            except:
-                raise
-            else:
-                success = True
+            success = True
 
         return success, ans_list
 
     # --------------------------------------------------------------------------
     #   query_diagnostics
     # --------------------------------------------------------------------------
 
-    def query_diagnostics(self, verbose=False):
+    def query_diagnostics(self, verbose: bool = False) -> bool:
         """
         Returns: True if all messages were sent and received successfully,
             False otherwise.
         """
         all_success = True
 
         # Retrieve relay cycle counts of internal DMM
         success, DMM_cycles = self.query_ascii_values("diag:dmm:cycl?")
         all_success &= success
 
-        if success:
-            [
-                self.diag.slot_1_DMM_cycles,
-                self.diag.slot_2_DMM_cycles,
-                self.diag.slot_3_DMM_cycles,
-            ] = DMM_cycles
+        if len(DMM_cycles) == 3:
+            self.diag.slot_1_DMM_cycles = DMM_cycles[0]
+            self.diag.slot_2_DMM_cycles = DMM_cycles[1]
+            self.diag.slot_3_DMM_cycles = DMM_cycles[2]
         else:
-            [
-                self.diag.slot_1_DMM_cycles,
-                self.diag.slot_2_DMM_cycles,
-                self.diag.slot_3_DMM_cycles,
-            ] = [np.nan] * 3
+            self.diag.slot_1_DMM_cycles = np.nan
+            self.diag.slot_2_DMM_cycles = np.nan
+            self.diag.slot_3_DMM_cycles = np.nan
 
         # Check all 3 slots for installed modules. Create a list of all
         # available channels if a multiplexer module is installed. This list
         # will be used to retreive the relay cycle count of each channel.
         ch_list_SCPI = ""
 
         for i in range(3):
             bank = 100 * (i + 1)
-            success, slot_ctype = self.query("syst:ctyp? %i" % bank)
+            success, slot_ctype = self.query(f"syst:ctyp? {bank}")
             all_success &= success
 
-            if success:
+            if isinstance(slot_ctype, str):
                 if slot_ctype.find(",0,0,0") > -1:
                     N_chans = 0
                     slot_ctype = "none"
                 elif slot_ctype.find("34901A") > -1:
                     N_chans = 20
                 elif slot_ctype.find("34902A") > -1:
                     N_chans = 16
                 else:
                     N_chans = 0
             else:
                 slot_ctype = "none"
                 N_chans = 0
 
             if slot_ctype == "none":
-                slot_label = np.nan
+                slot_label = ""
             else:
-                success, slot_label = self.query(
-                    "diag:peek:slot:data? %i" % bank
-                )
+                success, slot_label = self.query(f"diag:peek:slot:data? {bank}")
                 all_success &= success
 
-                if success:
+                if isinstance(slot_label, str):
                     slot_label = slot_label.strip('"')
+                else:
+                    slot_label = ""
 
             if N_chans > 0:
-                ch_list_SCPI = "%i:%i" % (bank + 1, bank + N_chans)
+                ch_list_SCPI = f"{bank + 1}:{bank + N_chans}"
                 success, relay_cycles = self.query_ascii_values(
-                    "diag:rel:cycl? (@%s)" % ch_list_SCPI
+                    f"diag:rel:cycl? (@{ch_list_SCPI})"
                 )
                 all_success &= success
 
                 if not success:
                     relay_cycles = []
             else:
                 relay_cycles = []
@@ -455,17 +471,17 @@
 
     # --------------------------------------------------------------------------
     #   report_diagnostics
     # --------------------------------------------------------------------------
 
     def report_diagnostics(self):
         print("  Relay cycle count internal DMM:")
-        print("    slot 1: %.1e" % self.diag.slot_1_DMM_cycles)
-        print("    slot 2: %.1e" % self.diag.slot_2_DMM_cycles)
-        print("    slot 3: %.1e" % self.diag.slot_3_DMM_cycles)
+        print(f"    slot 1: {self.diag.slot_1_DMM_cycles:.1e}")
+        print(f"    slot 2: {self.diag.slot_2_DMM_cycles:.1e}")
+        print(f"    slot 3: {self.diag.slot_3_DMM_cycles:.1e}")
         print("")
 
         for i in range(3):
             if i == 0:
                 slot_ctype = self.diag.slot_1_ctype
                 slot_label = self.diag.slot_1_label
                 relay_cycles = self.diag.slot_1_relay_cycles
@@ -474,36 +490,36 @@
                 slot_label = self.diag.slot_2_label
                 relay_cycles = self.diag.slot_2_relay_cycles
             if i == 2:
                 slot_ctype = self.diag.slot_3_ctype
                 slot_label = self.diag.slot_3_label
                 relay_cycles = self.diag.slot_3_relay_cycles
 
-            print("  Slot %i:" % (i + 1))
-            print("    %s" % slot_ctype)
+            print(f"  Slot {(i + 1)}:")
+            print(f"    {slot_ctype}")
             if slot_ctype != "none":
-                print("    Serial: %s" % slot_label)
-            if not (relay_cycles == []):
+                print(f"    Serial: {slot_label}")
+            if not relay_cycles == []:
                 print("    Relay cycle count")
-                for j in range(len(relay_cycles)):
-                    print("      ch %2i: %8i" % (j + 1, relay_cycles[j]))
+                for count, item in enumerate(relay_cycles):
+                    print(f"      ch {count + 1:2}: {item:8}")
             print("")
 
     # --------------------------------------------------------------------------
     #   System status related
     # --------------------------------------------------------------------------
 
-    def abort_reset_clear(self):
+    def abort_reset_clear(self) -> bool:
         """Abort measurement, reset device and clear status. Return when this
         operation has completed on the device. Blocking.
 
         Returns: True if the message was sent successfully, False otherwise.
         """
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return False
 
         # The reset operation can take a long time to complete. Momentarily
         # increase the timeout to 2000 msec if necessary.
         self.device.timeout = max(self.device.timeout, 2000)
 
@@ -535,107 +551,112 @@
         Will wait indefinitely for all device operations to complete. Blocking.
 
         Make sure that the ESR is set to signal bit 0 - OPC (operation complete)
         before you call this function. This can be done by calling
         'prepare_wait_for_OPC_indefinitely()'.
         """
 
+        if not self.is_alive or self.device is None:
+            print("ERROR: Device is not connected yet or already closed.")
+            return
+
         # Let the device set the ESR bit 0 - OPC (operation complete) to 1 after
         # all device operations have completed.
         self.write("*opc")
 
         # Poll the OPC status bit for 'operation complete'. This is the 5th
         # bit.
         while not (self.device.stb & 0b100000) == 0b100000:
             time.sleep(0.01)
 
         # Reset the ESR bit 0 - OPC back to 0.
         self.query("*esr?")
 
-    def prepare_wait_for_OPC_indefinitely(self):
+    def prepare_wait_for_OPC_indefinitely(self) -> bool:
         """Set the ESR to signal bit 0 - OPC (operation complete). Should be
         called only once after a '*rst' in case you want to make use of
         'wait_for_OPC_indefinitely()'.
 
         Returns: True if the message was sent successfully, False otherwise.
         """
         return self.write("*ese 1")
 
-    def query_error(self, verbose=False):
+    def query_error(self, verbose: bool = False) -> bool:
         """Pop one error string from the error queue of the device and store it
         in the 'State'-class member. A value of None indicates no error is left.
 
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, self.state.error = self.query("syst:err?")
-        if success:
+        success, reply = self.query("syst:err?")
+        if isinstance(reply, str):
+            self.state.error = reply
             if self.state.error.find(STR_NO_ERROR) == 0:
                 self.state.error = None
             else:
                 if verbose:  # DEBUG INFO
-                    print("  %s" % self.state.error)
+                    print(f"  {self.state.error}")
         return success
 
-    def query_all_errors_in_queue(self, verbose=False):
+    def query_all_errors_in_queue(self, verbose: bool = False):
         """Check if there are errors in the device queue and retrieve all if
         any and append these to 'state.all_errors'.
         """
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return
 
         if self.can_check_error_queue_by_polling_stb:
             # Fast polling method
             if (self.device.stb & 0b100) == 0b100:
                 # There are unread errors in the queue available. Retrieve all.
                 while True:
                     if self.query_error():
                         if self.state.error is None:
                             break
-                        else:
-                            self.state.all_errors.append(self.state.error)
+
+                        self.state.all_errors.append(self.state.error)
                     else:
                         break
         else:
             # Slow full query method
             while True:
                 if self.query_error():
                     if self.state.error is None:
                         break
-                    else:
-                        self.state.all_errors.append(self.state.error)
+
+                    self.state.all_errors.append(self.state.error)
                 else:
                     break
 
         if verbose:  # DEBUG INFO
             for error in self.state.all_errors:
-                print("  %s" % error)
+                print(f"  {error}")
 
-    def set_display_text(self, str_text):
+    def set_display_text(self, str_text) -> bool:
         """
         Returns: True if the message was sent successfully, False otherwise.
         """
-        return self.write("disp:text '%s'" % str_text)
+        return self.write(f"disp:text '{str_text}'")
 
     # --------------------------------------------------------------------------
     #   Acquisition related
     # --------------------------------------------------------------------------
 
-    def perform_SCPI_setup_commands(self):
+    def perform_SCPI_setup_commands(self) -> bool:
         """
         Returns: True if all messages were sent successfully, False otherwise.
         """
         success = True
         for command in self.SCPI_setup_commands:
             success &= self.write(command)
         self.wait_for_OPC()
 
         return success
 
-    def init_scan(self):
+    def init_scan(self) -> bool:
         """Initialize the scan, i.e. start with the acquisition of data over
         all channels as programmed. Non-blocking.
 
         You can check for the scan to have completed by calling
         'wait_for_OPC()' and subsequently retrieve the scanned data from the
         device buffer, like this:
             k3497xA.init_scan()
@@ -649,49 +670,53 @@
             k3497xA.wait_for_OPC_indefinitely()
             k3497xA.fetch_scan()
 
         Returns: True if the message was sent successfully, False otherwise.
         """
         return self.write("init")
 
-    def fetch_scan(self):
+    def fetch_scan(self) -> bool:
         """Retreive the last scanned data from the device buffer. The data
         will be stored in state variable 'state.readings'.
 
         Returns: True if the query was received successfully, False otherwise.
         """
         success, self.state.readings = self.query_ascii_values("fetc?")
 
         return success
 
-    def init_scan_and_wait_for_OPC_indefinitely_and_fetch(self):
+    def init_scan_and_wait_for_OPC_indefinitely_and_fetch(self) -> bool:
         """Blocking and mainly for testing purposes as there will be limited
         use for this series of instructions that could be blocking indefinitely.
         The scanned data will be stored in state variable 'state.readings'.
 
         Returns: True if the query was received successfully, False otherwise.
         """
         self.prepare_wait_for_OPC_indefinitely()
         success = self.init_scan()
         self.wait_for_OPC_indefinitely()
         success &= self.fetch_scan()
         # print(self.state.readings[1])
 
         return success
 
-    def query_all_scan_list_channels(self):
+    def query_all_scan_list_channels(self) -> bool:
         """Query the channels in the currently programmed scan list of the
         3497xA. This can be used to e.g. populate a table view with correct
         labels. The scan list channel names will be stored in state variable
-        'state.all_scan_list_channels'.
+        'state.all_scan_list_channels' and the total number of channels in
+        'state.N_channels'.
 
         Returns: True if the query was received successfully, False otherwise.
         """
 
-        success, str_ans = self.query("rout:scan?")
-        if success:
-            tmp = str_ans[str_ans.find("@") + 1 :].strip(")")
+        success, reply = self.query("rout:scan?")
+
+        if isinstance(reply, str):
+            tmp = reply[reply.find("@") + 1 :].strip(")")
             if tmp != "":
                 self.state.all_scan_list_channels = tmp.split(",")
-        self.wait_for_OPC()
 
+        self.state.N_channels = len(self.state.all_scan_list_channels)
+
+        self.wait_for_OPC()
         return success
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Keysight_3497xA_qdev.py` & `dvg-devices-1.4.0/src/dvg_devices/Keysight_3497xA_qdev.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,86 +6,29 @@
 This library is intended to be used with multiplexer board(s), as it will
 scan over the board's input channels to retrieve the readings. Hence, we also
 refer to this device as a multiplexer, or mux.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=broad-except
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, broad-except, multiple-statements
 
-import os
-import sys
 import time
+from typing import Union, List
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Slot  # type: ignore
 
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
-from dvg_pyqt_controls import (
-    create_Toggle_button,
-    SS_TEXTBOX_ERRORS,
-    SS_TEXTBOX_READ_ONLY,
-    SS_GROUP,
-)
+import dvg_pyqt_controls as controls
 from dvg_debug_functions import dprint, print_fancy_traceback as pft
-
 from dvg_qdeviceio import QDeviceIO, DAQ_TRIGGER
 from dvg_devices.Keysight_3497xA_protocol_SCPI import Keysight_3497xA
 
-
 # Monospace font
 FONT_MONOSPACE = QtGui.QFont("Monospace", 12, weight=QtGui.QFont.Weight.Bold)
 FONT_MONOSPACE.setStyleHint(QtGui.QFont.StyleHint.TypeWriter)
 
 FONT_MONOSPACE_SMALL = QtGui.QFont("Monospace", 9)
 FONT_MONOSPACE_SMALL.setStyleHint(QtGui.QFont.StyleHint.TypeWriter)
 
@@ -156,14 +99,15 @@
         DAQ_timer_type=QtCore.Qt.TimerType.CoarseTimer,
         critical_not_alive_count=3,
         DAQ_postprocess_MUX_scan_function=None,
         debug=False,
         **kwargs,
     ):
         super().__init__(dev, **kwargs)  # Pass kwargs onto QtCore.QObject()
+        self.dev: Keysight_3497xA  # Enforce type: removes `_NoDevice()`
 
         self.create_worker_DAQ(
             DAQ_trigger=DAQ_TRIGGER.INTERNAL_TIMER,
             DAQ_function=self.DAQ_function,
             DAQ_interval_ms=DAQ_interval_ms,
             DAQ_timer_type=DAQ_timer_type,
             critical_not_alive_count=critical_not_alive_count,
@@ -171,20 +115,20 @@
         )
 
         self.create_worker_jobs(jobs_function=self.jobs_function, debug=debug)
 
         self.DAQ_postprocess_MUX_scan_function = (
             DAQ_postprocess_MUX_scan_function
         )
-        self.is_MUX_scanning = False
+        self.is_MUX_scanning: bool = False
 
         # String format to use for the readings in the table widget.
         # When type is a single string, all rows will use this format.
         # When type is a list of strings, rows will be formatted consecutively.
-        self.table_readings_format = "%.3e"
+        self.table_readings_format: Union[str, List[str]] = ".5e"
 
         self.create_GUI()
         self.signal_DAQ_updated.connect(self.update_GUI)
 
         # Populate the table view with QTableWidgetItems.
         # I.e. add the correct number of rows to the table depending on the
         # full scan list.
@@ -222,76 +166,78 @@
         self.signal_DAQ_updated.emit()  # Show we stopped scanning
         QtWid.QApplication.processEvents()
 
     # --------------------------------------------------------------------------
     #   DAQ_function
     # --------------------------------------------------------------------------
 
-    def DAQ_function(self):
+    def DAQ_function(self) -> bool:
         tick = time.perf_counter()
+        print_debug = self.worker_DAQ is not None and self.worker_DAQ.debug
 
         # Clear input and output buffers of the device. Seems to resolve
         # intermittent communication time-outs.
-        self.dev.device.clear()
+        if self.dev.device is not None:
+            self.dev.device.clear()
 
         success = True
         if self.is_MUX_scanning:
             success &= self.dev.init_scan()  # Init scan
 
             if success:
                 self.dev.wait_for_OPC()  # Wait for OPC
-                if self.worker_DAQ.debug:
+                if print_debug:
                     tock = time.perf_counter()
-                    dprint("opc? in: %i" % (tock - tick))
+                    dprint(f"opc? in: {(tock - tick)*1000:4.0f} msec")
                     tick = tock
 
                 success &= self.dev.fetch_scan()  # Fetch scan
-                if self.worker_DAQ.debug:
+                if print_debug:
                     tock = time.perf_counter()
-                    dprint("fetc in: %i" % (tock - tick))
+                    dprint(f"fetc in: {(tock - tick)*1000:4.0f} msec")
                     tick = tock
 
             if success:
                 self.dev.wait_for_OPC()  # Wait for OPC
-                if self.worker_DAQ.debug:
+                if print_debug:
                     tock = time.perf_counter()
-                    dprint("opc? in: %i" % (tock - tick))
+                    dprint(f"opc? in: {(tock - tick)*1000:4.0f} msec")
                     tick = tock
 
         if success:
             # Do not throw additional timeout exceptions when .init_scan()
             # might have already failed. Hence this check for no success.
             self.dev.query_all_errors_in_queue()  # Query errors
-            if self.worker_DAQ.debug:
+            if print_debug:
                 tock = time.perf_counter()
-                dprint("err? in: %i" % (tock - tick))
+                dprint(f"err? in: {(tock - tick)*1000:4.0f} msec")
                 tick = tock
 
             # The next statement seems to trigger timeout, but very
             # intermittently (~once per 20 minutes). After this timeout,
             # everything times out.
             # self.dev.wait_for_OPC()
-            # if self.worker_DAQ.debug:
+            # if print_debug:
             #    tock = time.perf_counter()
-            #    dprint("opc? in: %i" % (tock - tick))
+            #    dprint(f"opc? in: {(tock - tick)*1000:4.0f} msec")
             #    tick = tock
 
             # NOTE: Another work-around to intermittent time-outs might
             # be sending self.dev.clear() every iter to clear the input and
             # output buffers. This is now done at the start of this function.
 
         # Optional user-supplied function to run. You can use this function to,
         # e.g., parse out the scan readings into separate variables and
         # post-process this data or log it.
         if self.DAQ_postprocess_MUX_scan_function is not None:
             self.DAQ_postprocess_MUX_scan_function()
 
-        if self.worker_DAQ.debug:
+        if print_debug:
             tock = time.perf_counter()
-            dprint("extf in: %i" % (tock - tick))
+            dprint(f"extf in: {(tock - tick)*1000:4.0f} msec")
             tick = tock
 
         return success
 
     # --------------------------------------------------------------------------
     #   jobs_function
     # --------------------------------------------------------------------------
@@ -310,41 +256,43 @@
 
     def create_GUI(self):
         p = {
             "alignment": QtCore.Qt.AlignmentFlag.AlignCenter,
             "font": FONT_MONOSPACE,
         }
         p2 = {
+            "parent": None,
             "alignment": QtCore.Qt.AlignmentFlag(
                 QtCore.Qt.AlignmentFlag.AlignCenter
                 + QtCore.Qt.AlignmentFlag.AlignVCenter
-            )
+            ),
         }
         # self.qlbl_mux = QtWid.QLabel("Keysight 34972a", **p2)
         self.qlbl_mux_state = QtWid.QLabel("Offline", **p)
-        self.qpbt_start_scan = create_Toggle_button("Start scan")
+        self.qpbt_start_scan = controls.create_Toggle_button("Start scan")
 
-        self.qpte_SCPI_commands = QtWid.QPlainTextEdit("", readOnly=True)
+        self.qpte_SCPI_commands = QtWid.QPlainTextEdit("")
+        self.qpte_SCPI_commands.setReadOnly(True)
         self.qpte_SCPI_commands.setLineWrapMode(
             QtWid.QPlainTextEdit.LineWrapMode.NoWrap
         )
-        self.qpte_SCPI_commands.setStyleSheet(SS_TEXTBOX_READ_ONLY)
+        self.qpte_SCPI_commands.setStyleSheet(controls.SS_TEXTBOX_READ_ONLY)
         self.qpte_SCPI_commands.setMaximumHeight(152)
         self.qpte_SCPI_commands.setMinimumWidth(200)
         self.qpte_SCPI_commands.setFont(FONT_MONOSPACE_SMALL)
 
         p = {"alignment": QtCore.Qt.AlignmentFlag.AlignRight, "readOnly": True}
         self.qled_scanning_interval_ms = QtWid.QLineEdit("", **p)
         self.qled_obtained_interval_ms = QtWid.QLineEdit("", **p)
 
         self.qpte_errors = QtWid.QPlainTextEdit("")
         self.qpte_errors.setLineWrapMode(
             QtWid.QPlainTextEdit.LineWrapMode.NoWrap
         )
-        self.qpte_errors.setStyleSheet(SS_TEXTBOX_ERRORS)
+        self.qpte_errors.setStyleSheet(controls.SS_TEXTBOX_ERRORS)
         self.qpte_errors.setMaximumHeight(90)
 
         # fmt: off
         self.qpbt_ackn_errors    = QtWid.QPushButton("Acknowledge errors")
         self.qpbt_reinit         = QtWid.QPushButton("Reinitialize")
         self.qlbl_update_counter = QtWid.QLabel("0")
         self.qpbt_debug_test     = QtWid.QPushButton("Debug test")
@@ -382,97 +330,99 @@
         grid.addWidget(self.qpbt_ackn_errors              , i, 0, 1, 2); i+=1
         grid.addWidget(self.qlbl_update_counter           , i, 0, 1, 2); i+=1
         # grid.addWidget(self.qpbt_debug_test             , i, 0, 1, 2); i+=1
         # fmt: on
 
         #  Table widget containing the readings of the current scan cycle
         # ----------------------------------------------------------------
-        self.qtbl_readings = QtWid.QTableWidget(columnCount=1)
+        self.qtbl_readings = QtWid.QTableWidget()
+        self.qtbl_readings.setColumnCount(1)
         self.qtbl_readings.setHorizontalHeaderLabels(["Readings"])
         self.qtbl_readings.horizontalHeaderItem(0).setFont(FONT_MONOSPACE_SMALL)
         self.qtbl_readings.verticalHeader().setFont(FONT_MONOSPACE_SMALL)
         self.qtbl_readings.verticalHeader().setDefaultSectionSize(24)
         self.qtbl_readings.setFont(FONT_MONOSPACE_SMALL)
         # self.qtbl_readings.setMinimumHeight(600)
         self.qtbl_readings.setFixedWidth(180)
         self.qtbl_readings.setColumnWidth(0, 110)
 
         grid.addWidget(self.qtbl_readings, 0, 2, i, 1)
 
-        self.qgrp = QtWid.QGroupBox("%s" % self.dev.name)
-        self.qgrp.setStyleSheet(SS_GROUP)
+        self.qgrp = QtWid.QGroupBox(f"{self.dev.name}")
         self.qgrp.setLayout(grid)
 
     # --------------------------------------------------------------------------
     #   update_GUI
     # --------------------------------------------------------------------------
 
     @Slot()
     def update_GUI(self):
         """NOTE: 'self.dev.mutex' is not being locked, because we are only
         reading 'state' for displaying purposes. We can do this because 'state'
         members are written and read atomicly, with the only exception being
         'str_all_errors', and it bears no consequences to read wrongly.
         Not locking the mutex might speed up the program.
         """
-        if self.dev.is_alive:
-            if self.is_MUX_scanning:
-                self.qlbl_mux_state.setText("Scanning")
-                self.qpbt_start_scan.setChecked(True)
-            else:
-                self.qlbl_mux_state.setText("Idle")
-                self.qpbt_start_scan.setChecked(False)
+        if not self.dev.is_alive:
+            self.qlbl_mux_state.setText("Offline")
+            self.qgrp.setEnabled(False)
+            return
 
-            self.qpte_errors.setReadOnly(self.dev.state.all_errors != [])
-            self.qpte_errors.setStyleSheet(SS_TEXTBOX_ERRORS)
-            self.qpte_errors.setPlainText(
-                "%s" % "\n".join(self.dev.state.all_errors)
-            )
+        if self.is_MUX_scanning:
+            self.qlbl_mux_state.setText("Scanning")
+            self.qpbt_start_scan.setChecked(True)
+        else:
+            self.qlbl_mux_state.setText("Idle")
+            self.qpbt_start_scan.setChecked(False)
 
-            self.qled_obtained_interval_ms.setText(
-                "%.0f" % self.obtained_DAQ_interval_ms
-            )
-            self.qlbl_update_counter.setText("%s" % self.update_counter_DAQ)
+        self.qpte_errors.setReadOnly(self.dev.state.all_errors != [])
+        self.qpte_errors.setStyleSheet(controls.SS_TEXTBOX_ERRORS)
+        self.qpte_errors.setPlainText(
+            f"{chr(10).join(self.dev.state.all_errors)}"
+        )
 
-            for i in range(len(self.dev.state.all_scan_list_channels)):
-                if i >= len(self.dev.state.readings):
-                    break
-                reading = self.dev.state.readings[i]
-                if reading > INFINITY_CAP:
-                    self.qtbl_readings.item(i, 0).setData(
-                        QtCore.Qt.DisplayRole, "Inf"
-                    )
-                else:
-                    if type(self.table_readings_format) == list:
-                        try:
-                            str_format = self.table_readings_format[i]
-                        except IndexError:
-                            str_format = self.table_readings_format[0]
-                    elif type(self.table_readings_format) == str:
-                        str_format = self.table_readings_format
-
-                    self.qtbl_readings.item(i, 0).setData(
-                        QtCore.Qt.DisplayRole, str_format % reading
-                    )
-        else:
-            self.qlbl_mux_state.setText("Offline")
-            self.qgrp.setEnabled(False)
+        self.qled_obtained_interval_ms.setText(
+            f"{self.obtained_DAQ_interval_ms:.0f}"
+        )
+        self.qlbl_update_counter.setText(f"{self.update_counter_DAQ}")
+
+        for i in range(len(self.dev.state.all_scan_list_channels)):
+            if i >= len(self.dev.state.readings):
+                break
+            reading = self.dev.state.readings[i]
+            if reading > INFINITY_CAP:
+                self.qtbl_readings.item(i, 0).setData(
+                    QtCore.Qt.ItemDataRole.DisplayRole, "Inf"
+                )
+            else:
+                if isinstance(self.table_readings_format, list):
+                    try:
+                        str_format = self.table_readings_format[i]
+                    except IndexError:
+                        str_format = self.table_readings_format[0]
+                elif isinstance(self.table_readings_format, str):
+                    str_format = self.table_readings_format
+
+                self.qtbl_readings.item(i, 0).setData(
+                    QtCore.Qt.ItemDataRole.DisplayRole,
+                    f"{reading:{str_format}}",
+                )
 
     # --------------------------------------------------------------------------
     #   populate_SCPI_commands
     # --------------------------------------------------------------------------
 
     def populate_SCPI_commands(self):
         self.qpte_SCPI_commands.setPlainText(
-            "%s" % "\n".join(self.dev.SCPI_setup_commands)
-        )
-        self.qled_scanning_interval_ms.setText(
-            "%i"
-            % self.worker_DAQ._DAQ_interval_ms  # pylint: disable=protected-access
+            f"{chr(10).join(self.dev.SCPI_setup_commands)}"
         )
+        if self.worker_DAQ is not None:
+            self.qled_scanning_interval_ms.setText(
+                f"{self.worker_DAQ._DAQ_interval_ms}"  # pylint: disable=protected-access
+            )
 
     # --------------------------------------------------------------------------
     #   Table widget related
     # --------------------------------------------------------------------------
 
     def populate_table_readings(self):
         self.qtbl_readings.setRowCount(
@@ -486,18 +436,26 @@
             item = QtWid.QTableWidgetItem("nan")
             item.setTextAlignment(
                 QtCore.Qt.AlignmentFlag.AlignRight
                 + QtCore.Qt.AlignmentFlag.AlignCenter
             )
             self.qtbl_readings.setItem(i, 0, item)
 
-    def set_table_readings_format(self, format_str):
-        # String format to use for the readings in the table widget
+    def set_table_readings_format(self, format_str: str):
+        # String format to use for the readings in the table widget.
         # When type is a single string, all rows will use this format.
         # When type is a list of strings, rows will be formatted consecutively.
+        # I.e. format_str = ".2f", or format_str = [".2f", ".1e"]
+
+        # Backwards compatibility fix. We have to remove any '%' characters that
+        # the end-user might have supplied when using the old-style formatting
+        # using %. The old `format_str` argument used "%.2f", for example. We
+        # now rely on f-strings for formatting.
+        format_str = format_str.replace("%", "")
+
         self.table_readings_format = format_str
 
     # --------------------------------------------------------------------------
     #   GUI functions
     # --------------------------------------------------------------------------
 
     @Slot()
@@ -506,36 +464,40 @@
             self.start_MUX_scan()
         else:
             self.stop_MUX_scan()
 
     @Slot()
     def process_qpbt_ackn_errors(self):
         # Lock the dev mutex because string operations are not atomic
-        locker = QtCore.QMutexLocker(self.dev.mutex)
+        locker = QtCore.QMutexLocker(self.dev.mutex)  # type: ignore
         self.dev.state.all_errors = []
         self.qpte_errors.setPlainText("")
         self.qpte_errors.setReadOnly(False)  # To change back to regular colors
         locker.unlock()
 
     @Slot()
     def process_qpbt_reinit(self):
-        str_msg = (
+        title = f"Reinitialize {self.dev.name}"
+        msg = (
             "Are you sure you want reinitialize the multiplexer?\n\n"
             "This would abort the current scan, reset the device\n"
             "and resend the SCPI scan command list."
         )
-        reply = QtWid.QMessageBox.question(
-            None,
-            ("Reinitialize %s" % self.dev.name),
-            str_msg,
-            QtWid.QMessageBox.Yes | QtWid.QMessageBox.No,
-            QtWid.QMessageBox.No,
+        msgbox = QtWid.QMessageBox()
+        msgbox.setIcon(QtWid.QMessageBox.Icon.Question)
+        msgbox.setWindowTitle(title)
+        msgbox.setText(msg)
+        msgbox.setStandardButtons(
+            QtWid.QMessageBox.StandardButton.Yes
+            | QtWid.QMessageBox.StandardButton.No
         )
+        msgbox.setDefaultButton(QtWid.QMessageBox.StandardButton.No)
+        reply = msgbox.exec()
 
-        if reply == QtWid.QMessageBox.Yes:
+        if reply == QtWid.QMessageBox.StandardButton.Yes:
             self.qpbt_start_scan.setChecked(False)
             self.stop_MUX_scan()
             self.add_to_jobs_queue(self.dev.wait_for_OPC)
             self.add_to_jobs_queue(self.dev.begin)
             self.process_jobs_queue()
 
     @Slot()
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Keysight_N8700_protocol_SCPI.py` & `dvg-devices-1.4.0/src/dvg_devices/Keysight_N8700_protocol_SCPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,35 +4,32 @@
 
 Communication errors will be handled as non-fatal. This means it will struggle
 on with the script while reporting error messages to the command line output,
 as opposed to terminating the program completely.
 
 State variables that read numpy.nan indicate that they are uninitialized or that
 the previous query resulted in a communication error.
-
-TODO: This module could be improved. See `Aim_TTi_PSU_protocol_RS232` which
-also uses the SCPI protocol.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "14-09-2022"
-__version__ = "1.0.0"
-# pylint: disable=try-except-raise, bare-except, pointless-string-statement
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, multiple-statements, broad-except
 
 import os
 import time
 from pathlib import Path
+from typing import Union, Tuple, List
 
-# NOTE: Current demanded requirement pyvisa~=1.11 was ~=1.9 before. 1.11 has
-# broken backwards comp. Still need to test if all is still fine.
 import pyvisa
 import numpy as np
 
-from dvg_debug_functions import print_fancy_traceback as pft
+from dvg_debug_functions import print_fancy_traceback
+from dvg_pid_controller import PID_Controller
 
 # 'No error left' reply from the PSU
 STR_NO_ERROR = "ERR 0"
 
 # VISA settings
 VISA_TIMEOUT = 4000  # 4000 [msec]
 
@@ -44,89 +41,100 @@
     class State:
         """Container for the process and measurement variables.
         [numpy.nan] values indicate that the parameter is not initialized or
         that the last query was unsuccessful in communication.
         """
 
         # fmt: off
-        V_source = 0        # Voltage to be sourced [V]
-        I_source = 0        # Current to be sourced [A]
-        P_source = 0        # Power to be sourced, when PID controller is on [W]
-        ENA_PID = False     # Is the PID controller on the power output enabled?
-
-        V_meas = np.nan         # Measured output voltage [V]
-        I_meas = np.nan         # Measured output current [A]
-        P_meas = np.nan         # Derived output power    [W]
-
-        OVP_level  = np.nan     # Over-voltage protection level [V]
-        ENA_OCP    = False      # Is over-current protection enabled?
-        ENA_output = False      # Is power output enabled (by software)?
+        V_source: float = 0     # Voltage to be sourced [V]
+        I_source: float = 0     # Current to be sourced [A]
+        P_source: float = 0     # Power to be sourced, when PID controller is on [W]
+        ENA_PID : bool = False  # Is the PID controller on the power output enabled?
+
+        V_meas: float = np.nan  # Measured output voltage [V]
+        I_meas: float = np.nan  # Measured output current [A]
+        P_meas: float = np.nan  # Derived output power    [W]
+
+        OVP_level : float = np.nan  # Over-voltage protection level [V]
+        ENA_OCP   : bool = False    # Is over-current protection enabled?
+        ENA_output: bool= False     # Is power output enabled (by software)?
         # fmt: on
 
-        # The error string retreived from the error queue of the device. None
-        # indicates no error is left in the queue.
-        error = None
+        # The single error string retreived from the error queue of the device.
+        # None indicates no error is left in the queue.
+        error: Union[str, None] = None
 
         # This list of strings is provided to be able to store all errors from
         # the device queue. This list is populated by calling 'query_error'
         # until no error is left in the queue. This list can then be printed to
         # screen or GUI and the user should 'acknowledge' the list, after which
         # the list can be emptied (=[]) again.
-        all_errors = []
+        all_errors: List[str] = []
 
         # Questionable condition status registers
         # fmt: off
-        status_QC_OV  = False   # Output disabled by over-voltage protection
-        status_QC_OC  = False   # Output disabled by over-current protection
-        status_QC_PF  = False   # Output disabled because AC power failed
-        status_QC_OT  = False   # Output disabled by over-temperature protection
-        status_QC_INH = False   # Output turned off by external J1 inhibit signal (ENABLE)
-        status_QC_UNR = False   # The output is unregulated
+        status_QC_OV : bool = False  # Output disabled by over-voltage protection
+        status_QC_OC : bool = False  # Output disabled by over-current protection
+        status_QC_PF : bool = False  # Output disabled because AC power failed
+        status_QC_OT : bool = False  # Output disabled by over-temperature protection
+        status_QC_INH: bool = False  # Output turned off by external J1 inhibit signal (ENABLE)
+        status_QC_UNR: bool = False  # The output is unregulated
 
         # Operation condition status registers
-        status_OC_WTG = False   # Unit waiting for transient trigger
-        status_OC_CV  = False   # Output in constant voltage
-        status_OC_CC  = False   # Output in constant current
+        status_OC_WTG: bool = False  # Unit waiting for transient trigger
+        status_OC_CV : bool = False  # Output in constant voltage
+        status_OC_CC : bool = False  # Output in constant current
         # fmt: on
 
     class Config:
         # fmt: off
-        V_source  = 120         # Voltage to be sourced [V]
-        I_source  = 1           # Current to be sourced [A]
-        P_source  = 0           # Power   to be sourced [W]
-        OVP_level = 126         # Over-voltage protection level [V]
-        ENA_OCP   = True        # Is over-current protection enabled?
+        V_source : float = 120       # Voltage to be sourced [V]
+        I_source : float = 1         # Current to be sourced [A]
+        P_source : float = 0         # Power   to be sourced [W]
+        OVP_level: float = 126       # Over-voltage protection level [V]
+        ENA_OCP  : bool  = True      # Is over-current protection enabled?
         # fmt: on
 
     # --------------------------------------------------------------------------
     #   __init__
     # --------------------------------------------------------------------------
 
-    def __init__(self, visa_address=None, path_config=PATH_CONFIG, name="PSU"):
+    def __init__(
+        self,
+        visa_address: str = "",
+        path_config=PATH_CONFIG,
+        name="PSU",
+    ):
         """
         Args:
-            visa_address (str): VISA device address of the power supply
-            path_config (pathlib.Path): path to the configuration file
+            visa_address (`str`):
+                VISA device address.
+
+            path_config (`pathlib.Path`):
+                Path to the configuration file.
         """
         self._visa_address = visa_address
         self.name = name
-        self._idn = None  # The identity of the device ("*IDN?")
+        self._idn: str = ""  # The identity of the device ("*IDN?")
 
-        # Placeholder for the VISA device instance referencing the PSU
-        self.device = None
+        # Placeholder for the VISA device instance
+        self.device: Union[pyvisa.resources.MessageBasedResource, None] = None
 
         # Is the connection to the device alive?
-        self.is_alive = False
+        self.is_alive: bool = False
 
         # Container for the process and measurement variables
         self.state = self.State()
         self.config = self.Config()
 
         # Location of the configuration file
-        self.path_config = path_config
+        self.path_config: Path = path_config
+
+        # Placeholder for a future PID controller on the power output
+        self.PID_power = PID_Controller(Kp=0, Ki=0, Kd=0)
 
     # --------------------------------------------------------------------------
     #   close
     # --------------------------------------------------------------------------
 
     def close(self):
         if (not self.is_alive) or (self.device is None):
@@ -136,103 +144,120 @@
             self.device.close()
             self.is_alive = False
 
     # --------------------------------------------------------------------------
     #   connect
     # --------------------------------------------------------------------------
 
-    def connect(self, rm):
+    def connect(self, rm: pyvisa.ResourceManager) -> bool:
         """Try to connect to the PSU over VISA at the given address. When
         successful the VISA device instance will be stored in member 'device'
         and its identity is queried and stored in '_idn'.
 
         Args:
-            rm: Instance of pyvisa.ResourceManager
+            rm `(pyvisa.ResourceManager)`:
+                Instance of VISA ResourceManager.
 
         Returns: True if successful, False otherwise.
         """
         self.is_alive = False
 
         print("Connect to: Keysight N8700 series PSU")
-        print("  @ %s : " % self._visa_address, end="")
+        print(f"  @ {self._visa_address} : ", end="")
+
         try:
-            self.device = rm.open_resource(
-                self._visa_address, timeout=VISA_TIMEOUT
-            )
-            self.device.clear()
+            device = rm.open_resource(self._visa_address, timeout=VISA_TIMEOUT)
+            device.clear()
         except pyvisa.VisaIOError:
             print("Could not open resource.\n")
             return False
-        except:
-            raise
+        except Exception as err:
+            raise err
+
+        if not isinstance(device, pyvisa.resources.MessageBasedResource):
+            print("ERROR: Device is not a `MessageBasedResource`.")
+            return False
+
         print("Success!")
+        self.device = device
         self.is_alive = True
 
-        success, self._idn = self.query("*idn?")
+        _success, reply = self.query("*idn?")
         self.wait_for_OPC()
-        if success:
-            print("  %s\n" % self._idn)
-            return True
 
-        return False
+        if not isinstance(reply, str):
+            return False
+
+        self._idn = reply
+        print(f"  {self._idn}\n")
+        return True
 
     # --------------------------------------------------------------------------
     #   begin
     # --------------------------------------------------------------------------
 
-    def begin(self):
+    def begin(self) -> bool:
         """This function should run directly after having established a
         connection to a Keysight PSU.
 
         Returns: True if all messages were sent and received successfully,
             False otherwise.
         """
         # Clear errors
         self.state.error = None
         self.state.all_errors = []
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return False
 
+        # We must clear the device to resolve intermittent I/O communication
+        # problems particular to this PSU.
+        self.device.clear()
+        time.sleep(0.01)
+
         success = True
         success &= self.set_PON_off()  # Force power-on state off for safety
 
         self.wait_for_OPC()
-        # self.prepare_wait_for_OPC_indefinitely() # COMMENTED OUT: .stb fails intermittently, perhaps due to the USB isolator
+        # BELOW IS COMMENTED OUT because .stb fails intermittently, perhaps due
+        # to the USB isolator
+        # self.prepare_wait_for_OPC_indefinitely()
 
         success &= self.query_OVP_level()
         success &= self.query_V_source()
         success &= self.query_I_source()
         success &= self.query_ENA_OCP()
         success &= self.query_status_QC()
         success &= self.query_status_OC()
 
         self.query_all_errors_in_queue()
 
-        # self.wait_for_OPC_indefinitely()         # COMMENTED OUT: .stb fails intermittently, perhaps due to the USB isolator
+        # BELOW IS COMMENTED OUT because .stb fails intermittently, perhaps due
+        # to the USB isolator
+        # self.wait_for_OPC_indefinitely()
         self.wait_for_OPC()
 
         return success
 
     # --------------------------------------------------------------------------
     #   reinitialize
     # --------------------------------------------------------------------------
 
-    def reinitialize(self):
+    def reinitialize(self) -> bool:
         """Reinitialize the PSU, including clear and reset
 
         Returns: True if all messages were sent and received successfully,
             False otherwise.
         """
         # Clear errors
         self.state.error = None
         self.state.all_errors = []
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return False
 
         # Clear device's input and output buffers
         self.device.clear()
 
         success = True
@@ -261,203 +286,212 @@
 
         return success
 
     # --------------------------------------------------------------------------
     #   write
     # --------------------------------------------------------------------------
 
-    def write(self, msg_str):
+    def write(self, msg_str) -> bool:
         """Try to write a command to the device.
 
         Args:
-            msg_str (string): Message to be sent.
+            msg_str (`str`):
+                Message to be sent.
 
         Returns: True if the message was sent successfully, False otherwise.
             NOTE: It does not indicate whether the message made sense to the
             device.
         """
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return False
 
         try:
             self.device.write(msg_str)
         except pyvisa.VisaIOError as err:
             # Print error and struggle on
-            pft(err)
+            print_fancy_traceback(err)
             return False
-        except:
-            raise
+        except Exception as err:
+            raise err
 
         return True
 
     # --------------------------------------------------------------------------
     #   query
     # --------------------------------------------------------------------------
 
-    def query(self, msg_str):
+    def query(self, msg_str: str) -> Tuple[bool, Union[str, None]]:
         """Try to query the device.
 
         Args:
-            msg_str (string): Message to be sent.
+            msg_str (`str`):
+                Message to be sent.
 
         Returns:
-            success (bool): True if the message was sent and a reply was
-                received successfully, False otherwise.
-            ans_str (string): Reply received from the device. [numpy.nan] if
-                unsuccessful.
+            success (`bool`):
+                True if the message was sent and a reply was received
+                successfully, False otherwise.
+
+            reply (`str` | `None`):
+                Reply received from the device. None if unsuccessful.
         """
         success = False
-        ans_str = np.nan
+        reply = None
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
+            return success, reply
+
+        try:
+            reply = self.device.query(msg_str)
+        except pyvisa.VisaIOError as err:
+            # Print error and struggle on
+            print_fancy_traceback(err)
+        except Exception as err:
+            raise err
         else:
-            try:
-                ans_str = self.device.query(msg_str)
-            except pyvisa.VisaIOError as err:
-                # Print error and struggle on
-                pft(err)
-            except:
-                raise
-            else:
-                ans_str = ans_str.strip()
-                success = True
+            reply = reply.strip()
+            success = True
 
-        return success, ans_str
+        return success, reply
 
     # --------------------------------------------------------------------------
     #   System status related
     # --------------------------------------------------------------------------
 
-    def clear_and_reset(self):
+    def clear_and_reset(self) -> bool:
         """Clear device status and reset. Return when this operation has
         completed on the device. Blocking.
 
         Returns: True if the message was sent successfully, False otherwise.
         """
 
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return False
-        else:
-            # The reset operation can take a long time to complete. Momentarily
-            # increase the timeout to 2000 msec if necessary.
-            self.device.timeout = max(self.device.timeout, 2000)
 
-            # Send clear and reset
-            success = self.write("*cls;*rst")
+        # The reset operation can take a long time to complete. Momentarily
+        # increase the timeout to 2000 msec if necessary.
+        self.device.timeout = max(self.device.timeout, 2000)
 
-            # Wait for the last operation to finish before timeout expires
-            self.wait_for_OPC()
+        # Send clear and reset
+        success = self.write("*cls;*rst")
+
+        # Wait for the last operation to finish before timeout expires
+        self.wait_for_OPC()
 
-            # Restore timeout
-            self.device.timeout = VISA_TIMEOUT
+        # Restore timeout
+        self.device.timeout = VISA_TIMEOUT
 
-            return success
+        return success
 
-    def wait_for_OPC(self):
+    def wait_for_OPC(self) -> bool:
         """'Operation complete' query, used for event synchronization.
 
         Will wait for all device operations to complete or until a timeout is
         triggered. Blocking.
 
         Returns True if successful, False otherwise.
         """
         # Returns an ASCII "+1" when all pending overlapped operations have been
         # completed.
-        success, ans = self.query("*opc?")
-        if success and ans == "1":
+        _success, reply = self.query("*opc?")
+        if reply == "1":
             return True
 
-        print("Warning: *opc? timed out at device %s" % self.name)
+        print(f"Warning: *opc? timed out at device {self.name}")
         return False
 
     def wait_for_OPC_indefinitely(self):
         """Poll OPC status bit for 'operation complete', used for event
         synchronization.
 
         Will wait indefinitely for all device operations to complete. Blocking.
 
         Make sure that the ESR is set to signal bit 0 - OPC (operation complete)
         before you call this function. This can be done by calling
         'prepare_wait_for_OPC_indefinitely()'.
         """
 
+        if not self.is_alive or self.device is None:
+            print("ERROR: Device is not connected yet or already closed.")
+            return
+
         # Let the device set the ESR bit 0 - OPC (operation complete) to 1 after
         # all device operations have completed.
         self.write("*opc")
 
         # Poll the OPC status bit for 'operation complete'. This is the 5th
         # bit.
         while not (self.device.stb & 0b100000) == 0b100000:
             time.sleep(0.01)
 
         # Reset the ESR bit 0 - OPC back to 0.
         self.query("*esr?")
 
-    def prepare_wait_for_OPC_indefinitely(self):
+    def prepare_wait_for_OPC_indefinitely(self) -> bool:
         """Set the ESR to signal bit 0 - OPC (operation complete). Should be
         called only once after a '*rst' in case you want to make use of
         'wait_for_OPC_indefinitely()'.
 
         Returns: True if the message was sent successfully, False otherwise.
         """
         return self.write("*ese 1")
 
-    def query_error(self, verbose=False):
+    def query_error(self, verbose: bool = False) -> bool:
         """Pop one error string from the error queue of the device and store it
         in the 'State'-class member. A value of None indicates no error is left.
 
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, str_ans = self.query("err?")
-        if success:
-            if str_ans == STR_NO_ERROR:
+        success, reply = self.query("err?")
+        if isinstance(reply, str):
+            if reply.find(STR_NO_ERROR) == 0:
                 self.state.error = None
             else:
-                self.state.error = str_ans.strip("ERR").strip()
+                self.state.error = reply.strip("ERR").strip()
                 if verbose:  # DEBUG INFO
-                    print("  %s" % self.state.error)
+                    print(f"  {self.state.error}")
         return success
 
-    def query_all_errors_in_queue(self, verbose=False):
+    def query_all_errors_in_queue(self, verbose: bool = False):
         """Check if there are errors in the device queue and retrieve all if
         any and append these to 'state.all_errors'.
         """
-        if not self.is_alive:
+        if not self.is_alive or self.device is None:
             print("ERROR: Device is not connected yet or already closed.")
             return
 
         # if (self.device.stb & 0b100) == 0b100:
         # There are unread errors in the queue available. Retrieve all.
         while True:
             if self.query_error():
                 if self.state.error is None:
                     break
-                else:
-                    self.state.all_errors.append(self.state.error)
+
+                self.state.all_errors.append(self.state.error)
             else:
                 break
 
         if verbose:  # DEBUG INFO
             for error in self.state.all_errors:
-                print("  %s" % error)
+                print(f"  {error}")
 
-    def query_status_QC(self, verbose=False):
+    def query_status_QC(self, verbose: bool = False) -> bool:
         """Read out the questionable condition status registers of the device
         and store them in the 'State'-class members.
 
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, ans = self.query("stat:ques:cond?")
-        if success:
+        success, reply = self.query("stat:ques:cond?")
+        if isinstance(reply, str):
             # fmt: off
-            status_code = int(ans)
+            status_code = int(reply)
             self.state.status_QC_OV  = bool(status_code & 1)
             self.state.status_QC_OC  = bool(status_code & 2)
             self.state.status_QC_PF  = bool(status_code & 4)
             self.state.status_QC_OT  = bool(status_code & 16)
             self.state.status_QC_INH = bool(status_code & 512)
             self.state.status_QC_UNR = bool(status_code & 1024)
 
@@ -468,24 +502,24 @@
                 if self.state.status_QC_OT:  print("  OT")
                 if self.state.status_QC_INH: print("  INH")
                 if self.state.status_QC_UNR: print("  UNH")
             # fmt: on
 
         return success
 
-    def query_status_OC(self, verbose=False):
+    def query_status_OC(self, verbose: bool = False) -> bool:
         """Read out the operation condition status registers of the device
         and store them in the 'State'-class members.
 
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, ans = self.query("stat:oper:cond?")
-        if success:
+        success, reply = self.query("stat:oper:cond?")
+        if isinstance(reply, str):
             # fmt: off
-            status_code = int(ans)
+            status_code = int(reply)
             self.state.status_OC_WTG = bool(status_code & 32)
             self.state.status_OC_CV  = bool(status_code & 256)
             self.state.status_OC_CC  = bool(status_code & 1024)
 
             if verbose:  # DEBUG INFO
                 if self.state.status_OC_WTG: print("  WTG")
                 if self.state.status_OC_CV : print("  CV")
@@ -494,26 +528,26 @@
 
         return success
 
     # --------------------------------------------------------------------------
     #   set_PON_off
     # --------------------------------------------------------------------------
 
-    def set_PON_off(self):
+    def set_PON_off(self) -> bool:
         """Set the power-on state of the PSU to off.
 
         Returns: True if the message was sent successfully, False otherwise.
         """
         return self.write("outp:pon:stat rst")
 
     # --------------------------------------------------------------------------
     #   Protection related
     # --------------------------------------------------------------------------
 
-    def clear_output_protection(self):
+    def clear_output_protection(self) -> bool:
         """Clear the latched signals that have disabled the output. The
         over-voltage and over-current conditions are always latching. The over-
         temperature condition, AC-fail condition, Enable pins, and SO pins are
         latching if OUTPut:PON:STATe is RST, and non-latching if
         OUTPut:PON:STATe is AUTO. All conditions that generate the fault must be
         removed before the latch can be cleared. The output is then restored to
         the state it was in before the fault condition occurred.
@@ -528,39 +562,40 @@
     constant current operation, the output is disabled and OC is set in the
     Questionable Condition status register. The *RST value = Off.
 
     An over-current condition can be cleared with the Output Protection Clear
     command after the cause of the condition is removed
     """
 
-    def set_ENA_OCP(self, flag=True):
+    def set_ENA_OCP(self, flag: bool = True) -> bool:
         """
         Returns: True if the message was sent successfully, False otherwise.
         """
         if flag:
             success = self.write("sour:curr:prot:stat on")
             if success:
                 self.state.ENA_OCP = True
         else:
             success = self.write("sour:curr:prot:stat off")
             if success:
                 self.state.ENA_OCP = False
         return success
 
-    def query_ENA_OCP(self, verbose=False):
+    def query_ENA_OCP(self, verbose: bool = False) -> bool:
         """
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, reply = self.query("sour:curr:prot:stat?")
-        if success:
+        _success, reply = self.query("sour:curr:prot:stat?")
+        if isinstance(reply, str):
             self.state.ENA_OCP = bool(int(reply))
-
             if verbose:  # DEBUG INFO
                 print(self.state.ENA_OCP)
-        return success
+            return True
+
+        return False
 
     """These commands set the over-voltage protection (OVP) level of the
     output. The values are programmed in volts. If the output voltage exceeds
     the OVP level, the output is disabled and OV is set in the Questionable
     Condition status register. The *RST value = Max.
 
     The range of values that can be programmed for this command is coupled with
@@ -569,172 +604,155 @@
     the immediate voltage setting multiplied by 1.05; whichever is higher. The
     maximum setting is the value in the table.
 
     An over-voltage condition can be cleared with the Output Protection Clear
     command after the condition that caused the OVP trip is removed.
     """
 
-    def set_OVP_level(self, voltage_V):
+    def set_OVP_level(self, voltage_V: float) -> bool:
         """
         Returns: True if the message was sent successfully, False otherwise.
         """
-        try:
-            voltage_V = float(voltage_V)
-        except (ValueError, TypeError):
-            voltage_V = 0.0
-        except:
-            raise
-
         self.state.OVP_level = voltage_V
-        return self.write("sour:volt:prot:lev %f" % voltage_V)
+        return self.write(f"sour:volt:prot:lev {voltage_V:.5f}")
 
-    def query_OVP_level(self, verbose=False):
+    def query_OVP_level(self, verbose: bool = False) -> bool:
         """
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, reply = self.query("sour:volt:prot:lev?")
-        if success:
+        _success, reply = self.query("sour:volt:prot:lev?")
+        if isinstance(reply, str):
             self.state.OVP_level = float(reply)
-
             if verbose:  # DEBUG INFO
                 print(self.state.OVP_level)
-        return success
+            return True
+
+        return False
 
     # --------------------------------------------------------------------------
     #   Output related
     # --------------------------------------------------------------------------
 
-    def clear_output_protection_and_turn_on(self):
+    def clear_output_protection_and_turn_on(self) -> bool:
         """Combine instructions 'clear output protection' and 'turn on output'
         into one SCPI message.
 
         Returns: True if the message was sent successfully, False otherwise.
         """
         success = self.write("outp:prot:cle;*opc;:outp on")
         if success:
             self.state.ENA_output = True
         return success
 
-    def turn_on(self):
+    def turn_on(self) -> bool:
         """
         Returns: True if the message was sent successfully, False otherwise.
         """
         return self.set_ENA_output(True)
 
-    def turn_off(self):
+    def turn_off(self) -> bool:
         """
         Returns: True if the message was sent successfully, False otherwise.
         """
         return self.set_ENA_output(False)
 
-    def set_ENA_output(self, flag):
+    def set_ENA_output(self, flag: bool) -> bool:
         """
         Returns: True if the message was sent successfully, False otherwise.
         """
         if flag:
             success = self.write("outp on")
             if success:
                 self.state.ENA_output = True
         else:
             success = self.write("outp off")
             if success:
                 self.state.ENA_output = False
         return success
 
-    def query_ENA_output(self, verbose=False):
+    def query_ENA_output(self, verbose: bool = False) -> bool:
         """
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, reply = self.query("outp?")
-        if success:
+        _success, reply = self.query("outp?")
+        if isinstance(reply, str):
             self.state.ENA_output = bool(int(reply))
-
             if verbose:  # DEBUG INFO
                 print(self.state.ENA_output)
-        return success
+            return True
 
-    def set_I_source(self, current_A):
+        return False
+
+    def set_I_source(self, current_A: float) -> bool:
         """
         Returns: True if the message was sent successfully, False otherwise.
         """
-        try:
-            current_A = float(current_A)
-        except (ValueError, TypeError):
-            current_A = 0.0
-        except:
-            raise
-
         self.state.I_source = current_A
-        return self.write("sour:curr %.5f" % current_A)
+        return self.write(f"sour:curr {current_A:.5f}")
 
-    def set_V_source(self, voltage_V):
+    def set_V_source(self, voltage_V: float) -> bool:
         """
         Returns: True if the message was sent successfully, False otherwise.
         """
-        try:
-            voltage_V = float(voltage_V)
-        except (ValueError, TypeError):
-            voltage_V = 0.0
-        except:
-            raise
-
         self.state.V_source = voltage_V
-        return self.write("sour:volt %.5f" % voltage_V)
+        return self.write(f"sour:volt {voltage_V:.5f}")
 
-    def query_I_source(self, verbose=False):
+    def query_I_source(self, verbose: bool = False) -> bool:
         """
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, reply = self.query("sour:curr?")
-        if success:
+        _success, reply = self.query("sour:curr?")
+        if isinstance(reply, str):
             self.state.I_source = float(reply)
-
             if verbose:  # DEBUG INFO
                 print(self.state.I_source)
-        return success
+            return True
 
-    def query_V_source(self, verbose=False):
+        return False
+
+    def query_V_source(self, verbose: bool = False) -> bool:
         """
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, reply = self.query("sour:volt?")
-        if success:
+        _success, reply = self.query("sour:volt?")
+        if isinstance(reply, str):
             self.state.V_source = float(reply)
-
             if verbose:  # DEBUG INFO
                 print(self.state.V_source)
-        return success
+            return True
+
+        return False
 
-    def query_I_meas(self, verbose=False):
+    def query_I_meas(self, verbose: bool = False) -> bool:
         """
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, reply = self.query("meas:curr?")
-        if success:
+        _success, reply = self.query("meas:curr?")
+        if isinstance(reply, str):
             self.state.I_meas = float(reply)
             self.state.P_meas = self.state.I_meas * self.state.V_meas
-
             if verbose:  # DEBUG INFO
                 print(self.state.I_meas)
+            return True
 
-        return success
+        return False
 
-    def query_V_meas(self, verbose=False):
+    def query_V_meas(self, verbose: bool = False) -> bool:
         """
         Returns: True if the query was received successfully, False otherwise.
         """
-        success, reply = self.query("meas:volt?")
-        if success:
+        _success, reply = self.query("meas:volt?")
+        if isinstance(reply, str):
             self.state.V_meas = float(reply)
             self.state.P_meas = self.state.I_meas * self.state.V_meas
-
             if verbose:  # DEBUG INFO
                 print(self.state.V_meas)
+            return True
 
-        return success
+        return False
 
     # --------------------------------------------------------------------------
     #   Speed tests for debugging
     # --------------------------------------------------------------------------
 
     def speed_test(self):
         """Results:
@@ -806,49 +824,49 @@
         print("  I_meas    [A]: ", end=''); self.query_I_meas(True)
         # fmt: on
 
     # --------------------------------------------------------------------------
     #   read_config_file
     # --------------------------------------------------------------------------
 
-    def read_config_file(self):
+    def read_config_file(self) -> bool:
         """Try to open the config textfile containing:
              V_source       # Voltage to be sourced [V]
              I_source       # Current to be sourced [A]
              P_source       # Power   to be sourced [W]
              OVP_level      # Over-voltage protection level [V]
              ENA_OCP        # Is over-current protection enabled?
 
         Do not panic if the file does not exist or cannot be read.
 
         Returns: True if successful, False otherwise.
         """
         if isinstance(self.path_config, Path):
             if self.path_config.is_file():
                 try:
-                    with self.path_config.open() as f:
+                    with self.path_config.open(encoding="utf-8") as f:
                         self.config.V_source = float(f.readline().strip())
                         self.config.I_source = float(f.readline().strip())
                         self.config.P_source = float(f.readline().strip())
                         self.config.OVP_level = float(f.readline().strip())
                         self.config.ENA_OCP = (
                             f.readline().strip().lower() == "true"
                         )
 
                     return True
-                except:
+                except Exception:
                     pass  # Do not panic and remain silent
 
         return False
 
     # --------------------------------------------------------------------------
     #   write_config_file
     # --------------------------------------------------------------------------
 
-    def write_config_file(self):
+    def write_config_file(self) -> bool:
         """Try to write the config textfile containing:
              V_source       # Voltage to be sourced [V]
              I_source       # Current to be sourced [A]
              P_source       # Power   to be sourced [W]
              OVP_level      # Over-voltage protection level [V]
              ENA_OCP        # Is over-current protection enabled?
 
@@ -857,28 +875,26 @@
         Returns: True if successful, False otherwise.
         """
         if isinstance(self.path_config, Path):
             if not self.path_config.parent.is_dir():
                 # Subfolder does not exists yet. Create.
                 try:
                     self.path_config.parent.mkdir()
-                except:
+                except Exception:
                     pass  # Do not panic and remain silent
 
             try:
                 # Write the config file
                 self.path_config.write_text(
-                    "%.2f\n%.3f\n%.2f\n%.2f\n%s"
-                    % (
-                        self.state.V_source,
-                        self.state.I_source,
-                        self.state.P_source,
-                        self.state.OVP_level,
-                        self.state.ENA_OCP,
-                    )
+                    f"{self.state.V_source:.2f}\n"
+                    f"{self.state.I_source:.3f}\n"
+                    f"{self.state.P_source:.2f}\n"
+                    f"{self.state.OVP_level:.2f}\n"
+                    f"{self.state.ENA_OCP}",
+                    encoding="utf-8",
                 )
-            except:
+            except Exception:
                 pass  # Do not panic and remain silent
             else:
                 return True
 
         return False
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Keysight_N8700_qdev.py` & `dvg-devices-1.4.0/src/dvg_devices/Keysight_N8700_qdev.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,97 +1,43 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """PyQt/PySide module to provide multithreaded communication and periodical data
 acquisition for a Keysight N8700 power supply (PSU).
+
+TODO: Right now, a PID controller on the power output is injected into the
+device instance as a object member. We should have the PID controller already
+be defined at the class level of 'Keysight_N8700_protocol_SCPI.Keysight_N8700`.
+We should also have the PID parameters be passed as arguments, instead of
+hard-coded here.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=try-except-raise, broad-except
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, multiple-statements, broad-except
 
-import os
-import sys
 import time
 
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt5.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt6.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-    from PySide2.QtCore import Signal                      # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-    from PySide6.QtCore import Signal                      # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Signal, Slot  # type: ignore
 import numpy as np
 
-from dvg_pyqt_controls import (
-    create_Toggle_button,
-    create_tiny_error_LED,
-    SS_TEXTBOX_ERRORS,
-    SS_GROUP,
-)
+import dvg_pyqt_controls as controls
 from dvg_debug_functions import dprint, print_fancy_traceback as pft
 from dvg_pid_controller import PID_Controller
 
 from dvg_qdeviceio import QDeviceIO, DAQ_TRIGGER
 from dvg_devices.Keysight_N8700_protocol_SCPI import Keysight_N8700
 
 # Monospace font
 FONT_MONOSPACE = QtGui.QFont("Monospace", 12, weight=QtGui.QFont.Weight.Bold)
 FONT_MONOSPACE.setStyleHint(QtGui.QFont.StyleHint.TypeWriter)
 
+
 # Enumeration
 class GUI_input_fields:
     [ALL, OVP_level, V_source, I_source, P_source] = range(5)
 
 
 class Keysight_N8700_qdev(QDeviceIO):
     """Manages multithreaded communication and periodical data acquisition for
@@ -128,17 +74,21 @@
         DAQ_interval_ms=200,
         DAQ_timer_type=QtCore.Qt.TimerType.CoarseTimer,
         critical_not_alive_count=1,
         debug=False,
         **kwargs,
     ):
         super().__init__(dev, **kwargs)  # Pass kwargs onto QtCore.QObject()
+        self.dev: Keysight_N8700  # Enforce type: removes `_NoDevice()`
 
         # Add PID controller on the power output
         # DvG, 25-06-2018: Kp=0.5, Ki=2, Kd=0
+        # TODO: Remove hard-coded PID values and have them passed as arguments
+        # via a to-be-written class method inside `Keysight_N8700_protocol_SCPI.
+        # Keysight_N8700`.
         self.dev.PID_power = PID_Controller(Kp=0.5, Ki=2, Kd=0)
 
         self.create_worker_DAQ(
             DAQ_trigger=DAQ_trigger,
             DAQ_function=self.DAQ_function,
             DAQ_interval_ms=DAQ_interval_ms,
             DAQ_timer_type=DAQ_timer_type,
@@ -147,31 +97,33 @@
         )
 
         self.create_worker_jobs(jobs_function=self.jobs_function, debug=debug)
 
         self.create_GUI()
         self.signal_DAQ_updated.connect(self.update_GUI)
         self.signal_GUI_input_field_update.connect(self.update_GUI_input_field)
-        self.connect_signals_to_slots()
 
+        # Update GUI immediately, instead of waiting for the first refresh
         self.update_GUI()
         self.update_GUI_input_field()
 
     # --------------------------------------------------------------------------
     #   DAQ_function
     # --------------------------------------------------------------------------
 
     def DAQ_function(self) -> bool:
         DEBUG_local = False
         if DEBUG_local:
             tick = time.perf_counter()
 
         # Clear input and output buffers of the device. Seems to resolve
         # intermittent communication time-outs.
-        self.dev.device.clear()
+        if self.dev.device is not None:
+            self.dev.device.clear()
+            time.sleep(0.01)
 
         # Finish all operations at the device first
         if not self.dev.wait_for_OPC():
             return False
 
         if not self.dev.query_V_meas():
             return False
@@ -233,25 +185,25 @@
             | self.dev.state.status_QC_INH
         ):
             self.dev.state.ENA_output = False
             self.dev.set_ENA_output(False)
 
         if DEBUG_local:
             tock = time.perf_counter()
-            dprint("%s: done in %i" % (self.dev.name, tock - tick))
+            dprint(f"{self.dev.name}: done in {tock - tick:.3f}")
 
         # Check if there are errors in the device queue and retrieve all
         # if any and append these to 'dev.state.all_errors'.
         if DEBUG_local:
-            dprint("%s: query errors" % self.dev.name)
+            dprint(f"{self.dev.name}: query errors")
             tick = time.perf_counter()
         self.dev.query_all_errors_in_queue()
         if DEBUG_local:
             tock = time.perf_counter()
-            dprint("%s: stb done in %i" % (self.dev.name, tock - tick))
+            dprint(f"{self.dev.name}: stb done in {tock - tick:.3f}")
 
         return True
 
     # --------------------------------------------------------------------------
     #   jobs_function
     # --------------------------------------------------------------------------
 
@@ -283,48 +235,61 @@
         self.P_meas = QtWid.QLabel("0.00  W   ", **p)
 
         # Source
         p = {
             "maximumWidth": 60,
             "alignment": QtCore.Qt.AlignmentFlag.AlignRight,
         }
-        self.pbtn_ENA_output = create_Toggle_button("Output OFF")
+        self.pbtn_ENA_output = controls.create_Toggle_button("Output OFF")
+        self.pbtn_ENA_output.clicked.connect(self.process_pbtn_ENA_output)
         self.V_source = QtWid.QLineEdit("0.00", **p)
         self.I_source = QtWid.QLineEdit("0.000", **p)
         self.P_source = QtWid.QLineEdit("0.00", **p)
-        self.pbtn_ENA_PID = create_Toggle_button(
-            "OFF", minimumHeight=28, minimumWidth=60
+        self.V_source.editingFinished.connect(self.send_V_source_from_textbox)
+        self.I_source.editingFinished.connect(self.send_I_source_from_textbox)
+        self.P_source.editingFinished.connect(self.set_P_source_from_textbox)
+        self.pbtn_ENA_PID = controls.create_Toggle_button(
+            "OFF",
+            minimumHeight=28,
+            minimumWidth=60,
         )
+        self.pbtn_ENA_PID.clicked.connect(self.process_pbtn_ENA_PID)
 
         # Protection
         self.OVP_level = QtWid.QLineEdit("0.000", **p)
-        self.pbtn_ENA_OCP = create_Toggle_button(
-            "OFF", minimumHeight=28, minimumWidth=60
+        self.OVP_level.editingFinished.connect(self.send_OVP_level_from_textbox)
+        self.pbtn_ENA_OCP = controls.create_Toggle_button(
+            "OFF",
+            minimumHeight=28,
+            minimumWidth=60,
         )
+        self.pbtn_ENA_OCP.clicked.connect(self.process_pbtn_ENA_OCP)
 
         # Questionable condition status registers
-        self.status_QC_OV = create_tiny_error_LED()
-        self.status_QC_OC = create_tiny_error_LED()
-        self.status_QC_PF = create_tiny_error_LED()
-        self.status_QC_OT = create_tiny_error_LED()
-        self.status_QC_INH = create_tiny_error_LED()
-        self.status_QC_UNR = create_tiny_error_LED()
+        self.status_QC_OV = controls.create_tiny_error_LED()
+        self.status_QC_OC = controls.create_tiny_error_LED()
+        self.status_QC_PF = controls.create_tiny_error_LED()
+        self.status_QC_OT = controls.create_tiny_error_LED()
+        self.status_QC_INH = controls.create_tiny_error_LED()
+        self.status_QC_UNR = controls.create_tiny_error_LED()
 
         # Operation condition status registers
-        self.status_OC_WTG = create_tiny_error_LED()
-        self.status_OC_CV = create_tiny_error_LED()
-        self.status_OC_CC = create_tiny_error_LED()
+        self.status_OC_WTG = controls.create_tiny_error_LED()
+        self.status_OC_CV = controls.create_tiny_error_LED()
+        self.status_OC_CC = controls.create_tiny_error_LED()
 
         # Final elements
         self.errors = QtWid.QLineEdit("")
-        self.errors.setStyleSheet(SS_TEXTBOX_ERRORS)
+        self.errors.setStyleSheet(controls.SS_TEXTBOX_ERRORS)
         self.pbtn_ackn_errors = QtWid.QPushButton("Acknowledge errors")
+        self.pbtn_ackn_errors.clicked.connect(self.process_pbtn_ackn_errors)
         self.pbtn_reinit = QtWid.QPushButton("Reinitialize")
+        self.pbtn_reinit.clicked.connect(self.process_pbtn_reinit)
         self.pbtn_save_defaults = QtWid.QPushButton("Save")
-        self.pbtn_debug_test = QtWid.QPushButton("Debug test")
+        self.pbtn_save_defaults.clicked.connect(self.process_pbtn_save_defaults)
         self.lbl_update_counter = QtWid.QLabel("0")
 
         i = 0
         grid = QtWid.QGridLayout()
         grid.setVerticalSpacing(0)
         # fmt: off
         grid.addWidget(self.V_meas                       , i, 0, 1, 4); i+=1
@@ -402,27 +367,25 @@
 
         hbox = QtWid.QHBoxLayout()
         hbox.addWidget(self.pbtn_save_defaults)
         hbox.addWidget(self.pbtn_reinit)
         grid.addLayout(hbox                              , i, 0, 1, 4); i+=1
         grid.addItem(QtWid.QSpacerItem(1, 4)             , i, 0)      ; i+=1
         grid.addWidget(self.lbl_update_counter           , i, 0, 1, 4); i+=1
-        # grid.addWidget(self.pbtn_debug_test              , i, 0, 1, 4); i+=1
         # fmt: on
 
         grid.setColumnStretch(0, 0)
         grid.setColumnStretch(1, 0)
         grid.setColumnStretch(2, 0)
         grid.setColumnStretch(3, 1)
         grid.setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
         # grid.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeft)
         self.grid = grid
 
-        self.grpb = QtWid.QGroupBox("%s" % self.dev.name)
-        self.grpb.setStyleSheet(SS_GROUP)
+        self.grpb = QtWid.QGroupBox(f"{self.dev.name}")
         self.grpb.setLayout(self.grid)
 
     # --------------------------------------------------------------------------
     #   update_GUI
     # --------------------------------------------------------------------------
 
     @Slot()
@@ -434,31 +397,31 @@
         Not locking the mutex might speed up the program.
         """
         if self.dev.is_alive:
             if self.dev.state.ENA_PID:
                 self.pbtn_ENA_PID.setChecked(True)
                 self.pbtn_ENA_PID.setText("ON")
                 self.V_source.setReadOnly(True)
-                self.V_source.setText("%.2f" % self.dev.state.V_source)
+                self.V_source.setText(f"{self.dev.state.V_source:.2f}")
             else:
                 self.pbtn_ENA_PID.setChecked(False)
                 self.pbtn_ENA_PID.setText("OFF")
                 self.V_source.setReadOnly(False)
 
             if self.dev.state.status_QC_INH:
                 self.V_meas.setText("")
                 self.I_meas.setText("Inhibited")
                 self.I_meas.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
                 self.P_meas.setText("")
             else:
                 # fmt: off
-                self.V_meas.setText("%.2f  V   " % self.dev.state.V_meas)
-                self.I_meas.setText("%.3f A   "  % self.dev.state.I_meas)
+                self.V_meas.setText(f"{self.dev.state.V_meas:.2f}  V   ")
+                self.I_meas.setText(f"{self.dev.state.I_meas:.3f} A   ")
                 self.I_meas.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
-                self.P_meas.setText("%.2f  W   " % self.dev.state.P_meas)
+                self.P_meas.setText(f"{self.dev.state.P_meas:.2f}  W   ")
                 # fmt: on
 
             self.pbtn_ENA_output.setChecked(self.dev.state.ENA_output)
             if self.pbtn_ENA_output.isChecked():
                 self.pbtn_ENA_output.setText("Output ON")
             else:
                 self.pbtn_ENA_output.setText("Output OFF")
@@ -477,17 +440,17 @@
             self.status_QC_UNR.setChecked(self.dev.state.status_QC_UNR)
 
             self.status_OC_WTG.setChecked(self.dev.state.status_OC_WTG)
             self.status_OC_CV.setChecked(self.dev.state.status_OC_CV)
             self.status_OC_CC.setChecked(self.dev.state.status_OC_CC)
 
             self.errors.setReadOnly(self.dev.state.all_errors != [])
-            self.errors.setText("%s" % ";".join(self.dev.state.all_errors))
+            self.errors.setText(";".join(self.dev.state.all_errors))
 
-            self.lbl_update_counter.setText("%s" % self.update_counter_DAQ)
+            self.lbl_update_counter.setText(f"{self.update_counter_DAQ}")
         else:
             self.V_meas.setText("")
             self.I_meas.setText("Offline")
             self.I_meas.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
             self.P_meas.setText("")
             self.grpb.setEnabled(False)
 
@@ -495,187 +458,183 @@
     #   update_GUI_input_field
     # --------------------------------------------------------------------------
 
     @Slot()
     @Slot(int)
     def update_GUI_input_field(self, GUI_input_field=GUI_input_fields.ALL):
         if GUI_input_field == GUI_input_fields.OVP_level:
-            self.OVP_level.setText("%.2f" % self.dev.state.OVP_level)
+            self.OVP_level.setText(f"{self.dev.state.OVP_level:.2f}")
             self.dev.PID_power.set_output_limits(
                 0, self.dev.state.OVP_level * 0.95
             )
 
         elif GUI_input_field == GUI_input_fields.V_source:
-            self.V_source.setText("%.2f" % self.dev.state.V_source)
+            self.V_source.setText(f"{self.dev.state.V_source:.2f}")
 
         elif GUI_input_field == GUI_input_fields.I_source:
-            self.I_source.setText("%.3f" % self.dev.state.I_source)
+            self.I_source.setText(f"{self.dev.state.I_source:.3f}")
 
         elif GUI_input_field == GUI_input_fields.P_source:
-            self.P_source.setText("%.2f" % self.dev.state.P_source)
+            self.P_source.setText(f"{self.dev.state.P_source:.2f}")
 
         else:
-            self.OVP_level.setText("%.2f" % self.dev.state.OVP_level)
+            self.OVP_level.setText(f"{self.dev.state.OVP_level:.2f}")
             self.dev.PID_power.set_output_limits(
                 0, self.dev.state.OVP_level * 0.95
             )
 
-            self.V_source.setText("%.2f" % self.dev.state.V_source)
-            self.I_source.setText("%.3f" % self.dev.state.I_source)
-            self.P_source.setText("%.2f" % self.dev.state.P_source)
+            self.V_source.setText(f"{self.dev.state.V_source:.2f}")
+            self.I_source.setText(f"{self.dev.state.I_source:.3f}")
+            self.P_source.setText(f"{self.dev.state.P_source:.2f}")
 
     # --------------------------------------------------------------------------
     #   GUI functions
     # --------------------------------------------------------------------------
 
+    @Slot()
     def process_pbtn_ENA_output(self):
         if self.pbtn_ENA_output.isChecked():
             # Clear output protection, if triggered and turn on output
             self.send(self.dev.clear_output_protection_and_turn_on)
         else:
             # Turn off output
             self.send(self.dev.turn_off)
 
+    @Slot()
     def process_pbtn_ENA_PID(self):
         self.dev.state.ENA_PID = self.pbtn_ENA_PID.isChecked()
 
+    @Slot()
     def process_pbtn_ENA_OCP(self):
         self.send(self.dev.set_ENA_OCP, self.pbtn_ENA_OCP.isChecked())
 
+    @Slot()
     def process_pbtn_ackn_errors(self):
         # Lock the dev mutex because string operations are not atomic
-        locker = QtCore.QMutexLocker(self.dev.mutex)
+        locker = QtCore.QMutexLocker(self.dev.mutex)  # type: ignore
         self.dev.state.all_errors = []
         self.errors.setText("")
         self.errors.setReadOnly(False)  # To change back to regular colors
         locker.unlock()
 
+    @Slot()
     def process_pbtn_reinit(self):
-        str_msg = "Are you sure you want reinitialize the power supply?"
-        reply = QtWid.QMessageBox.question(
-            None,
-            ("Reinitialize %s" % self.dev.name),
-            str_msg,
-            QtWid.QMessageBox.Yes | QtWid.QMessageBox.No,
-            QtWid.QMessageBox.No,
+        title = f"Reinitialize {self.dev.name}"
+        msg = "Are you sure you want reinitialize the power supply?"
+        msgbox = QtWid.QMessageBox()
+        msgbox.setIcon(QtWid.QMessageBox.Icon.Question)
+        msgbox.setWindowTitle(title)
+        msgbox.setText(msg)
+        msgbox.setStandardButtons(
+            QtWid.QMessageBox.StandardButton.Yes
+            | QtWid.QMessageBox.StandardButton.No
         )
+        msgbox.setDefaultButton(QtWid.QMessageBox.StandardButton.No)
+        reply = msgbox.exec()
 
-        if reply == QtWid.QMessageBox.Yes:
+        if reply == QtWid.QMessageBox.StandardButton.Yes:
             self.dev.read_config_file()
             self.add_to_jobs_queue(self.dev.reinitialize)
             self.add_to_jobs_queue(
                 "signal_GUI_input_field_update", GUI_input_fields.ALL
             )
             self.process_jobs_queue()
 
             self.dev.state.ENA_PID = False
 
+    @Slot()
     def process_pbtn_save_defaults(self):
-        str_title = "Save defaults %s" % self.dev.name
-        str_msg = (
+        title = f"Save defaults {self.dev.name}"
+        msg = (
             "Are you sure you want to save the current values:\n\n"
             "  - Source voltage\n"
             "  - Source current\n"
             "  - Source power\n"
             "  - OVP\n"
             "  - OCP\n\n"
             "as default?\n"
             "These will then automatically be loaded next time."
         )
-        reply = QtWid.QMessageBox.question(
-            None,
-            str_title,
-            str_msg,
-            QtWid.QMessageBox.Yes | QtWid.QMessageBox.No,
-            QtWid.QMessageBox.No,
+        msgbox = QtWid.QMessageBox()
+        msgbox.setIcon(QtWid.QMessageBox.Icon.Question)
+        msgbox.setWindowTitle(title)
+        msgbox.setText(msg)
+        msgbox.setStandardButtons(
+            QtWid.QMessageBox.StandardButton.Yes
+            | QtWid.QMessageBox.StandardButton.No
         )
+        msgbox.setDefaultButton(QtWid.QMessageBox.StandardButton.No)
+        reply = msgbox.exec()
 
-        if reply == QtWid.QMessageBox.Yes:
+        if reply == QtWid.QMessageBox.StandardButton.Yes:
             if self.dev.write_config_file():
-                QtWid.QMessageBox.information(
-                    None,
-                    str_title,
-                    "Successfully saved to disk:\n%s" % self.dev.path_config,
-                )
+                icon = QtWid.QMessageBox.Icon.Information
+                msg = f"Successfully saved to disk:\n{self.dev.path_config}"
             else:
-                QtWid.QMessageBox.critical(
-                    None,
-                    str_title,
-                    "Failed to save to disk:\n%s" % self.dev.path_config,
-                )
+                icon = QtWid.QMessageBox.Icon.Critical
+                msg = f"Failed to save to disk:\n{self.dev.path_config}"
 
-    def process_pbtn_debug_test(self):
-        pass
+            msgbox = QtWid.QMessageBox()
+            msgbox.setIcon(icon)
+            msgbox.setWindowTitle(title)
+            msgbox.setText(msg)
+            msgbox.exec()
 
+    @Slot()
     def send_V_source_from_textbox(self):
         try:
             voltage = float(self.V_source.text())
         except (TypeError, ValueError):
             voltage = 0.0
-        except:
-            raise
+        except Exception as err:
+            raise err
 
         self.add_to_jobs_queue(self.dev.set_V_source, max(voltage, 0))
         self.add_to_jobs_queue(self.dev.query_V_source)
         self.add_to_jobs_queue(
             "signal_GUI_input_field_update", GUI_input_fields.V_source
         )
         self.process_jobs_queue()
 
+    @Slot()
     def send_I_source_from_textbox(self):
         try:
             current = float(self.I_source.text())
         except (TypeError, ValueError):
             current = 0.0
-        except:
-            raise
+        except Exception as err:
+            raise err
 
         self.add_to_jobs_queue(self.dev.set_I_source, max(current, 0))
         self.add_to_jobs_queue(self.dev.query_I_source)
         self.add_to_jobs_queue(
             "signal_GUI_input_field_update", GUI_input_fields.I_source
         )
         self.process_jobs_queue()
 
+    @Slot()
     def set_P_source_from_textbox(self):
         try:
             power = float(self.P_source.text())
         except (TypeError, ValueError):
             power = 0.0
-        except:
-            raise
+        except Exception as err:
+            raise err
 
         self.dev.state.P_source = max(power, 0)
         self.update_GUI_input_field(GUI_input_fields.P_source)
 
+    @Slot()
     def send_OVP_level_from_textbox(self):
         try:
             OVP_level = float(self.OVP_level.text())
         except (TypeError, ValueError):
             OVP_level = 0.0
-        except:
-            raise
+        except Exception as err:
+            raise err
 
         self.add_to_jobs_queue(self.dev.set_OVP_level, OVP_level)
         self.add_to_jobs_queue(self.dev.query_OVP_level)
         self.add_to_jobs_queue(
             "signal_GUI_input_field_update", GUI_input_fields.OVP_level
         )
         self.process_jobs_queue()
-
-    # --------------------------------------------------------------------------
-    #   connect_signals_to_slots
-    # --------------------------------------------------------------------------
-
-    def connect_signals_to_slots(self):
-        self.pbtn_ENA_output.clicked.connect(self.process_pbtn_ENA_output)
-        self.pbtn_ENA_PID.clicked.connect(self.process_pbtn_ENA_PID)
-        self.pbtn_ENA_OCP.clicked.connect(self.process_pbtn_ENA_OCP)
-        self.pbtn_ackn_errors.clicked.connect(self.process_pbtn_ackn_errors)
-        self.pbtn_reinit.clicked.connect(self.process_pbtn_reinit)
-        self.pbtn_save_defaults.clicked.connect(self.process_pbtn_save_defaults)
-        self.pbtn_debug_test.clicked.connect(self.process_pbtn_debug_test)
-
-        self.V_source.editingFinished.connect(self.send_V_source_from_textbox)
-        self.I_source.editingFinished.connect(self.send_I_source_from_textbox)
-        self.P_source.editingFinished.connect(self.set_P_source_from_textbox)
-        self.OVP_level.editingFinished.connect(self.send_OVP_level_from_textbox)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Picotech_PT104_protocol_UDP.py` & `dvg-devices-1.4.0/src/dvg_devices/Picotech_PT104_protocol_UDP.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
+"""Ethernet UDP function library for a Picotech PT-104 pt100/1000 temperature
+logger.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "14-09-2022"
-__version__ = "1.0.0"
-# pylint: disable=try-except-raise
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, multiple-statements
 
 import socket
+from typing import Union, Tuple, List
+
 import numpy as np
 
 # ITS-90 resistance-temperature relation for PT100/PT1000
 # R_t = R_0 * (1 + A*t + B*t^2 + C*(t-100)*t^3)
 # R_t: resistance at T 'C   [Ohm]
 # R_0: resistance at 0 'C   [Ohm]
 # t  : temperature          ['C]
@@ -33,100 +36,100 @@
 # fmt: on
 
 # Timeout on the socket communication
 # Keep the timeout shorter than the scan rate of ~ 720 ms otherwise the method
 # 'scan_4_wire_temperature' will break.
 SOCKET_TIMEOUT = 0.5  # 0.5 [s]
 
-DEBUG = False
-
 
 class Picotech_PT104:
     class Eeprom:
         # Container for the PT-104 specific values retreived from its memory
         # fmt: off
-        serial     = None
-        calib_date = None
-        ch1_calib  = None
-        ch2_calib  = None
-        ch3_calib  = None
-        ch4_calib  = None
-        MAC        = None
-        checksum   = None
+        serial    : str = ""
+        calib_date: str = ""
+        ch1_calib : int = 0
+        ch2_calib : int = 0
+        ch3_calib : int = 0
+        ch4_calib : int = 0
+        MAC       : str = ""
+        checksum  : str = ""
         # fmt: on
 
     class State:
         # Container for the process and measurement variables
         # Resistance readings of channels 1 to 4 [Ohm]
-        ch1_R = np.nan
-        ch2_R = np.nan
-        ch3_R = np.nan
-        ch4_R = np.nan
+        ch1_R: float = np.nan
+        ch2_R: float = np.nan
+        ch3_R: float = np.nan
+        ch4_R: float = np.nan
         # Temperature readings of channels 1 to 4 ['C]
-        ch1_T = np.nan
-        ch2_T = np.nan
-        ch3_T = np.nan
-        ch4_T = np.nan
+        ch1_T: float = np.nan
+        ch2_T: float = np.nan
+        ch3_T: float = np.nan
+        ch4_T: float = np.nan
 
     # --------------------------------------------------------------------------
     #   __init__
     # --------------------------------------------------------------------------
 
-    def __init__(self, name="PT104"):
-        self.name = name
-        self._ip_address = None
-        self._port = None
-        self._sock = None
+    def __init__(self, name: str = "PT104"):
+        self.name: str = name
+        self._ip_address: str = ""
+        self._port: int = 0
+        self._sock: Union[socket.socket, None] = None
         self._eeprom = self.Eeprom()
 
         # List corresponding to channels 1 to 4, where
         #    0: channel off
         #    1: channel on
-        self._ENA_channels = [0, 0, 0, 0]
+        self._ENA_channels: list[int] = [0, 0, 0, 0]
 
         # List corresponding to channels 1 to 4, where
         #    0: 1x gain
         #    1: 21x gain (for 375 Ohm range)
-        self._gain_channels = [0, 0, 0, 0]
+        self._gain_channels: list[int] = [0, 0, 0, 0]
 
         # Resistance at 0 'C of channels 1 to 4 [Ohm]
         # For a PT100  probe this should be 100.000 Ohm
         # For a PT1000 probe this should be 1000.000 Ohm
-        self.ch1_R_0 = 100
-        self.ch2_R_0 = 100
-        self.ch3_R_0 = 100
-        self.ch4_R_0 = 100
+        self.ch1_R_0: float = 100.0
+        self.ch2_R_0: float = 100.0
+        self.ch3_R_0: float = 100.0
+        self.ch4_R_0: float = 100.0
 
         # Is the connection to the device alive?
-        self.is_alive = False
+        self.is_alive: bool = False
 
         # Container for the measurement variables
         self.state = self.State()
 
     # --------------------------------------------------------------------------
     #   close
     # --------------------------------------------------------------------------
 
     def close(self):
-        self._sock.close()
+        if self._sock is not None:
+            self._sock.close()
+
         self.is_alive = False
 
     # --------------------------------------------------------------------------
     #   connect
     # --------------------------------------------------------------------------
 
-    def connect(self, ip_address="10.10.100.2", port=1234):
+    def connect(self, ip_address: str = "10.10.100.2", port: int = 1234):
         """
         Returns: True if successful, False otherwise.
         """
         self._ip_address = ip_address
         self._port = port
 
         print("Connect to: PicoTech PT-104")
-        print("  @ ip=%s:%i : " % (ip_address, port), end="")
+        print(f"  @ ip={ip_address}:{port} : ", end="")
 
         # Open UDP socket
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.settimeout(SOCKET_TIMEOUT)  # timeout on commands
 
         # Try to acquire a lock to the PT-104
         success = self.lock()
@@ -140,147 +143,163 @@
 
         return success
 
     # --------------------------------------------------------------------------
     #   begin
     # --------------------------------------------------------------------------
 
-    def begin(self):
+    def begin(self) -> bool:
         """
         Returns: True if successful, False otherwise.
         """
         success = self.lock()
         success &= self.read_EEPROM()
         return success
 
     # --------------------------------------------------------------------------
     #   UDP_send
     # --------------------------------------------------------------------------
 
-    def UDP_send(self, msg_bytes):
+    def UDP_send(self, msg_bytes: bytes):
         """
         msg_bytes (bytes): Message to be sent over the UDP port.
         """
-        self._sock.sendto(msg_bytes, (self._ip_address, self._port))
+        if self._sock is not None:
+            self._sock.sendto(msg_bytes, (self._ip_address, self._port))
 
     # --------------------------------------------------------------------------
     #   UDP_recv
     # --------------------------------------------------------------------------
 
-    def UDP_recv(self):
+    def UDP_recv(self) -> Tuple[bool, Union[bytes, None]]:
         """Receive one UDP packet at a time when available.
 
         Returns:
             success (bool):
                 True if a packet was received successfully, False otherwise.
 
-            ans_bytes:
+            reply:
                 UDP packet received from the device. None if unsuccessful.
         """
         success = False
-        ans_bytes = None
+        reply = None
 
-        try:
-            ans_bytes = self._sock.recv(4096)
-            success = True
-        except socket.timeout:
-            # print("ERROR: socket.recv() timed out in query()")
-            pass  # Stay silent and continue
-        except:
-            raise
+        if self._sock is not None:
+            try:
+                reply = self._sock.recv(4096)
+                success = True
+            except socket.timeout:
+                # print("ERROR: socket.recv() timed out in query()")
+                pass  # Stay silent and continue
+            except Exception as err:
+                raise err
 
-        return success, ans_bytes
+        return success, reply
 
     # --------------------------------------------------------------------------
     #   UDP_query_and_check
     # --------------------------------------------------------------------------
 
-    def UDP_query_and_check(self, msg_bytes, check_ans_bytes):
+    def UDP_query_and_check(
+        self,
+        msg_bytes: bytes,
+        check_reply_bytes: bytes,
+    ) -> Tuple[bool, Union[bytes, None]]:
         """
         Args:
             msg_bytes (bytes):
                 Message to be sent over the UDP port.
 
+            check_reply_bytes (bytes):
+                Compare the reply received from the device against these bytes.
+                When the reply matches the check, we call it a success,
+                otherwise not.
+
         Returns:
             success (bool):
                 True if successful, False otherwise.
-            ans_bytes (bytes):
+
+            reply (bytes):
                 Reply received from the device. None if unsuccessful.
         """
         self.UDP_send(msg_bytes)
 
         # Try up to 3 times at maximum to receive the respective response
         # UDP packet belonging to above sent UDP packet.
         for _i in range(3):
-            success, ans_bytes = self.UDP_recv()
-            if success:
-                if ans_bytes[: len(check_ans_bytes)] == check_ans_bytes:
-                    return True, ans_bytes
+            _success, reply = self.UDP_recv()
+            if isinstance(reply, bytes):
+                if reply[: len(check_reply_bytes)] == check_reply_bytes:
+                    return True, reply
 
-                print("Failed %s: received %s" % (msg_bytes, ans_bytes))
+                print(f"Failed {msg_bytes}: received {reply}")
 
         return False, None
 
     # --------------------------------------------------------------------------
     #   PT-104 functions
     #   Will return True when successful, False when failed
     # --------------------------------------------------------------------------
 
-    def lock(self):
-        success, _ans = self.UDP_query_and_check(b"lock\r", b"Lock Success")
+    def lock(self) -> bool:
+        success, _reply = self.UDP_query_and_check(b"lock\r", b"Lock Success")
         return success
 
-    def set_mains_rejection_50Hz(self):
-        success, _ans = self.UDP_query_and_check(
+    def set_mains_rejection_50Hz(self) -> bool:
+        success, _reply = self.UDP_query_and_check(
             bytes([0x30, 0x00]), b"Mains Changed"
         )
         return success
 
-    def set_mains_rejection_60Hz(self):
-        success, _ans = self.UDP_query_and_check(
+    def set_mains_rejection_60Hz(self) -> bool:
+        success, _reply = self.UDP_query_and_check(
             bytes([0x30, 0x01]), b"Mains Changed"
         )
         return success
 
-    def keep_alive(self):
-        success, _ans = self.UDP_query_and_check(bytes([0x34]), b"Alive")
+    def keep_alive(self) -> bool:
+        success, _reply = self.UDP_query_and_check(bytes([0x34]), b"Alive")
         if not success:
             print("PT104 is not alive anymore.")
         return success
 
-    def read_EEPROM(self):
-        success, ans = self.UDP_query_and_check(bytes([0x32]), b"Eeprom")
+    def read_EEPROM(self) -> bool:
+        _success, reply = self.UDP_query_and_check(bytes([0x32]), b"Eeprom")
 
-        if success:
+        if isinstance(reply, bytes):
             # Parse
             # fmt: off
-            ans        = ans[7:]   # Discard the first 7 bytes reading 'Eeprom='
-            serial     = ans[19:29].decode("UTF8")
-            calib_date = ans[29:37].decode("UTF8")
-            ch1_calib  = int.from_bytes(ans[37:41], byteorder="little")
-            ch2_calib  = int.from_bytes(ans[41:45], byteorder="little")
-            ch3_calib  = int.from_bytes(ans[45:49], byteorder="little")
-            ch4_calib  = int.from_bytes(ans[49:53], byteorder="little")
-            MAC        = ":".join("%02x" % b for b in ans[53:59])
-            checksum   = " ".join("0x%02x" % b for b in ans[126:128])
+            reply      = reply[7:]  # Discard first 7 bytes reading 'Eeprom='
+            serial     = reply[19:29].decode("UTF8")
+            calib_date = reply[29:37].decode("UTF8")
+            ch1_calib  = int.from_bytes(reply[37:41], byteorder="little")
+            ch2_calib  = int.from_bytes(reply[41:45], byteorder="little")
+            ch3_calib  = int.from_bytes(reply[45:49], byteorder="little")
+            ch4_calib  = int.from_bytes(reply[49:53], byteorder="little")
+            MAC        = ":".join(f"{b:02x}" for b in reply[53:59])
+            checksum   = " ".join(f"0x{b:02x}" for b in reply[126:128])
 
             self._eeprom.serial     = serial
             self._eeprom.calib_date = calib_date
             self._eeprom.ch1_calib  = ch1_calib
             self._eeprom.ch2_calib  = ch2_calib
             self._eeprom.ch3_calib  = ch3_calib
             self._eeprom.ch4_calib  = ch4_calib
             self._eeprom.MAC        = MAC
             self._eeprom.checksum   = checksum
             # fmt: on
             return True
 
         return False
 
-    def start_conversion(self, ENA_channels=None, gain_channels=None):
+    def start_conversion(
+        self,
+        ENA_channels: Union[List[int], None] = None,
+        gain_channels: Union[List[int], None] = None,
+    ) -> bool:
         """
         Starts the continuous acquisition of measurements over channels 1 to 4
         ENA_channel is a list corresponding to channels 1 to 4, where
             0: channel off
             1: channel on
         gain_channels is a list corresponding to channels 1 to 4, where
             0: 1x gain
@@ -294,72 +313,71 @@
         )
 
         data_byte = 0
         data_byte += self._ENA_channels[0]
         data_byte += self._ENA_channels[1] * 2
         data_byte += self._ENA_channels[2] * 4
         data_byte += self._ENA_channels[3] * 8
-        data_byte += gain_channels[0] * 16
-        data_byte += gain_channels[1] * 32
-        data_byte += gain_channels[2] * 64
-        data_byte += gain_channels[3] * 128
+        data_byte += self._gain_channels[0] * 16
+        data_byte += self._gain_channels[1] * 32
+        data_byte += self._gain_channels[2] * 64
+        data_byte += self._gain_channels[3] * 128
 
-        success, _ans = self.UDP_query_and_check(
+        success, _reply = self.UDP_query_and_check(
             bytes([0x31, data_byte]), b"Converting"
         )
         return success
 
     # --------------------------------------------------------------------------
     #   report_EEPROM
     # --------------------------------------------------------------------------
 
     def report_EEPROM(self):
         print("EEPROM")
-        print("  serial    : %s" % self._eeprom.serial)
-        print("  calib_date: %s" % self._eeprom.calib_date)
-        print("  ch1_calib : %s" % self._eeprom.ch1_calib)
-        print("  ch2_calib : %s" % self._eeprom.ch2_calib)
-        print("  ch3_calib : %s" % self._eeprom.ch3_calib)
-        print("  ch4_calib : %s" % self._eeprom.ch4_calib)
-        print("  MAC       : %s" % self._eeprom.MAC)
-        print("  checksum  : %s" % self._eeprom.checksum)
+        print(f"  serial    : {self._eeprom.serial}")
+        print(f"  calib_date: {self._eeprom.calib_date}")
+        print(f"  ch1_calib : {self._eeprom.ch1_calib}")
+        print(f"  ch2_calib : {self._eeprom.ch2_calib}")
+        print(f"  ch3_calib : {self._eeprom.ch3_calib}")
+        print(f"  ch4_calib : {self._eeprom.ch4_calib}")
+        print(f"  MAC       : {self._eeprom.MAC}")
+        print(f"  checksum  : {self._eeprom.checksum}")
 
     # --------------------------------------------------------------------------
     #   scan_4_wire_temperature
     # --------------------------------------------------------------------------
 
-    def scan_4_wire_temperature(self):
+    def scan_4_wire_temperature(self) -> bool:
         """Reads the UDP port for any message, presumably the measurement of the
         channels reported by the PT104, after conversion has initiated.
         These readings are transformed into resistance (Ohm) using the
         calibration constants retreived from EEPROM, and again transformed to
         temperature ('C) using the ITS-90 resistance-temperature relation
         for PT100/PT1000. Four-wire measurements are assumed.
 
         Returns: True if successful, False otherwise.
         """
 
         ## Send keep alive signal. We care about the reply later.
         self.UDP_send(bytes([0x34]))
 
-        success, ans = self.UDP_recv()
-        while success:
-            if ans[0] == 0 or ans[0] == 4 or ans[0] == 8 or ans[0] == 12:
+        _success, reply = self.UDP_recv()
+        while isinstance(reply, bytes):
+            if (
+                reply[0] == 0
+                or reply[0] == 4
+                or reply[0] == 8
+                or reply[0] == 12
+            ):
                 # Packet containing temperature reading
-
-                ch = (
-                    ans[0] / 4 + 1
-                )  # Determine the channel number being reported
-                a_0 = int.from_bytes(ans[1:5], byteorder="big")
-                a_1 = int.from_bytes(ans[6:10], byteorder="big")
-                a_2 = int.from_bytes(ans[11:15], byteorder="big")
-                a_3 = int.from_bytes(ans[16:20], byteorder="big")
-
-                if DEBUG:
-                    print("CH %i" % ch)
+                ch = int(reply[0]) / 4 + 1
+                a_0 = int.from_bytes(reply[1:5], byteorder="big")
+                a_1 = int.from_bytes(reply[6:10], byteorder="big")
+                a_2 = int.from_bytes(reply[11:15], byteorder="big")
+                a_3 = int.from_bytes(reply[16:20], byteorder="big")
 
                 # fmt: off
                 if   ch==1: calib = self._eeprom.ch1_calib; R_0 = self.ch1_R_0
                 elif ch==2: calib = self._eeprom.ch2_calib; R_0 = self.ch2_R_0
                 elif ch==3: calib = self._eeprom.ch3_calib; R_0 = self.ch3_R_0
                 elif ch==4: calib = self._eeprom.ch4_calib; R_0 = self.ch4_R_0
                 # fmt: on
@@ -386,25 +404,25 @@
                 # fmt: off
                 if   ch == 1: self.state.ch1_R = R_T; self.state.ch1_T = T
                 elif ch == 2: self.state.ch2_R = R_T; self.state.ch2_T = T
                 elif ch == 3: self.state.ch3_R = R_T; self.state.ch3_T = T
                 elif ch == 4: self.state.ch4_R = R_T; self.state.ch4_T = T
                 # fmt: on
 
-            elif ans[:5] == b"Alive":
+            elif reply[:5] == b"Alive":
                 # Packet containing alive response. Stay silent.
                 pass
 
             else:
                 # Other packet?
-                print("  %s" % ans)
+                print(f"  {reply}")
                 return False
 
             # Receive a possible next packet from the UDP in-buffer
-            success, ans = self.UDP_recv()
+            _success, reply = self.UDP_recv()
 
         # No more packets
         return True
 
 
 # ------------------------------------------------------------------------------
 #   ITS90 transform functions
@@ -416,15 +434,15 @@
     # R_T = R_0 * (1 + A*T + B*T^2 + C*(T-100)*T^3)
     # R_T: resistance at T 'C   [Ohm]
     # R_0: resistance at 0 'C   [Ohm]
     # T  : temperature          ['C]
     # A = 3.9083e-3
     # B = -5.775e-7
     # C = -4.183e-12  # when below 0 'C, C = 0 when above 0 'C
-    return R_0 * (1 + A * T + B * T ** 2 + C * (T - 100) * T ** 3)
+    return R_0 * (1 + A * T + B * T**2 + C * (T - 100) * T**3)
 
 
 def ITS90_Ohm_to_degC(R_0, R_T):
     # ITS-90 resistance-temperature relation
     # R_T = R_0 * (1 + A*T + B*T^2 + C*(T-100)*T^3)
     # R_T: resistance at T 'C   [Ohm]
     # R_0: resistance at 0 'C   [Ohm]
@@ -432,19 +450,19 @@
     # A = 3.9083e-3
     # B = -5.775e-7
     # C = -4.183e-12  # when below 0 'C, C = 0 when above 0 'C
 
     if R_T >= R_0:
         # We are in the range T >= 0'C
         # Hence, simply solve quadratic equation because C = 0
-        sqrt_arg = A ** 2 - 4 * B * (1 - R_T / R_0)
+        sqrt_arg = A**2 - 4 * B * (1 - R_T / R_0)
         if sqrt_arg < 0:
             return np.nan
-        else:
-            T = (-A + np.sqrt(sqrt_arg)) / (2 * B)
+
+        T = (-A + np.sqrt(sqrt_arg)) / (2 * B)
 
     else:
         # We are in the range T < 0'C, hence we need to solve a quartic
         # equation. Difficult to solve by algebra. We do it numerically
         # up to a certain convergence error. A convergence of
         # 0.1 milli-Kelvin is more than sufficient for the PT-104 logger.
         CONV = 1e-4  # [K]
@@ -477,37 +495,37 @@
             # Next best guess
             T_g = (T_hi + T_lo) / 2.0
 
             i += 1
             if i > MAX_ITER:
                 print(
                     "WARNING: Loop in ITS90_Ohm_to_degC() terminated after "
-                    "%d iterations" % MAX_ITER
+                    f"{MAX_ITER} iterations"
                 )
                 break
 
         # We have reached convergence
         T = T_g
 
     if T > T_MAX:
-        print("WARNING: Temperature is out of range because > %.0f 'C" % T_MAX)
+        print(f"WARNING: Temperature is out of range because > {T_MAX:.0f} 'C")
+
     elif T <= T_MIN + 1e-4:
-        print("WARNING: Temperature is out of range because <= %.0f 'C" % T_MIN)
+        print(f"WARNING: Temperature is out of range because <= {T_MIN:.0f} 'C")
 
     return T
 
 
 # ------------------------------------------------------------------------------
 #   Debug functions
 # ------------------------------------------------------------------------------
 
 
-def print_as_hex(byte_list):
-    list(map(lambda x: print(format(x, "02x"), end=" "), byte_list))
-    print()
+def pretty_bytes_to_hex(values: bytes) -> str:
+    return " ".join(f"{b:02x}" for b in values)
 
 
 # ------------------------------------------------------------------------------
 #   Main
 # ------------------------------------------------------------------------------
 
 if __name__ == "__main__":
@@ -525,18 +543,19 @@
         pt104.report_EEPROM()
     else:
         print("ERROR: Could not connect to PT-104 and acquire a lock.")
         sys.exit(0)
 
     # Start the conversion (DAQ)
     if pt104.start_conversion(
-        ENA_channels=[1, 1, 0, 0], gain_channels=[1, 1, 0, 0]
+        ENA_channels=[1, 1, 0, 0],
+        gain_channels=[1, 1, 0, 0],
     ):
         print("\nConverting")
     else:
         print("\nERROR: Failed start_conversion()")
 
     # Continuous reading as fast as possible
     print("\nT1 ['C]\tT2 ['C]")
     while 1:
         pt104.scan_4_wire_temperature()
-        print("\r%.3f\t%.3f" % (pt104.state.ch1_T, pt104.state.ch2_T), end="")
+        print(f"\r{pt104.state.ch1_T:.3f}\t{pt104.state.ch2_T:.3f}", end="")
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Picotech_PT104_qdev.py` & `dvg-devices-1.4.0/src/dvg_devices/Picotech_PT104_qdev.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,76 +2,22 @@
 # -*- coding: utf-8 -*-
 """PyQt/PySide module to provide multithreaded communication and periodical data
 acquisition for a Picotech PT-104 pt100/1000 temperature logger.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-
-import os
-import sys
-
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring
 
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Slot  # type: ignore
 import numpy as np
 
-from dvg_pyqt_controls import SS_GROUP
-
 from dvg_qdeviceio import QDeviceIO, DAQ_TRIGGER
 from dvg_devices.Picotech_PT104_protocol_UDP import Picotech_PT104
 
 # Special characters
 CHAR_DEG_C = chr(176) + "C"
 
 
@@ -116,14 +62,15 @@
         DAQ_interval_ms=1000,
         DAQ_timer_type=QtCore.Qt.TimerType.CoarseTimer,
         critical_not_alive_count=np.nan,
         debug=False,
         **kwargs,
     ):
         super().__init__(dev, **kwargs)  # Pass kwargs onto QtCore.QObject()
+        self.dev: Picotech_PT104  # Enforce type: removes `_NoDevice()`
 
         self.create_worker_DAQ(
             DAQ_trigger=DAQ_TRIGGER.INTERNAL_TIMER,
             DAQ_function=self.DAQ_function,
             DAQ_interval_ms=DAQ_interval_ms,
             DAQ_timer_type=DAQ_timer_type,
             critical_not_alive_count=critical_not_alive_count,
@@ -135,38 +82,39 @@
         if not self.dev.is_alive:
             self.update_GUI()  # Correctly reflect an offline device
 
     # --------------------------------------------------------------------------
     #   DAQ_function
     # --------------------------------------------------------------------------
 
-    def DAQ_function(self):
+    def DAQ_function(self) -> bool:
         # print("Obtained interval: %.0f" % self.obtained_DAQ_interval_ms)
         return self.dev.scan_4_wire_temperature()
 
     # --------------------------------------------------------------------------
     #   create_GUI
     # --------------------------------------------------------------------------
 
     def create_GUI(self):
-        self.qlbl_offline = QtWid.QLabel(
-            "OFFLINE",
-            visible=False,
-            font=QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold),
-            alignment=QtCore.Qt.AlignmentFlag.AlignCenter,
+        self.qlbl_offline = QtWid.QLabel("OFFLINE")
+        self.qlbl_offline.setVisible(False)
+        self.qlbl_offline.setFont(
+            QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold)
         )
+        self.qlbl_offline.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
 
         p = {
             "alignment": QtCore.Qt.AlignmentFlag.AlignRight,
             "minimumWidth": 60,
+            "readOnly": True,
         }
-        self.qled_T_ch1 = QtWid.QLineEdit(**p, readOnly=True)
-        self.qled_T_ch2 = QtWid.QLineEdit(**p, readOnly=True)
-        self.qled_T_ch3 = QtWid.QLineEdit(**p, readOnly=True)
-        self.qled_T_ch4 = QtWid.QLineEdit(**p, readOnly=True)
+        self.qled_T_ch1 = QtWid.QLineEdit(**p)
+        self.qled_T_ch2 = QtWid.QLineEdit(**p)
+        self.qled_T_ch3 = QtWid.QLineEdit(**p)
+        self.qled_T_ch4 = QtWid.QLineEdit(**p)
         self.qlbl_update_counter = QtWid.QLabel("0")
 
         self.grid = QtWid.QGridLayout()
         self.grid.setVerticalSpacing(4)
         # fmt: off
         self.grid.addWidget(self.qlbl_offline       , 0, 0, 1, 3)
         self.grid.addWidget(QtWid.QLabel("Ch 1")    , 1, 0)
@@ -180,31 +128,30 @@
         self.grid.addWidget(QtWid.QLabel(CHAR_DEG_C), 3, 2)
         self.grid.addWidget(QtWid.QLabel("Ch 4")    , 4, 0)
         self.grid.addWidget(self.qled_T_ch4         , 4, 1)
         self.grid.addWidget(QtWid.QLabel(CHAR_DEG_C), 4, 2)
         self.grid.addWidget(self.qlbl_update_counter, 5, 0, 1, 3)
         # fmt: on
 
-        self.qgrp = QtWid.QGroupBox("%s" % self.dev.name)
-        self.qgrp.setStyleSheet(SS_GROUP)
+        self.qgrp = QtWid.QGroupBox(f"{self.dev.name}")
         self.qgrp.setLayout(self.grid)
 
     # --------------------------------------------------------------------------
     #   update_GUI
     # --------------------------------------------------------------------------
 
     @Slot()
     def update_GUI(self):
         """NOTE: 'self.dev.mutex' is not being locked, because we are only
         reading 'state' for displaying purposes. We can do this because 'state'
         members are written and read atomicly.
         Not locking the mutex might speed up the program.
         """
         if self.dev.is_alive:
-            self.qled_T_ch1.setText("%.3f" % self.dev.state.ch1_T)
-            self.qled_T_ch2.setText("%.3f" % self.dev.state.ch2_T)
-            self.qled_T_ch3.setText("%.3f" % self.dev.state.ch3_T)
-            self.qled_T_ch4.setText("%.3f" % self.dev.state.ch4_T)
-            self.qlbl_update_counter.setText("%s" % self.update_counter_DAQ)
+            self.qled_T_ch1.setText(f"{self.dev.state.ch1_T:.3f}")
+            self.qled_T_ch2.setText(f"{self.dev.state.ch2_T:.3f}")
+            self.qled_T_ch3.setText(f"{self.dev.state.ch3_T:.3f}")
+            self.qled_T_ch4.setText(f"{self.dev.state.ch4_T:.3f}")
+            self.qlbl_update_counter.setText(f"{self.update_counter_DAQ}")
         else:
             self.qgrp.setEnabled(False)
             self.qlbl_offline.setVisible(True)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/PolyScience_PD_bath_protocol_RS232.py` & `dvg-devices-1.4.0/src/dvg_devices/PolyScience_PD_bath_protocol_RS232.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     PD07R-20, PD07R-40, PD7LR-20, PD15R-30, PD15R-40, PD20R-30, PD28R-30,
     PD45R-20, PD07H200, PD15H200, PD20H200, PD28H200, PD15RCAL, PD15HCAL.
 Tested on model PD15R-30‐A12E
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "27-10-2022"
-__version__ = "0.3.0"
-# pylint: disable=try-except-raise, bare-except
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, multiple-statements
 
 import sys
 from typing import Tuple
 
 import numpy as np
 
 from dvg_debug_functions import print_fancy_traceback as pft
@@ -26,20 +26,24 @@
 BATH_MAX_SETPOINT_DEG_C = 87  # [deg C]
 
 
 class PolyScience_PD_bath(SerialDevice):
     class State:
         # Container for the process and measurement variables
         # fmt: off
-        setpoint = np.nan  # Setpoint read out of the bath              ['C]
-        P1_temp = np.nan   # Temperature measured by the bath           ['C]
-        P2_temp = np.nan   # Temperature measured by the external probe ['C]
+        setpoint: float = np.nan  # Setpoint read out of the bath          ['C]
+        P1_temp : float = np.nan  # Temperature measured by bath           ['C]
+        P2_temp : float = np.nan  # Temperature measured by external probe ['C]
         # fmt: on
 
-    def __init__(self, name="Bath", long_name="PolyScience PD bath"):
+    def __init__(
+        self,
+        name: str = "Bath",
+        long_name: str = "PolyScience PD bath",
+    ):
         super().__init__(name=name, long_name=long_name)
 
         # Default serial settings
         self.serial_settings = {
             "baudrate": 57600,
             "timeout": 0.5,
             "write_timeout": 0.5,
@@ -56,34 +60,36 @@
         # Container for the process and measurement variables
         self.state = self.State()
 
     # --------------------------------------------------------------------------
     #   ID_validation_query
     # --------------------------------------------------------------------------
 
-    def ID_validation_query(self) -> Tuple[str, str]:
+    def ID_validation_query(self) -> Tuple[str, None]:
         # We'll use the `Disable command echo` of the PolyScience bath and check
         # for the proper reply '!'.
         _success, reply = self.query("SE0")
-        broad_reply = reply.strip()  # Expected: "!"
+        if isinstance(reply, str):
+            broad_reply = reply.strip()  # Expected: "!"
+            return broad_reply, None
 
-        return (broad_reply, None)
+        return "", None
 
     # --------------------------------------------------------------------------
     #   query_P1_temp
     # --------------------------------------------------------------------------
 
     def query_P1_temp(self) -> bool:
         """Query the bath temperature and store it in the class member 'state'.
         Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query("RT")
-        if success:
+        _success, reply = self.query("RT")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
                 print(err)
             else:
                 self.state.P1_temp = num
@@ -98,16 +104,16 @@
 
     def query_P2_temp(self) -> bool:
         """Query the external probe and store it in the class member 'state'.
         Will be set to numpy.nan if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query("RR")
-        if success:
+        _success, reply = self.query("RR")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
                 print(err)
             else:
                 self.state.P2_temp = num
@@ -123,17 +129,16 @@
     def query_setpoint(self) -> bool:
         """Query the temperature setpoint in [deg C] set at the PolyScience bath
         and store it in the class member 'state'. Will be set to numpy.nan if
         unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        success, reply = self.query("RS")
-        # print("query_setpoint returns: %s" % reply)  # DEBUG
-        if success:
+        _success, reply = self.query("RS")
+        if isinstance(reply, str):
             try:
                 num = float(reply)
             except (TypeError, ValueError) as err:
                 pft(err)
                 print(err)
             else:
                 self.state.setpoint = num
@@ -142,53 +147,47 @@
         self.state.setpoint = np.nan
         return False
 
     # --------------------------------------------------------------------------
     #   send_setpoint
     # --------------------------------------------------------------------------
 
-    def send_setpoint(self, setpoint) -> bool:
+    def send_setpoint(self, setpoint: float) -> bool:
         """Send a new temperature setpoint in [deg C] to the PolyScience bath.
 
         Args:
             setpoint (float): temperature in [deg C].
 
         Returns: True if successful, False otherwise.
         """
-        try:
-            setpoint = float(setpoint)
-        except (TypeError, ValueError):
-            # Invalid number
-            print("WARNING: Received illegal setpoint value")
-            print("Setpoint not updated")
-            return False
-
         if setpoint < BATH_MIN_SETPOINT_DEG_C:
             setpoint = BATH_MIN_SETPOINT_DEG_C
             print(
-                "WARNING: setpoint is capped\nto the lower limit of %.2f 'C"
-                % BATH_MIN_SETPOINT_DEG_C
+                "WARNING: setpoint is capped\nto the lower limit of "
+                f"{BATH_MIN_SETPOINT_DEG_C:.2f} 'C"
             )
         elif setpoint > BATH_MAX_SETPOINT_DEG_C:
             setpoint = BATH_MAX_SETPOINT_DEG_C
             print(
-                "WARNING: setpoint is capped\nto the upper limit of %.2f 'C"
-                % BATH_MAX_SETPOINT_DEG_C
+                "WARNING: setpoint is capped\nto the upper limit of "
+                f"{BATH_MAX_SETPOINT_DEG_C:.2f} 'C"
             )
 
-        success, reply = self.query("SS%.2f" % setpoint)
-        # print("send_setpoint returns: %s" % reply)  # DEBUG
-        if success and reply == "!":  # Also check status reply
+        _success, reply = self.query(f"SS{setpoint:.2f}")
+        if reply == "!":
             return True
-        elif success and reply == "?":
+
+        if reply == "?":
             print("WARNING @ send_setpoint")
             print("PolyScience bath might be in stand-by mode.")
             return False
-        else:
-            return False
+
+        print("WARNING @ send_setpoint")
+        print(f"PolyScience bath communication failed with reply: {reply}")
+        return False
 
 
 # ------------------------------------------------------------------------------
 #   Main: Will show a demo when run from the terminal
 # ------------------------------------------------------------------------------
 
 if __name__ == "__main__":
@@ -196,15 +195,15 @@
     import time
 
     # Path to the config textfile containing the (last used) RS232 port
     PATH_CONFIG = "config/port_PolyScience.txt"
 
     bath = PolyScience_PD_bath()
     if bath.auto_connect(filepath_last_known_port=PATH_CONFIG):
-        # TO DO: display internal settings of the PolyScience bath, like
+        # TODO: Display internal settings of the PolyScience bath, like
         # its temperature limits, etc.
         pass
     else:
         time.sleep(1)
         sys.exit(0)
 
     if os.name == "nt":
@@ -219,49 +218,50 @@
         print("No other keyboard input possible because OS is not Windows.")
 
     # Prepare
     send_setpoint = 15.0
     do_send_setpoint = False
 
     bath.query_setpoint()
-    print("\nSet: %6.2f 'C" % bath.state.setpoint)
+    print(f"\nSet: {bath.state.setpoint:6.2f} 'C")
 
     # Loop
     done = False
     while not done:
         # Check if a new setpoint has to be send
         if do_send_setpoint:
             bath.send_setpoint(send_setpoint)
             # The bath needs time to process and update its setpoint, which is
             # found to be up to 1 seconds (!) long. Hence, we sleep.
             time.sleep(1)
             bath.query_setpoint()
-            print("\nSet: %6.2f 'C" % bath.state.setpoint)
+            print(f"\nSet: {bath.state.setpoint:6.2f} 'C")
             do_send_setpoint = False
 
         # Measure and report the temperatures
         bath.query_P1_temp()
         bath.query_P2_temp()
-        print("\rP1 : %6.2f 'C" % bath.state.P1_temp, end="")
-        print("  P2 : %6.2f 'C" % bath.state.P2_temp, end="")
+        print(f"\rP1 : {bath.state.P1_temp:6.2f} 'C", end="")
+        print(f"  P2 : {bath.state.P2_temp:6.2f} 'C", end="")
         sys.stdout.flush()
 
         # Process keyboard input
         if running_Windows:
             if msvcrt.kbhit():
                 key = msvcrt.getch()
                 if key == b"q":
                     print("\nAre you sure you want to quit [y/n]?")
                     if msvcrt.getch() == b"y":
                         print("Quitting.")
                         done = True
                     else:
                         do_send_setpoint = True  # Esthestics
+
                 elif key == b"s":
-                    send_setpoint = input("\nEnter new setpoint ['C]: ")
+                    send_setpoint = float(input("\nEnter new setpoint ['C]: "))
                     do_send_setpoint = True
 
         # Slow down update period
         time.sleep(0.5)
 
     bath.close()
     time.sleep(1)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/ThermoFlex_chiller_protocol_RS232.py` & `dvg-devices-1.4.0/src/dvg_devices/ThermoFlex_chiller_protocol_RS232.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 the previous query resulted in a communication error.
 
 When this module is directly run from the terminal a demo will be shown.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "14-09-2022"
-__version__ = "1.0.0"
-# pylint: disable=bare-except, broad-except, try-except-raise
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, broad-except
 
 import sys
-from typing import Union, Tuple
 import time
+from typing import Union, Tuple
 
 import numpy as np
 
 from dvg_debug_functions import print_fancy_traceback as pft
 from dvg_devices.BaseDevice import SerialDevice
 
 # RS232 header of binary serial communication
-RS232_START = [0xCA, 0x00, 0x01]
+RS232_START = b"\xCA\x00\x01"
 
 
 class Unit_of_measure:
     # fmt: off
     no_unit = 0
     deg_C   = 1     # Temperature in degrees Celsius
     deg_F   = 2     # Temperature in degrees Fahrenheit
     LPM     = 3     # Flow in liters per minute
     GPM     = 4     # Flow in gallons per minute
     sec     = 5     # Time in seconds
     PSI     = 6     # Pressure in pounds per square inch
-    bar     = 7     # Pressure in bars
+    bar     = 7     # Pressure in bars  # pylint: disable=disallowed-name
     MOhm_cm = 8     # Resistivity in mega-Ohms per centimeter
     percent = 9     # Percentage
     Volt    = 10    # Voltage in Volts
     kPa     = 11    # Pressure in kilo-Pascals
     # fmt: on
 
 
@@ -60,83 +60,83 @@
     [numpy.nan] values indicate that the parameter is not initialized or that
     the last query was unsuccessful in communication.
     """
 
     # fmt: off
     class Units:
         # Container for the units used and expected by the chiller
-        temp = np.nan       # Unit of measure index for the temperature
-        flow = np.nan       # Unit of measure index for the flow rate
-        pres = np.nan       # Unit of measure index for the pressure
+        temp: float = np.nan  # Unit of measure index for the temperature
+        flow: float = np.nan  # Unit of measure index for the flow rate
+        pres: float = np.nan  # Unit of measure index for the pressure
 
     class Values_alarm:
         # Container for the alarm values
-        LO_temp = np.nan    # Low temperature limit  ['C]
-        HI_temp = np.nan    # High temperature limit ['C]
-        LO_flow = np.nan    # Low flow rate limit    [LPM]
-        HI_flow = np.nan    # High flow rate limit   [LPM]
-        LO_pres = np.nan    # Low pressure limit     [bar]
-        HI_pres = np.nan    # High pressure limit    [bar]
+        LO_temp: float = np.nan  # Low temperature limit  ['C]
+        HI_temp: float = np.nan  # High temperature limit ['C]
+        LO_flow: float = np.nan  # Low flow rate limit    [LPM]
+        HI_flow: float = np.nan  # High flow rate limit   [LPM]
+        LO_pres: float = np.nan  # Low pressure limit     [bar]
+        HI_pres: float = np.nan  # High pressure limit    [bar]
 
     class Values_PID:
         # Container for the PID values
-        P = np.nan          # Proportional term      [% span of 100 'C]
-        I = np.nan          # Integral term          [repeats/minute]
-        D = np.nan          # Derivative term        [minutes]
+        P: float = np.nan        # Proportional term      [% span of 100 'C]
+        I: float = np.nan        # Integral term          [repeats/minute]
+        D: float = np.nan        # Derivative term        [minutes]
 
     class Status_bits:
         # Container for the status bits of the chiller
-        running               = np.nan
-        RTD1_open             = np.nan
-        RTD2_open             = np.nan
-        RTD3_open             = np.nan
-        high_temp_fixed_fault = np.nan
-        low_temp_fixed_fault  = np.nan
-        high_temp_fault       = np.nan
-        low_temp_fault        = np.nan
-        high_pressure_fault   = np.nan
-        low_pressure_fault    = np.nan
-        phase_monitor_fault   = np.nan
-        high_level_fault      = np.nan
-        drip_pan_fault        = np.nan
-        motor_overload_fault  = np.nan
-        LPC_fault             = np.nan
-        HPC_fault             = np.nan
-        external_EMO_fault    = np.nan
-        local_EMO_fault       = np.nan
-        low_flow_fault        = np.nan
-        low_level_fault       = np.nan
-        sense_5V_fault        = np.nan
-        invalid_level_fault   = np.nan
-        low_fixed_flow_warning      = np.nan
-        high_pressure_fault_factory = np.nan
-        low_pressure_fault_factory  = np.nan
-        powering_up           = np.nan
-        powering_down         = np.nan
-        fault_tripped         = np.nan
+        running                    : Union[int, float] = np.nan
+        RTD1_open                  : Union[int, float] = np.nan
+        RTD2_open                  : Union[int, float] = np.nan
+        RTD3_open                  : Union[int, float] = np.nan
+        high_temp_fixed_fault      : Union[int, float] = np.nan
+        low_temp_fixed_fault       : Union[int, float] = np.nan
+        high_temp_fault            : Union[int, float] = np.nan
+        low_temp_fault             : Union[int, float] = np.nan
+        high_pressure_fault        : Union[int, float] = np.nan
+        low_pressure_fault         : Union[int, float] = np.nan
+        phase_monitor_fault        : Union[int, float] = np.nan
+        high_level_fault           : Union[int, float] = np.nan
+        drip_pan_fault             : Union[int, float] = np.nan
+        motor_overload_fault       : Union[int, float] = np.nan
+        LPC_fault                  : Union[int, float] = np.nan
+        HPC_fault                  : Union[int, float] = np.nan
+        external_EMO_fault         : Union[int, float] = np.nan
+        local_EMO_fault            : Union[int, float] = np.nan
+        low_flow_fault             : Union[int, float] = np.nan
+        low_level_fault            : Union[int, float] = np.nan
+        sense_5V_fault             : Union[int, float] = np.nan
+        invalid_level_fault        : Union[int, float] = np.nan
+        low_fixed_flow_warning     : Union[int, float] = np.nan
+        high_pressure_fault_factory: Union[int, float] = np.nan
+        low_pressure_fault_factory : Union[int, float] = np.nan
+        powering_up                : Union[int, float] = np.nan
+        powering_down              : Union[int, float] = np.nan
+        fault_tripped              : Union[int, float] = np.nan
 
     class State:
         # Container for the process and measurement variables
-        setpoint     = np.nan   # Setpoint read out of the chiller         ['C]
-        temp         = np.nan   # Temperature measured by the chiller      ['C]
-        flow         = np.nan   # Flow rate measured by the chiller        [LPM]
-        supply_pres  = np.nan   # Supply pressure measured by the chiller  [bar]
-        suction_pres = np.nan   # Suction pressure measured by the chiller [bar]
+        setpoint    : float = np.nan  # Setpoint read out of the chiller         ['C]
+        temp        : float = np.nan  # Temperature measured by the chiller      ['C]
+        flow        : float = np.nan  # Flow rate measured by the chiller        [LPM]
+        supply_pres : float = np.nan  # Supply pressure measured by the chiller  [bar]
+        suction_pres: float = np.nan  # Suction pressure measured by the chiller [bar]
     # fmt: on
 
     # --------------------------------------------------------------------------
     #   __init__
     # --------------------------------------------------------------------------
 
     def __init__(
         self,
-        name="chiller",
-        long_name="ThermoFlex chiller",
-        min_setpoint_degC=10,
-        max_setpoint_degC=40,
+        name: str = "chiller",
+        long_name: str = "ThermoFlex chiller",
+        min_setpoint_degC: float = 10,
+        max_setpoint_degC: float = 40,
     ):
         super().__init__(name=name, long_name=long_name)
 
         # Default serial settings
         self.serial_settings = {
             "baudrate": 9600,
             "timeout": 1,
@@ -157,69 +157,91 @@
 
         # Software limits on the temperature setpoint
         self.min_setpoint_degC = min_setpoint_degC
         self.max_setpoint_degC = max_setpoint_degC
 
         # Container for the units used and expected by the chiller.
         # Gets updated by calling the alarm value queries (e.g.
-        # 'query_alarm_LO_flow()' etc.) or by calling 'begin()'.
+        # `query_alarm_LO_flow()` etc.) or by calling `begin()`.
         self.units = self.Units()
 
         # Container for the alarm values.
         # Gets updated by calling the alarm value queries (e.g.
-        # 'query_alarm_LO_flow()' etc.) or by calling 'begin()'.
+        # `query_alarm_LO_flow()` etc.) or by calling `begin()`.
         self.values_alarm = self.Values_alarm()
 
         # Container for the PID values
-        # Gets updated by calling the PID queries (e.g. 'query_PID_P()' etc.)
-        # or by calling 'begin()'.
+        # Gets updated by calling the PID queries (e.g. `query_PID_P()` etc.)
+        # or by calling `begin()`.
         self.values_PID = self.Values_PID()
 
         # Container for the status bits (faults and warnings of the chiller).
-        # Gets updated by calling 'query_status_bits()' or by calling 'begin()'.
+        # Gets updated by calling `query_status_bits()` or by calling `begin()`.
         self.status_bits = self.Status_bits()
 
         # Container for the process and measurement variables
         self.state = self.State()
 
     # --------------------------------------------------------------------------
     #   OVERRIDE: query
     # --------------------------------------------------------------------------
 
     def query(
         self,
         msg: Union[str, bytes],
         raises_on_timeout: bool = False,
-        returns_ascii: bool = True,
-    ) -> Tuple[bool, Union[str, bytes, None]]:
-        success, reply = super().query(
-            msg, raises_on_timeout, returns_ascii=False  # Binary I/O, not ASCII
+        returns_ascii: bool = False,
+    ) -> Tuple[bool, Union[bytes, None]]:
+        """Send a message to the ThermoFlex chiller and subsequently read the
+        reply.
+
+        Args:
+            msg (`str` | `bytes`):
+                ASCII string or bytes to be sent to the serial device.
+
+            raises_on_timeout (`bool`, optional):
+                Should an exception be raised when a write or read timeout
+                occurs?
+
+                Default: `False`
+
+            returns_ascii (`bool`, ignored):
+                Argument is ignored and is locked to True.
+
+        Returns:
+            success (`bool`):
+                True if successful, False otherwise.
+
+            reply (`bytes` | `None`):
+                Reply received from the device as bytes. `None` if unsuccessful.
+        """
+        _success, reply = super().query(
+            msg,
+            raises_on_timeout,
+            returns_ascii=False,  # Binary I/O, not ASCII
         )
 
         # The ThermoFlex is more complex in its replies than the average device.
         # Hence:
-        if success:
+        if isinstance(reply, bytes):
             if (len(reply) >= 4) and reply[3] == 0x0F:
                 # Error reported by chiller
                 if reply[5] == 1:
                     pft("Bad command received by chiller", 3)
                 elif reply[5] == 2:
                     pft("Bad data received by chiller", 3)
                 elif reply[5] == 3:
                     pft("Bad checksum received by chiller", 3)
-                success = False
-            else:
-                # We got a reply back from /a/ device, not necessarily a
-                # ThermoFlex chiller.
-                success = True
+                return False, None
 
-        if reply is None:
-            reply = np.nan
+            # We got a reply back from /a/ device, not necessarily a
+            # ThermoFlex chiller.
+            return True, reply
 
-        return success, reply
+        return False, None
 
     # --------------------------------------------------------------------------
     #   ID_validation_query
     # --------------------------------------------------------------------------
 
     def ID_validation_query(self) -> Tuple[bool, None]:
         return self.query_Ack(), None
@@ -256,74 +278,67 @@
         # Query setpoint
         self.query_setpoint()
 
     # --------------------------------------------------------------------------
     #   Query functions
     # --------------------------------------------------------------------------
 
-    def query_data_as_float_and_uom(self, msg_bytes):
-        """Query the serial device and parse its reply as data bytes decoding a
-        float value and an unit of measure index.
+    def query_data_as_float_and_uom(
+        self, msg_bytes: bytes
+    ) -> Tuple[bool, float, Union[int, float]]:
+        """Query the ThermoFlex chiller and parse its reply as data bytes
+        decoding a float value and an unit of measure index.
 
         Args:
-            msg_bytes (bytes): Message to be sent to the serial device.
+            msg_bytes (bytes): Message to be sent to the chiller.
 
         Returns:
-            success (bool): True if successful, False otherwise.
-            value  (float): The decoded float value. [numpy.nan] if unsuccessful.
-            uom      (int): Unit of measure index. [numpy.nan] if unsuccessful.
+            success (`bool`):
+                True if successful, False otherwise.
+
+            value (`float`):
+                The decoded float value. `numpy.nan` if unsuccessful.
+
+            uom (`int` | `float`):
+                Unit of measure index. `numpy.nan` if unsuccessful.
         """
-        value = np.nan
-        # print_as_hex(msg_bytes)                     # debug info
-        success, ans_bytes = self.query(msg_bytes)
-        # print_as_hex(ans_bytes)                     # debug info
-        if success:
-            value, uom = self.parse_data_bytes(ans_bytes)
-        if not np.isnan(value):
-            return True, value, uom
-
-        return False, np.nan, np.nan
-
-    # --------------------------------------------------------------------------
-    #   add_checksum
-    # --------------------------------------------------------------------------
-
-    def add_checksum(self, byte_list):
-        """The checksum runs over all bytes, except for the leading byte. It is
-        a bitwise inversion of the 1 byte sum of bytes. We mimic the overflow of
-        the 1 byte sum in Python by using the modulo operator '% 0x100'. The
-        inversion is done by using the XOR operator '^ 0xFF'
-        =
-        Usage example:
-          # request setpoint
-          msg_bytes = RS232_START + [0x70, 0x00]
-          add_checksum(msg_bytes)
-          # turn list into bytes ready to be sent
-          msg_bytes = bytes(msg_bytes)
-        """
-        chksum = (sum(byte_list[1:]) % 0x100) ^ 0xFF
-        byte_list.append(chksum)
-        # print_as_hex(byte_list)                     # debug info
+        # print(pretty_bytes_to_hex(msg_bytes))   # Debug info
+        _success, reply = self.query(msg_bytes)
+        # print(pretty_bytes_to_hex(reply))       # Debug info
+
+        if isinstance(reply, bytes):
+            value, uom = self.parse_data_bytes(reply)
+
+            if (not np.isnan(value)) and (not np.isnan(uom)):
+                return True, value, uom  # Success
+
+        return False, np.nan, np.nan  # Failed
 
     # --------------------------------------------------------------------------
     #   Parsing
     # --------------------------------------------------------------------------
 
-    def parse_data_bytes(self, ans_bytes):
-        """Parse the data bytes.
+    def parse_data_bytes(
+        self, ans_bytes: bytes
+    ) -> Tuple[float, Union[int, float]]:
+        """Parse the data bytes. The manual states:
+
+        data_bytes[0]:
+            The qualifier byte, where b.0 to b.3 indicates unit of measure index
+            and b.4 to b.7 indicates precision of measurement.
 
-        The manual states:
-            data_bytes[0] : the qualifier byte
-              b.0 to b.3 indicates unit of measure index
-              b.4 to b.7 indicates precision of measurement
-            data_bytes[1:]: value
+        data_bytes[1:]:
+            Value.
 
         Returns:
-            value (float): The decoded float value. [numpy.nan] if unsuccessful.
-            uom     (int): Unit of measure index. [numpy.nan] if unsuccessful.
+            value (`float`):
+                The decoded float value. [numpy.nan] if unsuccessful.
+
+            uom (`int` | `float`):
+                Unit of measure index. [numpy.nan] if unsuccessful.
         """
         value = np.nan
         uom = np.nan
         try:
             nn = ans_bytes[4]  # Number of data bytes to follow
             data_bytes = ans_bytes[5 : 5 + nn]
             pom = data_bytes[0] >> 4  # Precision of measurement
@@ -341,70 +356,70 @@
             elif pom == 2:
                 value = int_value * 0.01
             elif pom == 3:
                 value = int_value * 0.001
             elif pom == 4:
                 value = int_value * 0.0001
 
-        return (value, uom)
+        return value, uom
 
-    def parse_status_bits(self, ans_bytes):
+    def parse_status_bits(self, ans_bytes: bytes):
         """Parse the status bits, which are indicators for any faults and/or
         warnings of the chiller. This status gets stored in the class member
-        'status_bits'.
+        `status_bits`.
         """
         nn = ans_bytes[4]  # Number of data bytes to follow
         status_bits = ans_bytes[5 : 5 + nn]
         d1 = np.uint8(status_bits[0])
         d2 = np.uint8(status_bits[1])
         d3 = np.uint8(status_bits[2])
         d4 = np.uint8(status_bits[3])
 
-        [
+        (
             self.status_bits.low_temp_fault,
             self.status_bits.high_temp_fault,
             self.status_bits.low_temp_fixed_fault,
             self.status_bits.high_temp_fixed_fault,
             self.status_bits.RTD3_open,
             self.status_bits.RTD2_open,
             self.status_bits.RTD1_open,
             self.status_bits.running,
-        ] = np.unpackbits(d1)
-        [
+        ) = np.unpackbits(d1)
+        (
             self.status_bits.HPC_fault,
             self.status_bits.LPC_fault,
             self.status_bits.motor_overload_fault,
             self.status_bits.phase_monitor_fault,
             self.status_bits.high_level_fault,
             self.status_bits.drip_pan_fault,
             self.status_bits.low_pressure_fault,
             self.status_bits.high_pressure_fault,
-        ] = np.unpackbits(d2)
-        [
+        ) = np.unpackbits(d2)
+        (
             self.status_bits.high_pressure_fault_factory,
             self.status_bits.low_fixed_flow_warning,
             self.status_bits.invalid_level_fault,
             self.status_bits.sense_5V_fault,
             self.status_bits.low_level_fault,
             self.status_bits.low_flow_fault,
             self.status_bits.local_EMO_fault,
             self.status_bits.external_EMO_fault,
-        ] = np.unpackbits(d3)
-        [
-            dummy,
-            dummy,
-            dummy,
-            dummy,
-            dummy,
+        ) = np.unpackbits(d3)
+        (
+            _dummy,
+            _dummy,
+            _dummy,
+            _dummy,
+            _dummy,
             self.status_bits.powering_down,
             self.status_bits.powering_up,
             self.status_bits.low_pressure_fault_factory,
-        ] = np.unpackbits(d4)
+        ) = np.unpackbits(d4)
 
-        self.status_bits.fault_tripped = (
+        self.status_bits.fault_tripped = int(
             sum(
                 [
                     self.status_bits.high_temp_fixed_fault,
                     self.status_bits.low_temp_fixed_fault,
                     self.status_bits.high_temp_fault,
                     self.status_bits.low_temp_fault,
                     d2,
@@ -416,413 +431,420 @@
         )
 
         # print(np.unpackbits(d1))
         # print(np.unpackbits(d2))
         # print(np.unpackbits(d3))
         # print(np.unpackbits(d4))
 
-    def parse_ASCII_bytes(self, ans_bytes):
+    def parse_ASCII_bytes(self, ans_bytes: bytes) -> Union[str, None]:
         """Parse the ASCII-encoded text bytes.
 
-        Returns: The decoded text as (str), or None if unsuccessful.
+        Returns: The decoded text as `str`, or None if unsuccessful.
         """
         nn = ans_bytes[4]  # Number of data bytes to follow
         ASCII_bytes = ans_bytes[5 : 5 + nn]
         try:
             ans_str = ASCII_bytes.decode("ascii")
         except UnicodeDecodeError:
             return None
-        except:
+        except Exception:
             return None
-        else:
-            return ans_str
+
+        return ans_str
 
     # --------------------------------------------------------------------------
     #   ON/OFF
     # --------------------------------------------------------------------------
 
-    def turn_off(self):
+    def turn_off(self) -> Union[bool, float]:
         """Turn the chiller off.
 
         Returns: The effected on/off state of the chiller, or [numpy.nan] if
         unsuccessful.
         """
-        msg_bytes = bytes(
-            RS232_START + [0x81, 0x01, 0x00, 0x7C]
-        )  # includes checksum
-        success, ans_bytes = self.query(msg_bytes)
-        if success:
-            return bool(ans_bytes[5])  # return resulting on/off state
+        msg_bytes = RS232_START + b"\x81\x01\x00\x7C"  # With checksum
+        _success, reply = self.query(msg_bytes)
+        if isinstance(reply, bytes):
+            return bool(reply[5])  # return resulting on/off state
 
         return np.nan
 
-    def turn_on(self):
+    def turn_on(self) -> Union[bool, float]:
         """Turn the chiller on.
 
         Returns: The effected on/off state of the chiller, or [numpy.nan] if
         unsuccessful.
         """
-        msg_bytes = bytes(
-            RS232_START + [0x81, 0x01, 0x01, 0x7B]
-        )  # includes checksum
-        success, ans_bytes = self.query(msg_bytes)
-        if success:
-            return bool(ans_bytes[5])  # return resulting on/off state
+        msg_bytes = RS232_START + b"\x81\x01\x01\x7B"  # With checksum
+        _success, reply = self.query(msg_bytes)
+        if isinstance(reply, bytes):
+            return bool(reply[5])  # return resulting on/off state
 
         return np.nan
 
-    def query_is_on(self):
+    def query_is_on(self) -> Union[bool, float]:
         """Query the on/off state of the chiller.
-        This is identical to the status bit 'status.chiller_running'.
+        This is identical to the status bit `status.chiller_running`.
 
         Returns: The on/off state of the chiller, or [numpy.nan] if
         unsuccessful.
         """
-        msg_bytes = bytes(
-            RS232_START + [0x81, 0x01, 0x02, 0x7A]
-        )  # includes checksum
-        success, ans_bytes = self.query(msg_bytes)
-        if success:
-            return bool(ans_bytes[5])  # return resulting on/off state
+        msg_bytes = RS232_START + b"\x81\x01\x02\x7A"  # With checksum
+        _success, reply = self.query(msg_bytes)
+        if isinstance(reply, bytes):
+            return bool(reply[5])  # return resulting on/off state
 
         return np.nan
 
     # --------------------------------------------------------------------------
     #   query_Ack
     # --------------------------------------------------------------------------
 
-    def query_Ack(self):
+    def query_Ack(self) -> bool:
         """Query the 'Acknowledge' request (REQ ACK). Basically asking 'Are you
         a ThermoFlex chiller?' to the serial device.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x00, 0x00, 0xFE])  # includes checksum
-        success, ans_bytes = self.query(msg_bytes)
-        if success and (
-            (ans_bytes == bytes(RS232_START + [0x00, 0x02, 0x00, 0x00, 0xFC]))
-            | (ans_bytes == bytes(RS232_START + [0x00, 0x02, 0x00, 0x01, 0xFB]))
+        msg_bytes = RS232_START + b"\x00\x00\xFE"  # With checksum
+        _success, reply = self.query(msg_bytes)
+        if (reply == bytes(RS232_START + b"\x00\x02\x00\x00\xFC")) | (
+            reply == bytes(RS232_START + b"\x00\x02\x00\x01\xFB")
         ):
             return True
 
         return False
 
     # --------------------------------------------------------------------------
     #   Request HI/LO alarm values
     # --------------------------------------------------------------------------
 
-    def query_alarm_values_and_units(self):
-        """Query all alarm values and store in the class member 'values_alarm'.
-        Also stores the units of measure in class member 'units'.
+    def query_alarm_values_and_units(self) -> bool:
+        """Query all alarm values and store in the class member `values_alarm`.
+        Also stores the units of measure in class member `units`.
         Each will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
         return (
             self.query_alarm_LO_flow()
             & self.query_alarm_LO_temp()
             & self.query_alarm_LO_pres()
             & self.query_alarm_HI_flow()
             & self.query_alarm_HI_temp()
             & self.query_alarm_HI_pres()
         )
 
-    def query_alarm_LO_flow(self):
-        """Query the alarm value and store in the class member 'values_alarm'.
-        Also stores the unit of measure in class member 'units'.
+    def query_alarm_LO_flow(self) -> bool:
+        """Query the alarm value and store in the class member `values_alarm`.
+        Also stores the unit of measure in class member `units`.
         Both will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x30, 0x00, 0xCE])  # includes checksum
+        msg_bytes = RS232_START + b"\x30\x00\xCE"  # With checksum
         success, value, units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_alarm.LO_flow = value
         self.units.flow = units
         return success
 
-    def query_alarm_LO_temp(self):
-        """Query the alarm value and store in the class member 'values_alarm'.
-        Also stores the unit of measure in class member 'units'.
+    def query_alarm_LO_temp(self) -> bool:
+        """Query the alarm value and store in the class member `values_alarm`.
+        Also stores the unit of measure in class member `units`.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x40, 0x00, 0xBE])  # includes checksum
+        msg_bytes = RS232_START + b"\x40\x00\xBE"  # With checksum
         success, value, units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_alarm.LO_temp = value
         self.units.temp = units
         return success
 
-    def query_alarm_LO_pres(self):
-        """Query the alarm value and store in the class member 'values_alarm'.
-        Also stores the unit of measure in class member 'units'.
+    def query_alarm_LO_pres(self) -> bool:
+        """Query the alarm value and store in the class member `values_alarm`.
+        Also stores the unit of measure in class member `units`.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x48, 0x00, 0xB6])  # includes checksum
+        msg_bytes = RS232_START + b"\x48\x00\xB6"  # With checksum
         success, value, units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_alarm.LO_pres = value
         self.units.pres = units
         return success
 
-    def query_alarm_HI_flow(self):
-        """Query the alarm value and store in the class member 'values_alarm'.
-        Also stores the unit of measure in class member 'units'.
+    def query_alarm_HI_flow(self) -> bool:
+        """Query the alarm value and store in the class member `values_alarm`.
+        Also stores the unit of measure in class member `units`.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x50, 0x00, 0xAE])  # includes checksum
+        msg_bytes = RS232_START + b"\x50\x00\xAE"  # With checksum
         success, value, units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_alarm.HI_flow = value
         self.units.flow = units
         return success
 
-    def query_alarm_HI_temp(self):
-        """Query the alarm value and store in the class member 'values_alarm'.
-        Also stores the unit of measure in class member 'units'.
+    def query_alarm_HI_temp(self) -> bool:
+        """Query the alarm value and store in the class member `values_alarm`.
+        Also stores the unit of measure in class member `units`.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x60, 0x00, 0x9E])  # includes checksum
+        msg_bytes = RS232_START + b"\x60\x00\x9E"  # With checksum
         success, value, units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_alarm.HI_temp = value
         self.units.temp = units
         return success
 
-    def query_alarm_HI_pres(self):
-        """Query the alarm value and store in the class member 'values_alarm'.
-        Also stores the unit of measure in class member 'units'.
+    def query_alarm_HI_pres(self) -> bool:
+        """Query the alarm value and store in the class member `values_alarm`.
+        Also stores the unit of measure in class member `units`.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x68, 0x00, 0x96])  # includes checksum
+        msg_bytes = RS232_START + b"\x68\x00\x96"  # With checksum
         success, value, units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_alarm.HI_pres = value
         self.units.pres = units
         return success
 
     # --------------------------------------------------------------------------
     #   Query PID values
     # --------------------------------------------------------------------------
 
-    def query_PID_values(self):
-        """Query all PID values and store in the class member 'values_PID'.
+    def query_PID_values(self) -> bool:
+        """Query all PID values and store in the class member `values_PID`.
         Each will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
         return self.query_PID_P() & self.query_PID_I() & self.query_PID_D()
 
-    def query_PID_P(self):
-        """Query the PID value and store in the class member 'values_PID'.
+    def query_PID_P(self) -> bool:
+        """Query the PID value and store in the class member `values_PID`.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x74, 0x00, 0x8A])  # includes checksum
+        msg_bytes = RS232_START + b"\x74\x00\x8A"  # With checksum
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_PID.P = value
         return success
 
-    def query_PID_I(self):
-        """Query the PID value and store in the class member 'values_PID'.
+    def query_PID_I(self) -> bool:
+        """Query the PID value and store in the class member `values_PID`.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x75, 0x00, 0x89])  # includes checksum
+        msg_bytes = RS232_START + b"\x75\x00\x89"  # With checksum
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_PID.I = value
         return success
 
-    def query_PID_D(self):
-        """Query the PID value and store in the class member 'values_PID'.
+    def query_PID_D(self) -> bool:
+        """Query the PID value and store in the class member `values_PID`.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x76, 0x00, 0x88])  # includes checksum
+        msg_bytes = RS232_START + b"\x76\x00\x88"  # With checksum
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.values_PID.D = value
         return success
 
     # --------------------------------------------------------------------------
     #   query_status_bits
     # --------------------------------------------------------------------------
 
-    def query_status_bits(self):
+    def query_status_bits(self) -> bool:
         """Query and parse the status bits, which are indicators for any faults
         and/or warnings of the chiller. This status gets stored in the class
-        member 'status_bits.
+        member `status_bits`.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x09, 0x00, 0xF5])  # included checksum
-        success, ans_bytes = self.query(msg_bytes)
-        if success:
-            self.parse_status_bits(ans_bytes)
+        msg_bytes = RS232_START + b"\x09\x00\xF5"  # With checksum
+        success, reply = self.query(msg_bytes)
+        if isinstance(reply, bytes):
+            self.parse_status_bits(reply)
         return success
 
     # --------------------------------------------------------------------------
     #   Query state variables
     # --------------------------------------------------------------------------
 
-    def query_state(self):
+    def query_state(self) -> bool:
         """Query all process and measurement variables and store in the class
-        member 'state'.
+        member `state`.
         Each will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
         return (
             self.query_setpoint()
             & self.query_temp()
             & self.query_flow()
             & self.query_supply_pres()
             & self.query_suction_pres()
         )
 
-    def query_setpoint(self):
-        """Query and store in the class member 'state':
+    def query_setpoint(self) -> bool:
+        """Query and store in the class member `state`:
         The temperature setpoint value read from the chiller.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x70, 0x00, 0x8E])  # includes checksum
+        msg_bytes = RS232_START + b"\x70\x00\x8E"  # With checksum
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.state.setpoint = value
         return success
 
-    def query_temp(self):
-        """Query and store in the class member 'state':
+    def query_temp(self) -> bool:
+        """Query and store in the class member `state`:
         The temperature measured by the chiller.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x20, 0x00, 0xDE])  # includes checksum
+        msg_bytes = RS232_START + b"\x20\x00\xDE"  # With checksum
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.state.temp = value
         return success
 
-    def query_flow(self):
-        """Query and store in the class member 'state':
+    def query_flow(self) -> bool:
+        """Query and store in the class member `state`:
         The flow rate measured by the chiller.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x10, 0x00, 0xEE])  # includes checksum
+        msg_bytes = RS232_START + b"\x10\x00\xEE"  # With checksum
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.state.flow = value
         return success
 
-    def query_supply_pres(self):
-        """Query and store in the class member 'state':
+    def query_supply_pres(self) -> bool:
+        """Query and store in the class member `state`:
         The supply pressure measured by the chiller.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x28, 0x00, 0xD6])  # includes checksum
+        msg_bytes = RS232_START + b"\x28\x00\xD6"  # With checksum
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.state.supply_pres = value
         return success
 
-    def query_suction_pres(self):
-        """Query and store in the class member 'state':
+    def query_suction_pres(self) -> bool:
+        """Query and store in the class member `state`:
         The suction pressure measured by the chiller.
         Will be set to [numpy.nan] if unsuccessful.
 
         Returns: True if successful, False otherwise.
         """
-        msg_bytes = bytes(RS232_START + [0x29, 0x00, 0xD5])  # includes checksum
+        msg_bytes = RS232_START + b"\x29\x00\xD5"  # With checksum
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.state.suction_pres = value
         return success
 
     # --------------------------------------------------------------------------
     #   query_display_msg
     # --------------------------------------------------------------------------
 
-    def query_display_msg(self):
+    def query_display_msg(self) -> Union[str, None]:
         """Query the display text shown on the chiller.
 
-        Returns: The display text as (str), or None if unsuccessful.
+        Returns: The display text as `str`, or None if unsuccessful.
         """
-        msg_bytes = bytes(RS232_START + [0x07, 0x00, 0xF7])  # includes checksum
-        success, ans_bytes = self.query(msg_bytes)
-        if success:
-            return self.parse_ASCII_bytes(ans_bytes)
+        msg_bytes = RS232_START + b"\x07\x00\xF7"  # With checksum
+        _success, reply = self.query(msg_bytes)
+        if isinstance(reply, bytes):
+            return self.parse_ASCII_bytes(reply)
 
         return None
 
     # --------------------------------------------------------------------------
     #   send_setpoint
     # --------------------------------------------------------------------------
 
-    def send_setpoint(self, temp_deg_C):
+    def send_setpoint(self, temp_deg_C: float) -> bool:
         """Send a new temperature setpoint in [deg C.] to the chiller.
         Subsequently, the chiller replies with the currently set setpoint and
-        this value will be stored in the class member 'state'.
+        this value will be stored in the class member `state`.
 
         Args:
-            temp_deg_C (float): temperature in [deg C].
+            temp_deg_C (`float`):
+                Temperature in [deg C].
 
         Returns: True if successful, False otherwise.
         """
-        try:
-            temp_deg_C = float(temp_deg_C)
-        except (TypeError, ValueError):
-            # Invalid number
-            print("WARNING: Received illegal setpoint value")
-            print("Setpoint not updated")
-            return False
-
         if temp_deg_C < self.min_setpoint_degC:
             temp_deg_C = self.min_setpoint_degC
             print(
-                "WARNING: setpoint is capped\nto the lower limit of %.1f 'C"
-                % self.min_setpoint_degC
+                "WARNING: setpoint is capped\nto the lower limit of "
+                f"{self.min_setpoint_degC:.1f} 'C"
             )
         elif temp_deg_C > self.max_setpoint_degC:
             temp_deg_C = self.max_setpoint_degC
             print(
-                "WARNING: setpoint is capped\nto the upper limit of %.1f 'C"
-                % self.max_setpoint_degC
+                "WARNING: setpoint is capped\nto the upper limit of "
+                f"{self.max_setpoint_degC:.1f} 'C"
             )
 
         # Transform temperature to bytes
-        pom = 0.1  # precision of measurement, fixed to 0.1
-        temp_bytes = int(np.round(temp_deg_C / pom)).to_bytes(
-            2, byteorder="big"
-        )
-        msg = RS232_START + [0xF0, 0x02] + [temp_bytes[0], temp_bytes[1]]
-        self.add_checksum(msg)
-        msg_bytes = bytes(msg)
+        pom = 0.1  # Precision of measurement, fixed to 0.1
+        temp = int(np.round(temp_deg_C / pom)).to_bytes(2, byteorder="big")
+        msg_bytes = add_checksum(RS232_START + b"\xF0\x02" + temp)
 
         # Send setpoint to chiller and receive the set setpoint
         success, value, _units = self.query_data_as_float_and_uom(msg_bytes)
         self.state.setpoint = value
         return success
 
 
 # ------------------------------------------------------------------------------
+#   add_checksum
+# ------------------------------------------------------------------------------
+
+
+def add_checksum(bytes_in: bytes) -> bytes:
+    """Calculate a checksum over the passed `bytes_in` and return the bytes
+    extended with the checksum.
+
+    Usage example::
+
+        # Request setpoint
+        msg_bytes = RS232_START + b"\x70\x00"
+        msg_bytes = add_checksum(msg_bytes)
+    """
+    # The checksum runs over all bytes, except for the leading byte. It is a
+    # bitwise inversion of the 1 byte sum of bytes. We mimic the overflow of the
+    # 1 byte sum in Python by using the modulo operator `% 0x100`. The inversion
+    # is done by using the XOR operator `^ 0xFF`.
+
+    chksum = (sum(bytes_in[1:]) % 0x100) ^ 0xFF  # Is of tyype `int`
+    bytes_out = bytes_in + chksum.to_bytes(length=1, byteorder="big")
+    # print(pretty_bytes_to_hex(bytes_out))  # Debug info
+    return bytes_out
+
+
+# ------------------------------------------------------------------------------
 #   Debug functions
 # ------------------------------------------------------------------------------
 
 
-def print_as_hex(byte_list):
-    list(map(lambda x: print(format(x, "02x"), end=" "), byte_list))
-    print()
+def pretty_bytes_to_hex(values: bytes) -> str:
+    return " ".join(f"{b:02x}" for b in values)
 
 
 # -----------------------------------------------------------------------------
 #   Main: Will show a demo when run from the terminal
 # -----------------------------------------------------------------------------
 
 if __name__ == "__main__":
@@ -872,56 +894,64 @@
             print("Press Control + C to quit.")
             print("No other keyboard input possible because OS is not Windows.")
 
         print("\n------------------------")
         print("      ALARM VALUES")
         print("        LO  |  HI")
         print(
-            " flow: %4.1f | %4.1f  LPM"
-            % (chiller.values_alarm.LO_flow, chiller.values_alarm.HI_flow)
+            f" flow: {chiller.values_alarm.LO_flow:4.1f} | "
+            f"{chiller.values_alarm.HI_flow:4.1f}  LPM"
         )
         print(
-            " pres: %4.2f | %4.2f  bar"
-            % (chiller.values_alarm.LO_pres, chiller.values_alarm.HI_pres)
+            f" pres: {chiller.values_alarm.LO_pres:4.2f} | "
+            f"{chiller.values_alarm.HI_pres:4.2f}  bar"
         )
         print(
-            " temp: %4.1f | %4.1f  'C"
-            % (chiller.values_alarm.LO_temp, chiller.values_alarm.HI_temp)
+            f" temp: {chiller.values_alarm.LO_temp:4.1f} | "
+            f"{chiller.values_alarm.HI_temp:4.1f}  'C"
         )
         print("------------------------")
-        print(" P: %4.1f  %% span 100'C" % chiller.values_PID.P)
-        print(" I: %4.2f  repeats/minute" % chiller.values_PID.I)
-        print(" D: %4.1f  minutes" % chiller.values_PID.D)
+        print(f" P: {chiller.values_PID.P:4.1f}  %% span 100'C")
+        print(f" I: {chiller.values_PID.I:4.2f}  repeats/minute")
+        print(f" D: {chiller.values_PID.D:4.1f}  minutes")
         print("------------------------")
-        print(" running         : %i" % chiller.status_bits.running)
-        print(" powering up/down: %i" % chiller.status_bits.powering_down)
-        print(" fault_tripped   : %i" % chiller.status_bits.fault_tripped)
-        print(" MSG: %s" % chiller.query_display_msg())
+        print(f" running         : {chiller.status_bits.running}")
+        print(f" powering up/down: {chiller.status_bits.powering_down}")
+        print(f" fault_tripped   : {chiller.status_bits.fault_tripped}")
+        print(f" MSG: {chiller.query_display_msg()}")
         print("------------------------")
-        print(" setpoint: %6.1f 'C" % chiller.state.setpoint)
+        print(f" setpoint: {chiller.state.setpoint:6.1f} 'C")
         print("------------------------")
-        print(" temp    : %6.1f 'C" % chiller.state.temp)
-        print(" flow    : %6.1f LPM" % chiller.state.flow)
-        print(" supply  : %6.2f bar" % chiller.state.supply_pres)
-        print(" suction : %6.2f bar" % chiller.state.suction_pres)
+        print(f" temp    : {chiller.state.temp:6.1f} 'C")
+        print(f" flow    : {chiller.state.flow:6.1f} LPM")
+        print(f" supply  : {chiller.state.supply_pres:6.2f} bar")
+        print(f" suction : {chiller.state.suction_pres:6.2f} bar")
         print("------------------------")
         sys.stdout.flush()
 
         # Process keyboard input
         if running_Windows:
             if msvcrt.kbhit():
                 key = msvcrt.getch()
                 if key == b"q":
                     print("\nAre you sure you want to quit [y/n]?")
                     if msvcrt.getch() == b"y":
                         print("Switching off chiller and quitting.")
                         done = True
                 elif key == b"s":
-                    send_setpoint = input("\nEnter new setpoint [deg C]: ")
-                    do_send_setpoint = True
+                    input_str = input("\nEnter new setpoint [deg C]: ")
+                    try:
+                        input_float = float(input_str)
+                    except ValueError:
+                        print(
+                            "Illegal value entered. Setpoint remains unchanged."
+                        )
+                    else:
+                        send_setpoint = input_float
+                        do_send_setpoint = True
                 elif key == b"o":
                     if chiller.status_bits.running:
                         chiller.turn_off()
                     else:
                         chiller.turn_on()
 
         # Slow down update period
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/ThermoFlex_chiller_qdev.py` & `dvg-devices-1.4.0/src/dvg_devices/ThermoFlex_chiller_qdev.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,85 +2,23 @@
 # -*- coding: utf-8 -*-
 """PyQt/PySide module to provide multithreaded communication and periodical data
 acquisition for a Thermo Scientific ThermoFlex recirculating chiller.
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-dvg-devices"
-__date__ = "28-10-2022"
-__version__ = "1.0.0"
-# pylint: disable=broad-except, try-except-raise
-
-import os
-import sys
-
-# Mechanism to support both PyQt and PySide
-# -----------------------------------------
-
-PYQT5 = "PyQt5"
-PYQT6 = "PyQt6"
-PYSIDE2 = "PySide2"
-PYSIDE6 = "PySide6"
-QT_LIB_ORDER = [PYQT5, PYSIDE2, PYSIDE6, PYQT6]
-QT_LIB = None
-
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        if lib in sys.modules:
-            QT_LIB = lib
-            break
+__date__ = "23-05-2024"
+__version__ = "1.4.0"
+# pylint: disable=missing-function-docstring, broad-except
 
-if QT_LIB is None:
-    for lib in QT_LIB_ORDER:
-        try:
-            __import__(lib)
-            QT_LIB = lib
-            break
-        except ImportError:
-            pass
-
-if QT_LIB is None:
-    this_file = __file__.split(os.sep)[-1]
-    raise Exception(
-        f"{this_file} requires PyQt5, PyQt6, PySide2 or PySide6; "
-        "none of these packages could be imported."
-    )
-
-# fmt: off
-# pylint: disable=import-error, no-name-in-module
-if QT_LIB == PYQT5:
-    from PyQt5 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt5.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt5.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYQT6:
-    from PyQt6 import QtCore, QtGui, QtWidgets as QtWid    # type: ignore
-    from PyQt6.QtCore import pyqtSlot as Slot              # type: ignore
-    from PyQt6.QtCore import pyqtSignal as Signal          # type: ignore
-elif QT_LIB == PYSIDE2:
-    from PySide2 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide2.QtCore import Slot                        # type: ignore
-    from PySide2.QtCore import Signal                      # type: ignore
-elif QT_LIB == PYSIDE6:
-    from PySide6 import QtCore, QtGui, QtWidgets as QtWid  # type: ignore
-    from PySide6.QtCore import Slot                        # type: ignore
-    from PySide6.QtCore import Signal                      # type: ignore
-# pylint: enable=import-error, no-name-in-module
-# fmt: on
-
-# \end[Mechanism to support both PyQt and PySide]
-# -----------------------------------------------
-
-from dvg_pyqt_controls import (
-    create_Toggle_button,
-    create_error_LED,
-    create_tiny_error_LED,
-    SS_GROUP,
-)
-from dvg_debug_functions import print_fancy_traceback as pft
+from qtpy import QtCore, QtGui, QtWidgets as QtWid
+from qtpy.QtCore import Signal, Slot  # type: ignore
 
+import dvg_pyqt_controls as controls
+from dvg_debug_functions import print_fancy_traceback as pft
 from dvg_qdeviceio import QDeviceIO, DAQ_TRIGGER
 from dvg_devices.ThermoFlex_chiller_protocol_RS232 import ThermoFlex_chiller
 
 # Special characters
 CHAR_DEG_C = chr(176) + "C"
 
 
@@ -117,29 +55,34 @@
         DAQ_interval_ms=1000,
         DAQ_timer_type=QtCore.Qt.TimerType.CoarseTimer,
         critical_not_alive_count=1,
         debug=False,
         **kwargs,
     ):
         super().__init__(dev, **kwargs)  # Pass kwargs onto QtCore.QObject()
+        self.dev: ThermoFlex_chiller  # Enforce type: removes `_NoDevice()`
 
         self.create_worker_DAQ(
             DAQ_trigger=DAQ_TRIGGER.INTERNAL_TIMER,
             DAQ_function=self.DAQ_function,
             DAQ_interval_ms=DAQ_interval_ms,
             DAQ_timer_type=DAQ_timer_type,
             critical_not_alive_count=critical_not_alive_count,
             debug=debug,
         )
 
         self.create_worker_jobs(jobs_function=self.jobs_function, debug=debug)
 
         self.create_GUI()
         self.signal_DAQ_updated.connect(self.update_GUI)
-        self.connect_signals_to_slots()
+        self.signal_GUI_PID_values_update.connect(self.update_GUI_PID_values)
+        self.signal_GUI_alarm_values_update.connect(
+            self.update_GUI_alarm_values
+        )
+
         if not self.dev.is_alive:
             self.update_GUI()  # Correctly reflect an offline device
 
     # --------------------------------------------------------------------------
     #   DAQ_function
     # --------------------------------------------------------------------------
 
@@ -185,16 +128,19 @@
         self.HI_flow = QtWid.QLineEdit(**p)
         self.LO_pres = QtWid.QLineEdit(**p)
         self.HI_pres = QtWid.QLineEdit(**p)
         self.LO_temp = QtWid.QLineEdit(**p)
         self.HI_temp = QtWid.QLineEdit(**p)
         self.pbtn_read_alarm_values = QtWid.QPushButton("Read")
         self.pbtn_read_alarm_values.setMinimumSize(50, 30)
+        self.pbtn_read_alarm_values.clicked.connect(
+            self.process_pbtn_read_alarm_values
+        )
 
-        p = {"alignment": QtCore.Qt.AlignmentFlag.AlignCenter}
+        p = {"parent": None, "alignment": QtCore.Qt.AlignmentFlag.AlignCenter}
         grid = QtWid.QGridLayout()
         # fmt: off
         grid.addWidget(QtWid.QLabel("Values can be set in the chiller's menu",
                                     **p)          , 0, 0, 1, 4)
         grid.addWidget(QtWid.QLabel("LO")         , 1, 1)
         grid.addWidget(QtWid.QLabel("HI")         , 1, 2)
         grid.addWidget(QtWid.QLabel("Flow rate")  , 2, 0)
@@ -209,15 +155,14 @@
         grid.addWidget(self.LO_temp               , 4, 1)
         grid.addWidget(self.HI_temp               , 4, 2)
         grid.addWidget(QtWid.QLabel(CHAR_DEG_C)   , 4, 3)
         grid.addWidget(self.pbtn_read_alarm_values, 5, 0)
         # fmt: on
 
         self.grpb_alarms = QtWid.QGroupBox("Alarm values")
-        self.grpb_alarms.setStyleSheet(SS_GROUP)
         self.grpb_alarms.setLayout(grid)
 
         # Groupbox "PID feedback"
         # -----------------------
         p = {
             "alignment": QtCore.Qt.AlignmentFlag.AlignRight,
             "minimumWidth": 50,
@@ -225,16 +170,19 @@
             "readOnly": True,
         }
         self.PID_P = QtWid.QLineEdit(**p)
         self.PID_I = QtWid.QLineEdit(**p)
         self.PID_D = QtWid.QLineEdit(**p)
         self.pbtn_read_PID_values = QtWid.QPushButton("Read")
         self.pbtn_read_PID_values.setMinimumSize(50, 30)
+        self.pbtn_read_PID_values.clicked.connect(
+            self.process_pbtn_read_PID_values
+        )
 
-        p = {"alignment": QtCore.Qt.AlignmentFlag.AlignCenter}
+        p = {"parent": None, "alignment": QtCore.Qt.AlignmentFlag.AlignCenter}
         grid = QtWid.QGridLayout()
         # fmt: off
         grid.addWidget(QtWid.QLabel("Values can be set in the chiller's menu",
                                     **p)                          , 0, 0, 1, 3)
         grid.addWidget(QtWid.QLabel("P", **p)                     , 1, 0)
         grid.addWidget(self.PID_P                                 , 1, 1)
         grid.addWidget(QtWid.QLabel("% span of 100" + CHAR_DEG_C) , 1, 2)
@@ -244,47 +192,46 @@
         grid.addWidget(QtWid.QLabel("D", **p)                     , 3, 0)
         grid.addWidget(self.PID_D                                 , 3, 1)
         grid.addWidget(QtWid.QLabel("minutes")                    , 3, 2)
         grid.addWidget(self.pbtn_read_PID_values                  , 4, 0)
         # fmt: on
 
         self.grpb_PID = QtWid.QGroupBox("PID feedback")
-        self.grpb_PID.setStyleSheet(SS_GROUP)
         self.grpb_PID.setLayout(grid)
 
         # Groupbox "Status bits"
         # ----------------------
         # fmt: off
-        self.SB_tripped                = create_error_LED()
+        self.SB_tripped                = controls.create_error_LED()
         self.SB_tripped.setText("No faults")
-        self.SB_high_temp_fixed        = create_tiny_error_LED()
-        self.SB_low_temp_fixed         = create_tiny_error_LED()
-        self.SB_high_temp              = create_tiny_error_LED()
-        self.SB_low_temp               = create_tiny_error_LED()
-        self.SB_high_pressure          = create_tiny_error_LED()
-        self.SB_low_pressure           = create_tiny_error_LED()
-        self.SB_drip_pan               = create_tiny_error_LED()
-        self.SB_high_level             = create_tiny_error_LED()
-        self.SB_phase_monitor          = create_tiny_error_LED()
-        self.SB_motor_overload         = create_tiny_error_LED()
-        self.SB_LPC                    = create_tiny_error_LED()
-        self.SB_HPC                    = create_tiny_error_LED()
-        self.SB_external_EMO           = create_tiny_error_LED()
-        self.SB_local_EMO              = create_tiny_error_LED()
-        self.SB_low_flow               = create_tiny_error_LED()
-        self.SB_low_level              = create_tiny_error_LED()
-        self.SB_sense_5V               = create_tiny_error_LED()
-        self.SB_invalid_level          = create_tiny_error_LED()
-        self.SB_low_fixed_flow_warning = create_tiny_error_LED()
-        self.SB_high_pressure_factory  = create_tiny_error_LED()
-        self.SB_low_pressure_factory   = create_tiny_error_LED()
+        self.SB_high_temp_fixed        = controls.create_tiny_error_LED()
+        self.SB_low_temp_fixed         = controls.create_tiny_error_LED()
+        self.SB_high_temp              = controls.create_tiny_error_LED()
+        self.SB_low_temp               = controls.create_tiny_error_LED()
+        self.SB_high_pressure          = controls.create_tiny_error_LED()
+        self.SB_low_pressure           = controls.create_tiny_error_LED()
+        self.SB_drip_pan               = controls.create_tiny_error_LED()
+        self.SB_high_level             = controls.create_tiny_error_LED()
+        self.SB_phase_monitor          = controls.create_tiny_error_LED()
+        self.SB_motor_overload         = controls.create_tiny_error_LED()
+        self.SB_LPC                    = controls.create_tiny_error_LED()
+        self.SB_HPC                    = controls.create_tiny_error_LED()
+        self.SB_external_EMO           = controls.create_tiny_error_LED()
+        self.SB_local_EMO              = controls.create_tiny_error_LED()
+        self.SB_low_flow               = controls.create_tiny_error_LED()
+        self.SB_low_level              = controls.create_tiny_error_LED()
+        self.SB_sense_5V               = controls.create_tiny_error_LED()
+        self.SB_invalid_level          = controls.create_tiny_error_LED()
+        self.SB_low_fixed_flow_warning = controls.create_tiny_error_LED()
+        self.SB_high_pressure_factory  = controls.create_tiny_error_LED()
+        self.SB_low_pressure_factory   = controls.create_tiny_error_LED()
 
-        p = {'alignment': QtCore.Qt.AlignmentFlag.AlignRight}
+        p = {"parent":None, "alignment": QtCore.Qt.AlignmentFlag.AlignRight}
         grid = QtWid.QGridLayout()
-        grid.addWidget(self.SB_tripped                            , 0, 0, 1, 2)
+        grid.addWidget(self.SB_tripped                           , 0, 0, 1, 2)
         grid.addItem(QtWid.QSpacerItem(1, 12)                          , 1, 0)
         grid.addWidget(QtWid.QLabel("high temp fixed fault", **p)      , 2, 0)
         grid.addWidget(self.SB_high_temp_fixed                         , 2, 1)
         grid.addWidget(QtWid.QLabel("low temp fixed fault", **p)       , 3, 0)
         grid.addWidget(self.SB_low_temp_fixed                          , 3, 1)
         grid.addWidget(QtWid.QLabel("high temp fault/warning", **p)    , 4, 0)
         grid.addWidget(self.SB_high_temp                               , 4, 1)
@@ -323,88 +270,89 @@
         grid.addWidget(QtWid.QLabel("high pressure factory fault", **p), 21, 0)
         grid.addWidget(self.SB_high_pressure_factory                   , 21, 1)
         grid.addWidget(QtWid.QLabel("low pressure factory fault", **p) , 22, 0)
         grid.addWidget(self.SB_low_pressure_factory                    , 22, 1)
         # fmt: on
 
         self.grpb_SBs = QtWid.QGroupBox("Status bits")
-        self.grpb_SBs.setStyleSheet(SS_GROUP)
         self.grpb_SBs.setLayout(grid)
 
         # Groupbox "Control"
         # ------------------
         p = {
             "alignment": QtCore.Qt.AlignmentFlag.AlignRight,
             "minimumWidth": 50,
             "maximumWidth": 30,
         }
+        p2 = {**p, "readOnly": True}
 
-        self.lbl_offline = QtWid.QLabel(
-            "OFFLINE",
-            visible=False,
-            font=QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold),
-            alignment=QtCore.Qt.AlignmentFlag.AlignCenter,
+        self.lbl_offline = QtWid.QLabel("OFFLINE")
+        self.lbl_offline.setVisible(False)
+        self.lbl_offline.setFont(
+            QtGui.QFont("Palatino", 14, weight=QtGui.QFont.Weight.Bold)
         )
+        self.lbl_offline.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         # fmt: off
-        self.pbtn_on       = create_Toggle_button("Off")
-        self.powering_down = create_tiny_error_LED()
+        self.pbtn_on       = controls.create_Toggle_button("Off")
+        self.pbtn_on.clicked.connect(self.process_pbtn_on)
+        self.powering_down = controls.create_tiny_error_LED()
         self.send_setpoint = QtWid.QLineEdit(**p)
-        self.read_setpoint = QtWid.QLineEdit(**p, readOnly=True)
-        self.read_temp     = QtWid.QLineEdit(**p, readOnly=True)
-        self.read_flow     = QtWid.QLineEdit(**p, readOnly=True)
-        self.read_supply   = QtWid.QLineEdit(**p, readOnly=True)
-        self.read_suction  = QtWid.QLineEdit(**p, readOnly=True)
+        self.send_setpoint.editingFinished.connect(
+            self.send_setpoint_from_textbox
+        )
+        self.read_setpoint = QtWid.QLineEdit(**p2)
+        self.read_temp     = QtWid.QLineEdit(**p2)
+        self.read_flow     = QtWid.QLineEdit(**p2)
+        self.read_supply   = QtWid.QLineEdit(**p2)
+        self.read_suction  = QtWid.QLineEdit(**p2)
         self.lbl_update_counter = QtWid.QLabel("0")
 
+        p = {"parent": None, "alignment": QtCore.Qt.AlignmentFlag.AlignRight}
+
         grid = QtWid.QGridLayout()
-        grid.addWidget(self.lbl_offline                   , 0, 0, 1, 3)
-        grid.addWidget(self.pbtn_on                       , 1, 0, 1, 3)
-        grid.addWidget(QtWid.QLabel("Is powering up/down?",
-         alignment=QtCore.Qt.AlignmentFlag.AlignRight)    , 2, 0, 1, 2)
-        grid.addWidget(self.powering_down                 , 2, 2)
-        grid.addItem(QtWid.QSpacerItem(1, 12)             , 3, 0)
-        grid.addWidget(QtWid.QLabel("Send setpoint")      , 4, 0)
-        grid.addWidget(QtWid.QLabel("Read setpoint")      , 5, 0)
-        grid.addWidget(self.send_setpoint                 , 4, 1)
-        grid.addWidget(self.read_setpoint                 , 5, 1)
-        grid.addWidget(QtWid.QLabel(CHAR_DEG_C)           , 4, 2)
-        grid.addWidget(QtWid.QLabel(CHAR_DEG_C)           , 5, 2)
-        grid.addItem(QtWid.QSpacerItem(1, 12)             , 6, 0)
-        grid.addWidget(QtWid.QLabel("Read temp")          , 7, 0)
-        grid.addWidget(self.read_temp                     , 7, 1)
-        grid.addWidget(QtWid.QLabel(CHAR_DEG_C)           , 7, 2)
-        grid.addWidget(QtWid.QLabel("Read flow")          , 8, 0)
-        grid.addWidget(self.read_flow                     , 8, 1)
-        grid.addWidget(QtWid.QLabel("LPM")                , 8, 2)
-        grid.addWidget(QtWid.QLabel("Read supply")        , 9, 0)
-        grid.addWidget(self.read_supply                   , 9, 1)
-        grid.addWidget(QtWid.QLabel("bar")                , 9, 2)
-        grid.addWidget(QtWid.QLabel("Read suction")       , 10, 0)
-        grid.addWidget(self.read_suction                  , 10, 1)
-        grid.addWidget(QtWid.QLabel("bar")                , 10, 2)
+        grid.addWidget(self.lbl_offline                         , 0, 0, 1, 3)
+        grid.addWidget(self.pbtn_on                             , 1, 0, 1, 3)
+        grid.addWidget(QtWid.QLabel("Is powering up/down?", **p), 2, 0, 1, 2)
+        grid.addWidget(self.powering_down                       , 2, 2)
+        grid.addItem(QtWid.QSpacerItem(1, 12)                   , 3, 0)
+        grid.addWidget(QtWid.QLabel("Send setpoint")            , 4, 0)
+        grid.addWidget(QtWid.QLabel("Read setpoint")            , 5, 0)
+        grid.addWidget(self.send_setpoint                       , 4, 1)
+        grid.addWidget(self.read_setpoint                       , 5, 1)
+        grid.addWidget(QtWid.QLabel(CHAR_DEG_C)                 , 4, 2)
+        grid.addWidget(QtWid.QLabel(CHAR_DEG_C)                 , 5, 2)
+        grid.addItem(QtWid.QSpacerItem(1, 12)                   , 6, 0)
+        grid.addWidget(QtWid.QLabel("Read temp")                , 7, 0)
+        grid.addWidget(self.read_temp                           , 7, 1)
+        grid.addWidget(QtWid.QLabel(CHAR_DEG_C)                 , 7, 2)
+        grid.addWidget(QtWid.QLabel("Read flow")                , 8, 0)
+        grid.addWidget(self.read_flow                           , 8, 1)
+        grid.addWidget(QtWid.QLabel("LPM")                      , 8, 2)
+        grid.addWidget(QtWid.QLabel("Read supply")              , 9, 0)
+        grid.addWidget(self.read_supply                         , 9, 1)
+        grid.addWidget(QtWid.QLabel("bar")                      , 9, 2)
+        grid.addWidget(QtWid.QLabel("Read suction")             , 10, 0)
+        grid.addWidget(self.read_suction                        , 10, 1)
+        grid.addWidget(QtWid.QLabel("bar")                      , 10, 2)
 
         grid.addItem(QtWid.QSpacerItem(1, 12)                      , 11, 0)
         grid.addWidget(QtWid.QLabel("Nominal values @ 15-02-2018:"), 12, 0, 1, 3)
         grid.addWidget(QtWid.QLabel("Read flow")                   , 13, 0)
-        grid.addWidget(QtWid.QLabel("80  ",
-                      alignment=QtCore.Qt.AlignmentFlag.AlignRight), 13, 1)
+        grid.addWidget(QtWid.QLabel("80  ", **p)                   , 13, 1)
         grid.addWidget(QtWid.QLabel("LPM")                         , 13, 2)
         grid.addWidget(QtWid.QLabel("Read supply")                 , 14, 0)
-        grid.addWidget(QtWid.QLabel("2.9  ",
-                      alignment=QtCore.Qt.AlignmentFlag.AlignRight), 14, 1)
+        grid.addWidget(QtWid.QLabel("2.9  ", **p)                  , 14, 1)
         grid.addWidget(QtWid.QLabel("bar")                         , 14, 2)
         grid.addWidget(QtWid.QLabel("Read suction")                , 15, 0)
-        grid.addWidget(QtWid.QLabel("40  ",
-                      alignment=QtCore.Qt.AlignmentFlag.AlignRight), 15, 1)
+        grid.addWidget(QtWid.QLabel("40  ", **p)                   , 15, 1)
         grid.addWidget(QtWid.QLabel("bar")                         , 15, 2)
         grid.addWidget(self.lbl_update_counter                     , 16, 0, 1, 2)
         # fmt: on
 
         self.grpb_control = QtWid.QGroupBox("Control")
-        self.grpb_control.setStyleSheet(SS_GROUP)
         self.grpb_control.setLayout(grid)
 
         # --------------------------------------
         #   Round up final QtWid.QHBoxLayout()
         # --------------------------------------
 
         vbox = QtWid.QVBoxLayout()
@@ -441,95 +389,95 @@
         Not locking the mutex might speed up the program.
         """
         if self.dev.is_alive:
             # At startup
             if self.update_counter_DAQ == 1:
                 self.update_GUI_alarm_values()
                 self.update_GUI_PID_values()
-                self.send_setpoint.setText("%.1f" % self.dev.state.setpoint)
+                self.send_setpoint.setText(f"{self.dev.state.setpoint:.1f}")
 
             # State
             # fmt: off
-            self.read_setpoint.setText("%.1f" % self.dev.state.setpoint)
-            self.read_temp.setText    ("%.1f" % self.dev.state.temp)
-            self.read_flow.setText    ("%.1f" % self.dev.state.flow)
-            self.read_supply.setText  ("%.2f" % self.dev.state.supply_pres)
-            self.read_suction.setText ("%.2f" % self.dev.state.suction_pres)
+            self.read_setpoint.setText(f"{self.dev.state.setpoint:.1f}")
+            self.read_temp.setText    (f"{self.dev.state.temp:.1f}")
+            self.read_flow.setText    (f"{self.dev.state.flow:.1f}")
+            self.read_supply.setText  (f"{self.dev.state.supply_pres:.2f}")
+            self.read_suction.setText (f"{self.dev.state.suction_pres:.2f}")
             # fmt: on
 
             # Power
             SBs = self.dev.status_bits  # Short-hand
-            self.pbtn_on.setChecked(SBs.running)
+            self.pbtn_on.setChecked(bool(SBs.running))
             if SBs.running:
                 self.pbtn_on.setText("ON")
             else:
                 self.pbtn_on.setText("OFF")
-            self.powering_down.setChecked(SBs.powering_down)
+            self.powering_down.setChecked(bool(SBs.powering_down))
 
             # Status bits
-            self.SB_tripped.setChecked(SBs.fault_tripped)
+            self.SB_tripped.setChecked(bool(SBs.fault_tripped))
             if self.dev.status_bits.fault_tripped:
                 self.SB_tripped.setText("FAULT TRIPPED")
             else:
                 self.SB_tripped.setText("No faults")
-            self.SB_drip_pan.setChecked(SBs.drip_pan_fault)
-            self.SB_external_EMO.setChecked(SBs.external_EMO_fault)
-            self.SB_high_level.setChecked(SBs.high_level_fault)
-            self.SB_high_pressure.setChecked(SBs.high_pressure_fault)
+            self.SB_drip_pan.setChecked(bool(SBs.drip_pan_fault))
+            self.SB_external_EMO.setChecked(bool(SBs.external_EMO_fault))
+            self.SB_high_level.setChecked(bool(SBs.high_level_fault))
+            self.SB_high_pressure.setChecked(bool(SBs.high_pressure_fault))
             self.SB_high_pressure_factory.setChecked(
-                SBs.high_pressure_fault_factory
+                bool(SBs.high_pressure_fault_factory)
             )
-            self.SB_high_temp.setChecked(SBs.high_temp_fault)
-            self.SB_high_temp_fixed.setChecked(SBs.high_temp_fixed_fault)
-            self.SB_HPC.setChecked(SBs.HPC_fault)
-            self.SB_invalid_level.setChecked(SBs.invalid_level_fault)
-            self.SB_local_EMO.setChecked(SBs.local_EMO_fault)
+            self.SB_high_temp.setChecked(bool(SBs.high_temp_fault))
+            self.SB_high_temp_fixed.setChecked(bool(SBs.high_temp_fixed_fault))
+            self.SB_HPC.setChecked(bool(SBs.HPC_fault))
+            self.SB_invalid_level.setChecked(bool(SBs.invalid_level_fault))
+            self.SB_local_EMO.setChecked(bool(SBs.local_EMO_fault))
             self.SB_low_fixed_flow_warning.setChecked(
-                SBs.low_fixed_flow_warning
+                bool(SBs.low_fixed_flow_warning)
             )
-            self.SB_low_flow.setChecked(SBs.low_flow_fault)
-            self.SB_low_level.setChecked(SBs.low_level_fault)
-            self.SB_low_pressure.setChecked(SBs.low_pressure_fault)
+            self.SB_low_flow.setChecked(bool(SBs.low_flow_fault))
+            self.SB_low_level.setChecked(bool(SBs.low_level_fault))
+            self.SB_low_pressure.setChecked(bool(SBs.low_pressure_fault))
             self.SB_low_pressure_factory.setChecked(
-                SBs.low_pressure_fault_factory
+                bool(SBs.low_pressure_fault_factory)
             )
-            self.SB_low_temp.setChecked(SBs.low_temp_fault)
-            self.SB_low_temp_fixed.setChecked(SBs.low_temp_fixed_fault)
-            self.SB_LPC.setChecked(SBs.LPC_fault)
-            self.SB_motor_overload.setChecked(SBs.motor_overload_fault)
-            self.SB_phase_monitor.setChecked(SBs.phase_monitor_fault)
-            self.SB_sense_5V.setChecked(SBs.sense_5V_fault)
+            self.SB_low_temp.setChecked(bool(SBs.low_temp_fault))
+            self.SB_low_temp_fixed.setChecked(bool(SBs.low_temp_fixed_fault))
+            self.SB_LPC.setChecked(bool(SBs.LPC_fault))
+            self.SB_motor_overload.setChecked(bool(SBs.motor_overload_fault))
+            self.SB_phase_monitor.setChecked(bool(SBs.phase_monitor_fault))
+            self.SB_sense_5V.setChecked(bool(SBs.sense_5V_fault))
 
-            self.lbl_update_counter.setText("%s" % self.update_counter_DAQ)
+            self.lbl_update_counter.setText(f"{self.update_counter_DAQ}")
         else:
             self.grpb_alarms.setEnabled(False)
             self.grpb_PID.setEnabled(False)
             self.grpb_SBs.setEnabled(False)
             self.grpb_control.setEnabled(False)
 
             self.pbtn_on.setVisible(False)
             self.lbl_offline.setVisible(True)
 
     @Slot()
     def update_GUI_alarm_values(self):
-        self.LO_flow.setText("%.1f" % self.dev.values_alarm.LO_flow)
+        self.LO_flow.setText(f"{self.dev.values_alarm.LO_flow:.1f}")
         if self.dev.values_alarm.HI_flow == 0:
             self.HI_flow.setText("No limit")
         else:
-            self.HI_flow.setText("%.1f" % self.dev.values_alarm.HI_flow)
-        self.LO_pres.setText("%.2f" % self.dev.values_alarm.LO_pres)
-        self.HI_pres.setText("%.2f" % self.dev.values_alarm.HI_pres)
-        self.LO_temp.setText("%.1f" % self.dev.values_alarm.LO_temp)
-        self.HI_temp.setText("%.1f" % self.dev.values_alarm.HI_temp)
+            self.HI_flow.setText(f"{self.dev.values_alarm.HI_flow:.1f}")
+        self.LO_pres.setText(f"{self.dev.values_alarm.LO_pres:.2f}")
+        self.HI_pres.setText(f"{self.dev.values_alarm.HI_pres:.2f}")
+        self.LO_temp.setText(f"{self.dev.values_alarm.LO_temp:.1f}")
+        self.HI_temp.setText(f"{self.dev.values_alarm.HI_temp:.1f}")
 
     @Slot()
     def update_GUI_PID_values(self):
-        self.PID_P.setText("%.1f" % self.dev.values_PID.P)
-        self.PID_I.setText("%.2f" % self.dev.values_PID.I)
-        self.PID_D.setText("%.1f" % self.dev.values_PID.D)
+        self.PID_P.setText(f"{self.dev.values_PID.P:.1f}")
+        self.PID_I.setText(f"{self.dev.values_PID.I:.2f}")
+        self.PID_D.setText(f"{self.dev.values_PID.D:.1f}")
 
     # --------------------------------------------------------------------------
     #   GUI functions
     # --------------------------------------------------------------------------
 
     @Slot()
     def process_pbtn_on(self):
@@ -552,36 +500,15 @@
 
     @Slot()
     def send_setpoint_from_textbox(self):
         try:
             setpoint = float(self.send_setpoint.text())
         except (TypeError, ValueError):
             setpoint = 22.0
-        except:
-            raise
+        except Exception as err:
+            raise err
 
         setpoint = max(setpoint, self.dev.min_setpoint_degC)
         setpoint = min(setpoint, self.dev.max_setpoint_degC)
-        self.send_setpoint.setText("%.1f" % setpoint)
+        self.send_setpoint.setText(f"{setpoint:.1f}")
 
         self.send(self.dev.send_setpoint, setpoint)
-
-    # --------------------------------------------------------------------------
-    #   connect_signals_to_slots
-    # --------------------------------------------------------------------------
-
-    def connect_signals_to_slots(self):
-        self.pbtn_on.clicked.connect(self.process_pbtn_on)
-        self.pbtn_read_alarm_values.clicked.connect(
-            self.process_pbtn_read_alarm_values
-        )
-        self.pbtn_read_PID_values.clicked.connect(
-            self.process_pbtn_read_PID_values
-        )
-        self.send_setpoint.editingFinished.connect(
-            self.send_setpoint_from_textbox
-        )
-
-        self.signal_GUI_alarm_values_update.connect(
-            self.update_GUI_alarm_values
-        )
-        self.signal_GUI_PID_values_update.connect(self.update_GUI_PID_values)
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices/Traverse_layout.png` & `dvg-devices-1.4.0/src/dvg_devices/Traverse_layout.png`

 * *Files identical despite different names*

### Comparing `dvg-devices-1.3.0/src/dvg_devices.egg-info/PKG-INFO` & `dvg-devices-1.4.0/src/dvg_devices.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 Metadata-Version: 2.1
 Name: dvg-devices
-Version: 1.3.0
+Version: 1.4.0
 Summary: Collection of I/O interfaces to communicate with microcontroller boards and laboratory devices, with optional PyQt/PySide multithread support and graphical user-interfaces.
 Home-page: https://python-dvg-devices.readthedocs.io
 Author: Dennis van Gils
 Author-email: vangils.dennis@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Dennis-van-Gils/python-dvg-devices/issues
 Keywords: PyQt5,PyQt6,PySide2,PySide6,device I/O,automation,laboratory,science,control,experiment,multithread,Arduino,serial,VISA
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering 
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+Requires-Dist: dvg-debug-functions~=2.4
+Requires-Dist: dvg-pid-controller~=2.1
+Requires-Dist: dvg-pyqt-controls~=1.3
+Requires-Dist: dvg-pyqt-filelogger~=1.3
+Requires-Dist: dvg-pyqtgraph-threadsafe~=3.3
+Requires-Dist: dvg-qdeviceio~=1.2
+Requires-Dist: matplotlib~=3.1
+Requires-Dist: numpy~=1.15
+Requires-Dist: pyserial~=3.4
+Requires-Dist: pyvisa~=1.11
+Requires-Dist: qtpy
 Provides-Extra: pyqt5
+Requires-Dist: pyqt5~=5.12; extra == "pyqt5"
 Provides-Extra: pyqt6
+Requires-Dist: pyqt6; extra == "pyqt6"
 Provides-Extra: pyside2
+Requires-Dist: pyside2; extra == "pyside2"
 Provides-Extra: pyside6
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
+Requires-Dist: pyside6; extra == "pyside6"
 
-.. image:: https://img.shields.io/pypi/v/dvg-devices
+|pypi| |python| |readthedocs| |black| |license|
+
+.. |pypi| image:: https://img.shields.io/pypi/v/dvg-devices
     :target: https://pypi.org/project/dvg-devices
-.. image:: https://img.shields.io/pypi/pyversions/dvg-devices
+.. |python| image:: https://img.shields.io/pypi/pyversions/dvg-devices
     :target: https://pypi.org/project/dvg-devices
-.. image:: https://requires.io/github/Dennis-van-Gils/python-dvg-devices/requirements.svg?branch=master
-    :target: https://requires.io/github/Dennis-van-Gils/python-dvg-devices/requirements/?branch=master
-    :alt: Requirements Status
-.. image:: https://readthedocs.org/projects/python-dvg-devices/badge/?version=latest
+.. |readthedocs| image:: https://readthedocs.org/projects/python-dvg-devices/badge/?version=latest
     :target: https://python-dvg-devices.readthedocs.io/en/latest/?badge=latest
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
-.. image:: https://img.shields.io/badge/License-MIT-purple.svg
+.. |license| image:: https://img.shields.io/badge/License-MIT-purple.svg
     :target: https://github.com/Dennis-van-Gils/python-dvg-devices/blob/master/LICENSE.txt
 
 DvG_Devices
 =============
 *Collection of I/O interfaces to communicate with microcontroller boards and
 laboratory devices, with optional PyQt/PySide multithread support and graphical
 user-interfaces.*
@@ -59,33 +72,37 @@
 - Github: https://github.com/Dennis-van-Gils/python-dvg-devices
 - PyPI: https://pypi.org/project/dvg-devices
 
 Installation::
 
     pip install dvg-devices
 
-Installation with an optional Qt-library::
+To be able to run the several provided graphical user-interfaces, one has to install an additional Qt-library. This can be either PyQt5, PyQt6, PySide2 or PySide6. Installation with an optional Qt-library::
 
     pip install dvg-devices[pyqt5/pyqt6/pyside2/pyside6]
 
+If you wish to interface with an GPIB device you need to additionally install a Visa backend. See https://pyvisa.readthedocs.io/en/latest/introduction/getting.html
+
 Supported devices
 -----------------
 
-    =======================    =======================
-    Arduino, or similar        microcontroller board
-    Aim TTi QL series II       power supply
-    Bronkhorst EL-FLOW         mass flow controller
-    Julabo circulator          recirculating bath
-    Keysight 3497xA            digital multimeter
-    Keysight N8700             power supply
-    Parker Compax3             servo controller
-    Picotech PT104             temperature logger
-    PolyScience PD             recirculating bath
-    ThermoFisher ThermoFlex    chiller
-    =======================    =======================
+    =======================    ==============================
+    Arduino, or similar        Microcontroller board
+    Aim TTi QL series II       Power supply
+    Bronkhorst EL-FLOW         Mass flow controller
+    Julabo circulator          Recirculating bath
+    Keysight 3497xA            Digital multimeter
+    Keysight N8700             Power supply
+    Novanta IMS MDrive         Stepper motor controller
+    Parker Compax3             Servo controller
+    Picotech PT104             Temperature logger
+    PolyScience PD             Recirculating bath
+    ThermoFisher ThermoFlex    Chiller
+    Xylem Hydrovar HVL         Variable speed pump controller
+    =======================    ==============================
 
 Highlights
 ----------
 * Class ``SerialDevice()`` offering higher-level general I/O methods for
   a serial device, such as ``auto_connect()``, ``write()`` and ``query()``.
 
 * Class ``Arduino()`` which wraps around ``SerialDevice()``. In combination with
@@ -99,14 +116,31 @@
 
 * Ready-to-run PyQt/PySide demos to directly control many of the supported
   devices with a graphical user-interface.
 
 Changelog
 =========
 
+1.4.0 (2024-05-23)
+------------------
+Major clean-up and streamlining:
+
+* Using `qtpy` library instead of my own Qt5/6 mechanism
+* Changed all string formatting to f-strings
+* Extended type hinting and checking
+* Made demos uniform and passing `qdev` arguments to `MainWindow` now
+* Individual source files now follow the PyPi package version
+* Resolved nearly all Pylint / Pylance warnings
+* Removed Python 3.6 support
+
+New devices added:
+
+* Xylem Hydrovar HVL - Variable speed pump controller
+* Novanta IMS MDrive - Stepper motor controller
+
 1.3.0 (2023-02-23)
 ------------------
 * Added method ``BaseDevice.SerialDevice.query_bytes()``
 * Fixed type hints in ``BaseDevice.SerialDevice``
 
 1.2.0 (2022-09-14)
 ------------------
@@ -193,9 +227,7 @@
 ------------------
 * Major restructuring PyPI package
 * Implemented ``DvG_QDeviceIO``
 
 0.0.1 (2020-07-01)
 ------------------
 * First release on PyPI
-
-
```

### Comparing `dvg-devices-1.3.0/src/dvg_devices.egg-info/SOURCES.txt` & `dvg-devices-1.4.0/src/dvg_devices.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,22 +35,32 @@
 src/dvg_devices/Keysight_3497xA_demo.py
 src/dvg_devices/Keysight_3497xA_demo_logger.py
 src/dvg_devices/Keysight_3497xA_protocol_SCPI.py
 src/dvg_devices/Keysight_3497xA_qdev.py
 src/dvg_devices/Keysight_N8700_demo.py
 src/dvg_devices/Keysight_N8700_protocol_SCPI.py
 src/dvg_devices/Keysight_N8700_qdev.py
+src/dvg_devices/MDrive_example_motion_program_x.mxt
+src/dvg_devices/MDrive_example_motion_program_z.mxt
+src/dvg_devices/MDrive_stepper_demo.py
+src/dvg_devices/MDrive_stepper_protocol_RS422.py
+src/dvg_devices/MDrive_stepper_qdev.py
 src/dvg_devices/Picotech_PT104_demo.py
 src/dvg_devices/Picotech_PT104_protocol_UDP.py
 src/dvg_devices/Picotech_PT104_qdev.py
 src/dvg_devices/PolyScience_PD_bath_protocol_RS232.py
 src/dvg_devices/ThermoFlex_chiller_demo.py
 src/dvg_devices/ThermoFlex_chiller_protocol_RS232.py
 src/dvg_devices/ThermoFlex_chiller_qdev.py
 src/dvg_devices/Traverse_layout.png
+src/dvg_devices/XylemHydrovarHVL_CRC_tools.py
+src/dvg_devices/XylemHydrovarHVL_demo.py
+src/dvg_devices/XylemHydrovarHVL_protocol_RTU.py
+src/dvg_devices/XylemHydrovarHVL_qdev.py
+src/dvg_devices/_Qt_tests.py
 src/dvg_devices/_init_.py
 src/dvg_devices.egg-info/PKG-INFO
 src/dvg_devices.egg-info/SOURCES.txt
 src/dvg_devices.egg-info/dependency_links.txt
 src/dvg_devices.egg-info/not-zip-safe
 src/dvg_devices.egg-info/requires.txt
 src/dvg_devices.egg-info/top_level.txt
```

