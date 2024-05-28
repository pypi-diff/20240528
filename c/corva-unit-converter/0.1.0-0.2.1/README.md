# Comparing `tmp/corva-unit-converter-0.1.0.tar.gz` & `tmp/corva_unit_converter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corva-unit-converter-0.1.0.tar", last modified: Wed Apr 10 12:57:36 2024, max compression
+gzip compressed data, was "corva_unit_converter-0.2.1.tar", last modified: Tue May 28 15:30:09 2024, max compression
```

## Comparing `corva-unit-converter-0.1.0.tar` & `corva_unit_converter-0.2.1.tar`

### file list

```diff
@@ -1,79 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:57:36.001036 corva-unit-converter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-10 12:57:36.001036 corva-unit-converter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:57:36.001036 corva-unit-converter-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:57:35.985036 corva-unit-converter-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:57:35.985036 corva-unit-converter-0.1.0/src/corva_unit_converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:57:35.993035 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/acoustic_slowness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/angle_per_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/angular_velocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/area.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/current.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/density.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/digital.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/force.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/gas_concentration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/gas_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/inverse_pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/length.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/length_per_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/mass_flow_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/parts_per.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/permiability.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/porosity.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/power.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/pressure_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/revolution_per_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/torque.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/voltage.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/volume_concentration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/volume_flow_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/corva_unit_converter/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:57:35.997036 corva-unit-converter-0.1.0/src/corva_unit_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-10 12:57:35.000000 corva-unit-converter-0.1.0/src/corva_unit_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-10 12:57:35.000000 corva-unit-converter-0.1.0/src/corva_unit_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:57:35.000000 corva-unit-converter-0.1.0/src/corva_unit_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 12:57:35.000000 corva-unit-converter-0.1.0/src/corva_unit_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:57:35.997036 corva-unit-converter-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_acoustic_slowness.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_angle_per_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_angular_velocity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_force.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_gas_concentration.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_gas_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_inverse_pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_length_per_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_mass_flow_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_porosity.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_pressure_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_revolution_per_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_torque.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_volume_concentration.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 12:57:31.000000 corva-unit-converter-0.1.0/tests/test_volume_flow_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:30:09.623384 corva_unit_converter-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-28 15:30:09.623384 corva_unit_converter-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:30:09.623384 corva_unit_converter-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:30:09.607384 corva_unit_converter-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:30:09.611384 corva_unit_converter-0.2.1/src/corva_unit_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:30:09.619384 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/acoustic_slowness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/angle_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/angular_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/digital.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/gas_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/gas_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/inverse_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/length_per_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/mass_flow_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/parts_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/permiability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/porosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/pressure_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/proportion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/revolution_per_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/strokes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/volume_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/volume_flow_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/corva_unit_converter/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:30:09.623384 corva_unit_converter-0.2.1/src/corva_unit_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-28 15:30:09.000000 corva_unit_converter-0.2.1/src/corva_unit_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-28 15:30:09.000000 corva_unit_converter-0.2.1/src/corva_unit_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:30:09.000000 corva_unit_converter-0.2.1/src/corva_unit_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 15:30:09.000000 corva_unit_converter-0.2.1/src/corva_unit_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:30:09.623384 corva_unit_converter-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_acoustic_slowness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_angle_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_angular_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_gas_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_gas_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_inverse_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_length_per_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_mass_flow_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_pressure_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_proportion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_revolution_per_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_strokes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_volume_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 15:30:06.000000 corva_unit_converter-0.2.1/tests/test_volume_flow_rate.py
```

### Comparing `corva-unit-converter-0.1.0/PKG-INFO` & `corva_unit_converter-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corva-unit-converter
-Version: 0.1.0
+Version: 0.2.1
 Summary: Unit converter for O&G(and other) units
 Home-page: https://github.com/corva-ai/corva-convert-units-py
 Author: Yuliya Klimushina
 Author-email: yuliya.klimushina@corva.ai
 License: MIT
 Keywords: corva,unit converter
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8, <4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # Units Converter
 
 Library for converting between quantities in different units(including units specific to O&G).
 
 This is a python version of the existing javascript app.
 Credit goes to the creator and contributors of the original version https://github.com/corva-ai/corva-convert-units,
```

### Comparing `corva-unit-converter-0.1.0/README.md` & `corva_unit_converter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/setup.py` & `corva_unit_converter-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/converter.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,18 @@
     "mass": definitions.mass.rule,
     "mass_flow_rate": definitions.mass_flow_rate.rule,
     "mpl": definitions.mpl.rule,
     "porosity": definitions.porosity.rule,
     "power": definitions.power.rule,
     "pressure": definitions.pressure.rule,
     "pressure_gradient": definitions.pressure_gradient.rule,
+    "proportion": definitions.proportion.rule,
     "revolution_per_volume": definitions.revolution_per_volume.rule,
     "speed": definitions.speed.rule,
+    "strokes_rate": definitions.strokes_rate.rule,
     "temperature": definitions.temperature.rule,
     "time": definitions.time.rule,
     "torque": definitions.torque.rule,
     "volume_concentration": definitions.volume_concentration.rule,
     "volume_flow_rate": definitions.volume_flow_rate.rule,
 }
```

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/__init__.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,18 @@
     mpl,
     parts_per,
     permiability,
     porosity,
     power,
     pressure,
     pressure_gradient,
+    proportion,
     revolution_per_volume,
     speed,
+    strokes_rate,
     temperature,
     time,
     torque,
     voltage,
     volume_concentration,
     volume_flow_rate,
 )
@@ -54,16 +56,18 @@
     "mpl",
     "parts_per",
     "permiability",
     "porosity",
     "power",
     "pressure",
     "pressure_gradient",
+    "proportion",
     "revolution_per_volume",
     "speed",
+    "strokes_rate",
     "temperature",
     "time",
     "torque",
     "voltage",
     "volume_concentration",
     "volume_flow_rate"
 ]
```

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/acoustic_slowness.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/acoustic_slowness.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/angle.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/angle.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
          "grad"
       ]
    },
    "arcmin": {
       "name": {
          "singular": "arcminute",
          "plural": "arcminutes",
-         "display": "acrmin"
+         "display": "arcmin"
       },
       "to_anchor": 1/60,
       "aliases": [
          "arcmin"
       ]
    },
    "arcsec": {
```

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/angle_per_length.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/angle_per_length.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/angular_velocity.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/angular_velocity.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
         "name": {
             "singular": "revolution per second",
             "plural": "revolutions per second",
             "display": "1/s"
         },
         "to_anchor": 60,
         "aliases": [
-            "1/s"
+            "1/s",
+            "Hz"
         ]
     },
     "rev/s": {
         "name": {
             "singular": "revolution per second",
             "plural": "revolutions per second",
             "display": "1/s"
```

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/area.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/area.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/current.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/current.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/density.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/density.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/digital.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/digital.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/energy.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/energy.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/force.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/force.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/gas_concentration.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/gas_concentration.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/gas_volume.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/gas_volume.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/inverse_pressure.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/inverse_pressure.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/length.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/length.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/length_per_angle.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/length_per_angle.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/mass.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/mass.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/mass_flow_rate.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/mass_flow_rate.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/mpl.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/mpl.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/parts_per.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/parts_per.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/permiability.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/permiability.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/porosity.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/porosity.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/power.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/power.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/pressure.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/pressure.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/pressure_gradient.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/pressure_gradient.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/revolution_per_volume.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/revolution_per_volume.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/speed.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/speed.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/temperature.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/temperature.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/time.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/time.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/torque.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/torque.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/voltage.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/voltage.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/volume_concentration.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/volume_concentration.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter/definitions/volume_flow_rate.py` & `corva_unit_converter-0.2.1/src/corva_unit_converter/definitions/volume_flow_rate.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter.egg-info/PKG-INFO` & `corva_unit_converter-0.2.1/src/corva_unit_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corva-unit-converter
-Version: 0.1.0
+Version: 0.2.1
 Summary: Unit converter for O&G(and other) units
 Home-page: https://github.com/corva-ai/corva-convert-units-py
 Author: Yuliya Klimushina
 Author-email: yuliya.klimushina@corva.ai
 License: MIT
 Keywords: corva,unit converter
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8, <4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # Units Converter
 
 Library for converting between quantities in different units(including units specific to O&G).
 
 This is a python version of the existing javascript app.
 Credit goes to the creator and contributors of the original version https://github.com/corva-ai/corva-convert-units,
```

### Comparing `corva-unit-converter-0.1.0/src/corva_unit_converter.egg-info/SOURCES.txt` & `corva_unit_converter-0.2.1/src/corva_unit_converter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 pyproject.toml
 setup.py
 src/version.py
 src/corva_unit_converter/__init__.py
 src/corva_unit_converter/constants.py
 src/corva_unit_converter/converter.py
@@ -31,16 +32,18 @@
 src/corva_unit_converter/definitions/mpl.py
 src/corva_unit_converter/definitions/parts_per.py
 src/corva_unit_converter/definitions/permiability.py
 src/corva_unit_converter/definitions/porosity.py
 src/corva_unit_converter/definitions/power.py
 src/corva_unit_converter/definitions/pressure.py
 src/corva_unit_converter/definitions/pressure_gradient.py
+src/corva_unit_converter/definitions/proportion.py
 src/corva_unit_converter/definitions/revolution_per_volume.py
 src/corva_unit_converter/definitions/speed.py
+src/corva_unit_converter/definitions/strokes_rate.py
 src/corva_unit_converter/definitions/temperature.py
 src/corva_unit_converter/definitions/time.py
 src/corva_unit_converter/definitions/torque.py
 src/corva_unit_converter/definitions/voltage.py
 src/corva_unit_converter/definitions/volume_concentration.py
 src/corva_unit_converter/definitions/volume_flow_rate.py
 tests/test_acoustic_slowness.py
@@ -58,14 +61,16 @@
 tests/test_mass.py
 tests/test_mass_flow_rate.py
 tests/test_mpl.py
 tests/test_porosity.py
 tests/test_power.py
 tests/test_pressure.py
 tests/test_pressure_gradient.py
+tests/test_proportion.py
 tests/test_revolution_per_volume.py
 tests/test_speed.py
+tests/test_strokes_rate.py
 tests/test_temperature.py
 tests/test_time.py
 tests/test_torque.py
 tests/test_volume_concentration.py
 tests/test_volume_flow_rate.py
```

### Comparing `corva-unit-converter-0.1.0/tests/test_angular_velocity.py` & `corva_unit_converter-0.2.1/tests/test_angular_velocity.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/tests/test_density.py` & `corva_unit_converter-0.2.1/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/tests/test_gas_concentration.py` & `corva_unit_converter-0.2.1/tests/test_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/tests/test_length.py` & `corva_unit_converter-0.2.1/tests/test_length.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/tests/test_pressure.py` & `corva_unit_converter-0.2.1/tests/test_pressure.py`

 * *Files identical despite different names*

### Comparing `corva-unit-converter-0.1.0/tests/test_speed.py` & `corva_unit_converter-0.2.1/tests/test_speed.py`

 * *Files identical despite different names*

