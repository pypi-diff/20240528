# Comparing `tmp/faebryk-2.0.0.tar.gz` & `tmp/faebryk-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faebryk-2.0.0.tar", last modified: Fri Oct 28 11:21:54 2022, max compression
+gzip compressed data, was "faebryk-3.0.0.tar", max compression
```

## Comparing `faebryk-2.0.0.tar` & `faebryk-3.0.0.tar`

### file list

```diff
@@ -1,61 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.780840 faebryk-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-28 11:21:45.000000 faebryk-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7932 2022-10-28 11:21:54.780840 faebryk-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-10-28 11:21:45.000000 faebryk-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-10-28 11:21:45.000000 faebryk-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-28 11:21:54.780840 faebryk-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.768840 faebryk-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.772840 faebryk-2.0.0/src/faebryk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.768840 faebryk-2.0.0/src/faebryk/exporters/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.772840 faebryk-2.0.0/src/faebryk/exporters/netlist/
--rw-r--r--   0 runner    (1001) docker     (121)     5961 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/exporters/netlist/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.772840 faebryk-2.0.0/src/faebryk/exporters/netlist/kicad/
--rw-r--r--   0 runner    (1001) docker     (121)     8845 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/exporters/netlist/kicad/netlist_kicad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/exporters/netlist/kicad/sexp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5533 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/exporters/netlist/netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.768840 faebryk-2.0.0/src/faebryk/exporters/project/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.772840 faebryk-2.0.0/src/faebryk/exporters/project/faebryk/
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/exporters/project/faebryk/project_faebryk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.768840 faebryk-2.0.0/src/faebryk/importers/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.768840 faebryk-2.0.0/src/faebryk/importers/netlist/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.772840 faebryk-2.0.0/src/faebryk/importers/netlist/kicad/
--rw-r--r--   0 runner    (1001) docker     (121)     4431 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/importers/netlist/kicad/netlist_kicad.py
--rw-r--r--   0 runner    (1001) docker     (121)     9478 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/importers/netlist/kicad/schematic_kicad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.772840 faebryk-2.0.0/src/faebryk/library/
--rw-r--r--   0 runner    (1001) docker     (121)     9363 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/kicad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.776840 faebryk-2.0.0/src/faebryk/library/library/
--rw-r--r--   0 runner    (1001) docker     (121)    15864 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/library/components.py
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/library/footprints.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/library/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/library/links.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/library/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.776840 faebryk-2.0.0/src/faebryk/library/trait_impl/
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/trait_impl/component.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/trait_impl/footprint.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/trait_impl/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/trait_impl/link.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/trait_impl/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.776840 faebryk-2.0.0/src/faebryk/library/traits/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/traits/component.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/traits/footprint.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/traits/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/traits/link.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/traits/parameter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/library/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.780840 faebryk-2.0.0/src/faebryk/libs/
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/libs/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/libs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.780840 faebryk-2.0.0/src/faebryk/libs/experiments/
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/libs/experiments/buildutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.780840 faebryk-2.0.0/src/faebryk/libs/kicad/
--rw-r--r--   0 runner    (1001) docker     (121)    13160 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/libs/kicad/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/libs/pycodegen.py
--rw-r--r--   0 runner    (1001) docker     (121)     4124 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/libs/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-10-28 11:21:45.000000 faebryk-2.0.0/src/faebryk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:21:54.772840 faebryk-2.0.0/src/faebryk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7932 2022-10-28 11:21:54.000000 faebryk-2.0.0/src/faebryk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-10-28 11:21:54.000000 faebryk-2.0.0/src/faebryk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 11:21:54.000000 faebryk-2.0.0/src/faebryk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-28 11:21:54.000000 faebryk-2.0.0/src/faebryk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-28 11:21:54.000000 faebryk-2.0.0/src/faebryk.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1064 2024-05-28 16:50:10.925615 faebryk-3.0.0/LICENSE
+-rw-r--r--   0        0        0     6826 2024-05-28 16:50:10.925615 faebryk-3.0.0/README.md
+-rw-r--r--   0        0        0     2680 2024-05-28 16:50:10.949616 faebryk-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    37259 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/core/core.py
+-rw-r--r--   0        0        0     1735 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/core/graph.py
+-rw-r--r--   0        0        0    13149 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/core/util.py
+-rw-r--r--   0        0        0     2560 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/esphome/esphome.py
+-rw-r--r--   0        0        0     5838 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/netlist/graph.py
+-rw-r--r--   0        0        0     9591 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/netlist/kicad/netlist_kicad.py
+-rw-r--r--   0        0        0     2228 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/netlist/netlist.py
+-rw-r--r--   0        0        0    24590 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/pcb/kicad/transformer.py
+-rw-r--r--   0        0        0      431 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/pcb/routing/README.md
+-rw-r--r--   0        0        0    21253 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/pcb/routing/grid.py
+-rw-r--r--   0        0        0     8720 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/pcb/routing/routing.py
+-rw-r--r--   0        0        0     6016 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/project/faebryk/project_faebryk.py
+-rw-r--r--   0        0        0    15232 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/exporters/visualize/graph.py
+-rw-r--r--   0        0        0     1329 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/importers/netlist/kicad/netlist_kicad.py
+-rw-r--r--   0        0        0     9552 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/importers/netlist/kicad/schematic_kicad.py
+-rw-r--r--   0        0        0      622 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/ANY.py
+-rw-r--r--   0        0        0     1524 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/BJT.py
+-rw-r--r--   0        0        0      675 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Battery.py
+-rw-r--r--   0        0        0     1817 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/ButtonCell.py
+-rw-r--r--   0        0        0      601 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/CD4011.py
+-rw-r--r--   0        0        0     1769 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Capacitor.py
+-rw-r--r--   0        0        0     1855 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Constant.py
+-rw-r--r--   0        0        0     1256 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/DIP.py
+-rw-r--r--   0        0        0      442 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/DifferentialPair.py
+-rw-r--r--   0        0        0     1555 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Diode.py
+-rw-r--r--   0        0        0    16398 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/ESP32.py
+-rw-r--r--   0        0        0     7341 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/ElectricLogic.py
+-rw-r--r--   0        0        0     1432 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/ElectricLogicGate.py
+-rw-r--r--   0        0        0     1055 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/ElectricLogicGates.py
+-rw-r--r--   0        0        0     2546 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/ElectricPower.py
+-rw-r--r--   0        0        0      368 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Electrical.py
+-rw-r--r--   0        0        0      421 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Ethernet.py
+-rw-r--r--   0        0        0     1286 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Fuse.py
+-rw-r--r--   0        0        0     1642 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/I2C.py
+-rw-r--r--   0        0        0      915 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/JTAG.py
+-rw-r--r--   0        0        0     1290 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/KicadFootprint.py
+-rw-r--r--   0        0        0     1962 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/LED.py
+-rw-r--r--   0        0        0      993 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/LEDIndicator.py
+-rw-r--r--   0        0        0      161 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Logic.py
+-rw-r--r--   0        0        0     2174 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/Logic74xx.py
+-rw-r--r--   0        0        0     2373 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/LogicGate.py
+-rw-r--r--   0        0        0      951 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/LogicGates.py
+-rw-r--r--   0        0        0     1388 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/LogicOps.py
+-rw-r--r--   0        0        0     2173 2024-05-28 16:50:10.949616 faebryk-3.0.0/src/faebryk/library/M24C08_FMN6TP.py
+-rw-r--r--   0        0        0     1165 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/MOSFET.py
+-rw-r--r--   0        0        0      545 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/MultiSPI.py
+-rw-r--r--   0        0        0     2321 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Net.py
+-rw-r--r--   0        0        0     1505 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Operation.py
+-rw-r--r--   0        0        0      568 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/PJ398SM.py
+-rw-r--r--   0        0        0     1244 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Potentiometer.py
+-rw-r--r--   0        0        0      161 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Power.py
+-rw-r--r--   0        0        0     2383 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/PowerSwitchMOSFET.py
+-rw-r--r--   0        0        0      995 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/PoweredLED.py
+-rw-r--r--   0        0        0     1984 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/QFN.py
+-rw-r--r--   0        0        0     1313 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/RJ45_Receptacle.py
+-rw-r--r--   0        0        0      651 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/RS232.py
+-rw-r--r--   0        0        0      389 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/RS485.py
+-rw-r--r--   0        0        0     2776 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Range.py
+-rw-r--r--   0        0        0     3565 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Resistor.py
+-rw-r--r--   0        0        0     1855 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/SMDTwoPin.py
+-rw-r--r--   0        0        0     1357 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/SOIC.py
+-rw-r--r--   0        0        0      492 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/SPI.py
+-rw-r--r--   0        0        0      684 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/SWD.py
+-rw-r--r--   0        0        0      668 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Sercom.py
+-rw-r--r--   0        0        0     1095 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Set.py
+-rw-r--r--   0        0        0     1024 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/Switch.py
+-rw-r--r--   0        0        0      469 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/TBD.py
+-rw-r--r--   0        0        0     1481 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/TI_CD4011BE.py
+-rw-r--r--   0        0        0      397 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/TVS.py
+-rw-r--r--   0        0        0      566 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/UART.py
+-rw-r--r--   0        0        0      968 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/UART_Base.py
+-rw-r--r--   0        0        0      845 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/USB2_0.py
+-rw-r--r--   0        0        0     1013 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/USB3.py
+-rw-r--r--   0        0        0     1026 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/USB_C.py
+-rw-r--r--   0        0        0     1557 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/USB_C_5V_PSU.py
+-rw-r--r--   0        0        0     1433 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/USB_C_PowerOnly.py
+-rw-r--r--   0        0        0     2505 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/USB_Type_C_Receptacle_24_pin.py
+-rw-r--r--   0        0        0     7809 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/_F.py
+-rw-r--r--   0        0        0      282 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_attach_to_footprint.py
+-rw-r--r--   0        0        0      713 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_attach_to_footprint_symmetrically.py
+-rw-r--r--   0        0        0      763 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_attach_to_footprint_via_pinmap.py
+-rw-r--r--   0        0        0      334 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_attach_via_pinmap.py
+-rw-r--r--   0        0        0      589 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_attach_via_pinmap_equal.py
+-rw-r--r--   0        0        0      653 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_attach_via_pinmap_pinlist.py
+-rw-r--r--   0        0        0      365 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_be_decoupled.py
+-rw-r--r--   0        0        0      935 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_be_decoupled_defined.py
+-rw-r--r--   0        0        0      371 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_be_surge_protected.py
+-rw-r--r--   0        0        0     1317 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_be_surge_protected_defined.py
+-rw-r--r--   0        0        0      433 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_bridge.py
+-rw-r--r--   0        0        0      400 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_bridge_defined.py
+-rw-r--r--   0        0        0      328 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_switch_power.py
+-rw-r--r--   0        0        0      839 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/can_switch_power_defined.py
+-rw-r--r--   0        0        0      274 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_capacitance.py
+-rw-r--r--   0        0        0      253 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_datasheet.py
+-rw-r--r--   0        0        0      361 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_datasheet_defined.py
+-rw-r--r--   0        0        0      438 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_defined_capacitance.py
+-rw-r--r--   0        0        0      879 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_defined_descriptive_properties.py
+-rw-r--r--   0        0        0      390 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_defined_footprint.py
+-rw-r--r--   0        0        0      331 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_defined_kicad_ref.py
+-rw-r--r--   0        0        0      429 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_defined_resistance.py
+-rw-r--r--   0        0        0      345 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_descriptive_properties.py
+-rw-r--r--   0        0        0      255 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_designator.py
+-rw-r--r--   0        0        0      350 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_designator_defined.py
+-rw-r--r--   0        0        0      258 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_designator_prefix.py
+-rw-r--r--   0        0        0      378 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_designator_prefix_defined.py
+-rw-r--r--   0        0        0      326 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_equal_pins.py
+-rw-r--r--   0        0        0      297 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_equal_pins_in_ifs.py
+-rw-r--r--   0        0        0      252 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_esphome_config.py
+-rw-r--r--   0        0        0      363 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_esphome_config_defined.py
+-rw-r--r--   0        0        0      270 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_footprint.py
+-rw-r--r--   0        0        0      759 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_footprint_impl.py
+-rw-r--r--   0        0        0      513 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_kicad_footprint.py
+-rw-r--r--   0        0        0      376 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_kicad_footprint_equal_ifs.py
+-rw-r--r--   0        0        0      388 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_kicad_footprint_equal_ifs_defined.py
+-rw-r--r--   0        0        0      521 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_kicad_manual_footprint.py
+-rw-r--r--   0        0        0      215 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_kicad_ref.py
+-rw-r--r--   0        0        0      253 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_overriden_name.py
+-rw-r--r--   0        0        0      369 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_overriden_name_defined.py
+-rw-r--r--   0        0        0      431 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_pcb_position.py
+-rw-r--r--   0        0        0      406 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_pcb_position_defined.py
+-rw-r--r--   0        0        0      272 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_resistance.py
+-rw-r--r--   0        0        0      267 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_simple_value_representation.py
+-rw-r--r--   0        0        0      865 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_simple_value_representation_based_on_param.py
+-rw-r--r--   0        0        0      449 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_simple_value_representation_defined.py
+-rw-r--r--   0        0        0      275 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_single_connection.py
+-rw-r--r--   0        0        0      341 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_single_connection_impl.py
+-rw-r--r--   0        0        0      332 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_single_electric_reference.py
+-rw-r--r--   0        0        0      502 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/has_single_electric_reference_defined.py
+-rw-r--r--   0        0        0      347 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/is_decoupled.py
+-rw-r--r--   0        0        0      461 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/is_decoupled_nodes.py
+-rw-r--r--   0        0        0      660 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/is_esphome_bus.py
+-rw-r--r--   0        0        0      345 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/is_esphome_bus_defined.py
+-rw-r--r--   0        0        0      287 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/is_representable_by_single_value.py
+-rw-r--r--   0        0        0      461 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/is_representable_by_single_value_defined.py
+-rw-r--r--   0        0        0      367 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/is_surge_protected.py
+-rw-r--r--   0        0        0      476 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/library/is_surge_protected_defined.py
+-rw-r--r--   0        0        0      777 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/algorithm.py
+-rw-r--r--   0        0        0     5156 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/app/designators.py
+-rw-r--r--   0        0        0     4817 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/app/erc.py
+-rw-r--r--   0        0        0     2274 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/app/kicad_netlist.py
+-rw-r--r--   0        0        0      950 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/app/parameters.py
+-rw-r--r--   0        0        0      190 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/exceptions.py
+-rw-r--r--   0        0        0     2148 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/experiments/buildutil.py
+-rw-r--r--   0        0        0     8646 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/experiments/pickers.py
+-rw-r--r--   0        0        0    13813 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/kicad/parser.py
+-rw-r--r--   0        0        0    15540 2024-05-28 16:50:10.953616 faebryk-3.0.0/src/faebryk/libs/kicad/pcb.py
+-rw-r--r--   0        0        0     2273 2024-05-28 16:50:10.957616 faebryk-3.0.0/src/faebryk/libs/kicad/sexp.py
+-rw-r--r--   0        0        0     1619 2024-05-28 16:50:10.957616 faebryk-3.0.0/src/faebryk/libs/logging.py
+-rw-r--r--   0        0        0     4718 2024-05-28 16:50:10.957616 faebryk-3.0.0/src/faebryk/libs/picker/lcsc.py
+-rw-r--r--   0        0        0     4309 2024-05-28 16:50:10.957616 faebryk-3.0.0/src/faebryk/libs/picker/picker.py
+-rw-r--r--   0        0        0     1980 2024-05-28 16:50:10.957616 faebryk-3.0.0/src/faebryk/libs/pycodegen.py
+-rw-r--r--   0        0        0      208 2024-05-28 16:50:10.957616 faebryk-3.0.0/src/faebryk/libs/units.py
+-rw-r--r--   0        0        0     8409 2024-05-28 16:50:10.957616 faebryk-3.0.0/src/faebryk/libs/util.py
+-rw-r--r--   0        0        0     8899 1970-01-01 00:00:00.000000 faebryk-3.0.0/PKG-INFO
```

### Comparing `faebryk-2.0.0/LICENSE` & `faebryk-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faebryk-2.0.0/PKG-INFO` & `faebryk-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,496 +1,557 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 6562  : 2.1.Name: faeb
-00000020: 7279 6b0a 5665 7273 696f 6e3a 2032 2e30  ryk.Version: 2.0
+00000020: 7279 6b0a 5665 7273 696f 6e3a 2033 2e30  ryk.Version: 3.0
 00000030: 2e30 0a53 756d 6d61 7279 3a20 4f70 656e  .0.Summary: Open
 00000040: 2d73 6f75 7263 6520 736f 6674 7761 7265  -source software
-00000050: 2d64 6566 696e 6564 2045 4441 0a41 7574  -defined EDA.Aut
-00000060: 686f 722d 656d 6169 6c3a 2069 6f61 6e6e  hor-email: ioann
-00000070: 6973 5f69 7465 6e67 203c 696f 616e 6e69  is_iteng <ioanni
-00000080: 7340 6974 656e 672e 6e6c 3e0a 4c69 6365  s@iteng.nl>.Lice
-00000090: 6e73 653a 204d 4954 204c 6963 656e 7365  nse: MIT License
-000000a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000000b0: 2020 436f 7079 7269 6768 7420 2863 2920    Copyright (c) 
-000000c0: 3230 3231 2066 6165 6272 796b 0a20 2020  2021 faebryk.   
-000000d0: 2020 2020 200a 2020 2020 2020 2020 5065       .        Pe
-000000e0: 726d 6973 7369 6f6e 2069 7320 6865 7265  rmission is here
-000000f0: 6279 2067 7261 6e74 6564 2c20 6672 6565  by granted, free
-00000100: 206f 6620 6368 6172 6765 2c20 746f 2061   of charge, to a
-00000110: 6e79 2070 6572 736f 6e20 6f62 7461 696e  ny person obtain
-00000120: 696e 6720 6120 636f 7079 0a20 2020 2020  ing a copy.     
-00000130: 2020 206f 6620 7468 6973 2073 6f66 7477     of this softw
-00000140: 6172 6520 616e 6420 6173 736f 6369 6174  are and associat
-00000150: 6564 2064 6f63 756d 656e 7461 7469 6f6e  ed documentation
-00000160: 2066 696c 6573 2028 7468 6520 2253 6f66   files (the "Sof
-00000170: 7477 6172 6522 292c 2074 6f20 6465 616c  tware"), to deal
-00000180: 0a20 2020 2020 2020 2069 6e20 7468 6520  .        in the 
-00000190: 536f 6674 7761 7265 2077 6974 686f 7574  Software without
-000001a0: 2072 6573 7472 6963 7469 6f6e 2c20 696e   restriction, in
-000001b0: 636c 7564 696e 6720 7769 7468 6f75 7420  cluding without 
-000001c0: 6c69 6d69 7461 7469 6f6e 2074 6865 2072  limitation the r
-000001d0: 6967 6874 730a 2020 2020 2020 2020 746f  ights.        to
-000001e0: 2075 7365 2c20 636f 7079 2c20 6d6f 6469   use, copy, modi
-000001f0: 6679 2c20 6d65 7267 652c 2070 7562 6c69  fy, merge, publi
-00000200: 7368 2c20 6469 7374 7269 6275 7465 2c20  sh, distribute, 
-00000210: 7375 626c 6963 656e 7365 2c20 616e 642f  sublicense, and/
-00000220: 6f72 2073 656c 6c0a 2020 2020 2020 2020  or sell.        
-00000230: 636f 7069 6573 206f 6620 7468 6520 536f  copies of the So
-00000240: 6674 7761 7265 2c20 616e 6420 746f 2070  ftware, and to p
-00000250: 6572 6d69 7420 7065 7273 6f6e 7320 746f  ermit persons to
-00000260: 2077 686f 6d20 7468 6520 536f 6674 7761   whom the Softwa
-00000270: 7265 2069 730a 2020 2020 2020 2020 6675  re is.        fu
-00000280: 726e 6973 6865 6420 746f 2064 6f20 736f  rnished to do so
-00000290: 2c20 7375 626a 6563 7420 746f 2074 6865  , subject to the
-000002a0: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6469   following condi
-000002b0: 7469 6f6e 733a 0a20 2020 2020 2020 200a  tions:.        .
-000002c0: 2020 2020 2020 2020 5468 6520 6162 6f76          The abov
-000002d0: 6520 636f 7079 7269 6768 7420 6e6f 7469  e copyright noti
-000002e0: 6365 2061 6e64 2074 6869 7320 7065 726d  ce and this perm
-000002f0: 6973 7369 6f6e 206e 6f74 6963 6520 7368  ission notice sh
-00000300: 616c 6c20 6265 2069 6e63 6c75 6465 6420  all be included 
-00000310: 696e 2061 6c6c 0a20 2020 2020 2020 2063  in all.        c
-00000320: 6f70 6965 7320 6f72 2073 7562 7374 616e  opies or substan
-00000330: 7469 616c 2070 6f72 7469 6f6e 7320 6f66  tial portions of
-00000340: 2074 6865 2053 6f66 7477 6172 652e 0a20   the Software.. 
-00000350: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000360: 5448 4520 534f 4654 5741 5245 2049 5320  THE SOFTWARE IS 
-00000370: 5052 4f56 4944 4544 2022 4153 2049 5322  PROVIDED "AS IS"
-00000380: 2c20 5749 5448 4f55 5420 5741 5252 414e  , WITHOUT WARRAN
-00000390: 5459 204f 4620 414e 5920 4b49 4e44 2c20  TY OF ANY KIND, 
-000003a0: 4558 5052 4553 5320 4f52 0a20 2020 2020  EXPRESS OR.     
-000003b0: 2020 2049 4d50 4c49 4544 2c20 494e 434c     IMPLIED, INCL
-000003c0: 5544 494e 4720 4255 5420 4e4f 5420 4c49  UDING BUT NOT LI
-000003d0: 4d49 5445 4420 544f 2054 4845 2057 4152  MITED TO THE WAR
-000003e0: 5241 4e54 4945 5320 4f46 204d 4552 4348  RANTIES OF MERCH
-000003f0: 414e 5441 4249 4c49 5459 2c0a 2020 2020  ANTABILITY,.    
-00000400: 2020 2020 4649 544e 4553 5320 464f 5220      FITNESS FOR 
-00000410: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
-00000420: 504f 5345 2041 4e44 204e 4f4e 494e 4652  POSE AND NONINFR
-00000430: 494e 4745 4d45 4e54 2e20 494e 204e 4f20  INGEMENT. IN NO 
-00000440: 4556 454e 5420 5348 414c 4c20 5448 450a  EVENT SHALL THE.
-00000450: 2020 2020 2020 2020 4155 5448 4f52 5320          AUTHORS 
-00000460: 4f52 2043 4f50 5952 4947 4854 2048 4f4c  OR COPYRIGHT HOL
-00000470: 4445 5253 2042 4520 4c49 4142 4c45 2046  DERS BE LIABLE F
-00000480: 4f52 2041 4e59 2043 4c41 494d 2c20 4441  OR ANY CLAIM, DA
-00000490: 4d41 4745 5320 4f52 204f 5448 4552 0a20  MAGES OR OTHER. 
-000004a0: 2020 2020 2020 204c 4941 4249 4c49 5459         LIABILITY
-000004b0: 2c20 5748 4554 4845 5220 494e 2041 4e20  , WHETHER IN AN 
-000004c0: 4143 5449 4f4e 204f 4620 434f 4e54 5241  ACTION OF CONTRA
-000004d0: 4354 2c20 544f 5254 204f 5220 4f54 4845  CT, TORT OR OTHE
-000004e0: 5257 4953 452c 2041 5249 5349 4e47 2046  RWISE, ARISING F
-000004f0: 524f 4d2c 0a20 2020 2020 2020 204f 5554  ROM,.        OUT
-00000500: 204f 4620 4f52 2049 4e20 434f 4e4e 4543   OF OR IN CONNEC
-00000510: 5449 4f4e 2057 4954 4820 5448 4520 534f  TION WITH THE SO
-00000520: 4654 5741 5245 204f 5220 5448 4520 5553  FTWARE OR THE US
-00000530: 4520 4f52 204f 5448 4552 2044 4541 4c49  E OR OTHER DEALI
-00000540: 4e47 5320 494e 2054 4845 0a20 2020 2020  NGS IN THE.     
-00000550: 2020 2053 4f46 5457 4152 452e 0a20 2020     SOFTWARE..   
-00000560: 2020 2020 200a 5072 6f6a 6563 742d 5552       .Project-UR
-00000570: 4c3a 2048 6f6d 6570 6167 652c 2068 7474  L: Homepage, htt
-00000580: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000590: 6661 6562 7279 6b2f 6661 6562 7279 6b20  faebryk/faebryk 
-000005a0: 0a50 726f 6a65 6374 2d55 524c 3a20 4275  .Project-URL: Bu
-000005b0: 6720 5472 6163 6b65 722c 2068 7474 7073  g Tracker, https
-000005c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
-000005d0: 6562 7279 6b2f 6661 6562 7279 6b2f 6973  ebryk/faebryk/is
-000005e0: 7375 6573 200a 436c 6173 7369 6669 6572  sues .Classifier
-000005f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000600: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000610: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
-00000620: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000630: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000640: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
-00000650: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000660: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000670: 7065 6e64 656e 740a 5265 7175 6972 6573  pendent.Requires
-00000680: 2d50 7974 686f 6e3a 203e 3d33 2e39 0a44  -Python: >=3.9.D
-00000690: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000006a0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000006b0: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
-000006c0: 696c 653a 204c 4943 454e 5345 0a0a 3c64  ile: LICENSE..<d
-000006d0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
-000006e0: 223e 0a0a 2320 6661 6562 7279 6b0a 0a23  ">..# faebryk..#
-000006f0: 2323 205c 5b66 cb88 c99b 62c9 b9c9 aa6b  ## \[f....b....k
-00000700: 5c5d 0a0a 3c61 2068 7265 663d 2268 7474  \]..<a href="htt
-00000710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000720: 6661 6562 7279 6b2f 6661 6562 7279 6b22  faebryk/faebryk"
-00000730: 3e0a 3c69 6d67 2068 6569 6768 743d 3330  >.<img height=30
-00000740: 3020 7769 6474 683d 3330 3020 7372 633d  0 width=300 src=
-00000750: 222e 2f66 6165 6272 796b 5f6c 6f67 6f2e  "./faebryk_logo.
-00000760: 706e 6722 2f3e 0a3c 2f61 3e0a 3c62 722f  png"/>.</a>.<br/
-00000770: 3e0a 0a4f 7065 6e2d 736f 7572 6365 2073  >..Open-source s
-00000780: 6f66 7477 6172 652d 6465 6669 6e65 6420  oftware-defined 
-00000790: 4544 4120 746f 6f6c 0a0a 5b21 5b56 6572  EDA tool..[![Ver
-000007a0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-000007b0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-000007c0: 6875 622f 762f 7461 672f 6661 6562 7279  hub/v/tag/faebry
-000007d0: 6b2f 6661 6562 7279 6b29 5d28 6874 7470  k/faebryk)](http
-000007e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-000007f0: 6165 6272 796b 2f66 6165 6272 796b 2f72  aebryk/faebryk/r
-00000800: 656c 6561 7365 732f 6c61 7465 7374 2920  eleases/latest) 
-00000810: 5b21 5b4c 6963 656e 7365 3a20 4d49 545d  [![License: MIT]
-00000820: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000830: 656c 6473 2e69 6f2f 6261 6467 652f 4c69  elds.io/badge/Li
-00000840: 6365 6e73 652d 4d49 542d 7965 6c6c 6f77  cense-MIT-yellow
-00000850: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000860: 6974 6875 622e 636f 6d2f 6661 6562 7279  ithub.com/faebry
-00000870: 6b2f 6661 6562 7279 6b2f 626c 6f62 2f6d  k/faebryk/blob/m
-00000880: 6169 6e2f 4c49 4345 4e53 4529 205b 215b  ain/LICENSE) [![
-00000890: 5075 6c6c 2072 6571 7565 7374 7320 6f70  Pull requests op
-000008a0: 656e 5d28 6874 7470 733a 2f2f 696d 672e  en](https://img.
-000008b0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-000008c0: 622f 6973 7375 6573 2d70 722f 6661 6562  b/issues-pr/faeb
-000008d0: 7279 6b2f 6661 6562 7279 6b29 5d28 6874  ryk/faebryk)](ht
-000008e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000008f0: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
-00000900: 2f70 756c 6c73 2920 5b21 5b49 7373 7565  /pulls) [![Issue
-00000910: 7320 6f70 656e 5d28 6874 7470 733a 2f2f  s open](https://
-00000920: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-00000930: 6974 6875 622f 6973 7375 6573 2f66 6165  ithub/issues/fae
-00000940: 6272 796b 2f66 6165 6272 796b 295d 2868  bryk/faebryk)](h
-00000950: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000960: 6d2f 6661 6562 7279 6b2f 6661 6562 7279  m/faebryk/faebry
-00000970: 6b2f 6973 7375 6573 290a 5b21 5b44 6973  k/issues).[![Dis
-00000980: 636f 7264 5d28 6874 7470 733a 2f2f 696d  cord](https://im
-00000990: 672e 7368 6965 6c64 732e 696f 2f64 6973  g.shields.io/dis
-000009a0: 636f 7264 2f39 3037 3637 3533 3333 3335  cord/90767533335
-000009b0: 3038 3039 3630 303f 6c61 6265 6c3d 4469  0809600?label=Di
-000009c0: 7363 6f72 6429 5d28 6874 7470 733a 2f2f  scord)](https://
-000009d0: 6469 7363 6f72 642e 636f 6d2f 6368 616e  discord.com/chan
-000009e0: 6e65 6c73 2f39 3037 3637 3533 3333 3335  nels/90767533335
-000009f0: 3038 3039 3630 3029 205b 215b 5079 5049  0809600) [![PyPI
-00000a00: 202d 2044 6f77 6e6c 6f61 6473 5d28 6874   - Downloads](ht
-00000a10: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000a20: 732e 696f 2f70 7970 692f 646d 2f66 6165  s.io/pypi/dm/fae
-00000a30: 6272 796b 3f6c 6162 656c 3d50 7950 6925  bryk?label=PyPi%
-00000a40: 3230 446f 776e 6c6f 6164 7329 5d28 6874  20Downloads)](ht
-00000a50: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000a60: 726f 6a65 6374 2f66 6165 6272 796b 2f29  roject/faebryk/)
-00000a70: 205b 215b 4769 7448 7562 2063 6f6d 6d69   [![GitHub commi
-00000a80: 7420 6163 7469 7669 7479 5d28 6874 7470  t activity](http
-00000a90: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000aa0: 696f 2f67 6974 6875 622f 636f 6d6d 6974  io/github/commit
-00000ab0: 2d61 6374 6976 6974 792f 6d2f 6661 6562  -activity/m/faeb
-00000ac0: 7279 6b2f 6661 6562 7279 6b29 5d28 6874  ryk/faebryk)](ht
-00000ad0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ae0: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
-00000af0: 2f63 6f6d 6d69 7473 2f6d 6169 6e29 0a0a  /commits/main)..
-00000b00: 5b21 5b43 6f64 6520 7374 796c 653a 2062  [![Code style: b
-00000b10: 6c61 636b 5d28 6874 7470 733a 2f2f 696d  lack](https://im
-00000b20: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000b30: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
-00000b40: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
-00000b50: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000b60: 622e 636f 6d2f 7073 662f 626c 6163 6b29  b.com/psf/black)
-00000b70: 0a0a 3c2f 6469 763e 0a0a 2d2d 2d0a 0a23  ..</div>..---..#
-00000b80: 2320 4162 6f75 740a 0a23 2323 2057 6861  # About..### Wha
-00000b90: 7420 5c5b 6973 2066 6165 6272 796b 5c5d  t \[is faebryk\]
-00000ba0: 0a0a 6661 6562 7279 6b20 6973 2061 6e20  ..faebryk is an 
-00000bb0: 6f70 656e 2d73 6f75 7263 6520 736f 6674  open-source soft
-00000bc0: 7761 7265 2d64 6566 696e 6564 2065 6c65  ware-defined ele
-00000bd0: 6374 726f 6e69 6320 6465 7369 676e 2061  ctronic design a
-00000be0: 7574 6f6d 6174 696f 6e20 2845 4441 2920  utomation (EDA) 
-00000bf0: 746f 6f6c 2e0a 5468 696e 6b20 6f66 2069  tool..Think of i
-00000c00: 7420 6c69 6b65 2074 6865 2065 766f 6c75  t like the evolu
-00000c10: 7469 6f6e 2066 726f 6d20 4544 4120 746f  tion from EDA to
-00000c20: 6f6c 7320 6c69 6b65 204b 6943 4144 2c20  ols like KiCAD, 
-00000c30: 416c 7469 756d 2c20 4561 676c 652e 2e2e  Altium, Eagle...
-00000c40: 0a69 6e20 7468 6520 7761 7920 7468 6f73  .in the way thos
-00000c50: 6520 7765 7265 2074 6865 206e 6578 7420  e were the next 
-00000c60: 7374 6570 2066 726f 6d20 6465 7369 676e  step from design
-00000c70: 696e 6720 656c 6563 7472 6f6e 6963 2063  ing electronic c
-00000c80: 6972 6375 6974 7320 6f6e 2070 6170 6572  ircuits on paper
-00000c90: 2e0a 5468 6520 6d61 696e 2069 6465 6120  ..The main idea 
-00000ca0: 6f66 2066 6165 6272 796b 2069 7320 746f  of faebryk is to
-00000cb0: 202a 2a64 6573 6372 6962 6520 796f 7572   **describe your
-00000cc0: 2070 726f 6475 6374 206f 6e20 7468 6520   product on the 
-00000cd0: 6869 6768 6573 7420 6c65 7665 6c2a 2a20  highest level** 
-00000ce0: 706f 7373 6962 6c65 2061 6e64 2074 6865  possible and the
-00000cf0: 6e20 6974 6572 6174 6976 656c 7920 7265  n iteratively re
-00000d00: 6669 6e69 6e67 2074 6865 2064 6573 6372  fining the descr
-00000d10: 6970 7469 6f6e 2074 6f20 6172 7269 7665  iption to arrive
-00000d20: 206f 6e20 6120 636f 6d70 6c65 7465 2061   on a complete a
-00000d30: 6e64 2064 6574 6169 6c65 6420 696d 706c  nd detailed impl
-00000d40: 656d 656e 7461 7469 6f6e 2e0a 496e 2063  ementation..In c
-00000d50: 6f6d 7061 7269 736f 6e20 746f 2063 6c61  omparison to cla
-00000d60: 7373 6963 2045 4441 2061 6e64 2064 6573  ssic EDA and des
-00000d70: 6967 6e20 746f 6f6c 7320 7768 6963 6820  ign tools which 
-00000d80: 7573 6520 4755 4973 2c20 6661 6562 7279  use GUIs, faebry
-00000d90: 6b20 7573 6573 2063 6f64 6520 2850 7974  k uses code (Pyt
-00000da0: 686f 6e29 2074 6f20 6372 6561 7465 2064  hon) to create d
-00000db0: 6573 6967 6e73 2e0a 5768 696c 6520 7468  esigns..While th
-00000dc0: 6520 6d61 696e 2066 6f63 7573 2069 7320  e main focus is 
-00000dd0: 6f6e 2074 6865 2045 4441 2070 6172 7420  on the EDA part 
-00000de0: 6375 7272 656e 746c 792c 2066 6165 6272  currently, faebr
-00000df0: 796b 2061 696d 7320 746f 2062 6563 6f6d  yk aims to becom
-00000e00: 6520 6120 686f 6c69 7374 6963 2073 7973  e a holistic sys
-00000e10: 7465 6d20 6465 7369 676e 2074 6f6f 6c2e  tem design tool.
-00000e20: 0a0a 2323 2320 486f 7720 5c5b 646f 6573  ..### How \[does
-00000e30: 2064 6573 6967 6e69 6e67 2077 6974 6820   designing with 
-00000e40: 6661 6562 7279 6b20 776f 726b 5c5d 0a0a  faebryk work\]..
-00000e50: 6661 6562 7279 6b20 6974 7365 6c66 2069  faebryk itself i
-00000e60: 7320 6a75 7374 2061 202a 2a70 7974 686f  s just a **pytho
-00000e70: 6e20 6c69 6272 6172 792a 2a20 7468 6174  n library** that
-00000e80: 2079 6f75 2069 6e63 6c75 6465 2069 6e20   you include in 
-00000e90: 796f 7572 2070 726f 6a65 6374 2e20 4974  your project. It
-00000ea0: 2069 7320 7072 6f76 6964 696e 6720 796f   is providing yo
-00000eb0: 7520 7769 7468 2061 6c6c 2074 6865 2074  u with all the t
-00000ec0: 6f6f 6c73 2074 6f20 6465 7363 7269 6265  ools to describe
-00000ed0: 2061 6e64 2064 6573 6967 6e20 796f 7572   and design your
-00000ee0: 2073 7973 7465 6d20 616e 6420 746f 2065   system and to e
-00000ef0: 7870 6f72 7420 7468 6174 2064 6573 6967  xport that desig
-00000f00: 6e20 696e 746f 2073 6f6d 6574 6869 6e67  n into something
-00000f10: 2075 7365 6675 6c20 6c69 6b65 2066 6f72   useful like for
-00000f20: 2065 7861 6d70 6c65 2061 206e 6574 6c69   example a netli
-00000f30: 7374 2c20 6120 6465 7669 6365 7472 6565  st, a devicetree
-00000f40: 2c20 6765 7262 6572 7320 6574 632c 2077  , gerbers etc, w
-00000f50: 6869 6368 2079 6f75 2074 6865 6e20 6361  hich you then ca
-00000f60: 6e20 7573 6520 696e 2074 6865 206e 6578  n use in the nex
-00000f70: 7420 7374 6570 7320 6f66 2079 6f75 7220  t steps of your 
-00000f80: 7072 6f6a 6563 742e 204b 6579 2063 6f6e  project. Key con
-00000f90: 6365 7074 7320 6f66 2066 6165 6272 796b  cepts of faebryk
-00000fa0: 2061 7265 2074 6865 2067 7261 7068 2c20   are the graph, 
-00000fb0: 696d 706f 7274 6572 732c 2065 7870 6f72  importers, expor
-00000fc0: 7465 7273 2c20 7468 6520 6c69 6272 6172  ters, the librar
-00000fd0: 7920 616e 6420 7468 6520 7573 6572 2061  y and the user a
-00000fe0: 7070 6c69 6361 7469 6f6e 2e0a 546f 2075  pplication..To u
-00000ff0: 6e64 6572 7374 616e 6420 686f 7720 746f  nderstand how to
-00001000: 2075 7365 2066 6165 6272 796b 2069 6e20   use faebryk in 
-00001010: 796f 7572 2070 726f 6a65 6374 2073 6565  your project see
-00001020: 205b 7573 696e 6720 6661 6562 7279 6b5d   [using faebryk]
-00001030: 2823 7573 696e 672d 6661 6562 7279 6b29  (#using-faebryk)
-00001040: 2e0a 0a23 2323 2057 686f 205c 5b69 7320  ...### Who \[is 
-00001050: 6661 6562 7279 6b5c 5d0a 0a66 6165 6272  faebryk\]..faebr
-00001060: 796b 2069 7320 6120 636f 6d6d 756e 6974  yk is a communit
-00001070: 7920 6472 6976 656e 2070 726f 6a65 6374  y driven project
-00001080: 2e20 5468 6174 206d 6561 6e73 2066 6165  . That means fae
-00001090: 6272 796b 2064 6f65 7320 6e6f 7420 6f6e  bryk does not on
-000010a0: 6c79 2063 6f6e 7369 7374 206f 7574 206f  ly consist out o
-000010b0: 6620 636f 7265 2064 6576 656c 6f70 6572  f core developer
-000010c0: 7320 6275 7420 616c 736f 2075 7365 7273  s but also users
-000010d0: 2c20 6578 7465 726e 616c 2063 6f6e 7472  , external contr
-000010e0: 6962 7574 6f72 732c 206d 6f64 6572 6174  ibutors, moderat
-000010f0: 6f72 7320 616e 6420 796f 7521 2049 7420  ors and you! It 
-00001100: 6973 2066 6f75 6e64 6564 2062 7920 6120  is founded by a 
-00001110: 6772 6f75 7020 6f66 2065 6d62 6564 6465  group of embedde
-00001120: 642c 2065 6c65 6374 7269 6361 6c2c 2070  d, electrical, p
-00001130: 726f 6475 6374 2064 6573 6967 6e20 616e  roduct design an
-00001140: 6420 736f 6674 7761 7265 2065 6e67 696e  d software engin
-00001150: 6565 7273 2077 6974 6820 6120 6c6f 7665  eers with a love
-00001160: 2066 6f72 206d 616b 696e 672e 0a0a 2323   for making...##
-00001170: 2320 5768 7920 5c5b 646f 2077 6520 6d61  # Why \[do we ma
-00001180: 6b65 2066 6165 6272 796b 5c5d 0a0a 5765  ke faebryk\]..We
-00001190: 206e 6f74 6963 6564 2074 6861 7420 7468   noticed that th
-000011a0: 6520 696e 6e6f 7661 7469 6f6e 7320 6f66  e innovations of
-000011b0: 2073 6f66 7477 6172 6520 656e 6769 6e65   software engine
-000011c0: 6572 696e 6720 7468 6174 206d 616b 6520  ering that make 
-000011d0: 6661 7374 2c20 7363 616c 6162 6c65 2c20  fast, scalable, 
-000011e0: 726f 6275 7374 2073 6f6c 7574 696f 6e73  robust solutions
-000011f0: 2070 6f73 7369 626c 6520 6861 7665 206e   possible have n
-00001200: 6f74 2066 6f75 6e64 2074 6865 6972 2077  ot found their w
-00001210: 6179 2069 6e74 6f20 6861 7264 7761 7265  ay into hardware
-00001220: 2064 6573 6967 6e2e 2046 7572 7468 6572   design. Further
-00001230: 6d6f 7265 2074 6865 7265 2069 7320 6120  more there is a 
-00001240: 6c6f 7420 6f66 2064 7570 6c69 6361 7465  lot of duplicate
-00001250: 2077 6f72 6b20 646f 6e65 2e20 5468 696e   work done. Thin
-00001260: 6b20 6f66 2064 6574 6572 6d69 6e69 6e67  k of determining
-00001270: 2074 6865 2070 696e 6f75 7420 6f66 2061   the pinout of a
-00001280: 2053 6f43 2061 6e64 2074 6865 6e20 6861   SoC and then ha
-00001290: 7669 6e67 2074 6f20 7472 616e 736c 6174  ving to translat
-000012a0: 6520 7468 6174 2065 7861 6374 2070 696e  e that exact pin
-000012b0: 6f75 7420 696e 746f 2073 6f66 7477 6172  out into softwar
-000012c0: 6520 6167 6169 6e20 6f72 2068 6176 696e  e again or havin
-000012d0: 6720 746f 2063 6f6e 7374 616e 746c 7920  g to constantly 
-000012e0: 6164 6170 7420 6465 7369 676e 7320 666f  adapt designs fo
-000012f0: 7220 7375 7070 6c79 2063 6861 696e 2069  r supply chain i
-00001300: 7373 7565 732e 0a41 6464 6974 696f 6e61  ssues..Additiona
-00001310: 6c6c 792c 2068 6172 6477 6172 6520 6465  lly, hardware de
-00001320: 7369 676e 2068 6173 2071 7569 7465 2061  sign has quite a
-00001330: 2062 6967 2062 6172 7269 6572 206f 6620   big barrier of 
-00001340: 656e 7472 7920 666f 7220 6d61 6b65 7273  entry for makers
-00001350: 2c20 6275 7420 7765 2064 6f6e 2774 2074  , but we don't t
-00001360: 6869 6e6b 2069 7420 6861 7320 746f 2e0a  hink it has to..
-00001370: 4375 7272 656e 746c 7920 6861 7264 7761  Currently hardwa
-00001380: 7265 2064 6573 6967 6e20 6973 2061 6c73  re design is als
-00001390: 6f20 7175 6974 6520 6c61 626f 7220 696e  o quite labor in
-000013a0: 7465 6e73 6976 6520 7769 7468 2076 6572  tensive with ver
-000013b0: 7920 6c69 7474 6c65 2061 7574 6f6d 6174  y little automat
-000013c0: 696f 6e2e 0a66 6165 6272 796b 2061 696d  ion..faebryk aim
-000013d0: 7320 746f 2074 6163 6b6c 6520 616c 6c20  s to tackle all 
-000013e0: 7468 6f73 6520 6973 7375 6573 2061 6e64  those issues and
-000013f0: 2061 6c73 6f20 6f70 656e 7320 7570 2073   also opens up s
-00001400: 6f6d 6520 6578 6369 7469 6e67 2070 6f73  ome exciting pos
-00001410: 7369 6269 6c69 7469 6573 2c20 7375 6368  sibilities, such
-00001420: 2061 7320 6265 6e65 6669 7469 6e67 2066   as benefiting f
-00001430: 726f 6d20 7468 6520 7665 7273 696f 6e20  rom the version 
-00001440: 6d61 6e61 6765 6d65 6e74 2061 6e64 2063  management and c
-00001450: 6f6c 6c61 626f 7261 7469 6f6e 2074 6f6f  ollaboration too
-00001460: 6c73 2074 6861 7420 6172 6520 7573 6564  ls that are used
-00001470: 2069 6e20 6d6f 6465 726e 2073 6f66 7477   in modern softw
-00001480: 6172 6520 6465 7665 6c6f 706d 656e 742e  are development.
-00001490: 0a0a 2323 2320 5768 656e 205c 5b69 7320  ..### When \[is 
-000014a0: 6661 6562 7279 6b20 6265 696e 6720 6465  faebryk being de
-000014b0: 7665 6c6f 7065 645c 5d0a 0a66 6165 6272  veloped\]..faebr
-000014c0: 796b 2069 7320 6265 696e 6720 636f 6e74  yk is being cont
-000014d0: 696e 756f 7573 6c79 2064 6576 656c 6f70  inuously develop
-000014e0: 6564 2e0a 5468 6520 636f 7265 2074 6561  ed..The core tea
-000014f0: 6d20 666f 6375 7365 7320 6f6e 2063 6f72  m focuses on cor
-00001500: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
-00001510: 616e 6420 6665 6174 7572 6573 206f 6620  and features of 
-00001520: 6661 6562 7279 6b2c 2061 7320 7765 6c6c  faebryk, as well
-00001530: 2061 7320 7468 6520 6765 6e65 7261 6c20   as the general 
-00001540: 6469 7265 6374 696f 6e20 6f66 2074 6865  direction of the
-00001550: 2070 726f 6a65 6374 2e0a 5468 6520 7374   project..The st
-00001560: 7265 6e67 7468 206f 6620 7468 6520 636f  rength of the co
-00001570: 6d6d 756e 6974 7920 6361 6e20 7265 616c  mmunity can real
-00001580: 6c79 2073 6869 6e65 2077 6974 6820 7468  ly shine with th
-00001590: 6520 6465 7665 6c6f 706d 656e 7420 6f66  e development of
-000015a0: 2069 6d70 6f72 7465 7273 2c20 6578 706f   importers, expo
-000015b0: 7274 6572 732c 206c 6962 7261 7269 6573  rters, libraries
-000015c0: 2c20 616e 6420 7072 6f6a 6563 7473 2c20  , and projects, 
-000015d0: 6275 7420 6576 6572 796f 6e65 2069 7320  but everyone is 
-000015e0: 7765 6c63 6f6d 6520 746f 205b 6865 6c70  welcome to [help
-000015f0: 5d28 2363 6f6d 6d75 6e69 7479 2d73 7570  ](#community-sup
-00001600: 706f 7274 2920 6f75 7420 7768 6572 6520  port) out where 
-00001610: 7468 6579 2063 616e 2e0a 0a23 2323 2057  they can...### W
-00001620: 6865 7265 205c 5b64 6f20 7765 2064 6576  here \[do we dev
-00001630: 656c 6f70 2066 6165 6272 796b 5c5d 0a0a  elop faebryk\]..
-00001640: 6661 6562 7279 6b20 6973 2062 6569 6e67  faebryk is being
-00001650: 2064 6576 656c 6f70 6564 2063 6f6d 706c   developed compl
-00001660: 6574 656c 7920 696e 2074 6865 206f 7065  etely in the ope
-00001670: 6e20 6f6e 2047 6974 6875 622e 0a41 6c6c  n on Github..All
-00001680: 2074 6865 2069 6e66 6f72 6d61 7469 6f6e   the information
-00001690: 2079 6f75 206e 6565 6420 746f 2073 7461   you need to sta
-000016a0: 7274 2075 7369 6e67 2061 6e64 2063 6f6e  rt using and con
-000016b0: 7472 6962 7574 696e 6720 746f 2066 6165  tributing to fae
-000016c0: 6272 796b 2077 696c 6c20 6265 2069 6e20  bryk will be in 
-000016d0: 6f72 206c 696e 6b65 6420 746f 2066 726f  or linked to fro
-000016e0: 6d20 5b74 6869 7320 7265 706f 7369 746f  m [this reposito
-000016f0: 7279 5d28 6874 7470 733a 2f2f 6769 7468  ry](https://gith
-00001700: 7562 2e63 6f6d 2f66 6165 6272 796b 2f66  ub.com/faebryk/f
-00001710: 6165 6272 796b 292e 0a49 6620 796f 7520  aebryk)..If you 
-00001720: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
-00001730: 6e73 2079 6f75 2063 616e 2061 736b 2074  ns you can ask t
-00001740: 6865 6d20 6f6e 206f 7572 205b 4469 7363  hem on our [Disc
-00001750: 6f72 645d 2868 7474 7073 3a2f 2f64 6973  ord](https://dis
-00001760: 636f 7264 2e67 672f 3935 6a59 7550 6d6e  cord.gg/95jYuPmn
-00001770: 5557 292e 0a46 6f72 2070 756c 6c20 7265  UW)..For pull re
-00001780: 7175 6573 7473 2061 6e64 2062 7567 2d72  quests and bug-r
-00001790: 6570 6f72 7473 2c20 7365 6520 6f75 7220  eports, see our 
-000017a0: 5b63 6f6e 7472 6962 7574 696e 6720 6775  [contributing gu
-000017b0: 6964 656c 696e 6573 5d28 646f 6373 2f43  idelines](docs/C
-000017c0: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
-000017d0: 0a0a 2d2d 2d0a 0a23 2320 5573 696e 6720  ..---..## Using 
-000017e0: 6661 6562 7279 6b0a 0a23 2323 2046 726f  faebryk..### Fro
-000017f0: 6d20 7069 700a 0a53 6574 7570 0a0a 6060  m pip..Setup..``
-00001800: 6062 6173 680a 3e20 2320 6f70 7469 6f6e  `bash.> # option
-00001810: 616c 3a20 7573 6520 7665 6e76 0a3e 2070  al: use venv.> p
-00001820: 7974 686f 6e20 2d6d 2076 656e 7620 7665  ython -m venv ve
-00001830: 6e76 0a3e 202e 2076 656e 762f 6269 6e2f  nv.> . venv/bin/
-00001840: 6163 7469 7661 7465 0a3e 0a3e 2070 6970  activate.>.> pip
-00001850: 2069 6e73 7461 6c6c 2066 6165 6272 796b   install faebryk
-00001860: 0a60 6060 0a0a 5275 6e6e 696e 6720 7361  .```..Running sa
-00001870: 6d70 6c65 730a 0a60 6060 6261 7368 0a3e  mples..```bash.>
-00001880: 206d 6b64 6972 206d 795f 6661 6562 7279   mkdir my_faebry
-00001890: 6b5f 7072 6f6a 6563 740a 3e20 6364 206d  k_project.> cd m
-000018a0: 795f 6661 6562 7279 6b5f 7072 6f6a 6563  y_faebryk_projec
-000018b0: 740a 3e20 2320 646f 776e 6c6f 6164 2061  t.> # download a
-000018c0: 2073 616d 706c 6520 6672 6f6d 2074 6865   sample from the
-000018d0: 2067 6974 6875 6220 7265 706f 2069 6e20   github repo in 
-000018e0: 2f73 616d 706c 6573 0a3e 2070 7974 686f  /samples.> pytho
-000018f0: 6e33 203c 7361 6d70 6c65 5f6e 616d 652e  n3 <sample_name.
-00001900: 7079 3e20 7c20 7461 696c 202d 6e31 203e  py> | tail -n1 >
-00001910: 206e 6574 6c69 7374 2e6e 6574 0a60 6060   netlist.net.```
-00001920: 0a0a 2323 2320 4672 6f6d 2073 6f75 7263  ..### From sourc
-00001930: 650a 0a53 6574 7570 0a0a 6060 6062 6173  e..Setup..```bas
-00001940: 680a 3e20 6769 7420 636c 6f6e 6520 6874  h.> git clone ht
-00001950: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001960: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
-00001970: 2e67 6974 0a3e 2063 6420 6661 6562 7279  .git.> cd faebry
-00001980: 6b0a 3e0a 3e20 2320 6372 6561 7465 2076  k.>.> # create v
-00001990: 656e 760a 3e20 7079 7468 6f6e 202d 6d20  env.> python -m 
-000019a0: 7665 6e76 2076 656e 760a 3e20 2e20 7665  venv venv.> . ve
-000019b0: 6e76 2f62 696e 2f61 6374 6976 6174 650a  nv/bin/activate.
-000019c0: 3e0a 3e20 2320 7265 7175 6972 6573 2070  >.> # requires p
-000019d0: 6970 2076 6572 7369 6f6e 203e 3d20 3231  ip version >= 21
-000019e0: 2e33 0a3e 2070 6970 2069 6e73 7461 6c6c  .3.> pip install
-000019f0: 202d 7220 7265 7175 6972 656d 656e 7473   -r requirements
-00001a00: 2e74 7874 0a3e 2070 6970 2069 6e73 7461  .txt.> pip insta
-00001a10: 6c6c 202d 2d65 6469 7461 626c 6520 2e0a  ll --editable ..
-00001a20: 6060 600a 0a52 756e 6e69 6e67 2073 616d  ```..Running sam
-00001a30: 706c 6573 0a0a 6060 6062 6173 680a 3e20  ples..```bash.> 
-00001a40: 2e2f 7361 6d70 6c65 732f 3c73 616d 706c  ./samples/<sampl
-00001a50: 655f 6e61 6d65 3e2e 7079 207c 2074 6169  e_name>.py | tai
-00001a60: 6c20 2d6e 3120 3e20 6e65 746c 6973 742e  l -n1 > netlist.
-00001a70: 6e65 740a 6060 600a 0a2d 2d2d 0a0a 2323  net.```..---..##
-00001a80: 2044 6576 656c 6f70 6d65 6e74 0a0a 2323   Development..##
-00001a90: 2320 5665 7273 696f 6e69 6e67 0a0a 6661  # Versioning..fa
-00001aa0: 6562 7279 6b20 7573 6573 205b 7365 6d61  ebryk uses [sema
-00001ab0: 6e74 6963 2076 6572 7369 6f6e 696e 675d  ntic versioning]
-00001ac0: 2868 7474 7073 3a2f 2f73 656d 7665 722e  (https://semver.
-00001ad0: 6f72 672f 2920 696e 2074 6865 205b 7265  org/) in the [re
-00001ae0: 6c65 6173 6573 5d28 6874 7470 733a 2f2f  leases](https://
-00001af0: 6769 7468 7562 2e63 6f6d 2f66 6165 6272  github.com/faebr
-00001b00: 796b 2f66 6165 6272 796b 2f72 656c 6561  yk/faebryk/relea
-00001b10: 7365 7329 2e0a 0a41 7320 6665 6162 7279  ses)...As feabry
-00001b20: 6b20 6973 2073 7469 6c6c 2069 6e20 7468  k is still in th
-00001b30: 6520 6561 726c 7920 7374 6167 6573 206f  e early stages o
-00001b40: 6620 6465 7665 6c6f 706d 656e 7420 6e65  f development ne
-00001b50: 7720 7265 6c65 6173 6573 2077 696c 6c20  w releases will 
-00001b60: 6861 7665 2061 206c 6f74 206f 6620 2862  have a lot of (b
-00001b70: 7265 616b 696e 6729 2063 6861 6e67 6573  reaking) changes
-00001b80: 2069 6e20 7468 656d 2e0a 4f75 7220 5b72   in them..Our [r
-00001b90: 6f61 646d 6170 5d28 2376 6572 7369 6f6e  oadmap](#version
-00001ba0: 696e 6729 2854 4f44 4f29 2077 696c 6c20  ing)(TODO) will 
-00001bb0: 7368 6f77 2079 6f75 2077 6865 7265 2074  show you where t
-00001bc0: 6865 2070 726f 6a65 6374 2069 7320 676f  he project is go
-00001bd0: 696e 6720 746f 2061 6e64 2077 6861 7420  ing to and what 
-00001be0: 796f 7520 6361 6e20 6578 7065 6374 2069  you can expect i
-00001bf0: 6e20 6675 7475 7265 2072 656c 6561 7365  n future release
-00001c00: 732e 0a0a 2323 2320 436f 6e74 7269 6275  s...### Contribu
-00001c10: 7469 6e67 0a0a 5365 6520 5b43 4f4e 5452  ting..See [CONTR
-00001c20: 4942 5554 494e 472e 6d64 5d28 646f 6373  IBUTING.md](docs
-00001c30: 2f43 4f4e 5452 4942 5554 494e 472e 6d64  /CONTRIBUTING.md
-00001c40: 290a 0a54 6f20 6765 7420 696e 7370 6972  )..To get inspir
-00001c50: 6174 696f 6e20 6f6e 2074 6869 6e67 7320  ation on things 
-00001c60: 746f 2077 6f72 6b20 6f6e 2063 6865 636b  to work on check
-00001c70: 206f 7574 2074 6865 2069 7373 7565 732e   out the issues.
-00001c80: 0a0a 2323 2323 2052 756e 6e69 6e67 2079  ..#### Running y
-00001c90: 6f75 7220 6f77 6e20 6578 7065 7269 6d65  our own experime
-00001ca0: 6e74 732f 4d61 6b69 6e67 2073 616d 706c  nts/Making sampl
-00001cb0: 6573 0a0a 4669 7273 7420 666f 6c6c 6f77  es..First follow
-00001cc0: 2074 6865 2073 7465 7073 2069 6e20 6765   the steps in ge
-00001cd0: 7420 7275 6e6e 696e 6720 6672 6f6d 2073  t running from s
-00001ce0: 6f75 7263 652e 0a54 6865 6e20 6164 6420  ource..Then add 
-00001cf0: 6120 6669 6c65 2069 6e20 7361 6d70 6c65  a file in sample
-00001d00: 732f 2028 796f 7520 6361 6e20 7573 6520  s/ (you can use 
-00001d10: 6f6e 6520 6f66 2074 6865 2073 616d 706c  one of the sampl
-00001d20: 6573 2061 7320 7465 6d70 6c61 7465 292e  es as template).
-00001d30: 0a43 616c 6c20 796f 7572 2066 696c 6520  .Call your file 
-00001d40: 7769 7468 2060 7079 7468 6f6e 3320 7361  with `python3 sa
-00001d50: 6d70 6c65 732f 3c79 6f75 7266 696c 653e  mples/<yourfile>
-00001d60: 2e70 7960 2e0a 0a23 2323 2320 5275 6e6e  .py`...#### Runn
-00001d70: 696e 6720 7465 7374 730a 0a52 756e 0a0a  ing tests..Run..
-00001d80: 6060 6062 6173 680a 3e20 7079 7465 7374  ```bash.> pytest
-00001d90: 2074 6573 740a 6060 600a 0a23 2320 436f   test.```..## Co
-00001da0: 6d6d 756e 6974 7920 5375 7070 6f72 740a  mmunity Support.
-00001db0: 0a43 6f6d 6d75 6e69 7479 2073 7570 706f  .Community suppo
-00001dc0: 7274 2069 7320 7072 6f76 6964 6564 2076  rt is provided v
-00001dd0: 6961 2044 6973 636f 7264 3b20 7365 6520  ia Discord; see 
-00001de0: 7468 6520 5265 736f 7572 6365 7320 6265  the Resources be
-00001df0: 6c6f 7720 666f 7220 6465 7461 696c 732e  low for details.
-00001e00: 0a0a 2323 2320 5265 736f 7572 6365 730a  ..### Resources.
-00001e10: 0a2d 2053 6f75 7263 6520 436f 6465 3a20  .- Source Code: 
-00001e20: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00001e30: 636f 6d2f 6661 6562 7279 6b2f 6661 6562  com/faebryk/faeb
-00001e40: 7279 6b3e 0a2d 2043 6861 743a 2052 6561  ryk>.- Chat: Rea
-00001e50: 6c2d 7469 6d65 2063 6861 7420 6861 7070  l-time chat happ
-00001e60: 656e 7320 696e 2066 6165 6272 796b 2773  ens in faebryk's
-00001e70: 2044 6973 636f 7264 2053 6572 7665 722e   Discord Server.
-00001e80: 2055 7365 2074 6869 7320 4469 7363 6f72   Use this Discor
-00001e90: 6420 5b49 6e76 6974 655d 2868 7474 7073  d [Invite](https
-00001ea0: 3a2f 2f64 6973 636f 7264 2e67 672f 3935  ://discord.gg/95
-00001eb0: 6a59 7550 6d6e 5557 2920 746f 2072 6567  jYuPmnUW) to reg
-00001ec0: 6973 7465 720a 2d20 4973 7375 6573 3a20  ister.- Issues: 
-00001ed0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00001ee0: 636f 6d2f 6661 6562 7279 6b2f 6661 6562  com/faebryk/faeb
-00001ef0: 7279 6b2f 6973 7375 6573 3e0a            ryk/issues>.
+00000050: 2d64 6566 696e 6564 2045 4441 0a48 6f6d  -defined EDA.Hom
+00000060: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000070: 6769 7468 7562 2e63 6f6d 2f66 6165 6272  github.com/faebr
+00000080: 796b 2f66 6165 6272 796b 0a4c 6963 656e  yk/faebryk.Licen
+00000090: 7365 3a20 4d49 540a 4175 7468 6f72 3a20  se: MIT.Author: 
+000000a0: 696f 616e 6e69 735f 6974 656e 670a 4175  ioannis_iteng.Au
+000000b0: 7468 6f72 2d65 6d61 696c 3a20 696f 616e  thor-email: ioan
+000000c0: 6e69 7340 6974 656e 672e 6e6c 0a52 6571  nis@iteng.nl.Req
+000000d0: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+000000e0: 332e 3132 2c3c 332e 3133 0a43 6c61 7373  3.12,<3.13.Class
+000000f0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+00000100: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000110: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
+00000120: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000130: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000140: 2049 6e64 6570 656e 6465 6e74 0a43 6c61   Independent.Cla
+00000150: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000160: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000170: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
+00000180: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000190: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001a0: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
+000001b0: 5265 7175 6972 6573 2d44 6973 743a 2062  Requires-Dist: b
+000001c0: 6c61 636b 2028 3e3d 3234 2e34 2e32 2c3c  lack (>=24.4.2,<
+000001d0: 3235 2e30 2e30 290a 5265 7175 6972 6573  25.0.0).Requires
+000001e0: 2d44 6973 743a 2065 6173 7965 6461 326b  -Dist: easyeda2k
+000001f0: 6963 6164 2028 3e3d 302e 362e 332c 3c30  icad (>=0.6.3,<0
+00000200: 2e37 2e30 290a 5265 7175 6972 6573 2d44  .7.0).Requires-D
+00000210: 6973 743a 206d 6174 706c 6f74 6c69 6220  ist: matplotlib 
+00000220: 283e 3d33 2e37 2e31 2c3c 342e 302e 3029  (>=3.7.1,<4.0.0)
+00000230: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000240: 6e65 7477 6f72 6b78 2028 3e3d 332e 312c  networkx (>=3.1,
+00000250: 3c34 2e30 290a 5265 7175 6972 6573 2d44  <4.0).Requires-D
+00000260: 6973 743a 206e 756d 7079 2028 3e3d 312e  ist: numpy (>=1.
+00000270: 3234 2e33 2c3c 322e 302e 3029 0a52 6571  24.3,<2.0.0).Req
+00000280: 7569 7265 732d 4469 7374 3a20 7079 6461  uires-Dist: pyda
+00000290: 6e74 6963 2028 3e3d 312e 352c 3c32 2e30  ntic (>=1.5,<2.0
+000002a0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+000002b0: 2073 6369 7079 2028 3e3d 312e 3131 2e31   scipy (>=1.11.1
+000002c0: 2c3c 322e 302e 3029 0a52 6571 7569 7265  ,<2.0.0).Require
+000002d0: 732d 4469 7374 3a20 7365 7870 6461 7461  s-Dist: sexpdata
+000002e0: 2028 3d3d 312e 302e 3029 0a52 6571 7569   (==1.0.0).Requi
+000002f0: 7265 732d 4469 7374 3a20 7368 6170 656c  res-Dist: shapel
+00000300: 7920 283e 3d32 2e30 2e31 2c3c 332e 302e  y (>=2.0.1,<3.0.
+00000310: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000320: 3a20 7479 7069 6e67 2d65 7874 656e 7369  : typing-extensi
+00000330: 6f6e 7320 283e 3d34 2e36 2e33 2c3c 352e  ons (>=4.6.3,<5.
+00000340: 302e 3029 0a50 726f 6a65 6374 2d55 524c  0.0).Project-URL
+00000350: 3a20 4275 6720 5472 6163 6b65 722c 2068  : Bug Tracker, h
+00000360: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000370: 6d2f 6661 6562 7279 6b2f 6661 6562 7279  m/faebryk/faebry
+00000380: 6b2f 6973 7375 6573 200a 5072 6f6a 6563  k/issues .Projec
+00000390: 742d 5552 4c3a 2052 6570 6f73 6974 6f72  t-URL: Repositor
+000003a0: 792c 2068 7474 7073 3a2f 2f67 6974 6875  y, https://githu
+000003b0: 622e 636f 6d2f 6661 6562 7279 6b2f 6661  b.com/faebryk/fa
+000003c0: 6562 7279 6b0a 4465 7363 7269 7074 696f  ebryk.Descriptio
+000003d0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+000003e0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
+000003f0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00000400: 7222 3e0a 0a23 2066 6165 6272 796b 0a0a  r">..# faebryk..
+00000410: 2323 2320 5c5b 66cb 88c9 9b62 c9b9 c9aa  ### \[f....b....
+00000420: 6b5c 5d0a 0a3c 6120 6872 6566 3d22 6874  k\]..<a href="ht
+00000430: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000440: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
+00000450: 223e 0a3c 696d 6720 6865 6967 6874 3d33  ">.<img height=3
+00000460: 3030 2077 6964 7468 3d33 3030 2073 7263  00 width=300 src
+00000470: 3d22 2e2f 6661 6562 7279 6b5f 6c6f 676f  ="./faebryk_logo
+00000480: 2e70 6e67 222f 3e0a 3c2f 613e 0a3c 6272  .png"/>.</a>.<br
+00000490: 2f3e 0a0a 4f70 656e 2d73 6f75 7263 6520  />..Open-source 
+000004a0: 736f 6674 7761 7265 2d64 6566 696e 6564  software-defined
+000004b0: 2045 4441 2074 6f6f 6c0a 0a5b 215b 5665   EDA tool..[![Ve
+000004c0: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
+000004d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+000004e0: 7468 7562 2f76 2f74 6167 2f66 6165 6272  thub/v/tag/faebr
+000004f0: 796b 2f66 6165 6272 796b 295d 2868 7474  yk/faebryk)](htt
+00000500: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000510: 6661 6562 7279 6b2f 6661 6562 7279 6b2f  faebryk/faebryk/
+00000520: 7265 6c65 6173 6573 2f6c 6174 6573 7429  releases/latest)
+00000530: 205b 215b 4c69 6365 6e73 653a 204d 4954   [![License: MIT
+00000540: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000550: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+00000560: 6963 656e 7365 2d4d 4954 2d79 656c 6c6f  icense-MIT-yello
+00000570: 772e 7376 6729 5d28 6874 7470 733a 2f2f  w.svg)](https://
+00000580: 6769 7468 7562 2e63 6f6d 2f66 6165 6272  github.com/faebr
+00000590: 796b 2f66 6165 6272 796b 2f62 6c6f 622f  yk/faebryk/blob/
+000005a0: 6d61 696e 2f4c 4943 454e 5345 2920 5b21  main/LICENSE) [!
+000005b0: 5b50 756c 6c20 7265 7175 6573 7473 206f  [Pull requests o
+000005c0: 7065 6e5d 2868 7474 7073 3a2f 2f69 6d67  pen](https://img
+000005d0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000005e0: 7562 2f69 7373 7565 732d 7072 2f66 6165  ub/issues-pr/fae
+000005f0: 6272 796b 2f66 6165 6272 796b 295d 2868  bryk/faebryk)](h
+00000600: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000610: 6d2f 6661 6562 7279 6b2f 6661 6562 7279  m/faebryk/faebry
+00000620: 6b2f 7075 6c6c 7329 205b 215b 4973 7375  k/pulls) [![Issu
+00000630: 6573 206f 7065 6e5d 2868 7474 7073 3a2f  es open](https:/
+00000640: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000650: 6769 7468 7562 2f69 7373 7565 732f 6661  github/issues/fa
+00000660: 6562 7279 6b2f 6661 6562 7279 6b29 5d28  ebryk/faebryk)](
+00000670: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000680: 6f6d 2f66 6165 6272 796b 2f66 6165 6272  om/faebryk/faebr
+00000690: 796b 2f69 7373 7565 7329 0a5b 215b 4469  yk/issues).[![Di
+000006a0: 7363 6f72 645d 2868 7474 7073 3a2f 2f69  scord](https://i
+000006b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6469  mg.shields.io/di
+000006c0: 7363 6f72 642f 3930 3736 3735 3333 3333  scord/9076753333
+000006d0: 3530 3830 3936 3030 3f6c 6162 656c 3d44  50809600?label=D
+000006e0: 6973 636f 7264 295d 2868 7474 7073 3a2f  iscord)](https:/
+000006f0: 2f64 6973 636f 7264 2e63 6f6d 2f63 6861  /discord.com/cha
+00000700: 6e6e 656c 732f 3930 3736 3735 3333 3333  nnels/9076753333
+00000710: 3530 3830 3936 3030 2920 5b21 5b50 7950  50809600) [![PyP
+00000720: 4920 2d20 446f 776e 6c6f 6164 735d 2868  I - Downloads](h
+00000730: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000740: 6473 2e69 6f2f 7079 7069 2f64 6d2f 6661  ds.io/pypi/dm/fa
+00000750: 6562 7279 6b3f 6c61 6265 6c3d 5079 5069  ebryk?label=PyPi
+00000760: 2532 3044 6f77 6e6c 6f61 6473 295d 2868  %20Downloads)](h
+00000770: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000780: 7072 6f6a 6563 742f 6661 6562 7279 6b2f  project/faebryk/
+00000790: 2920 5b21 5b47 6974 4875 6220 636f 6d6d  ) [![GitHub comm
+000007a0: 6974 2061 6374 6976 6974 795d 2868 7474  it activity](htt
+000007b0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000007c0: 2e69 6f2f 6769 7468 7562 2f63 6f6d 6d69  .io/github/commi
+000007d0: 742d 6163 7469 7669 7479 2f6d 2f66 6165  t-activity/m/fae
+000007e0: 6272 796b 2f66 6165 6272 796b 295d 2868  bryk/faebryk)](h
+000007f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000800: 6d2f 6661 6562 7279 6b2f 6661 6562 7279  m/faebryk/faebry
+00000810: 6b2f 636f 6d6d 6974 732f 6d61 696e 290a  k/commits/main).
+00000820: 0a5b 215b 436f 6465 2073 7479 6c65 3a20  .[![Code style: 
+00000830: 626c 6163 6b5d 2868 7474 7073 3a2f 2f69  black](https://i
+00000840: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000850: 6467 652f 636f 6465 2532 3073 7479 6c65  dge/code%20style
+00000860: 2d62 6c61 636b 2d30 3030 3030 302e 7376  -black-000000.sv
+00000870: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00000880: 7562 2e63 6f6d 2f70 7366 2f62 6c61 636b  ub.com/psf/black
+00000890: 290a 0a3c 2f64 6976 3e0a 0a49 6e20 7368  )..</div>..In sh
+000008a0: 6f72 7420 6661 6562 7279 6b20 6973 2061  ort faebryk is a
+000008b0: 2070 7974 686f 6e20 6c69 6272 6172 7920   python library 
+000008c0: 7468 6174 2061 6c6c 6f77 7320 796f 7520  that allows you 
+000008d0: 746f 2064 6573 6967 6e20 7265 6164 792d  to design ready-
+000008e0: 746f 2d6f 7264 6572 2065 6c65 6374 726f  to-order electro
+000008f0: 6e69 6373 2028 5043 4273 2c20 7363 6865  nics (PCBs, sche
+00000900: 6d61 7469 6373 2c20 6574 6329 2069 6e20  matics, etc) in 
+00000910: 636f 6465 2e20 4974 2061 696d 7320 746f  code. It aims to
+00000920: 2072 6564 7563 6520 7468 6520 656e 7472   reduce the entr
+00000930: 792d 6261 7272 6965 7220 666f 7220 6861  y-barrier for ha
+00000940: 7264 7761 7265 2064 6573 6967 6e20 6279  rdware design by
+00000950: 2062 7269 6467 696e 6720 7468 6520 6761   bridging the ga
+00000960: 7020 6265 7477 6565 6e20 736f 6674 7761  p between softwa
+00000970: 7265 2061 6e64 2068 6172 6477 6172 6520  re and hardware 
+00000980: 6465 7369 676e 2e0a 0a2d 2d2d 0a0a 0a23  design...---...#
+00000990: 2320 5573 696e 6720 6661 6562 7279 6b0a  # Using faebryk.
+000009a0: 0a60 6060 6261 7368 0a3e 2070 6970 2069  .```bash.> pip i
+000009b0: 6e73 7461 6c6c 2066 6165 6272 796b 0a60  nstall faebryk.`
+000009c0: 6060 0a0a 0a60 6060 7079 7468 6f6e 0a69  ``...```python.i
+000009d0: 6d70 6f72 7420 6661 6562 7279 6b2e 6c69  mport faebryk.li
+000009e0: 6272 6172 792e 5f46 2061 7320 460a 6672  brary._F as F.fr
+000009f0: 6f6d 2066 6165 6272 796b 2e63 6f72 652e  om faebryk.core.
+00000a00: 636f 7265 2069 6d70 6f72 7420 4d6f 6475  core import Modu
+00000a10: 6c65 0a66 726f 6d20 6661 6562 7279 6b2e  le.from faebryk.
+00000a20: 6c69 6273 2e65 7870 6572 696d 656e 7473  libs.experiments
+00000a30: 2e62 7569 6c64 7574 696c 2069 6d70 6f72  .buildutil impor
+00000a40: 7420 280a 2020 2020 7461 675f 616e 645f  t (.    tag_and_
+00000a50: 6578 706f 7274 5f6d 6f64 756c 655f 746f  export_module_to
+00000a60: 5f6e 6574 6c69 7374 0a29 0a0a 636c 6173  _netlist.)..clas
+00000a70: 7320 4170 7028 4d6f 6475 6c65 293a 200a  s App(Module): .
+00000a80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00000a90: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00000aa0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00000ab0: 5f5f 696e 6974 5f5f 2829 0a0a 2020 2020  __init__()..    
+00000ac0: 2020 2020 636c 6173 7320 5f4e 4f44 4553      class _NODES
+00000ad0: 284d 6f64 756c 652e 4e4f 4445 5328 2929  (Module.NODES())
+00000ae0: 3a0a 2020 2020 2020 2020 2020 2020 6c65  :.            le
+00000af0: 6420 3d20 462e 506f 7765 7265 644c 4544  d = F.PoweredLED
+00000b00: 2829 0a20 2020 2020 2020 2020 2020 2062  ().            b
+00000b10: 6174 7465 7279 203d 2046 2e42 6174 7465  attery = F.Batte
+00000b20: 7279 2829 0a0a 2020 2020 2020 2020 7365  ry()..        se
+00000b30: 6c66 2e4e 4f44 4573 203d 205f 4e4f 4445  lf.NODEs = _NODE
+00000b40: 5328 7365 6c66 290a 0a20 2020 2020 2020  S(self)..       
+00000b50: 2023 2043 6f6e 6e65 6374 696f 6e73 0a20   # Connections. 
+00000b60: 2020 2020 2020 2073 656c 662e 4e4f 4445         self.NODE
+00000b70: 732e 6c65 642e 4946 732e 706f 7765 722e  s.led.IFs.power.
+00000b80: 636f 6e6e 6563 7428 0a20 2020 2020 2020  connect(.       
+00000b90: 2020 2020 2073 656c 662e 4e4f 4445 732e       self.NODEs.
+00000ba0: 6261 7474 6572 792e 4946 732e 706f 7765  battery.IFs.powe
+00000bb0: 7229 0a0a 2020 2020 2020 2020 2320 5061  r)..        # Pa
+00000bc0: 7261 6d65 7472 697a 650a 2020 2020 2020  rametrize.      
+00000bd0: 2020 7365 6c66 2e4e 4f44 4573 2e6c 6564    self.NODEs.led
+00000be0: 2e4e 4f44 4573 2e6c 6564 2e50 4152 414d  .NODEs.led.PARAM
+00000bf0: 732e 636f 6c6f 722e 6d65 7267 6528 0a20  s.color.merge(. 
+00000c00: 2020 2020 2020 2020 2020 2046 2e4c 4544             F.LED
+00000c10: 2e43 6f6c 6f72 2e59 454c 4c4f 5729 0a20  .Color.YELLOW). 
+00000c20: 2020 2020 2020 2073 656c 662e 4e4f 4445         self.NODE
+00000c30: 732e 6c65 642e 4e4f 4445 732e 6c65 642e  s.led.NODEs.led.
+00000c40: 5041 5241 4d73 2e62 7269 6768 746e 6573  PARAMs.brightnes
+00000c50: 732e 6d65 7267 6528 0a20 2020 2020 2020  s.merge(.       
+00000c60: 2020 2020 2046 2e52 616e 6765 2e6c 6f77       F.Range.low
+00000c70: 6572 5f62 6f75 6e64 2833 3065 2d33 2929  er_bound(30e-3))
+00000c80: 0a0a 0a74 6167 5f61 6e64 5f65 7870 6f72  ...tag_and_expor
+00000c90: 745f 6d6f 6475 6c65 5f74 6f5f 6e65 746c  t_module_to_netl
+00000ca0: 6973 7428 4170 7028 2929 0a60 6060 0a0a  ist(App()).```..
+00000cb0: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000cc0: 6572 223e 0a0a 215b 5d28 646f 6373 2f69  er">..![](docs/i
+00000cd0: 6d67 2f64 656d 6f2e 6769 6629 0a0a 3c2f  mg/demo.gif)..</
+00000ce0: 6469 763e 0a0a 2d2d 2d0a 0a23 2320 4162  div>..---..## Ab
+00000cf0: 6f75 740a 0a23 2323 2057 6861 7420 5c5b  out..### What \[
+00000d00: 6973 2066 6165 6272 796b 5c5d 0a0a 6661  is faebryk\]..fa
+00000d10: 6562 7279 6b20 6973 2061 6e20 6f70 656e  ebryk is an open
+00000d20: 2d73 6f75 7263 6520 736f 6674 7761 7265  -source software
+00000d30: 2d64 6566 696e 6564 2065 6c65 6374 726f  -defined electro
+00000d40: 6e69 6320 6465 7369 676e 2061 7574 6f6d  nic design autom
+00000d50: 6174 696f 6e20 2845 4441 2920 746f 6f6c  ation (EDA) tool
+00000d60: 2e0a 5468 696e 6b20 6f66 2069 7420 6c69  ..Think of it li
+00000d70: 6b65 2074 6865 2065 766f 6c75 7469 6f6e  ke the evolution
+00000d80: 2066 726f 6d20 4544 4120 746f 6f6c 7320   from EDA tools 
+00000d90: 6c69 6b65 204b 6943 4144 2c20 416c 7469  like KiCAD, Alti
+00000da0: 756d 2c20 4561 676c 652e 2e2e 0a69 6e20  um, Eagle....in 
+00000db0: 7468 6520 7761 7920 7468 6f73 6520 7765  the way those we
+00000dc0: 7265 2074 6865 206e 6578 7420 7374 6570  re the next step
+00000dd0: 2066 726f 6d20 6465 7369 676e 696e 6720   from designing 
+00000de0: 656c 6563 7472 6f6e 6963 2063 6972 6375  electronic circu
+00000df0: 6974 7320 6f6e 2070 6170 6572 2e0a 5468  its on paper..Th
+00000e00: 6520 6d61 696e 2069 6465 6120 6f66 2066  e main idea of f
+00000e10: 6165 6272 796b 2069 7320 746f 202a 2a64  aebryk is to **d
+00000e20: 6573 6372 6962 6520 796f 7572 2070 726f  escribe your pro
+00000e30: 6475 6374 206f 6e20 7468 6520 6869 6768  duct on the high
+00000e40: 6573 7420 6c65 7665 6c2a 2a20 706f 7373  est level** poss
+00000e50: 6962 6c65 2061 6e64 2074 6865 6e20 6974  ible and then it
+00000e60: 6572 6174 6976 656c 7920 7265 6669 6e69  eratively refini
+00000e70: 6e67 2074 6865 2064 6573 6372 6970 7469  ng the descripti
+00000e80: 6f6e 2074 6f20 6172 7269 7665 206f 6e20  on to arrive on 
+00000e90: 6120 636f 6d70 6c65 7465 2061 6e64 2064  a complete and d
+00000ea0: 6574 6169 6c65 6420 696d 706c 656d 656e  etailed implemen
+00000eb0: 7461 7469 6f6e 2e0a 496e 2063 6f6d 7061  tation..In compa
+00000ec0: 7269 736f 6e20 746f 2063 6c61 7373 6963  rison to classic
+00000ed0: 2045 4441 2061 6e64 2064 6573 6967 6e20   EDA and design 
+00000ee0: 746f 6f6c 7320 7768 6963 6820 7573 6520  tools which use 
+00000ef0: 4755 4973 2c20 6661 6562 7279 6b20 7573  GUIs, faebryk us
+00000f00: 6573 2063 6f64 6520 2850 7974 686f 6e29  es code (Python)
+00000f10: 2074 6f20 6372 6561 7465 2064 6573 6967   to create desig
+00000f20: 6e73 2e0a 5768 696c 6520 7468 6520 6d61  ns..While the ma
+00000f30: 696e 2066 6f63 7573 2069 7320 6f6e 2074  in focus is on t
+00000f40: 6865 2045 4441 2070 6172 7420 6375 7272  he EDA part curr
+00000f50: 656e 746c 792c 2066 6165 6272 796b 2061  ently, faebryk a
+00000f60: 696d 7320 746f 2062 6563 6f6d 6520 6120  ims to become a 
+00000f70: 686f 6c69 7374 6963 2073 7973 7465 6d20  holistic system 
+00000f80: 6465 7369 676e 2074 6f6f 6c2e 0a0a 2323  design tool...##
+00000f90: 2320 486f 7720 5c5b 646f 6573 2064 6573  # How \[does des
+00000fa0: 6967 6e69 6e67 2077 6974 6820 6661 6562  igning with faeb
+00000fb0: 7279 6b20 776f 726b 5c5d 0a0a 6661 6562  ryk work\]..faeb
+00000fc0: 7279 6b20 6974 7365 6c66 2069 7320 6a75  ryk itself is ju
+00000fd0: 7374 2061 202a 2a70 7974 686f 6e20 6c69  st a **python li
+00000fe0: 6272 6172 792a 2a20 7468 6174 2079 6f75  brary** that you
+00000ff0: 2069 6e63 6c75 6465 2069 6e20 796f 7572   include in your
+00001000: 2070 726f 6a65 6374 2e20 4974 2069 7320   project. It is 
+00001010: 7072 6f76 6964 696e 6720 796f 7520 7769  providing you wi
+00001020: 7468 2061 6c6c 2074 6865 2074 6f6f 6c73  th all the tools
+00001030: 2074 6f20 6465 7363 7269 6265 2061 6e64   to describe and
+00001040: 2064 6573 6967 6e20 796f 7572 2073 7973   design your sys
+00001050: 7465 6d20 616e 6420 746f 2065 7870 6f72  tem and to expor
+00001060: 7420 7468 6174 2064 6573 6967 6e20 696e  t that design in
+00001070: 746f 2073 6f6d 6574 6869 6e67 2075 7365  to something use
+00001080: 6675 6c20 6c69 6b65 2066 6f72 2065 7861  ful like for exa
+00001090: 6d70 6c65 2061 206e 6574 6c69 7374 2c20  mple a netlist, 
+000010a0: 6120 6465 7669 6365 7472 6565 2c20 6765  a devicetree, ge
+000010b0: 7262 6572 7320 6574 632c 2077 6869 6368  rbers etc, which
+000010c0: 2079 6f75 2074 6865 6e20 6361 6e20 7573   you then can us
+000010d0: 6520 696e 2074 6865 206e 6578 7420 7374  e in the next st
+000010e0: 6570 7320 6f66 2079 6f75 7220 7072 6f6a  eps of your proj
+000010f0: 6563 742e 204b 6579 2063 6f6e 6365 7074  ect. Key concept
+00001100: 7320 6f66 2066 6165 6272 796b 2061 7265  s of faebryk are
+00001110: 2074 6865 2067 7261 7068 2c20 696d 706f   the graph, impo
+00001120: 7274 6572 732c 2065 7870 6f72 7465 7273  rters, exporters
+00001130: 2c20 7468 6520 6c69 6272 6172 7920 616e  , the library an
+00001140: 6420 7468 6520 7573 6572 2061 7070 6c69  d the user appli
+00001150: 6361 7469 6f6e 2e0a 546f 2075 6e64 6572  cation..To under
+00001160: 7374 616e 6420 686f 7720 746f 2075 7365  stand how to use
+00001170: 2066 6165 6272 796b 2069 6e20 796f 7572   faebryk in your
+00001180: 2070 726f 6a65 6374 2073 6565 205b 7573   project see [us
+00001190: 696e 6720 6661 6562 7279 6b5d 2823 7573  ing faebryk](#us
+000011a0: 696e 672d 6661 6562 7279 6b29 2e0a 0a23  ing-faebryk)...#
+000011b0: 2323 2057 686f 205c 5b69 7320 6661 6562  ## Who \[is faeb
+000011c0: 7279 6b5c 5d0a 0a66 6165 6272 796b 2069  ryk\]..faebryk i
+000011d0: 7320 6120 636f 6d6d 756e 6974 7920 6472  s a community dr
+000011e0: 6976 656e 2070 726f 6a65 6374 2e20 5468  iven project. Th
+000011f0: 6174 206d 6561 6e73 2066 6165 6272 796b  at means faebryk
+00001200: 2064 6f65 7320 6e6f 7420 6f6e 6c79 2063   does not only c
+00001210: 6f6e 7369 7374 206f 7574 206f 6620 636f  onsist out of co
+00001220: 7265 2064 6576 656c 6f70 6572 7320 6275  re developers bu
+00001230: 7420 616c 736f 2075 7365 7273 2c20 6578  t also users, ex
+00001240: 7465 726e 616c 2063 6f6e 7472 6962 7574  ternal contribut
+00001250: 6f72 732c 206d 6f64 6572 6174 6f72 7320  ors, moderators 
+00001260: 616e 6420 796f 7521 2049 7420 6973 2066  and you! It is f
+00001270: 6f75 6e64 6564 2062 7920 6120 6772 6f75  ounded by a grou
+00001280: 7020 6f66 2065 6d62 6564 6465 642c 2065  p of embedded, e
+00001290: 6c65 6374 7269 6361 6c2c 2070 726f 6475  lectrical, produ
+000012a0: 6374 2064 6573 6967 6e20 616e 6420 736f  ct design and so
+000012b0: 6674 7761 7265 2065 6e67 696e 6565 7273  ftware engineers
+000012c0: 2077 6974 6820 6120 6c6f 7665 2066 6f72   with a love for
+000012d0: 206d 616b 696e 672e 0a0a 2323 2320 5768   making...### Wh
+000012e0: 7920 5c5b 646f 2077 6520 6d61 6b65 2066  y \[do we make f
+000012f0: 6165 6272 796b 5c5d 0a0a 5765 206e 6f74  aebryk\]..We not
+00001300: 6963 6564 2074 6861 7420 7468 6520 696e  iced that the in
+00001310: 6e6f 7661 7469 6f6e 7320 6f66 2073 6f66  novations of sof
+00001320: 7477 6172 6520 656e 6769 6e65 6572 696e  tware engineerin
+00001330: 6720 7468 6174 206d 616b 6520 6661 7374  g that make fast
+00001340: 2c20 7363 616c 6162 6c65 2c20 726f 6275  , scalable, robu
+00001350: 7374 2073 6f6c 7574 696f 6e73 2070 6f73  st solutions pos
+00001360: 7369 626c 6520 6861 7665 206e 6f74 2066  sible have not f
+00001370: 6f75 6e64 2074 6865 6972 2077 6179 2069  ound their way i
+00001380: 6e74 6f20 6861 7264 7761 7265 2064 6573  nto hardware des
+00001390: 6967 6e2e 2046 7572 7468 6572 6d6f 7265  ign. Furthermore
+000013a0: 2074 6865 7265 2069 7320 6120 6c6f 7420   there is a lot 
+000013b0: 6f66 2064 7570 6c69 6361 7465 2077 6f72  of duplicate wor
+000013c0: 6b20 646f 6e65 2e20 5468 696e 6b20 6f66  k done. Think of
+000013d0: 2064 6574 6572 6d69 6e69 6e67 2074 6865   determining the
+000013e0: 2070 696e 6f75 7420 6f66 2061 2053 6f43   pinout of a SoC
+000013f0: 2061 6e64 2074 6865 6e20 6861 7669 6e67   and then having
+00001400: 2074 6f20 7472 616e 736c 6174 6520 7468   to translate th
+00001410: 6174 2065 7861 6374 2070 696e 6f75 7420  at exact pinout 
+00001420: 696e 746f 2073 6f66 7477 6172 6520 6167  into software ag
+00001430: 6169 6e20 6f72 2068 6176 696e 6720 746f  ain or having to
+00001440: 2063 6f6e 7374 616e 746c 7920 6164 6170   constantly adap
+00001450: 7420 6465 7369 676e 7320 666f 7220 7375  t designs for su
+00001460: 7070 6c79 2063 6861 696e 2069 7373 7565  pply chain issue
+00001470: 732e 0a41 6464 6974 696f 6e61 6c6c 792c  s..Additionally,
+00001480: 2068 6172 6477 6172 6520 6465 7369 676e   hardware design
+00001490: 2068 6173 2071 7569 7465 2061 2062 6967   has quite a big
+000014a0: 2062 6172 7269 6572 206f 6620 656e 7472   barrier of entr
+000014b0: 7920 666f 7220 6d61 6b65 7273 2c20 6275  y for makers, bu
+000014c0: 7420 7765 2064 6f6e 2774 2074 6869 6e6b  t we don't think
+000014d0: 2069 7420 6861 7320 746f 2e0a 4375 7272   it has to..Curr
+000014e0: 656e 746c 7920 6861 7264 7761 7265 2064  ently hardware d
+000014f0: 6573 6967 6e20 6973 2061 6c73 6f20 7175  esign is also qu
+00001500: 6974 6520 6c61 626f 7220 696e 7465 6e73  ite labor intens
+00001510: 6976 6520 7769 7468 2076 6572 7920 6c69  ive with very li
+00001520: 7474 6c65 2061 7574 6f6d 6174 696f 6e2e  ttle automation.
+00001530: 0a66 6165 6272 796b 2061 696d 7320 746f  .faebryk aims to
+00001540: 2074 6163 6b6c 6520 616c 6c20 7468 6f73   tackle all thos
+00001550: 6520 6973 7375 6573 2061 6e64 2061 6c73  e issues and als
+00001560: 6f20 6f70 656e 7320 7570 2073 6f6d 6520  o opens up some 
+00001570: 6578 6369 7469 6e67 2070 6f73 7369 6269  exciting possibi
+00001580: 6c69 7469 6573 2c20 7375 6368 2061 7320  lities, such as 
+00001590: 6265 6e65 6669 7469 6e67 2066 726f 6d20  benefiting from 
+000015a0: 7468 6520 7665 7273 696f 6e20 6d61 6e61  the version mana
+000015b0: 6765 6d65 6e74 2061 6e64 2063 6f6c 6c61  gement and colla
+000015c0: 626f 7261 7469 6f6e 2074 6f6f 6c73 2074  boration tools t
+000015d0: 6861 7420 6172 6520 7573 6564 2069 6e20  hat are used in 
+000015e0: 6d6f 6465 726e 2073 6f66 7477 6172 6520  modern software 
+000015f0: 6465 7665 6c6f 706d 656e 742e 0a0a 2323  development...##
+00001600: 2320 5768 656e 205c 5b69 7320 6661 6562  # When \[is faeb
+00001610: 7279 6b20 6265 696e 6720 6465 7665 6c6f  ryk being develo
+00001620: 7065 645c 5d0a 0a66 6165 6272 796b 2069  ped\]..faebryk i
+00001630: 7320 6265 696e 6720 636f 6e74 696e 756f  s being continuo
+00001640: 7573 6c79 2064 6576 656c 6f70 6564 2e0a  usly developed..
+00001650: 5468 6520 636f 7265 2074 6561 6d20 666f  The core team fo
+00001660: 6375 7365 7320 6f6e 2063 6f72 6520 6675  cuses on core fu
+00001670: 6e63 7469 6f6e 616c 6974 7920 616e 6420  nctionality and 
+00001680: 6665 6174 7572 6573 206f 6620 6661 6562  features of faeb
+00001690: 7279 6b2c 2061 7320 7765 6c6c 2061 7320  ryk, as well as 
+000016a0: 7468 6520 6765 6e65 7261 6c20 6469 7265  the general dire
+000016b0: 6374 696f 6e20 6f66 2074 6865 2070 726f  ction of the pro
+000016c0: 6a65 6374 2e0a 5468 6520 7374 7265 6e67  ject..The streng
+000016d0: 7468 206f 6620 7468 6520 636f 6d6d 756e  th of the commun
+000016e0: 6974 7920 6361 6e20 7265 616c 6c79 2073  ity can really s
+000016f0: 6869 6e65 2077 6974 6820 7468 6520 6465  hine with the de
+00001700: 7665 6c6f 706d 656e 7420 6f66 2069 6d70  velopment of imp
+00001710: 6f72 7465 7273 2c20 6578 706f 7274 6572  orters, exporter
+00001720: 732c 206c 6962 7261 7269 6573 2c20 616e  s, libraries, an
+00001730: 6420 7072 6f6a 6563 7473 2c20 6275 7420  d projects, but 
+00001740: 6576 6572 796f 6e65 2069 7320 7765 6c63  everyone is welc
+00001750: 6f6d 6520 746f 205b 6865 6c70 5d28 2363  ome to [help](#c
+00001760: 6f6d 6d75 6e69 7479 2d73 7570 706f 7274  ommunity-support
+00001770: 2920 6f75 7420 7768 6572 6520 7468 6579  ) out where they
+00001780: 2063 616e 2e0a 0a23 2323 2057 6865 7265   can...### Where
+00001790: 205c 5b64 6f20 7765 2064 6576 656c 6f70   \[do we develop
+000017a0: 2066 6165 6272 796b 5c5d 0a0a 6661 6562   faebryk\]..faeb
+000017b0: 7279 6b20 6973 2062 6569 6e67 2064 6576  ryk is being dev
+000017c0: 656c 6f70 6564 2063 6f6d 706c 6574 656c  eloped completel
+000017d0: 7920 696e 2074 6865 206f 7065 6e20 6f6e  y in the open on
+000017e0: 2047 6974 6875 622e 0a41 6c6c 2074 6865   Github..All the
+000017f0: 2069 6e66 6f72 6d61 7469 6f6e 2079 6f75   information you
+00001800: 206e 6565 6420 746f 2073 7461 7274 2075   need to start u
+00001810: 7369 6e67 2061 6e64 2063 6f6e 7472 6962  sing and contrib
+00001820: 7574 696e 6720 746f 2066 6165 6272 796b  uting to faebryk
+00001830: 2077 696c 6c20 6265 2069 6e20 6f72 206c   will be in or l
+00001840: 696e 6b65 6420 746f 2066 726f 6d20 5b74  inked to from [t
+00001850: 6869 7320 7265 706f 7369 746f 7279 5d28  his repository](
+00001860: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001870: 6f6d 2f66 6165 6272 796b 2f66 6165 6272  om/faebryk/faebr
+00001880: 796b 292e 0a49 6620 796f 7520 6861 7665  yk)..If you have
+00001890: 2061 6e79 2071 7565 7374 696f 6e73 2079   any questions y
+000018a0: 6f75 2063 616e 2061 736b 2074 6865 6d20  ou can ask them 
+000018b0: 6f6e 206f 7572 205b 4469 7363 6f72 645d  on our [Discord]
+000018c0: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
+000018d0: 2e67 672f 3935 6a59 7550 6d6e 5557 292e  .gg/95jYuPmnUW).
+000018e0: 0a46 6f72 2070 756c 6c20 7265 7175 6573  .For pull reques
+000018f0: 7473 2061 6e64 2062 7567 2d72 6570 6f72  ts and bug-repor
+00001900: 7473 2c20 7365 6520 6f75 7220 5b63 6f6e  ts, see our [con
+00001910: 7472 6962 7574 696e 6720 6775 6964 656c  tributing guidel
+00001920: 696e 6573 5d28 646f 6373 2f43 4f4e 5452  ines](docs/CONTR
+00001930: 4942 5554 494e 472e 6d64 292e 0a0a 2d2d  IBUTING.md)...--
+00001940: 2d0a 0a23 2320 4465 7665 6c6f 706d 656e  -..## Developmen
+00001950: 740a 0a23 2323 2049 6e73 7461 6c6c 696e  t..### Installin
+00001960: 6720 6672 6f6d 2073 6f75 7263 650a 5365  g from source.Se
+00001970: 7475 700a 0a60 6060 6261 7368 0a3e 2067  tup..```bash.> g
+00001980: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00001990: 2f67 6974 6875 622e 636f 6d2f 6661 6562  /github.com/faeb
+000019a0: 7279 6b2f 6661 6562 7279 6b2e 6769 740a  ryk/faebryk.git.
+000019b0: 3e20 6364 2066 6165 6272 796b 0a3e 0a3e  > cd faebryk.>.>
+000019c0: 2070 6f65 7472 7920 696e 7374 616c 6c0a   poetry install.
+000019d0: 6060 600a 0a52 756e 6e69 6e67 2065 7861  ```..Running exa
+000019e0: 6d70 6c65 730a 0a60 6060 6261 7368 0a3e  mples..```bash.>
+000019f0: 2070 6f65 7472 7920 7368 656c 6c0a 3e20   poetry shell.> 
+00001a00: 7079 7468 6f6e 202e 2f65 7861 6d70 6c65  python ./example
+00001a10: 732f 3c73 616d 706c 655f 6e61 6d65 3e2e  s/<sample_name>.
+00001a20: 7079 0a60 6060 0a0a 2323 2320 5665 7273  py.```..### Vers
+00001a30: 696f 6e69 6e67 0a0a 6661 6562 7279 6b20  ioning..faebryk 
+00001a40: 7573 6573 205b 7365 6d61 6e74 6963 2076  uses [semantic v
+00001a50: 6572 7369 6f6e 696e 675d 2868 7474 7073  ersioning](https
+00001a60: 3a2f 2f73 656d 7665 722e 6f72 672f 2920  ://semver.org/) 
+00001a70: 696e 2074 6865 205b 7265 6c65 6173 6573  in the [releases
+00001a80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001a90: 2e63 6f6d 2f66 6165 6272 796b 2f66 6165  .com/faebryk/fae
+00001aa0: 6272 796b 2f72 656c 6561 7365 7329 2e0a  bryk/releases)..
+00001ab0: 0a41 7320 6665 6162 7279 6b20 6973 2073  .As feabryk is s
+00001ac0: 7469 6c6c 2069 6e20 7468 6520 6561 726c  till in the earl
+00001ad0: 7920 7374 6167 6573 206f 6620 6465 7665  y stages of deve
+00001ae0: 6c6f 706d 656e 7420 6e65 7720 7265 6c65  lopment new rele
+00001af0: 6173 6573 2077 696c 6c20 6861 7665 2061  ases will have a
+00001b00: 206c 6f74 206f 6620 2862 7265 616b 696e   lot of (breakin
+00001b10: 6729 2063 6861 6e67 6573 2069 6e20 7468  g) changes in th
+00001b20: 656d 2e0a 4f75 7220 5b72 6f61 646d 6170  em..Our [roadmap
+00001b30: 5d28 2376 6572 7369 6f6e 696e 6729 2854  ](#versioning)(T
+00001b40: 4f44 4f29 2077 696c 6c20 7368 6f77 2079  ODO) will show y
+00001b50: 6f75 2077 6865 7265 2074 6865 2070 726f  ou where the pro
+00001b60: 6a65 6374 2069 7320 676f 696e 6720 746f  ject is going to
+00001b70: 2061 6e64 2077 6861 7420 796f 7520 6361   and what you ca
+00001b80: 6e20 6578 7065 6374 2069 6e20 6675 7475  n expect in futu
+00001b90: 7265 2072 656c 6561 7365 732e 0a0a 2323  re releases...##
+00001ba0: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00001bb0: 5365 6520 5b43 4f4e 5452 4942 5554 494e  See [CONTRIBUTIN
+00001bc0: 472e 6d64 5d28 646f 6373 2f43 4f4e 5452  G.md](docs/CONTR
+00001bd0: 4942 5554 494e 472e 6d64 290a 0a54 6f20  IBUTING.md)..To 
+00001be0: 6765 7420 696e 7370 6972 6174 696f 6e20  get inspiration 
+00001bf0: 6f6e 2074 6869 6e67 7320 746f 2077 6f72  on things to wor
+00001c00: 6b20 6f6e 2063 6865 636b 206f 7574 2074  k on check out t
+00001c10: 6865 2069 7373 7565 732e 0a0a 2323 2323  he issues...####
+00001c20: 2052 756e 6e69 6e67 2079 6f75 7220 6f77   Running your ow
+00001c30: 6e20 6578 7065 7269 6d65 6e74 732f 4d61  n experiments/Ma
+00001c40: 6b69 6e67 2073 616d 706c 6573 0a0a 4669  king samples..Fi
+00001c50: 7273 7420 666f 6c6c 6f77 2074 6865 2073  rst follow the s
+00001c60: 7465 7073 2069 6e20 6765 7420 7275 6e6e  teps in get runn
+00001c70: 696e 6720 6672 6f6d 2073 6f75 7263 652e  ing from source.
+00001c80: 0a54 6865 6e20 6164 6420 6120 6669 6c65  .Then add a file
+00001c90: 2069 6e20 6578 616d 706c 6573 2f20 2879   in examples/ (y
+00001ca0: 6f75 2063 616e 2075 7365 206f 6e65 206f  ou can use one o
+00001cb0: 6620 7468 6520 6578 616d 706c 6573 2061  f the examples a
+00001cc0: 7320 7465 6d70 6c61 7465 292e 0a43 616c  s template)..Cal
+00001cd0: 6c20 796f 7572 2066 696c 6520 7769 7468  l your file with
+00001ce0: 2060 7079 7468 6f6e 3320 6578 616d 706c   `python3 exampl
+00001cf0: 6573 2f3c 796f 7572 6669 6c65 3e2e 7079  es/<yourfile>.py
+00001d00: 602e 0a0a 2323 2323 2052 756e 6e69 6e67  `...#### Running
+00001d10: 2074 6573 7473 0a0a 5275 6e0a 0a60 6060   tests..Run..```
+00001d20: 6261 7368 0a3e 2070 7974 6573 7420 7465  bash.> pytest te
+00001d30: 7374 0a60 6060 0a0a 2323 2043 6f6d 6d75  st.```..## Commu
+00001d40: 6e69 7479 2053 7570 706f 7274 0a0a 436f  nity Support..Co
+00001d50: 6d6d 756e 6974 7920 7375 7070 6f72 7420  mmunity support 
+00001d60: 6973 2070 726f 7669 6465 6420 7669 6120  is provided via 
+00001d70: 4469 7363 6f72 643b 2073 6565 2074 6865  Discord; see the
+00001d80: 2052 6573 6f75 7263 6573 2062 656c 6f77   Resources below
+00001d90: 2066 6f72 2064 6574 6169 6c73 2e0a 0a23   for details...#
+00001da0: 2323 2052 6573 6f75 7263 6573 0a0a 2d20  ## Resources..- 
+00001db0: 536f 7572 6365 2043 6f64 653a 203c 6874  Source Code: <ht
+00001dc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001dd0: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
+00001de0: 3e0a 2d20 4368 6174 3a20 5265 616c 2d74  >.- Chat: Real-t
+00001df0: 696d 6520 6368 6174 2068 6170 7065 6e73  ime chat happens
+00001e00: 2069 6e20 6661 6562 7279 6b27 7320 4469   in faebryk's Di
+00001e10: 7363 6f72 6420 5365 7276 6572 2e20 5573  scord Server. Us
+00001e20: 6520 7468 6973 2044 6973 636f 7264 205b  e this Discord [
+00001e30: 496e 7669 7465 5d28 6874 7470 733a 2f2f  Invite](https://
+00001e40: 6469 7363 6f72 642e 6767 2f39 356a 5975  discord.gg/95jYu
+00001e50: 506d 6e55 5729 2074 6f20 7265 6769 7374  PmnUW) to regist
+00001e60: 6572 0a2d 2049 7373 7565 733a 203c 6874  er.- Issues: <ht
+00001e70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001e80: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
+00001e90: 2f69 7373 7565 733e 0a0a 4d49 5420 4c69  /issues>..MIT Li
+00001ea0: 6365 6e73 650a 0a43 6f70 7972 6967 6874  cense..Copyright
+00001eb0: 2028 6329 2032 3032 3120 6661 6562 7279   (c) 2021 faebry
+00001ec0: 6b0a 0a50 6572 6d69 7373 696f 6e20 6973  k..Permission is
+00001ed0: 2068 6572 6562 7920 6772 616e 7465 642c   hereby granted,
+00001ee0: 2066 7265 6520 6f66 2063 6861 7267 652c   free of charge,
+00001ef0: 2074 6f20 616e 7920 7065 7273 6f6e 206f   to any person o
+00001f00: 6274 6169 6e69 6e67 2061 2063 6f70 790a  btaining a copy.
+00001f10: 6f66 2074 6869 7320 736f 6674 7761 7265  of this software
+00001f20: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
+00001f30: 646f 6375 6d65 6e74 6174 696f 6e20 6669  documentation fi
+00001f40: 6c65 7320 2874 6865 2022 536f 6674 7761  les (the "Softwa
+00001f50: 7265 2229 2c20 746f 2064 6561 6c0a 696e  re"), to deal.in
+00001f60: 2074 6865 2053 6f66 7477 6172 6520 7769   the Software wi
+00001f70: 7468 6f75 7420 7265 7374 7269 6374 696f  thout restrictio
+00001f80: 6e2c 2069 6e63 6c75 6469 6e67 2077 6974  n, including wit
+00001f90: 686f 7574 206c 696d 6974 6174 696f 6e20  hout limitation 
+00001fa0: 7468 6520 7269 6768 7473 0a74 6f20 7573  the rights.to us
+00001fb0: 652c 2063 6f70 792c 206d 6f64 6966 792c  e, copy, modify,
+00001fc0: 206d 6572 6765 2c20 7075 626c 6973 682c   merge, publish,
+00001fd0: 2064 6973 7472 6962 7574 652c 2073 7562   distribute, sub
+00001fe0: 6c69 6365 6e73 652c 2061 6e64 2f6f 7220  license, and/or 
+00001ff0: 7365 6c6c 0a63 6f70 6965 7320 6f66 2074  sell.copies of t
+00002000: 6865 2053 6f66 7477 6172 652c 2061 6e64  he Software, and
+00002010: 2074 6f20 7065 726d 6974 2070 6572 736f   to permit perso
+00002020: 6e73 2074 6f20 7768 6f6d 2074 6865 2053  ns to whom the S
+00002030: 6f66 7477 6172 6520 6973 0a66 7572 6e69  oftware is.furni
+00002040: 7368 6564 2074 6f20 646f 2073 6f2c 2073  shed to do so, s
+00002050: 7562 6a65 6374 2074 6f20 7468 6520 666f  ubject to the fo
+00002060: 6c6c 6f77 696e 6720 636f 6e64 6974 696f  llowing conditio
+00002070: 6e73 3a0a 0a54 6865 2061 626f 7665 2063  ns:..The above c
+00002080: 6f70 7972 6967 6874 206e 6f74 6963 6520  opyright notice 
+00002090: 616e 6420 7468 6973 2070 6572 6d69 7373  and this permiss
+000020a0: 696f 6e20 6e6f 7469 6365 2073 6861 6c6c  ion notice shall
+000020b0: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
+000020c0: 616c 6c0a 636f 7069 6573 206f 7220 7375  all.copies or su
+000020d0: 6273 7461 6e74 6961 6c20 706f 7274 696f  bstantial portio
+000020e0: 6e73 206f 6620 7468 6520 536f 6674 7761  ns of the Softwa
+000020f0: 7265 2e0a 0a54 4845 2053 4f46 5457 4152  re...THE SOFTWAR
+00002100: 4520 4953 2050 524f 5649 4445 4420 2241  E IS PROVIDED "A
+00002110: 5320 4953 222c 2057 4954 484f 5554 2057  S IS", WITHOUT W
+00002120: 4152 5241 4e54 5920 4f46 2041 4e59 204b  ARRANTY OF ANY K
+00002130: 494e 442c 2045 5850 5245 5353 204f 520a  IND, EXPRESS OR.
+00002140: 494d 504c 4945 442c 2049 4e43 4c55 4449  IMPLIED, INCLUDI
+00002150: 4e47 2042 5554 204e 4f54 204c 494d 4954  NG BUT NOT LIMIT
+00002160: 4544 2054 4f20 5448 4520 5741 5252 414e  ED TO THE WARRAN
+00002170: 5449 4553 204f 4620 4d45 5243 4841 4e54  TIES OF MERCHANT
+00002180: 4142 494c 4954 592c 0a46 4954 4e45 5353  ABILITY,.FITNESS
+00002190: 2046 4f52 2041 2050 4152 5449 4355 4c41   FOR A PARTICULA
+000021a0: 5220 5055 5250 4f53 4520 414e 4420 4e4f  R PURPOSE AND NO
+000021b0: 4e49 4e46 5249 4e47 454d 454e 542e 2049  NINFRINGEMENT. I
+000021c0: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
+000021d0: 2054 4845 0a41 5554 484f 5253 204f 5220   THE.AUTHORS OR 
+000021e0: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
+000021f0: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
+00002200: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
+00002210: 4553 204f 5220 4f54 4845 520a 4c49 4142  ES OR OTHER.LIAB
+00002220: 494c 4954 592c 2057 4845 5448 4552 2049  ILITY, WHETHER I
+00002230: 4e20 414e 2041 4354 494f 4e20 4f46 2043  N AN ACTION OF C
+00002240: 4f4e 5452 4143 542c 2054 4f52 5420 4f52  ONTRACT, TORT OR
+00002250: 204f 5448 4552 5749 5345 2c20 4152 4953   OTHERWISE, ARIS
+00002260: 494e 4720 4652 4f4d 2c0a 4f55 5420 4f46  ING FROM,.OUT OF
+00002270: 204f 5220 494e 2043 4f4e 4e45 4354 494f   OR IN CONNECTIO
+00002280: 4e20 5749 5448 2054 4845 2053 4f46 5457  N WITH THE SOFTW
+00002290: 4152 4520 4f52 2054 4845 2055 5345 204f  ARE OR THE USE O
+000022a0: 5220 4f54 4845 5220 4445 414c 494e 4753  R OTHER DEALINGS
+000022b0: 2049 4e20 5448 450a 534f 4654 5741 5245   IN THE.SOFTWARE
+000022c0: 2e0a 0a                                  ...
```

### Comparing `faebryk-2.0.0/src/faebryk/exporters/netlist/kicad/netlist_kicad.py` & `faebryk-3.0.0/src/faebryk/exporters/netlist/kicad/netlist_kicad.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # This file is part of the faebryk project
 # SPDX-License-Identifier: MIT
 
 import itertools
 import logging
 
-logger = logging.getLogger("netlist")
+import faebryk.libs.kicad.sexp as sexp
+from faebryk.libs.util import duplicates
 
-import faebryk.exporters.netlist.kicad.sexp as sexp
+logger = logging.getLogger(__name__)
 
 
 # Generators ------------------------------------------------------------------
 def _gen_node(ref, pin):
     return {
         "node": {
             "ref": ref,
@@ -52,14 +53,18 @@
             "num": num,
             "name": name,
             "type": type,
         }
     }
 
 
+def _gen_property(name, value):
+    return {"property": {"name": name, "value": value}}
+
+
 def _gen_libpart(lib, part, description, docs, footprints, fields, pins):
     return {
         "libpart": {
             "lib": lib,
             "part": part,
             "description": description,
             "docs": docs,
@@ -70,38 +75,43 @@
     }
 
 
 def _gen_comp(
     ref,
     value,
     footprint,
+    properties,
     datasheet,
     fields,
     libsource_lib,
     libsource_part,
     libsource_description,
     sheetpath_names,
     sheetpath_tstamps,
     tstamp,
 ):
     return {
-        "comp": {
-            "ref": ref,
-            "value": value,
-            "footprint": footprint,
-            "datasheet": datasheet,
-            "fields": sexp.multi_key_dict(*fields),
-            "libsource": {
-                "lib": libsource_lib,
-                "part": libsource_part,
-                "description": libsource_description,
-            },
-            "sheetpath": {"names": sheetpath_names, "tstamps": sheetpath_tstamps},
-            "tstamp": tstamp,
-        }
+        "comp": sexp.multi_key_dict(
+            ("ref", ref),
+            ("value", value),
+            ("footprint", footprint),
+            ("datasheet", datasheet),
+            ("fields", [_gen_field(k, v) for k, v in fields]),
+            (
+                "libsource",
+                {
+                    "lib": libsource_lib,
+                    "part": libsource_part,
+                    "description": libsource_description,
+                },
+            ),
+            ("sheetpath", {"names": sheetpath_names, "tstamps": sheetpath_tstamps}),
+            ("tstamp", tstamp),
+            *[_gen_property(k, v) for k, v in properties.items()],
+        )
     }
 
 
 def _gen_comment(number, value):
     return {
         "comment": {
             "number": number,
@@ -125,15 +135,14 @@
     title_block_source,
     title_block_comments,
     components,
     libparts,
     libraries,
     nets,
 ):
-
     return _clean_none_and_empty(
         {
             "export": {
                 "version": version,
                 "design": {
                     "source": source,
                     "date": date,
@@ -234,79 +243,85 @@
         components=components,
         libparts=[],
         libraries=[],
         nets=nets,
     )
 
 
-def _defaulted_comp(ref, value, footprint, tstamp):
+def _defaulted_comp(ref, value, footprint, tstamp, fields, properties):
     return _gen_comp(
         ref=ref,
         value=value,
         footprint=footprint,
         datasheet=None,
-        fields=[],
+        fields=fields,
+        properties=properties,
         libsource_lib=None,
         libsource_part=None,
         libsource_description=None,
         sheetpath_names=None,
         sheetpath_tstamps=None,
         tstamp=tstamp,
     )
 
 
 # Test stuff ------------------------------------------------------------------
-def from_faebryk_t2_netlist(netlist):
+def from_faebryk_t2_netlist(t2_netlist):
     tstamp = itertools.count(1)
     net_code = itertools.count(1)
 
-    # t2_netlist = [(properties, vertices=[comp=(name, value, properties), pin)])]
+    netlist = t2_netlist["nets"]
+    pre_comps = t2_netlist["comps"]
+
+    # t2_netlist = {"nets":
+    #       [(properties, vertices=[comp=(name, value, properties), pin)])],
+    #   "comps": [comp]}
 
     # kicad_netlist = {
     #   comps:  [(ref, value, fp, tstamp)],
     #   nets:   [(code, name, [node=(ref, pin)])],
     # }
 
     # KiCAD Constraints:
     #   - name has to be unique
     #   - vertex properties has to contain footprint
     #   - tstamps can be generated (unique)
     #   - net_code can be generated (ascending, continuous)
     #   - components unique
 
-    def kicad_fp(fp):
-        # TODO implement
-        # This needs to translate a faebryk footprint to a kicad footprint
-        return fp
-
     def gen_net_name(net):
         import random
 
         return hex(random.randrange(1 << 31))
 
-    def unique(non_unique):
-        out_unique = []
-        for x in non_unique:
-            if x not in out_unique:
-                out_unique.append(x)
-        return out_unique
-
-    pre_comps = unique([vertex.component for net in netlist for vertex in net.vertices])
+    dupes = duplicates(pre_comps, lambda comp: comp.name)
+    assert not dupes, f"Duplicate comps {dupes}"
 
     comps = [
         _defaulted_comp(
             ref=comp.name,
             value=comp.value,
-            footprint=kicad_fp(comp.properties["footprint"]),
+            footprint=comp.properties["footprint"],
+            properties={k: v for k, v in comp.properties.items() if k != "footprint"},
             tstamp=next(tstamp),
+            fields=list(comp.properties.get("fields", [])),
         )
         for comp in sorted(pre_comps, key=lambda comp: comp.name)  # pre_comps
         # sort because tstamp determined by pos
     ]
 
+    # check if all vertices have a component in pre_comps
+    # not sure if this is necessary
+    pre_comp_names = {comp.name for comp in pre_comps}
+    for net in netlist:
+        for vertex in net.vertices:
+            assert (
+                vertex.component.name in pre_comp_names
+            ), f"Missing {vertex.component}"
+
     nets = [
         _gen_net(
             code=next(net_code),
             name=net.properties.get("name", gen_net_name(net)),
             nodes=[
                 _gen_node(
                     ref=vertex.component.name,
@@ -325,9 +340,11 @@
 
     out_netlist = _defaulted_netlist(
         components=comps,
         nets=nets,
     )
 
     sexp_netlist = sexp.gensexp(out_netlist)
+    assert isinstance(sexp_netlist, str)
+    sexp_netlist = sexp.prettify_sexp_string(sexp_netlist)
 
     return sexp_netlist
```

### Comparing `faebryk-2.0.0/src/faebryk/exporters/netlist/kicad/sexp.py` & `faebryk-3.0.0/src/faebryk/libs/kicad/sexp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,40 @@
 # This file is part of the faebryk project
 # SPDX-License-Identifier: MIT
 
 import logging
 import re
 
-logger = logging.getLogger("sexp")
+logger = logging.getLogger(__name__)
+
+
+def prettify_sexp_string(raw: str) -> str:
+    out = ""
+    level = 0
+    in_quotes = False
+    for c in raw:
+        if c == '"':
+            in_quotes = not in_quotes
+        if in_quotes:
+            ...
+        elif c == "\n":
+            continue
+        elif c == " " and out[-1] == " ":
+            continue
+        elif c == "(":
+            if level != 0:
+                out += "\n" + " " * 4 * level
+            level += 1
+        elif c == ")":
+            level -= 1
+        out += c
+
+    # if i > 0 no strip is a kicad bug(?) workaround
+    out = "\n".join(x.rstrip() if i > 0 else x for i, x in enumerate(out.splitlines()))
+    return out
 
 
 class multi_key_dict:
     def __init__(self, *args, **kwargs):
         self.dict_ = kwargs
         self.tuple_list = list(args)
 
@@ -43,15 +69,15 @@
 def gensexp(obj):
     # Basecase
     if obj is None:
         return None
 
     if not _expandable(obj):
         strrepr = str(obj)
-        if re.search("[ ()]", strrepr) is not None:
+        if re.search(r"[ ()\[\]]", strrepr) is not None:
             strrepr = f'"{strrepr}"'
         return strrepr
 
     # Recursion
     # TODO: key with empty val
 
     # Dict
```

### Comparing `faebryk-2.0.0/src/faebryk/exporters/project/faebryk/project_faebryk.py` & `faebryk-3.0.0/src/faebryk/exporters/project/faebryk/project_faebryk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 # This file is part of the faebryk project
 # SPDX-License-Identifier: MIT
 
 """
 """
 
+# TODO BROKEN
+
 import logging
 import re
 
 import black
-
 from faebryk.libs.pycodegen import sanitize_name
 from faebryk.libs.util import NotNone
 
-logger = logging.getLogger("export_faebryk")
+logger = logging.getLogger(__name__)
 
 template = """
 # This file was generated by faebryk netlist exporter
 {header}
 
 \"""
 {docstring}
 \"""
 from pathlib import Path
 import logging
 
-logger = logging.getLogger("main")
+logger = logging.getLogger(__name__)
 
 
 # function imports
 from faebryk.exporters.netlist.kicad.netlist_kicad import from_faebryk_t2_netlist
 from faebryk.exporters.netlist.netlist import make_t2_netlist_from_t1
 from faebryk.exporters.netlist.graph import (
     make_graph_from_components,
     make_t1_netlist_from_graph,
 )
 {function_imports}
 
 # library imports
-from faebryk.library.core import Component
-from faebryk.library.library.parameters import Constant
-from faebryk.library.library.interfaces import Electrical
-from faebryk.library.trait_impl.component import (
-    has_defined_footprint,
-    has_defined_footprint_pinmap,
-    has_defined_type_description,
-)
-from faebryk.library.kicad import (
-    has_defined_kicad_ref,
-    KicadFootprint,
-)
+#TODO
 {library_imports}
 
 from faebryk.libs.experiments.buildutil import export_graph, export_netlist
 
 def run_experiment():
 
     {definitions}
@@ -127,15 +117,14 @@
     #   properties,
     #   neighbors,
     #   value,
     components = t1_netlist
     project = template
 
     comp_names = {}
-    if_names = {}
 
     def comp_to_faebryk(component):
         def get_comp_name(component):
             if component["name"].startswith("COMP["):
                 class_name = NotNone(
                     re.search(r"\[(.*):.*\]", component["name"])
                 ).group(1)
@@ -217,17 +206,18 @@
         for pin, neighbors in comp["neighbors"].items():
             for neighbor in neighbors:
                 neighborcname = name_map[neighbor["vertex"]["name"]]
                 npin = neighbor["pin"]
                 if ((neighborcname, npin), (cname, pin)) in connections:
                     # don't add connection if symmetric connection already exists
                     continue
-                connections[
-                    ((cname, pin), (neighborcname, npin))
-                ] = f"{pinmap[pin][0].format(name=cname)}.connect({named_comps[neighborcname][1][npin][0].format(name=neighborcname)})"
+                connections[((cname, pin), (neighborcname, npin))] = (
+                    f"{pinmap[pin][0].format(name=cname)}.connect("
+                    f"{named_comps[neighborcname][1][npin][0].format(name=neighborcname)})"
+                )
 
     project = project.format(
         header="",
         docstring="",
         function_imports="",
         library_imports="",
         definitions="\n        ".join([c[0] for c in named_comps.values()]),
```

### Comparing `faebryk-2.0.0/src/faebryk/importers/netlist/kicad/schematic_kicad.py` & `faebryk-3.0.0/src/faebryk/importers/netlist/kicad/schematic_kicad.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     import pprint
 
     # pprint.pprint(schematic, indent=4)
     from pathlib import Path
 
     path = Path("./build/faebryk_sch")
     path.write_text(pprint.pformat(schematic, indent=4))
+
     # -------------------------------------------------------------------------
     def load_sheet_nets(sheet_schematic):
         def subname_to_tpl(subname: str):
             split = subname.split("_")
             return split[-2], split[-1]
 
         pins = {
@@ -188,16 +189,19 @@
                         pts[1][0], pts[0][0]
                     ):
                         continue
 
                     # a = (pts[1][1]-pts[0][1])/(pts[1][0]-pts[0][0]) #dy/dx
                     # matches = (lpt[0]-pts[0][0])*a + pts[0][1] == lpt[1]
                     # matches = (lpt[0]-pts[0][0])*a == lpt[1] - pts[0][1]
-                    # matches = (lpt[0]-pts[0][0])*(pts[1][1]-pts[0][1])/(pts[1][0]-pts[0][0]) == lpt[1] - pts[0][1]
-                    # matches = (lpt[0]-pts[0][0])*(pts[1][1]-pts[0][1]) == (lpt[1] - pts[0][1]) * (pts[1][0]-pts[0][0])
+                    # matches = (lpt[0]-pts[0][0])
+                    #   *(pts[1][1]-pts[0][1])/(pts[1][0]-pts[0][0])
+                    #   == lpt[1] - pts[0][1]
+                    # matches = (lpt[0]-pts[0][0])*(pts[1][1]-pts[0][1])
+                    #   == (lpt[1] - pts[0][1]) * (pts[1][0]-pts[0][0])
                     matches = round(
                         (lpt[0] - pts[0][0]) * (pts[1][1] - pts[0][1]), 2
                     ) == round((lpt[1] - pts[0][1]) * (pts[1][0] - pts[0][0]), 2)
 
                     if matches:
                         bridges.append([lpt, pts[0]])
                         # print("Found", label, "on", wire)
```

### Comparing `faebryk-2.0.0/src/faebryk/libs/algorithm.py` & `faebryk-3.0.0/src/faebryk/libs/algorithm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# This file is part of the faebryk project
+# SPDX-License-Identifier: MIT
+
+
 class ufds:
     parent_node = {}
     rank = {}
 
     def make_set(self, u):
         for i in u:
             self.parent_node[i] = i
```

### Comparing `faebryk-2.0.0/src/faebryk/libs/kicad/parser.py` & `faebryk-3.0.0/src/faebryk/libs/kicad/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+# This file is part of the faebryk project
+# SPDX-License-Identifier: MIT
+
 # import sexp_parser
 import logging
 
 from faebryk.libs.util import get_dict
-from sexpdata import SExpBase, loads
+from sexpdata import Symbol, loads
 
-logger = logging.getLogger("parse")
+logger = logging.getLogger(__name__)
 
 
 def _cleanparsed(parsed):
-    if isinstance(parsed, SExpBase):
+    if isinstance(parsed, Symbol):
         return parsed.value()
 
     if type(parsed) is list:
         return tuple(map(_cleanparsed, parsed))
 
     return parsed
 
@@ -47,16 +50,15 @@
 # -----------------------------------------------------------------------------
 
 
 def parse_symbol(obj):
     symbol = {}
     name = obj[1]
     symbol["name"] = name
-    # symbol["_raw"] = obj
-    # TODO reenable
+    symbol["_raw"] = obj
 
     def parse_pin_name(obj):
         pin_names = {}
         for i in obj[1:]:
             if type(i) is tuple and i[0] in ["offset"]:
                 pin_names[i[0]] = i[1]
             elif i == "hide":
@@ -99,66 +101,67 @@
                     "inverted_clock",
                     "low",
                     "clock_low",
                     "input_low",
                     "output_low",
                     "falling_edge_clock",
                 ]:
-                    pass
+                    ...
                 elif type(i) is tuple and i[0] in ["length"]:
-                    pass
+                    ...
                 elif type(i) is tuple and i[0] in "name":
                     pin["name"] = i[1]
                 elif type(i) is tuple and i[0] in "at":
                     pin[i[0]] = i[1:3]
                 elif type(i) is tuple and i[0] == "number":
                     key = i[1]
                     pin["number"] = i[1]
                 elif type(i) is tuple and i[0] == "alternate":
                     # no idea what this is
-                    pass
+                    ...
                 elif i == "hide":
                     pin["hide"] = True
                 else:
-                    assert (
-                        False
-                    ), f"encountered unexpected token [{i}] in pin [{obj}] symbol [{symbol}]"
+                    assert False, (
+                        f"encountered unexpected token"
+                        f"[{i}] in pin [{obj}] symbol [{symbol}]"
+                    )
 
             symbol_2["pins"][key] = pin
 
         for i in obj[2:]:
             if type(i) is tuple and i[0] in ["pin"]:
                 parse_pin(i)
             elif type(i) is tuple and i[0] in [
                 "rectangle",
                 "polyline",
                 "text",
                 "arc",
                 "circle",
             ]:
-                pass
+                ...
             else:
                 assert False, i
 
         symbol["symbols"][name] = symbol_2
 
     for i in obj[2:]:
         key = i[0]
         if key in ["pin_numbers", "in_bom", "on_board", "extends"]:
             symbol[key] = i[1]
         elif key == "pin_names":
             # parse_pin_name(i)
-            pass  # TODO test
+            ...  # TODO test
         elif key == "property":
             parse_property(i)
         elif key == "symbol":
             parse_symbol_2(i)
         elif key == "power":
             # symbol[key] = True
-            pass
+            ...
         else:
             assert (
                 False
             ), f"encountered unexpected token [{i}] in symbol [{name}]:[{obj}]"
 
     return symbol
 
@@ -192,28 +195,49 @@
         assert obj[0] == "components"
         components = {}
 
         def parse_comp(obj):
             assert obj[0] == "comp"
             comp = {}
 
+            def parse_property(obj):
+                if "properties" not in comp:
+                    comp["properties"] = {}
+
+                pkey = None
+                pval = None
+                for i in obj:
+                    key = i[0]
+                    val = i[1]
+
+                    if key == "name":
+                        pkey = val
+                    elif key == "value":
+                        pval = val
+
+                if pkey and pval:
+                    comp["properties"][pkey] = pval
+
+            # rest dont care tbh
+
             for i in obj[1:]:
                 key = i[0]
                 if key in [
                     "tstamp",
                     "tstamps",
                     "sheetpath",
-                    "property",
                     "libsource",
                     "datasheet",
                     "fields",
                 ]:
-                    pass
+                    ...
                 elif key in ["ref", "value", "footprint"]:
                     comp[key] = i[1]
+                elif key == "property":
+                    parse_property(i)
                 else:
                     assert False, f"encountered unexpected token [{i}] in comp"
 
             components[comp["ref"]] = comp
 
         for i in obj[1:]:
             key = i[0]
@@ -236,26 +260,26 @@
             def parse_node(obj):
                 assert obj[0] == "node"
                 node = {}
 
                 for i in obj[1:]:
                     key = i[0]
                     if key in ["pintype", "pinfunction"]:
-                        pass
+                        ...
                     elif key in ["ref", "pin"]:
                         node[key] = i[1]
                     else:
                         assert False, f"encountered unexpected token [{i}] in node"
 
                 net["nodes"].append(node)
 
             for i in obj[1:]:
                 key = i[0]
                 if key in ["code"]:
-                    pass
+                    ...
                 elif key in ["name"]:
                     net[key] = i[1]
                 elif key in ["node"]:
                     parse_node(i)
                 else:
                     assert False, f"encountered unexpected token [{i}] in net"
 
@@ -271,21 +295,21 @@
         netlist["nets"] = nets
 
     for i in obj[1:]:
         key = i[0]
         if key in ["version"]:
             netlist[key] = i[1]
         elif key in ["design"]:
-            pass
+            ...
         elif key in ["components"]:
             parse_components(i)
         elif key in ["nets"]:
             parse_nets(i)
         elif key in ["libparts", "libraries"]:
-            pass
+            ...
         else:
             assert False, f"encountered unexpected token [{i}] in netlist"
 
     return netlist
 
 
 def parse_schematic(obj, file_loader=None):
@@ -313,15 +337,15 @@
                     assert False, f"encountered unexpected token [{i}] in pts"
 
             wire["points"] = pts
 
         for i in obj[1:]:
             key = i[0]
             if key in ["stroke", "type", "color", "uuid"]:
-                pass
+                ...
             elif key in ["pts"]:
                 parse_pts(i)
             else:
                 assert False, f"encountered unexpected token [{i}] in wire"
 
         schematic["wires" if obj[0] == "wire" else "buses"].append(wire)
 
@@ -329,15 +353,15 @@
         assert obj[0] == "symbol"
         symbol = {}
         symbol["properties"] = {}
 
         for i in obj[1:]:
             key = i[0]
             if key in ["in_bom", "on_board", "fields_autoplaced", "uuid", "pin"]:
-                pass
+                ...
             elif key in ["at", "unit", "lib_id", "convert", "mirror"]:
                 symbol[key] = i[1:] if len(i[1:]) > 1 else i[1]
             elif key in ["property"]:
                 symbol["properties"][i[1]] = i[2]
             else:
                 assert False, f"encountered unexpected token [{i}] in symbol"
 
@@ -373,15 +397,15 @@
         def parse_at(obj):
             assert obj[0] in ["at"]
             label["coord"] = (obj[1], obj[2])
 
         for i in obj[2:]:
             key = i[0]
             if key in ["shape", "effects", "uuid", "fields_autoplaced", "property"]:
-                pass
+                ...
             elif key in ["at"]:
                 parse_at(i)
             else:
                 assert False, f"encountered unexpected token [{i}] in label"
 
         get_dict(schematic["labels"], label["name"], list).append(label)
 
@@ -399,26 +423,26 @@
             def parse_at(obj):
                 assert obj[0] in ["at"]
                 pin["coord"] = (obj[1], obj[1])
 
             for i in obj[2:]:
                 key = i[0] if type(i) is tuple else i
                 if key in ["input", "effects", "uuid"]:
-                    pass
+                    ...
                 elif key in ["at"]:
                     parse_at(i)
                 else:
                     assert False, f"encountered unexpected token [{i}] in sheet"
 
             sheet["pins"][pin["name"]] = pin
 
         for i in obj[1:]:
             key = i[0]
             if key in ["at", "size", "fields_autoplaced", "stroke", "fill", "uuid"]:
-                pass
+                ...
             elif key in ["property"]:
                 sheet["properties"][i[1]] = i[2]
             elif key in ["pin"]:
                 parse_pin(i)
             else:
                 assert False, f"encountered unexpected token [{i}] in sheet"
 
@@ -452,15 +476,15 @@
             "paper",
             "junction",
             "bus_entry",
             "symbol_instances",
             "sheet_instances",
             "text",
         ]:
-            pass
+            ...
         else:
             assert False, f"encountered unexpected token [{i}] in schematic"
 
     a = {}
     a.get("A")
 
     return schematic
```

### Comparing `faebryk-2.0.0/src/faebryk/libs/pycodegen.py` & `faebryk-3.0.0/src/faebryk/libs/pycodegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of the faebryk project
 # SPDX-License-Identifier: MIT
 
 import logging
 import re
 
-logger = logging.getLogger("pycodegen")
+logger = logging.getLogger(__name__)
 
 
 def sanitize_name(raw):
     sanitized = raw
     # braces
     sanitized = sanitized.replace("(", "")
     sanitized = sanitized.replace(")", "")
```

### Comparing `faebryk-2.0.0/src/faebryk.egg-info/PKG-INFO` & `faebryk-3.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,496 +1,427 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 6562  : 2.1.Name: faeb
-00000020: 7279 6b0a 5665 7273 696f 6e3a 2032 2e30  ryk.Version: 2.0
-00000030: 2e30 0a53 756d 6d61 7279 3a20 4f70 656e  .0.Summary: Open
-00000040: 2d73 6f75 7263 6520 736f 6674 7761 7265  -source software
-00000050: 2d64 6566 696e 6564 2045 4441 0a41 7574  -defined EDA.Aut
-00000060: 686f 722d 656d 6169 6c3a 2069 6f61 6e6e  hor-email: ioann
-00000070: 6973 5f69 7465 6e67 203c 696f 616e 6e69  is_iteng <ioanni
-00000080: 7340 6974 656e 672e 6e6c 3e0a 4c69 6365  s@iteng.nl>.Lice
-00000090: 6e73 653a 204d 4954 204c 6963 656e 7365  nse: MIT License
-000000a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000000b0: 2020 436f 7079 7269 6768 7420 2863 2920    Copyright (c) 
-000000c0: 3230 3231 2066 6165 6272 796b 0a20 2020  2021 faebryk.   
-000000d0: 2020 2020 200a 2020 2020 2020 2020 5065       .        Pe
-000000e0: 726d 6973 7369 6f6e 2069 7320 6865 7265  rmission is here
-000000f0: 6279 2067 7261 6e74 6564 2c20 6672 6565  by granted, free
-00000100: 206f 6620 6368 6172 6765 2c20 746f 2061   of charge, to a
-00000110: 6e79 2070 6572 736f 6e20 6f62 7461 696e  ny person obtain
-00000120: 696e 6720 6120 636f 7079 0a20 2020 2020  ing a copy.     
-00000130: 2020 206f 6620 7468 6973 2073 6f66 7477     of this softw
-00000140: 6172 6520 616e 6420 6173 736f 6369 6174  are and associat
-00000150: 6564 2064 6f63 756d 656e 7461 7469 6f6e  ed documentation
-00000160: 2066 696c 6573 2028 7468 6520 2253 6f66   files (the "Sof
-00000170: 7477 6172 6522 292c 2074 6f20 6465 616c  tware"), to deal
-00000180: 0a20 2020 2020 2020 2069 6e20 7468 6520  .        in the 
-00000190: 536f 6674 7761 7265 2077 6974 686f 7574  Software without
-000001a0: 2072 6573 7472 6963 7469 6f6e 2c20 696e   restriction, in
-000001b0: 636c 7564 696e 6720 7769 7468 6f75 7420  cluding without 
-000001c0: 6c69 6d69 7461 7469 6f6e 2074 6865 2072  limitation the r
-000001d0: 6967 6874 730a 2020 2020 2020 2020 746f  ights.        to
-000001e0: 2075 7365 2c20 636f 7079 2c20 6d6f 6469   use, copy, modi
-000001f0: 6679 2c20 6d65 7267 652c 2070 7562 6c69  fy, merge, publi
-00000200: 7368 2c20 6469 7374 7269 6275 7465 2c20  sh, distribute, 
-00000210: 7375 626c 6963 656e 7365 2c20 616e 642f  sublicense, and/
-00000220: 6f72 2073 656c 6c0a 2020 2020 2020 2020  or sell.        
-00000230: 636f 7069 6573 206f 6620 7468 6520 536f  copies of the So
-00000240: 6674 7761 7265 2c20 616e 6420 746f 2070  ftware, and to p
-00000250: 6572 6d69 7420 7065 7273 6f6e 7320 746f  ermit persons to
-00000260: 2077 686f 6d20 7468 6520 536f 6674 7761   whom the Softwa
-00000270: 7265 2069 730a 2020 2020 2020 2020 6675  re is.        fu
-00000280: 726e 6973 6865 6420 746f 2064 6f20 736f  rnished to do so
-00000290: 2c20 7375 626a 6563 7420 746f 2074 6865  , subject to the
-000002a0: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6469   following condi
-000002b0: 7469 6f6e 733a 0a20 2020 2020 2020 200a  tions:.        .
-000002c0: 2020 2020 2020 2020 5468 6520 6162 6f76          The abov
-000002d0: 6520 636f 7079 7269 6768 7420 6e6f 7469  e copyright noti
-000002e0: 6365 2061 6e64 2074 6869 7320 7065 726d  ce and this perm
-000002f0: 6973 7369 6f6e 206e 6f74 6963 6520 7368  ission notice sh
-00000300: 616c 6c20 6265 2069 6e63 6c75 6465 6420  all be included 
-00000310: 696e 2061 6c6c 0a20 2020 2020 2020 2063  in all.        c
-00000320: 6f70 6965 7320 6f72 2073 7562 7374 616e  opies or substan
-00000330: 7469 616c 2070 6f72 7469 6f6e 7320 6f66  tial portions of
-00000340: 2074 6865 2053 6f66 7477 6172 652e 0a20   the Software.. 
-00000350: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000360: 5448 4520 534f 4654 5741 5245 2049 5320  THE SOFTWARE IS 
-00000370: 5052 4f56 4944 4544 2022 4153 2049 5322  PROVIDED "AS IS"
-00000380: 2c20 5749 5448 4f55 5420 5741 5252 414e  , WITHOUT WARRAN
-00000390: 5459 204f 4620 414e 5920 4b49 4e44 2c20  TY OF ANY KIND, 
-000003a0: 4558 5052 4553 5320 4f52 0a20 2020 2020  EXPRESS OR.     
-000003b0: 2020 2049 4d50 4c49 4544 2c20 494e 434c     IMPLIED, INCL
-000003c0: 5544 494e 4720 4255 5420 4e4f 5420 4c49  UDING BUT NOT LI
-000003d0: 4d49 5445 4420 544f 2054 4845 2057 4152  MITED TO THE WAR
-000003e0: 5241 4e54 4945 5320 4f46 204d 4552 4348  RANTIES OF MERCH
-000003f0: 414e 5441 4249 4c49 5459 2c0a 2020 2020  ANTABILITY,.    
-00000400: 2020 2020 4649 544e 4553 5320 464f 5220      FITNESS FOR 
-00000410: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
-00000420: 504f 5345 2041 4e44 204e 4f4e 494e 4652  POSE AND NONINFR
-00000430: 494e 4745 4d45 4e54 2e20 494e 204e 4f20  INGEMENT. IN NO 
-00000440: 4556 454e 5420 5348 414c 4c20 5448 450a  EVENT SHALL THE.
-00000450: 2020 2020 2020 2020 4155 5448 4f52 5320          AUTHORS 
-00000460: 4f52 2043 4f50 5952 4947 4854 2048 4f4c  OR COPYRIGHT HOL
-00000470: 4445 5253 2042 4520 4c49 4142 4c45 2046  DERS BE LIABLE F
-00000480: 4f52 2041 4e59 2043 4c41 494d 2c20 4441  OR ANY CLAIM, DA
-00000490: 4d41 4745 5320 4f52 204f 5448 4552 0a20  MAGES OR OTHER. 
-000004a0: 2020 2020 2020 204c 4941 4249 4c49 5459         LIABILITY
-000004b0: 2c20 5748 4554 4845 5220 494e 2041 4e20  , WHETHER IN AN 
-000004c0: 4143 5449 4f4e 204f 4620 434f 4e54 5241  ACTION OF CONTRA
-000004d0: 4354 2c20 544f 5254 204f 5220 4f54 4845  CT, TORT OR OTHE
-000004e0: 5257 4953 452c 2041 5249 5349 4e47 2046  RWISE, ARISING F
-000004f0: 524f 4d2c 0a20 2020 2020 2020 204f 5554  ROM,.        OUT
-00000500: 204f 4620 4f52 2049 4e20 434f 4e4e 4543   OF OR IN CONNEC
-00000510: 5449 4f4e 2057 4954 4820 5448 4520 534f  TION WITH THE SO
-00000520: 4654 5741 5245 204f 5220 5448 4520 5553  FTWARE OR THE US
-00000530: 4520 4f52 204f 5448 4552 2044 4541 4c49  E OR OTHER DEALI
-00000540: 4e47 5320 494e 2054 4845 0a20 2020 2020  NGS IN THE.     
-00000550: 2020 2053 4f46 5457 4152 452e 0a20 2020     SOFTWARE..   
-00000560: 2020 2020 200a 5072 6f6a 6563 742d 5552       .Project-UR
-00000570: 4c3a 2048 6f6d 6570 6167 652c 2068 7474  L: Homepage, htt
-00000580: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000590: 6661 6562 7279 6b2f 6661 6562 7279 6b20  faebryk/faebryk 
-000005a0: 0a50 726f 6a65 6374 2d55 524c 3a20 4275  .Project-URL: Bu
-000005b0: 6720 5472 6163 6b65 722c 2068 7474 7073  g Tracker, https
-000005c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
-000005d0: 6562 7279 6b2f 6661 6562 7279 6b2f 6973  ebryk/faebryk/is
-000005e0: 7375 6573 200a 436c 6173 7369 6669 6572  sues .Classifier
-000005f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000600: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000610: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
-00000620: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000630: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000640: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
-00000650: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000660: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000670: 7065 6e64 656e 740a 5265 7175 6972 6573  pendent.Requires
-00000680: 2d50 7974 686f 6e3a 203e 3d33 2e39 0a44  -Python: >=3.9.D
-00000690: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000006a0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000006b0: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
-000006c0: 696c 653a 204c 4943 454e 5345 0a0a 3c64  ile: LICENSE..<d
-000006d0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
-000006e0: 223e 0a0a 2320 6661 6562 7279 6b0a 0a23  ">..# faebryk..#
-000006f0: 2323 205c 5b66 cb88 c99b 62c9 b9c9 aa6b  ## \[f....b....k
-00000700: 5c5d 0a0a 3c61 2068 7265 663d 2268 7474  \]..<a href="htt
-00000710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000720: 6661 6562 7279 6b2f 6661 6562 7279 6b22  faebryk/faebryk"
-00000730: 3e0a 3c69 6d67 2068 6569 6768 743d 3330  >.<img height=30
-00000740: 3020 7769 6474 683d 3330 3020 7372 633d  0 width=300 src=
-00000750: 222e 2f66 6165 6272 796b 5f6c 6f67 6f2e  "./faebryk_logo.
-00000760: 706e 6722 2f3e 0a3c 2f61 3e0a 3c62 722f  png"/>.</a>.<br/
-00000770: 3e0a 0a4f 7065 6e2d 736f 7572 6365 2073  >..Open-source s
-00000780: 6f66 7477 6172 652d 6465 6669 6e65 6420  oftware-defined 
-00000790: 4544 4120 746f 6f6c 0a0a 5b21 5b56 6572  EDA tool..[![Ver
-000007a0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-000007b0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-000007c0: 6875 622f 762f 7461 672f 6661 6562 7279  hub/v/tag/faebry
-000007d0: 6b2f 6661 6562 7279 6b29 5d28 6874 7470  k/faebryk)](http
-000007e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-000007f0: 6165 6272 796b 2f66 6165 6272 796b 2f72  aebryk/faebryk/r
-00000800: 656c 6561 7365 732f 6c61 7465 7374 2920  eleases/latest) 
-00000810: 5b21 5b4c 6963 656e 7365 3a20 4d49 545d  [![License: MIT]
-00000820: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000830: 656c 6473 2e69 6f2f 6261 6467 652f 4c69  elds.io/badge/Li
-00000840: 6365 6e73 652d 4d49 542d 7965 6c6c 6f77  cense-MIT-yellow
-00000850: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000860: 6974 6875 622e 636f 6d2f 6661 6562 7279  ithub.com/faebry
-00000870: 6b2f 6661 6562 7279 6b2f 626c 6f62 2f6d  k/faebryk/blob/m
-00000880: 6169 6e2f 4c49 4345 4e53 4529 205b 215b  ain/LICENSE) [![
-00000890: 5075 6c6c 2072 6571 7565 7374 7320 6f70  Pull requests op
-000008a0: 656e 5d28 6874 7470 733a 2f2f 696d 672e  en](https://img.
-000008b0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-000008c0: 622f 6973 7375 6573 2d70 722f 6661 6562  b/issues-pr/faeb
-000008d0: 7279 6b2f 6661 6562 7279 6b29 5d28 6874  ryk/faebryk)](ht
-000008e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000008f0: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
-00000900: 2f70 756c 6c73 2920 5b21 5b49 7373 7565  /pulls) [![Issue
-00000910: 7320 6f70 656e 5d28 6874 7470 733a 2f2f  s open](https://
-00000920: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-00000930: 6974 6875 622f 6973 7375 6573 2f66 6165  ithub/issues/fae
-00000940: 6272 796b 2f66 6165 6272 796b 295d 2868  bryk/faebryk)](h
-00000950: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000960: 6d2f 6661 6562 7279 6b2f 6661 6562 7279  m/faebryk/faebry
-00000970: 6b2f 6973 7375 6573 290a 5b21 5b44 6973  k/issues).[![Dis
-00000980: 636f 7264 5d28 6874 7470 733a 2f2f 696d  cord](https://im
-00000990: 672e 7368 6965 6c64 732e 696f 2f64 6973  g.shields.io/dis
-000009a0: 636f 7264 2f39 3037 3637 3533 3333 3335  cord/90767533335
-000009b0: 3038 3039 3630 303f 6c61 6265 6c3d 4469  0809600?label=Di
-000009c0: 7363 6f72 6429 5d28 6874 7470 733a 2f2f  scord)](https://
-000009d0: 6469 7363 6f72 642e 636f 6d2f 6368 616e  discord.com/chan
-000009e0: 6e65 6c73 2f39 3037 3637 3533 3333 3335  nels/90767533335
-000009f0: 3038 3039 3630 3029 205b 215b 5079 5049  0809600) [![PyPI
-00000a00: 202d 2044 6f77 6e6c 6f61 6473 5d28 6874   - Downloads](ht
-00000a10: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000a20: 732e 696f 2f70 7970 692f 646d 2f66 6165  s.io/pypi/dm/fae
-00000a30: 6272 796b 3f6c 6162 656c 3d50 7950 6925  bryk?label=PyPi%
-00000a40: 3230 446f 776e 6c6f 6164 7329 5d28 6874  20Downloads)](ht
-00000a50: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000a60: 726f 6a65 6374 2f66 6165 6272 796b 2f29  roject/faebryk/)
-00000a70: 205b 215b 4769 7448 7562 2063 6f6d 6d69   [![GitHub commi
-00000a80: 7420 6163 7469 7669 7479 5d28 6874 7470  t activity](http
-00000a90: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000aa0: 696f 2f67 6974 6875 622f 636f 6d6d 6974  io/github/commit
-00000ab0: 2d61 6374 6976 6974 792f 6d2f 6661 6562  -activity/m/faeb
-00000ac0: 7279 6b2f 6661 6562 7279 6b29 5d28 6874  ryk/faebryk)](ht
-00000ad0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ae0: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
-00000af0: 2f63 6f6d 6d69 7473 2f6d 6169 6e29 0a0a  /commits/main)..
-00000b00: 5b21 5b43 6f64 6520 7374 796c 653a 2062  [![Code style: b
-00000b10: 6c61 636b 5d28 6874 7470 733a 2f2f 696d  lack](https://im
-00000b20: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000b30: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
-00000b40: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
-00000b50: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000b60: 622e 636f 6d2f 7073 662f 626c 6163 6b29  b.com/psf/black)
-00000b70: 0a0a 3c2f 6469 763e 0a0a 2d2d 2d0a 0a23  ..</div>..---..#
-00000b80: 2320 4162 6f75 740a 0a23 2323 2057 6861  # About..### Wha
-00000b90: 7420 5c5b 6973 2066 6165 6272 796b 5c5d  t \[is faebryk\]
-00000ba0: 0a0a 6661 6562 7279 6b20 6973 2061 6e20  ..faebryk is an 
-00000bb0: 6f70 656e 2d73 6f75 7263 6520 736f 6674  open-source soft
-00000bc0: 7761 7265 2d64 6566 696e 6564 2065 6c65  ware-defined ele
-00000bd0: 6374 726f 6e69 6320 6465 7369 676e 2061  ctronic design a
-00000be0: 7574 6f6d 6174 696f 6e20 2845 4441 2920  utomation (EDA) 
-00000bf0: 746f 6f6c 2e0a 5468 696e 6b20 6f66 2069  tool..Think of i
-00000c00: 7420 6c69 6b65 2074 6865 2065 766f 6c75  t like the evolu
-00000c10: 7469 6f6e 2066 726f 6d20 4544 4120 746f  tion from EDA to
-00000c20: 6f6c 7320 6c69 6b65 204b 6943 4144 2c20  ols like KiCAD, 
-00000c30: 416c 7469 756d 2c20 4561 676c 652e 2e2e  Altium, Eagle...
-00000c40: 0a69 6e20 7468 6520 7761 7920 7468 6f73  .in the way thos
-00000c50: 6520 7765 7265 2074 6865 206e 6578 7420  e were the next 
-00000c60: 7374 6570 2066 726f 6d20 6465 7369 676e  step from design
-00000c70: 696e 6720 656c 6563 7472 6f6e 6963 2063  ing electronic c
-00000c80: 6972 6375 6974 7320 6f6e 2070 6170 6572  ircuits on paper
-00000c90: 2e0a 5468 6520 6d61 696e 2069 6465 6120  ..The main idea 
-00000ca0: 6f66 2066 6165 6272 796b 2069 7320 746f  of faebryk is to
-00000cb0: 202a 2a64 6573 6372 6962 6520 796f 7572   **describe your
-00000cc0: 2070 726f 6475 6374 206f 6e20 7468 6520   product on the 
-00000cd0: 6869 6768 6573 7420 6c65 7665 6c2a 2a20  highest level** 
-00000ce0: 706f 7373 6962 6c65 2061 6e64 2074 6865  possible and the
-00000cf0: 6e20 6974 6572 6174 6976 656c 7920 7265  n iteratively re
-00000d00: 6669 6e69 6e67 2074 6865 2064 6573 6372  fining the descr
-00000d10: 6970 7469 6f6e 2074 6f20 6172 7269 7665  iption to arrive
-00000d20: 206f 6e20 6120 636f 6d70 6c65 7465 2061   on a complete a
-00000d30: 6e64 2064 6574 6169 6c65 6420 696d 706c  nd detailed impl
-00000d40: 656d 656e 7461 7469 6f6e 2e0a 496e 2063  ementation..In c
-00000d50: 6f6d 7061 7269 736f 6e20 746f 2063 6c61  omparison to cla
-00000d60: 7373 6963 2045 4441 2061 6e64 2064 6573  ssic EDA and des
-00000d70: 6967 6e20 746f 6f6c 7320 7768 6963 6820  ign tools which 
-00000d80: 7573 6520 4755 4973 2c20 6661 6562 7279  use GUIs, faebry
-00000d90: 6b20 7573 6573 2063 6f64 6520 2850 7974  k uses code (Pyt
-00000da0: 686f 6e29 2074 6f20 6372 6561 7465 2064  hon) to create d
-00000db0: 6573 6967 6e73 2e0a 5768 696c 6520 7468  esigns..While th
-00000dc0: 6520 6d61 696e 2066 6f63 7573 2069 7320  e main focus is 
-00000dd0: 6f6e 2074 6865 2045 4441 2070 6172 7420  on the EDA part 
-00000de0: 6375 7272 656e 746c 792c 2066 6165 6272  currently, faebr
-00000df0: 796b 2061 696d 7320 746f 2062 6563 6f6d  yk aims to becom
-00000e00: 6520 6120 686f 6c69 7374 6963 2073 7973  e a holistic sys
-00000e10: 7465 6d20 6465 7369 676e 2074 6f6f 6c2e  tem design tool.
-00000e20: 0a0a 2323 2320 486f 7720 5c5b 646f 6573  ..### How \[does
-00000e30: 2064 6573 6967 6e69 6e67 2077 6974 6820   designing with 
-00000e40: 6661 6562 7279 6b20 776f 726b 5c5d 0a0a  faebryk work\]..
-00000e50: 6661 6562 7279 6b20 6974 7365 6c66 2069  faebryk itself i
-00000e60: 7320 6a75 7374 2061 202a 2a70 7974 686f  s just a **pytho
-00000e70: 6e20 6c69 6272 6172 792a 2a20 7468 6174  n library** that
-00000e80: 2079 6f75 2069 6e63 6c75 6465 2069 6e20   you include in 
-00000e90: 796f 7572 2070 726f 6a65 6374 2e20 4974  your project. It
-00000ea0: 2069 7320 7072 6f76 6964 696e 6720 796f   is providing yo
-00000eb0: 7520 7769 7468 2061 6c6c 2074 6865 2074  u with all the t
-00000ec0: 6f6f 6c73 2074 6f20 6465 7363 7269 6265  ools to describe
-00000ed0: 2061 6e64 2064 6573 6967 6e20 796f 7572   and design your
-00000ee0: 2073 7973 7465 6d20 616e 6420 746f 2065   system and to e
-00000ef0: 7870 6f72 7420 7468 6174 2064 6573 6967  xport that desig
-00000f00: 6e20 696e 746f 2073 6f6d 6574 6869 6e67  n into something
-00000f10: 2075 7365 6675 6c20 6c69 6b65 2066 6f72   useful like for
-00000f20: 2065 7861 6d70 6c65 2061 206e 6574 6c69   example a netli
-00000f30: 7374 2c20 6120 6465 7669 6365 7472 6565  st, a devicetree
-00000f40: 2c20 6765 7262 6572 7320 6574 632c 2077  , gerbers etc, w
-00000f50: 6869 6368 2079 6f75 2074 6865 6e20 6361  hich you then ca
-00000f60: 6e20 7573 6520 696e 2074 6865 206e 6578  n use in the nex
-00000f70: 7420 7374 6570 7320 6f66 2079 6f75 7220  t steps of your 
-00000f80: 7072 6f6a 6563 742e 204b 6579 2063 6f6e  project. Key con
-00000f90: 6365 7074 7320 6f66 2066 6165 6272 796b  cepts of faebryk
-00000fa0: 2061 7265 2074 6865 2067 7261 7068 2c20   are the graph, 
-00000fb0: 696d 706f 7274 6572 732c 2065 7870 6f72  importers, expor
-00000fc0: 7465 7273 2c20 7468 6520 6c69 6272 6172  ters, the librar
-00000fd0: 7920 616e 6420 7468 6520 7573 6572 2061  y and the user a
-00000fe0: 7070 6c69 6361 7469 6f6e 2e0a 546f 2075  pplication..To u
-00000ff0: 6e64 6572 7374 616e 6420 686f 7720 746f  nderstand how to
-00001000: 2075 7365 2066 6165 6272 796b 2069 6e20   use faebryk in 
-00001010: 796f 7572 2070 726f 6a65 6374 2073 6565  your project see
-00001020: 205b 7573 696e 6720 6661 6562 7279 6b5d   [using faebryk]
-00001030: 2823 7573 696e 672d 6661 6562 7279 6b29  (#using-faebryk)
-00001040: 2e0a 0a23 2323 2057 686f 205c 5b69 7320  ...### Who \[is 
-00001050: 6661 6562 7279 6b5c 5d0a 0a66 6165 6272  faebryk\]..faebr
-00001060: 796b 2069 7320 6120 636f 6d6d 756e 6974  yk is a communit
-00001070: 7920 6472 6976 656e 2070 726f 6a65 6374  y driven project
-00001080: 2e20 5468 6174 206d 6561 6e73 2066 6165  . That means fae
-00001090: 6272 796b 2064 6f65 7320 6e6f 7420 6f6e  bryk does not on
-000010a0: 6c79 2063 6f6e 7369 7374 206f 7574 206f  ly consist out o
-000010b0: 6620 636f 7265 2064 6576 656c 6f70 6572  f core developer
-000010c0: 7320 6275 7420 616c 736f 2075 7365 7273  s but also users
-000010d0: 2c20 6578 7465 726e 616c 2063 6f6e 7472  , external contr
-000010e0: 6962 7574 6f72 732c 206d 6f64 6572 6174  ibutors, moderat
-000010f0: 6f72 7320 616e 6420 796f 7521 2049 7420  ors and you! It 
-00001100: 6973 2066 6f75 6e64 6564 2062 7920 6120  is founded by a 
-00001110: 6772 6f75 7020 6f66 2065 6d62 6564 6465  group of embedde
-00001120: 642c 2065 6c65 6374 7269 6361 6c2c 2070  d, electrical, p
-00001130: 726f 6475 6374 2064 6573 6967 6e20 616e  roduct design an
-00001140: 6420 736f 6674 7761 7265 2065 6e67 696e  d software engin
-00001150: 6565 7273 2077 6974 6820 6120 6c6f 7665  eers with a love
-00001160: 2066 6f72 206d 616b 696e 672e 0a0a 2323   for making...##
-00001170: 2320 5768 7920 5c5b 646f 2077 6520 6d61  # Why \[do we ma
-00001180: 6b65 2066 6165 6272 796b 5c5d 0a0a 5765  ke faebryk\]..We
-00001190: 206e 6f74 6963 6564 2074 6861 7420 7468   noticed that th
-000011a0: 6520 696e 6e6f 7661 7469 6f6e 7320 6f66  e innovations of
-000011b0: 2073 6f66 7477 6172 6520 656e 6769 6e65   software engine
-000011c0: 6572 696e 6720 7468 6174 206d 616b 6520  ering that make 
-000011d0: 6661 7374 2c20 7363 616c 6162 6c65 2c20  fast, scalable, 
-000011e0: 726f 6275 7374 2073 6f6c 7574 696f 6e73  robust solutions
-000011f0: 2070 6f73 7369 626c 6520 6861 7665 206e   possible have n
-00001200: 6f74 2066 6f75 6e64 2074 6865 6972 2077  ot found their w
-00001210: 6179 2069 6e74 6f20 6861 7264 7761 7265  ay into hardware
-00001220: 2064 6573 6967 6e2e 2046 7572 7468 6572   design. Further
-00001230: 6d6f 7265 2074 6865 7265 2069 7320 6120  more there is a 
-00001240: 6c6f 7420 6f66 2064 7570 6c69 6361 7465  lot of duplicate
-00001250: 2077 6f72 6b20 646f 6e65 2e20 5468 696e   work done. Thin
-00001260: 6b20 6f66 2064 6574 6572 6d69 6e69 6e67  k of determining
-00001270: 2074 6865 2070 696e 6f75 7420 6f66 2061   the pinout of a
-00001280: 2053 6f43 2061 6e64 2074 6865 6e20 6861   SoC and then ha
-00001290: 7669 6e67 2074 6f20 7472 616e 736c 6174  ving to translat
-000012a0: 6520 7468 6174 2065 7861 6374 2070 696e  e that exact pin
-000012b0: 6f75 7420 696e 746f 2073 6f66 7477 6172  out into softwar
-000012c0: 6520 6167 6169 6e20 6f72 2068 6176 696e  e again or havin
-000012d0: 6720 746f 2063 6f6e 7374 616e 746c 7920  g to constantly 
-000012e0: 6164 6170 7420 6465 7369 676e 7320 666f  adapt designs fo
-000012f0: 7220 7375 7070 6c79 2063 6861 696e 2069  r supply chain i
-00001300: 7373 7565 732e 0a41 6464 6974 696f 6e61  ssues..Additiona
-00001310: 6c6c 792c 2068 6172 6477 6172 6520 6465  lly, hardware de
-00001320: 7369 676e 2068 6173 2071 7569 7465 2061  sign has quite a
-00001330: 2062 6967 2062 6172 7269 6572 206f 6620   big barrier of 
-00001340: 656e 7472 7920 666f 7220 6d61 6b65 7273  entry for makers
-00001350: 2c20 6275 7420 7765 2064 6f6e 2774 2074  , but we don't t
-00001360: 6869 6e6b 2069 7420 6861 7320 746f 2e0a  hink it has to..
-00001370: 4375 7272 656e 746c 7920 6861 7264 7761  Currently hardwa
-00001380: 7265 2064 6573 6967 6e20 6973 2061 6c73  re design is als
-00001390: 6f20 7175 6974 6520 6c61 626f 7220 696e  o quite labor in
-000013a0: 7465 6e73 6976 6520 7769 7468 2076 6572  tensive with ver
-000013b0: 7920 6c69 7474 6c65 2061 7574 6f6d 6174  y little automat
-000013c0: 696f 6e2e 0a66 6165 6272 796b 2061 696d  ion..faebryk aim
-000013d0: 7320 746f 2074 6163 6b6c 6520 616c 6c20  s to tackle all 
-000013e0: 7468 6f73 6520 6973 7375 6573 2061 6e64  those issues and
-000013f0: 2061 6c73 6f20 6f70 656e 7320 7570 2073   also opens up s
-00001400: 6f6d 6520 6578 6369 7469 6e67 2070 6f73  ome exciting pos
-00001410: 7369 6269 6c69 7469 6573 2c20 7375 6368  sibilities, such
-00001420: 2061 7320 6265 6e65 6669 7469 6e67 2066   as benefiting f
-00001430: 726f 6d20 7468 6520 7665 7273 696f 6e20  rom the version 
-00001440: 6d61 6e61 6765 6d65 6e74 2061 6e64 2063  management and c
-00001450: 6f6c 6c61 626f 7261 7469 6f6e 2074 6f6f  ollaboration too
-00001460: 6c73 2074 6861 7420 6172 6520 7573 6564  ls that are used
-00001470: 2069 6e20 6d6f 6465 726e 2073 6f66 7477   in modern softw
-00001480: 6172 6520 6465 7665 6c6f 706d 656e 742e  are development.
-00001490: 0a0a 2323 2320 5768 656e 205c 5b69 7320  ..### When \[is 
-000014a0: 6661 6562 7279 6b20 6265 696e 6720 6465  faebryk being de
-000014b0: 7665 6c6f 7065 645c 5d0a 0a66 6165 6272  veloped\]..faebr
-000014c0: 796b 2069 7320 6265 696e 6720 636f 6e74  yk is being cont
-000014d0: 696e 756f 7573 6c79 2064 6576 656c 6f70  inuously develop
-000014e0: 6564 2e0a 5468 6520 636f 7265 2074 6561  ed..The core tea
-000014f0: 6d20 666f 6375 7365 7320 6f6e 2063 6f72  m focuses on cor
-00001500: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
-00001510: 616e 6420 6665 6174 7572 6573 206f 6620  and features of 
-00001520: 6661 6562 7279 6b2c 2061 7320 7765 6c6c  faebryk, as well
-00001530: 2061 7320 7468 6520 6765 6e65 7261 6c20   as the general 
-00001540: 6469 7265 6374 696f 6e20 6f66 2074 6865  direction of the
-00001550: 2070 726f 6a65 6374 2e0a 5468 6520 7374   project..The st
-00001560: 7265 6e67 7468 206f 6620 7468 6520 636f  rength of the co
-00001570: 6d6d 756e 6974 7920 6361 6e20 7265 616c  mmunity can real
-00001580: 6c79 2073 6869 6e65 2077 6974 6820 7468  ly shine with th
-00001590: 6520 6465 7665 6c6f 706d 656e 7420 6f66  e development of
-000015a0: 2069 6d70 6f72 7465 7273 2c20 6578 706f   importers, expo
-000015b0: 7274 6572 732c 206c 6962 7261 7269 6573  rters, libraries
-000015c0: 2c20 616e 6420 7072 6f6a 6563 7473 2c20  , and projects, 
-000015d0: 6275 7420 6576 6572 796f 6e65 2069 7320  but everyone is 
-000015e0: 7765 6c63 6f6d 6520 746f 205b 6865 6c70  welcome to [help
-000015f0: 5d28 2363 6f6d 6d75 6e69 7479 2d73 7570  ](#community-sup
-00001600: 706f 7274 2920 6f75 7420 7768 6572 6520  port) out where 
-00001610: 7468 6579 2063 616e 2e0a 0a23 2323 2057  they can...### W
-00001620: 6865 7265 205c 5b64 6f20 7765 2064 6576  here \[do we dev
-00001630: 656c 6f70 2066 6165 6272 796b 5c5d 0a0a  elop faebryk\]..
-00001640: 6661 6562 7279 6b20 6973 2062 6569 6e67  faebryk is being
-00001650: 2064 6576 656c 6f70 6564 2063 6f6d 706c   developed compl
-00001660: 6574 656c 7920 696e 2074 6865 206f 7065  etely in the ope
-00001670: 6e20 6f6e 2047 6974 6875 622e 0a41 6c6c  n on Github..All
-00001680: 2074 6865 2069 6e66 6f72 6d61 7469 6f6e   the information
-00001690: 2079 6f75 206e 6565 6420 746f 2073 7461   you need to sta
-000016a0: 7274 2075 7369 6e67 2061 6e64 2063 6f6e  rt using and con
-000016b0: 7472 6962 7574 696e 6720 746f 2066 6165  tributing to fae
-000016c0: 6272 796b 2077 696c 6c20 6265 2069 6e20  bryk will be in 
-000016d0: 6f72 206c 696e 6b65 6420 746f 2066 726f  or linked to fro
-000016e0: 6d20 5b74 6869 7320 7265 706f 7369 746f  m [this reposito
-000016f0: 7279 5d28 6874 7470 733a 2f2f 6769 7468  ry](https://gith
-00001700: 7562 2e63 6f6d 2f66 6165 6272 796b 2f66  ub.com/faebryk/f
-00001710: 6165 6272 796b 292e 0a49 6620 796f 7520  aebryk)..If you 
-00001720: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
-00001730: 6e73 2079 6f75 2063 616e 2061 736b 2074  ns you can ask t
-00001740: 6865 6d20 6f6e 206f 7572 205b 4469 7363  hem on our [Disc
-00001750: 6f72 645d 2868 7474 7073 3a2f 2f64 6973  ord](https://dis
-00001760: 636f 7264 2e67 672f 3935 6a59 7550 6d6e  cord.gg/95jYuPmn
-00001770: 5557 292e 0a46 6f72 2070 756c 6c20 7265  UW)..For pull re
-00001780: 7175 6573 7473 2061 6e64 2062 7567 2d72  quests and bug-r
-00001790: 6570 6f72 7473 2c20 7365 6520 6f75 7220  eports, see our 
-000017a0: 5b63 6f6e 7472 6962 7574 696e 6720 6775  [contributing gu
-000017b0: 6964 656c 696e 6573 5d28 646f 6373 2f43  idelines](docs/C
-000017c0: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
-000017d0: 0a0a 2d2d 2d0a 0a23 2320 5573 696e 6720  ..---..## Using 
-000017e0: 6661 6562 7279 6b0a 0a23 2323 2046 726f  faebryk..### Fro
-000017f0: 6d20 7069 700a 0a53 6574 7570 0a0a 6060  m pip..Setup..``
-00001800: 6062 6173 680a 3e20 2320 6f70 7469 6f6e  `bash.> # option
-00001810: 616c 3a20 7573 6520 7665 6e76 0a3e 2070  al: use venv.> p
-00001820: 7974 686f 6e20 2d6d 2076 656e 7620 7665  ython -m venv ve
-00001830: 6e76 0a3e 202e 2076 656e 762f 6269 6e2f  nv.> . venv/bin/
-00001840: 6163 7469 7661 7465 0a3e 0a3e 2070 6970  activate.>.> pip
-00001850: 2069 6e73 7461 6c6c 2066 6165 6272 796b   install faebryk
-00001860: 0a60 6060 0a0a 5275 6e6e 696e 6720 7361  .```..Running sa
-00001870: 6d70 6c65 730a 0a60 6060 6261 7368 0a3e  mples..```bash.>
-00001880: 206d 6b64 6972 206d 795f 6661 6562 7279   mkdir my_faebry
-00001890: 6b5f 7072 6f6a 6563 740a 3e20 6364 206d  k_project.> cd m
-000018a0: 795f 6661 6562 7279 6b5f 7072 6f6a 6563  y_faebryk_projec
-000018b0: 740a 3e20 2320 646f 776e 6c6f 6164 2061  t.> # download a
-000018c0: 2073 616d 706c 6520 6672 6f6d 2074 6865   sample from the
-000018d0: 2067 6974 6875 6220 7265 706f 2069 6e20   github repo in 
-000018e0: 2f73 616d 706c 6573 0a3e 2070 7974 686f  /samples.> pytho
-000018f0: 6e33 203c 7361 6d70 6c65 5f6e 616d 652e  n3 <sample_name.
-00001900: 7079 3e20 7c20 7461 696c 202d 6e31 203e  py> | tail -n1 >
-00001910: 206e 6574 6c69 7374 2e6e 6574 0a60 6060   netlist.net.```
-00001920: 0a0a 2323 2320 4672 6f6d 2073 6f75 7263  ..### From sourc
-00001930: 650a 0a53 6574 7570 0a0a 6060 6062 6173  e..Setup..```bas
-00001940: 680a 3e20 6769 7420 636c 6f6e 6520 6874  h.> git clone ht
-00001950: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001960: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
-00001970: 2e67 6974 0a3e 2063 6420 6661 6562 7279  .git.> cd faebry
-00001980: 6b0a 3e0a 3e20 2320 6372 6561 7465 2076  k.>.> # create v
-00001990: 656e 760a 3e20 7079 7468 6f6e 202d 6d20  env.> python -m 
-000019a0: 7665 6e76 2076 656e 760a 3e20 2e20 7665  venv venv.> . ve
-000019b0: 6e76 2f62 696e 2f61 6374 6976 6174 650a  nv/bin/activate.
-000019c0: 3e0a 3e20 2320 7265 7175 6972 6573 2070  >.> # requires p
-000019d0: 6970 2076 6572 7369 6f6e 203e 3d20 3231  ip version >= 21
-000019e0: 2e33 0a3e 2070 6970 2069 6e73 7461 6c6c  .3.> pip install
-000019f0: 202d 7220 7265 7175 6972 656d 656e 7473   -r requirements
-00001a00: 2e74 7874 0a3e 2070 6970 2069 6e73 7461  .txt.> pip insta
-00001a10: 6c6c 202d 2d65 6469 7461 626c 6520 2e0a  ll --editable ..
-00001a20: 6060 600a 0a52 756e 6e69 6e67 2073 616d  ```..Running sam
-00001a30: 706c 6573 0a0a 6060 6062 6173 680a 3e20  ples..```bash.> 
-00001a40: 2e2f 7361 6d70 6c65 732f 3c73 616d 706c  ./samples/<sampl
-00001a50: 655f 6e61 6d65 3e2e 7079 207c 2074 6169  e_name>.py | tai
-00001a60: 6c20 2d6e 3120 3e20 6e65 746c 6973 742e  l -n1 > netlist.
-00001a70: 6e65 740a 6060 600a 0a2d 2d2d 0a0a 2323  net.```..---..##
-00001a80: 2044 6576 656c 6f70 6d65 6e74 0a0a 2323   Development..##
-00001a90: 2320 5665 7273 696f 6e69 6e67 0a0a 6661  # Versioning..fa
-00001aa0: 6562 7279 6b20 7573 6573 205b 7365 6d61  ebryk uses [sema
-00001ab0: 6e74 6963 2076 6572 7369 6f6e 696e 675d  ntic versioning]
-00001ac0: 2868 7474 7073 3a2f 2f73 656d 7665 722e  (https://semver.
-00001ad0: 6f72 672f 2920 696e 2074 6865 205b 7265  org/) in the [re
-00001ae0: 6c65 6173 6573 5d28 6874 7470 733a 2f2f  leases](https://
-00001af0: 6769 7468 7562 2e63 6f6d 2f66 6165 6272  github.com/faebr
-00001b00: 796b 2f66 6165 6272 796b 2f72 656c 6561  yk/faebryk/relea
-00001b10: 7365 7329 2e0a 0a41 7320 6665 6162 7279  ses)...As feabry
-00001b20: 6b20 6973 2073 7469 6c6c 2069 6e20 7468  k is still in th
-00001b30: 6520 6561 726c 7920 7374 6167 6573 206f  e early stages o
-00001b40: 6620 6465 7665 6c6f 706d 656e 7420 6e65  f development ne
-00001b50: 7720 7265 6c65 6173 6573 2077 696c 6c20  w releases will 
-00001b60: 6861 7665 2061 206c 6f74 206f 6620 2862  have a lot of (b
-00001b70: 7265 616b 696e 6729 2063 6861 6e67 6573  reaking) changes
-00001b80: 2069 6e20 7468 656d 2e0a 4f75 7220 5b72   in them..Our [r
-00001b90: 6f61 646d 6170 5d28 2376 6572 7369 6f6e  oadmap](#version
-00001ba0: 696e 6729 2854 4f44 4f29 2077 696c 6c20  ing)(TODO) will 
-00001bb0: 7368 6f77 2079 6f75 2077 6865 7265 2074  show you where t
-00001bc0: 6865 2070 726f 6a65 6374 2069 7320 676f  he project is go
-00001bd0: 696e 6720 746f 2061 6e64 2077 6861 7420  ing to and what 
-00001be0: 796f 7520 6361 6e20 6578 7065 6374 2069  you can expect i
-00001bf0: 6e20 6675 7475 7265 2072 656c 6561 7365  n future release
-00001c00: 732e 0a0a 2323 2320 436f 6e74 7269 6275  s...### Contribu
-00001c10: 7469 6e67 0a0a 5365 6520 5b43 4f4e 5452  ting..See [CONTR
-00001c20: 4942 5554 494e 472e 6d64 5d28 646f 6373  IBUTING.md](docs
-00001c30: 2f43 4f4e 5452 4942 5554 494e 472e 6d64  /CONTRIBUTING.md
-00001c40: 290a 0a54 6f20 6765 7420 696e 7370 6972  )..To get inspir
-00001c50: 6174 696f 6e20 6f6e 2074 6869 6e67 7320  ation on things 
-00001c60: 746f 2077 6f72 6b20 6f6e 2063 6865 636b  to work on check
-00001c70: 206f 7574 2074 6865 2069 7373 7565 732e   out the issues.
-00001c80: 0a0a 2323 2323 2052 756e 6e69 6e67 2079  ..#### Running y
-00001c90: 6f75 7220 6f77 6e20 6578 7065 7269 6d65  our own experime
-00001ca0: 6e74 732f 4d61 6b69 6e67 2073 616d 706c  nts/Making sampl
-00001cb0: 6573 0a0a 4669 7273 7420 666f 6c6c 6f77  es..First follow
-00001cc0: 2074 6865 2073 7465 7073 2069 6e20 6765   the steps in ge
-00001cd0: 7420 7275 6e6e 696e 6720 6672 6f6d 2073  t running from s
-00001ce0: 6f75 7263 652e 0a54 6865 6e20 6164 6420  ource..Then add 
-00001cf0: 6120 6669 6c65 2069 6e20 7361 6d70 6c65  a file in sample
-00001d00: 732f 2028 796f 7520 6361 6e20 7573 6520  s/ (you can use 
-00001d10: 6f6e 6520 6f66 2074 6865 2073 616d 706c  one of the sampl
-00001d20: 6573 2061 7320 7465 6d70 6c61 7465 292e  es as template).
-00001d30: 0a43 616c 6c20 796f 7572 2066 696c 6520  .Call your file 
-00001d40: 7769 7468 2060 7079 7468 6f6e 3320 7361  with `python3 sa
-00001d50: 6d70 6c65 732f 3c79 6f75 7266 696c 653e  mples/<yourfile>
-00001d60: 2e70 7960 2e0a 0a23 2323 2320 5275 6e6e  .py`...#### Runn
-00001d70: 696e 6720 7465 7374 730a 0a52 756e 0a0a  ing tests..Run..
-00001d80: 6060 6062 6173 680a 3e20 7079 7465 7374  ```bash.> pytest
-00001d90: 2074 6573 740a 6060 600a 0a23 2320 436f   test.```..## Co
-00001da0: 6d6d 756e 6974 7920 5375 7070 6f72 740a  mmunity Support.
-00001db0: 0a43 6f6d 6d75 6e69 7479 2073 7570 706f  .Community suppo
-00001dc0: 7274 2069 7320 7072 6f76 6964 6564 2076  rt is provided v
-00001dd0: 6961 2044 6973 636f 7264 3b20 7365 6520  ia Discord; see 
-00001de0: 7468 6520 5265 736f 7572 6365 7320 6265  the Resources be
-00001df0: 6c6f 7720 666f 7220 6465 7461 696c 732e  low for details.
-00001e00: 0a0a 2323 2320 5265 736f 7572 6365 730a  ..### Resources.
-00001e10: 0a2d 2053 6f75 7263 6520 436f 6465 3a20  .- Source Code: 
-00001e20: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00001e30: 636f 6d2f 6661 6562 7279 6b2f 6661 6562  com/faebryk/faeb
-00001e40: 7279 6b3e 0a2d 2043 6861 743a 2052 6561  ryk>.- Chat: Rea
-00001e50: 6c2d 7469 6d65 2063 6861 7420 6861 7070  l-time chat happ
-00001e60: 656e 7320 696e 2066 6165 6272 796b 2773  ens in faebryk's
-00001e70: 2044 6973 636f 7264 2053 6572 7665 722e   Discord Server.
-00001e80: 2055 7365 2074 6869 7320 4469 7363 6f72   Use this Discor
-00001e90: 6420 5b49 6e76 6974 655d 2868 7474 7073  d [Invite](https
-00001ea0: 3a2f 2f64 6973 636f 7264 2e67 672f 3935  ://discord.gg/95
-00001eb0: 6a59 7550 6d6e 5557 2920 746f 2072 6567  jYuPmnUW) to reg
-00001ec0: 6973 7465 720a 2d20 4973 7375 6573 3a20  ister.- Issues: 
-00001ed0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00001ee0: 636f 6d2f 6661 6562 7279 6b2f 6661 6562  com/faebryk/faeb
-00001ef0: 7279 6b2f 6973 7375 6573 3e0a            ryk/issues>.
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a0a 2320 6661 6562 7279 6b0a  er">..# faebryk.
+00000020: 0a23 2323 205c 5b66 cb88 c99b 62c9 b9c9  .### \[f....b...
+00000030: aa6b 5c5d 0a0a 3c61 2068 7265 663d 2268  .k\]..<a href="h
+00000040: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000050: 6d2f 6661 6562 7279 6b2f 6661 6562 7279  m/faebryk/faebry
+00000060: 6b22 3e0a 3c69 6d67 2068 6569 6768 743d  k">.<img height=
+00000070: 3330 3020 7769 6474 683d 3330 3020 7372  300 width=300 sr
+00000080: 633d 222e 2f66 6165 6272 796b 5f6c 6f67  c="./faebryk_log
+00000090: 6f2e 706e 6722 2f3e 0a3c 2f61 3e0a 3c62  o.png"/>.</a>.<b
+000000a0: 722f 3e0a 0a4f 7065 6e2d 736f 7572 6365  r/>..Open-source
+000000b0: 2073 6f66 7477 6172 652d 6465 6669 6e65   software-define
+000000c0: 6420 4544 4120 746f 6f6c 0a0a 5b21 5b56  d EDA tool..[![V
+000000d0: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
+000000e0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+000000f0: 6974 6875 622f 762f 7461 672f 6661 6562  ithub/v/tag/faeb
+00000100: 7279 6b2f 6661 6562 7279 6b29 5d28 6874  ryk/faebryk)](ht
+00000110: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000120: 2f66 6165 6272 796b 2f66 6165 6272 796b  /faebryk/faebryk
+00000130: 2f72 656c 6561 7365 732f 6c61 7465 7374  /releases/latest
+00000140: 2920 5b21 5b4c 6963 656e 7365 3a20 4d49  ) [![License: MI
+00000150: 545d 2868 7474 7073 3a2f 2f69 6d67 2e73  T](https://img.s
+00000160: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000170: 4c69 6365 6e73 652d 4d49 542d 7965 6c6c  License-MIT-yell
+00000180: 6f77 2e73 7667 295d 2868 7474 7073 3a2f  ow.svg)](https:/
+00000190: 2f67 6974 6875 622e 636f 6d2f 6661 6562  /github.com/faeb
+000001a0: 7279 6b2f 6661 6562 7279 6b2f 626c 6f62  ryk/faebryk/blob
+000001b0: 2f6d 6169 6e2f 4c49 4345 4e53 4529 205b  /main/LICENSE) [
+000001c0: 215b 5075 6c6c 2072 6571 7565 7374 7320  ![Pull requests 
+000001d0: 6f70 656e 5d28 6874 7470 733a 2f2f 696d  open](https://im
+000001e0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000001f0: 6875 622f 6973 7375 6573 2d70 722f 6661  hub/issues-pr/fa
+00000200: 6562 7279 6b2f 6661 6562 7279 6b29 5d28  ebryk/faebryk)](
+00000210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000220: 6f6d 2f66 6165 6272 796b 2f66 6165 6272  om/faebryk/faebr
+00000230: 796b 2f70 756c 6c73 2920 5b21 5b49 7373  yk/pulls) [![Iss
+00000240: 7565 7320 6f70 656e 5d28 6874 7470 733a  ues open](https:
+00000250: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000260: 2f67 6974 6875 622f 6973 7375 6573 2f66  /github/issues/f
+00000270: 6165 6272 796b 2f66 6165 6272 796b 295d  aebryk/faebryk)]
+00000280: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000290: 636f 6d2f 6661 6562 7279 6b2f 6661 6562  com/faebryk/faeb
+000002a0: 7279 6b2f 6973 7375 6573 290a 5b21 5b44  ryk/issues).[![D
+000002b0: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+000002c0: 696d 672e 7368 6965 6c64 732e 696f 2f64  img.shields.io/d
+000002d0: 6973 636f 7264 2f39 3037 3637 3533 3333  iscord/907675333
+000002e0: 3335 3038 3039 3630 303f 6c61 6265 6c3d  350809600?label=
+000002f0: 4469 7363 6f72 6429 5d28 6874 7470 733a  Discord)](https:
+00000300: 2f2f 6469 7363 6f72 642e 636f 6d2f 6368  //discord.com/ch
+00000310: 616e 6e65 6c73 2f39 3037 3637 3533 3333  annels/907675333
+00000320: 3335 3038 3039 3630 3029 205b 215b 5079  350809600) [![Py
+00000330: 5049 202d 2044 6f77 6e6c 6f61 6473 5d28  PI - Downloads](
+00000340: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000350: 6c64 732e 696f 2f70 7970 692f 646d 2f66  lds.io/pypi/dm/f
+00000360: 6165 6272 796b 3f6c 6162 656c 3d50 7950  aebryk?label=PyP
+00000370: 6925 3230 446f 776e 6c6f 6164 7329 5d28  i%20Downloads)](
+00000380: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000390: 2f70 726f 6a65 6374 2f66 6165 6272 796b  /project/faebryk
+000003a0: 2f29 205b 215b 4769 7448 7562 2063 6f6d  /) [![GitHub com
+000003b0: 6d69 7420 6163 7469 7669 7479 5d28 6874  mit activity](ht
+000003c0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000003d0: 732e 696f 2f67 6974 6875 622f 636f 6d6d  s.io/github/comm
+000003e0: 6974 2d61 6374 6976 6974 792f 6d2f 6661  it-activity/m/fa
+000003f0: 6562 7279 6b2f 6661 6562 7279 6b29 5d28  ebryk/faebryk)](
+00000400: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000410: 6f6d 2f66 6165 6272 796b 2f66 6165 6272  om/faebryk/faebr
+00000420: 796b 2f63 6f6d 6d69 7473 2f6d 6169 6e29  yk/commits/main)
+00000430: 0a0a 5b21 5b43 6f64 6520 7374 796c 653a  ..[![Code style:
+00000440: 2062 6c61 636b 5d28 6874 7470 733a 2f2f   black](https://
+00000450: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000460: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
+00000470: 652d 626c 6163 6b2d 3030 3030 3030 2e73  e-black-000000.s
+00000480: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000490: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
+000004a0: 6b29 0a0a 3c2f 6469 763e 0a0a 496e 2073  k)..</div>..In s
+000004b0: 686f 7274 2066 6165 6272 796b 2069 7320  hort faebryk is 
+000004c0: 6120 7079 7468 6f6e 206c 6962 7261 7279  a python library
+000004d0: 2074 6861 7420 616c 6c6f 7773 2079 6f75   that allows you
+000004e0: 2074 6f20 6465 7369 676e 2072 6561 6479   to design ready
+000004f0: 2d74 6f2d 6f72 6465 7220 656c 6563 7472  -to-order electr
+00000500: 6f6e 6963 7320 2850 4342 732c 2073 6368  onics (PCBs, sch
+00000510: 656d 6174 6963 732c 2065 7463 2920 696e  ematics, etc) in
+00000520: 2063 6f64 652e 2049 7420 6169 6d73 2074   code. It aims t
+00000530: 6f20 7265 6475 6365 2074 6865 2065 6e74  o reduce the ent
+00000540: 7279 2d62 6172 7269 6572 2066 6f72 2068  ry-barrier for h
+00000550: 6172 6477 6172 6520 6465 7369 676e 2062  ardware design b
+00000560: 7920 6272 6964 6769 6e67 2074 6865 2067  y bridging the g
+00000570: 6170 2062 6574 7765 656e 2073 6f66 7477  ap between softw
+00000580: 6172 6520 616e 6420 6861 7264 7761 7265  are and hardware
+00000590: 2064 6573 6967 6e2e 0a0a 2d2d 2d0a 0a0a   design...---...
+000005a0: 2323 2055 7369 6e67 2066 6165 6272 796b  ## Using faebryk
+000005b0: 0a0a 6060 6062 6173 680a 3e20 7069 7020  ..```bash.> pip 
+000005c0: 696e 7374 616c 6c20 6661 6562 7279 6b0a  install faebryk.
+000005d0: 6060 600a 0a0a 6060 6070 7974 686f 6e0a  ```...```python.
+000005e0: 696d 706f 7274 2066 6165 6272 796b 2e6c  import faebryk.l
+000005f0: 6962 7261 7279 2e5f 4620 6173 2046 0a66  ibrary._F as F.f
+00000600: 726f 6d20 6661 6562 7279 6b2e 636f 7265  rom faebryk.core
+00000610: 2e63 6f72 6520 696d 706f 7274 204d 6f64  .core import Mod
+00000620: 756c 650a 6672 6f6d 2066 6165 6272 796b  ule.from faebryk
+00000630: 2e6c 6962 732e 6578 7065 7269 6d65 6e74  .libs.experiment
+00000640: 732e 6275 696c 6475 7469 6c20 696d 706f  s.buildutil impo
+00000650: 7274 2028 0a20 2020 2074 6167 5f61 6e64  rt (.    tag_and
+00000660: 5f65 7870 6f72 745f 6d6f 6475 6c65 5f74  _export_module_t
+00000670: 6f5f 6e65 746c 6973 740a 290a 0a63 6c61  o_netlist.)..cla
+00000680: 7373 2041 7070 284d 6f64 756c 6529 3a20  ss App(Module): 
+00000690: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000006a0: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
+000006b0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+000006c0: 2e5f 5f69 6e69 745f 5f28 290a 0a20 2020  .__init__()..   
+000006d0: 2020 2020 2063 6c61 7373 205f 4e4f 4445       class _NODE
+000006e0: 5328 4d6f 6475 6c65 2e4e 4f44 4553 2829  S(Module.NODES()
+000006f0: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+00000700: 6564 203d 2046 2e50 6f77 6572 6564 4c45  ed = F.PoweredLE
+00000710: 4428 290a 2020 2020 2020 2020 2020 2020  D().            
+00000720: 6261 7474 6572 7920 3d20 462e 4261 7474  battery = F.Batt
+00000730: 6572 7928 290a 0a20 2020 2020 2020 2073  ery()..        s
+00000740: 656c 662e 4e4f 4445 7320 3d20 5f4e 4f44  elf.NODEs = _NOD
+00000750: 4553 2873 656c 6629 0a0a 2020 2020 2020  ES(self)..      
+00000760: 2020 2320 436f 6e6e 6563 7469 6f6e 730a    # Connections.
+00000770: 2020 2020 2020 2020 7365 6c66 2e4e 4f44          self.NOD
+00000780: 4573 2e6c 6564 2e49 4673 2e70 6f77 6572  Es.led.IFs.power
+00000790: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
+000007a0: 2020 2020 2020 7365 6c66 2e4e 4f44 4573        self.NODEs
+000007b0: 2e62 6174 7465 7279 2e49 4673 2e70 6f77  .battery.IFs.pow
+000007c0: 6572 290a 0a20 2020 2020 2020 2023 2050  er)..        # P
+000007d0: 6172 616d 6574 7269 7a65 0a20 2020 2020  arametrize.     
+000007e0: 2020 2073 656c 662e 4e4f 4445 732e 6c65     self.NODEs.le
+000007f0: 642e 4e4f 4445 732e 6c65 642e 5041 5241  d.NODEs.led.PARA
+00000800: 4d73 2e63 6f6c 6f72 2e6d 6572 6765 280a  Ms.color.merge(.
+00000810: 2020 2020 2020 2020 2020 2020 462e 4c45              F.LE
+00000820: 442e 436f 6c6f 722e 5945 4c4c 4f57 290a  D.Color.YELLOW).
+00000830: 2020 2020 2020 2020 7365 6c66 2e4e 4f44          self.NOD
+00000840: 4573 2e6c 6564 2e4e 4f44 4573 2e6c 6564  Es.led.NODEs.led
+00000850: 2e50 4152 414d 732e 6272 6967 6874 6e65  .PARAMs.brightne
+00000860: 7373 2e6d 6572 6765 280a 2020 2020 2020  ss.merge(.      
+00000870: 2020 2020 2020 462e 5261 6e67 652e 6c6f        F.Range.lo
+00000880: 7765 725f 626f 756e 6428 3330 652d 3329  wer_bound(30e-3)
+00000890: 290a 0a0a 7461 675f 616e 645f 6578 706f  )...tag_and_expo
+000008a0: 7274 5f6d 6f64 756c 655f 746f 5f6e 6574  rt_module_to_net
+000008b0: 6c69 7374 2841 7070 2829 290a 6060 600a  list(App()).```.
+000008c0: 0a3c 6469 7620 616c 6967 6e3d 2263 656e  .<div align="cen
+000008d0: 7465 7222 3e0a 0a21 5b5d 2864 6f63 732f  ter">..![](docs/
+000008e0: 696d 672f 6465 6d6f 2e67 6966 290a 0a3c  img/demo.gif)..<
+000008f0: 2f64 6976 3e0a 0a2d 2d2d 0a0a 2323 2041  /div>..---..## A
+00000900: 626f 7574 0a0a 2323 2320 5768 6174 205c  bout..### What \
+00000910: 5b69 7320 6661 6562 7279 6b5c 5d0a 0a66  [is faebryk\]..f
+00000920: 6165 6272 796b 2069 7320 616e 206f 7065  aebryk is an ope
+00000930: 6e2d 736f 7572 6365 2073 6f66 7477 6172  n-source softwar
+00000940: 652d 6465 6669 6e65 6420 656c 6563 7472  e-defined electr
+00000950: 6f6e 6963 2064 6573 6967 6e20 6175 746f  onic design auto
+00000960: 6d61 7469 6f6e 2028 4544 4129 2074 6f6f  mation (EDA) too
+00000970: 6c2e 0a54 6869 6e6b 206f 6620 6974 206c  l..Think of it l
+00000980: 696b 6520 7468 6520 6576 6f6c 7574 696f  ike the evolutio
+00000990: 6e20 6672 6f6d 2045 4441 2074 6f6f 6c73  n from EDA tools
+000009a0: 206c 696b 6520 4b69 4341 442c 2041 6c74   like KiCAD, Alt
+000009b0: 6975 6d2c 2045 6167 6c65 2e2e 2e0a 696e  ium, Eagle....in
+000009c0: 2074 6865 2077 6179 2074 686f 7365 2077   the way those w
+000009d0: 6572 6520 7468 6520 6e65 7874 2073 7465  ere the next ste
+000009e0: 7020 6672 6f6d 2064 6573 6967 6e69 6e67  p from designing
+000009f0: 2065 6c65 6374 726f 6e69 6320 6369 7263   electronic circ
+00000a00: 7569 7473 206f 6e20 7061 7065 722e 0a54  uits on paper..T
+00000a10: 6865 206d 6169 6e20 6964 6561 206f 6620  he main idea of 
+00000a20: 6661 6562 7279 6b20 6973 2074 6f20 2a2a  faebryk is to **
+00000a30: 6465 7363 7269 6265 2079 6f75 7220 7072  describe your pr
+00000a40: 6f64 7563 7420 6f6e 2074 6865 2068 6967  oduct on the hig
+00000a50: 6865 7374 206c 6576 656c 2a2a 2070 6f73  hest level** pos
+00000a60: 7369 626c 6520 616e 6420 7468 656e 2069  sible and then i
+00000a70: 7465 7261 7469 7665 6c79 2072 6566 696e  teratively refin
+00000a80: 696e 6720 7468 6520 6465 7363 7269 7074  ing the descript
+00000a90: 696f 6e20 746f 2061 7272 6976 6520 6f6e  ion to arrive on
+00000aa0: 2061 2063 6f6d 706c 6574 6520 616e 6420   a complete and 
+00000ab0: 6465 7461 696c 6564 2069 6d70 6c65 6d65  detailed impleme
+00000ac0: 6e74 6174 696f 6e2e 0a49 6e20 636f 6d70  ntation..In comp
+00000ad0: 6172 6973 6f6e 2074 6f20 636c 6173 7369  arison to classi
+00000ae0: 6320 4544 4120 616e 6420 6465 7369 676e  c EDA and design
+00000af0: 2074 6f6f 6c73 2077 6869 6368 2075 7365   tools which use
+00000b00: 2047 5549 732c 2066 6165 6272 796b 2075   GUIs, faebryk u
+00000b10: 7365 7320 636f 6465 2028 5079 7468 6f6e  ses code (Python
+00000b20: 2920 746f 2063 7265 6174 6520 6465 7369  ) to create desi
+00000b30: 676e 732e 0a57 6869 6c65 2074 6865 206d  gns..While the m
+00000b40: 6169 6e20 666f 6375 7320 6973 206f 6e20  ain focus is on 
+00000b50: 7468 6520 4544 4120 7061 7274 2063 7572  the EDA part cur
+00000b60: 7265 6e74 6c79 2c20 6661 6562 7279 6b20  rently, faebryk 
+00000b70: 6169 6d73 2074 6f20 6265 636f 6d65 2061  aims to become a
+00000b80: 2068 6f6c 6973 7469 6320 7379 7374 656d   holistic system
+00000b90: 2064 6573 6967 6e20 746f 6f6c 2e0a 0a23   design tool...#
+00000ba0: 2323 2048 6f77 205c 5b64 6f65 7320 6465  ## How \[does de
+00000bb0: 7369 676e 696e 6720 7769 7468 2066 6165  signing with fae
+00000bc0: 6272 796b 2077 6f72 6b5c 5d0a 0a66 6165  bryk work\]..fae
+00000bd0: 6272 796b 2069 7473 656c 6620 6973 206a  bryk itself is j
+00000be0: 7573 7420 6120 2a2a 7079 7468 6f6e 206c  ust a **python l
+00000bf0: 6962 7261 7279 2a2a 2074 6861 7420 796f  ibrary** that yo
+00000c00: 7520 696e 636c 7564 6520 696e 2079 6f75  u include in you
+00000c10: 7220 7072 6f6a 6563 742e 2049 7420 6973  r project. It is
+00000c20: 2070 726f 7669 6469 6e67 2079 6f75 2077   providing you w
+00000c30: 6974 6820 616c 6c20 7468 6520 746f 6f6c  ith all the tool
+00000c40: 7320 746f 2064 6573 6372 6962 6520 616e  s to describe an
+00000c50: 6420 6465 7369 676e 2079 6f75 7220 7379  d design your sy
+00000c60: 7374 656d 2061 6e64 2074 6f20 6578 706f  stem and to expo
+00000c70: 7274 2074 6861 7420 6465 7369 676e 2069  rt that design i
+00000c80: 6e74 6f20 736f 6d65 7468 696e 6720 7573  nto something us
+00000c90: 6566 756c 206c 696b 6520 666f 7220 6578  eful like for ex
+00000ca0: 616d 706c 6520 6120 6e65 746c 6973 742c  ample a netlist,
+00000cb0: 2061 2064 6576 6963 6574 7265 652c 2067   a devicetree, g
+00000cc0: 6572 6265 7273 2065 7463 2c20 7768 6963  erbers etc, whic
+00000cd0: 6820 796f 7520 7468 656e 2063 616e 2075  h you then can u
+00000ce0: 7365 2069 6e20 7468 6520 6e65 7874 2073  se in the next s
+00000cf0: 7465 7073 206f 6620 796f 7572 2070 726f  teps of your pro
+00000d00: 6a65 6374 2e20 4b65 7920 636f 6e63 6570  ject. Key concep
+00000d10: 7473 206f 6620 6661 6562 7279 6b20 6172  ts of faebryk ar
+00000d20: 6520 7468 6520 6772 6170 682c 2069 6d70  e the graph, imp
+00000d30: 6f72 7465 7273 2c20 6578 706f 7274 6572  orters, exporter
+00000d40: 732c 2074 6865 206c 6962 7261 7279 2061  s, the library a
+00000d50: 6e64 2074 6865 2075 7365 7220 6170 706c  nd the user appl
+00000d60: 6963 6174 696f 6e2e 0a54 6f20 756e 6465  ication..To unde
+00000d70: 7273 7461 6e64 2068 6f77 2074 6f20 7573  rstand how to us
+00000d80: 6520 6661 6562 7279 6b20 696e 2079 6f75  e faebryk in you
+00000d90: 7220 7072 6f6a 6563 7420 7365 6520 5b75  r project see [u
+00000da0: 7369 6e67 2066 6165 6272 796b 5d28 2375  sing faebryk](#u
+00000db0: 7369 6e67 2d66 6165 6272 796b 292e 0a0a  sing-faebryk)...
+00000dc0: 2323 2320 5768 6f20 5c5b 6973 2066 6165  ### Who \[is fae
+00000dd0: 6272 796b 5c5d 0a0a 6661 6562 7279 6b20  bryk\]..faebryk 
+00000de0: 6973 2061 2063 6f6d 6d75 6e69 7479 2064  is a community d
+00000df0: 7269 7665 6e20 7072 6f6a 6563 742e 2054  riven project. T
+00000e00: 6861 7420 6d65 616e 7320 6661 6562 7279  hat means faebry
+00000e10: 6b20 646f 6573 206e 6f74 206f 6e6c 7920  k does not only 
+00000e20: 636f 6e73 6973 7420 6f75 7420 6f66 2063  consist out of c
+00000e30: 6f72 6520 6465 7665 6c6f 7065 7273 2062  ore developers b
+00000e40: 7574 2061 6c73 6f20 7573 6572 732c 2065  ut also users, e
+00000e50: 7874 6572 6e61 6c20 636f 6e74 7269 6275  xternal contribu
+00000e60: 746f 7273 2c20 6d6f 6465 7261 746f 7273  tors, moderators
+00000e70: 2061 6e64 2079 6f75 2120 4974 2069 7320   and you! It is 
+00000e80: 666f 756e 6465 6420 6279 2061 2067 726f  founded by a gro
+00000e90: 7570 206f 6620 656d 6265 6464 6564 2c20  up of embedded, 
+00000ea0: 656c 6563 7472 6963 616c 2c20 7072 6f64  electrical, prod
+00000eb0: 7563 7420 6465 7369 676e 2061 6e64 2073  uct design and s
+00000ec0: 6f66 7477 6172 6520 656e 6769 6e65 6572  oftware engineer
+00000ed0: 7320 7769 7468 2061 206c 6f76 6520 666f  s with a love fo
+00000ee0: 7220 6d61 6b69 6e67 2e0a 0a23 2323 2057  r making...### W
+00000ef0: 6879 205c 5b64 6f20 7765 206d 616b 6520  hy \[do we make 
+00000f00: 6661 6562 7279 6b5c 5d0a 0a57 6520 6e6f  faebryk\]..We no
+00000f10: 7469 6365 6420 7468 6174 2074 6865 2069  ticed that the i
+00000f20: 6e6e 6f76 6174 696f 6e73 206f 6620 736f  nnovations of so
+00000f30: 6674 7761 7265 2065 6e67 696e 6565 7269  ftware engineeri
+00000f40: 6e67 2074 6861 7420 6d61 6b65 2066 6173  ng that make fas
+00000f50: 742c 2073 6361 6c61 626c 652c 2072 6f62  t, scalable, rob
+00000f60: 7573 7420 736f 6c75 7469 6f6e 7320 706f  ust solutions po
+00000f70: 7373 6962 6c65 2068 6176 6520 6e6f 7420  ssible have not 
+00000f80: 666f 756e 6420 7468 6569 7220 7761 7920  found their way 
+00000f90: 696e 746f 2068 6172 6477 6172 6520 6465  into hardware de
+00000fa0: 7369 676e 2e20 4675 7274 6865 726d 6f72  sign. Furthermor
+00000fb0: 6520 7468 6572 6520 6973 2061 206c 6f74  e there is a lot
+00000fc0: 206f 6620 6475 706c 6963 6174 6520 776f   of duplicate wo
+00000fd0: 726b 2064 6f6e 652e 2054 6869 6e6b 206f  rk done. Think o
+00000fe0: 6620 6465 7465 726d 696e 696e 6720 7468  f determining th
+00000ff0: 6520 7069 6e6f 7574 206f 6620 6120 536f  e pinout of a So
+00001000: 4320 616e 6420 7468 656e 2068 6176 696e  C and then havin
+00001010: 6720 746f 2074 7261 6e73 6c61 7465 2074  g to translate t
+00001020: 6861 7420 6578 6163 7420 7069 6e6f 7574  hat exact pinout
+00001030: 2069 6e74 6f20 736f 6674 7761 7265 2061   into software a
+00001040: 6761 696e 206f 7220 6861 7669 6e67 2074  gain or having t
+00001050: 6f20 636f 6e73 7461 6e74 6c79 2061 6461  o constantly ada
+00001060: 7074 2064 6573 6967 6e73 2066 6f72 2073  pt designs for s
+00001070: 7570 706c 7920 6368 6169 6e20 6973 7375  upply chain issu
+00001080: 6573 2e0a 4164 6469 7469 6f6e 616c 6c79  es..Additionally
+00001090: 2c20 6861 7264 7761 7265 2064 6573 6967  , hardware desig
+000010a0: 6e20 6861 7320 7175 6974 6520 6120 6269  n has quite a bi
+000010b0: 6720 6261 7272 6965 7220 6f66 2065 6e74  g barrier of ent
+000010c0: 7279 2066 6f72 206d 616b 6572 732c 2062  ry for makers, b
+000010d0: 7574 2077 6520 646f 6e27 7420 7468 696e  ut we don't thin
+000010e0: 6b20 6974 2068 6173 2074 6f2e 0a43 7572  k it has to..Cur
+000010f0: 7265 6e74 6c79 2068 6172 6477 6172 6520  rently hardware 
+00001100: 6465 7369 676e 2069 7320 616c 736f 2071  design is also q
+00001110: 7569 7465 206c 6162 6f72 2069 6e74 656e  uite labor inten
+00001120: 7369 7665 2077 6974 6820 7665 7279 206c  sive with very l
+00001130: 6974 746c 6520 6175 746f 6d61 7469 6f6e  ittle automation
+00001140: 2e0a 6661 6562 7279 6b20 6169 6d73 2074  ..faebryk aims t
+00001150: 6f20 7461 636b 6c65 2061 6c6c 2074 686f  o tackle all tho
+00001160: 7365 2069 7373 7565 7320 616e 6420 616c  se issues and al
+00001170: 736f 206f 7065 6e73 2075 7020 736f 6d65  so opens up some
+00001180: 2065 7863 6974 696e 6720 706f 7373 6962   exciting possib
+00001190: 696c 6974 6965 732c 2073 7563 6820 6173  ilities, such as
+000011a0: 2062 656e 6566 6974 696e 6720 6672 6f6d   benefiting from
+000011b0: 2074 6865 2076 6572 7369 6f6e 206d 616e   the version man
+000011c0: 6167 656d 656e 7420 616e 6420 636f 6c6c  agement and coll
+000011d0: 6162 6f72 6174 696f 6e20 746f 6f6c 7320  aboration tools 
+000011e0: 7468 6174 2061 7265 2075 7365 6420 696e  that are used in
+000011f0: 206d 6f64 6572 6e20 736f 6674 7761 7265   modern software
+00001200: 2064 6576 656c 6f70 6d65 6e74 2e0a 0a23   development...#
+00001210: 2323 2057 6865 6e20 5c5b 6973 2066 6165  ## When \[is fae
+00001220: 6272 796b 2062 6569 6e67 2064 6576 656c  bryk being devel
+00001230: 6f70 6564 5c5d 0a0a 6661 6562 7279 6b20  oped\]..faebryk 
+00001240: 6973 2062 6569 6e67 2063 6f6e 7469 6e75  is being continu
+00001250: 6f75 736c 7920 6465 7665 6c6f 7065 642e  ously developed.
+00001260: 0a54 6865 2063 6f72 6520 7465 616d 2066  .The core team f
+00001270: 6f63 7573 6573 206f 6e20 636f 7265 2066  ocuses on core f
+00001280: 756e 6374 696f 6e61 6c69 7479 2061 6e64  unctionality and
+00001290: 2066 6561 7475 7265 7320 6f66 2066 6165   features of fae
+000012a0: 6272 796b 2c20 6173 2077 656c 6c20 6173  bryk, as well as
+000012b0: 2074 6865 2067 656e 6572 616c 2064 6972   the general dir
+000012c0: 6563 7469 6f6e 206f 6620 7468 6520 7072  ection of the pr
+000012d0: 6f6a 6563 742e 0a54 6865 2073 7472 656e  oject..The stren
+000012e0: 6774 6820 6f66 2074 6865 2063 6f6d 6d75  gth of the commu
+000012f0: 6e69 7479 2063 616e 2072 6561 6c6c 7920  nity can really 
+00001300: 7368 696e 6520 7769 7468 2074 6865 2064  shine with the d
+00001310: 6576 656c 6f70 6d65 6e74 206f 6620 696d  evelopment of im
+00001320: 706f 7274 6572 732c 2065 7870 6f72 7465  porters, exporte
+00001330: 7273 2c20 6c69 6272 6172 6965 732c 2061  rs, libraries, a
+00001340: 6e64 2070 726f 6a65 6374 732c 2062 7574  nd projects, but
+00001350: 2065 7665 7279 6f6e 6520 6973 2077 656c   everyone is wel
+00001360: 636f 6d65 2074 6f20 5b68 656c 705d 2823  come to [help](#
+00001370: 636f 6d6d 756e 6974 792d 7375 7070 6f72  community-suppor
+00001380: 7429 206f 7574 2077 6865 7265 2074 6865  t) out where the
+00001390: 7920 6361 6e2e 0a0a 2323 2320 5768 6572  y can...### Wher
+000013a0: 6520 5c5b 646f 2077 6520 6465 7665 6c6f  e \[do we develo
+000013b0: 7020 6661 6562 7279 6b5c 5d0a 0a66 6165  p faebryk\]..fae
+000013c0: 6272 796b 2069 7320 6265 696e 6720 6465  bryk is being de
+000013d0: 7665 6c6f 7065 6420 636f 6d70 6c65 7465  veloped complete
+000013e0: 6c79 2069 6e20 7468 6520 6f70 656e 206f  ly in the open o
+000013f0: 6e20 4769 7468 7562 2e0a 416c 6c20 7468  n Github..All th
+00001400: 6520 696e 666f 726d 6174 696f 6e20 796f  e information yo
+00001410: 7520 6e65 6564 2074 6f20 7374 6172 7420  u need to start 
+00001420: 7573 696e 6720 616e 6420 636f 6e74 7269  using and contri
+00001430: 6275 7469 6e67 2074 6f20 6661 6562 7279  buting to faebry
+00001440: 6b20 7769 6c6c 2062 6520 696e 206f 7220  k will be in or 
+00001450: 6c69 6e6b 6564 2074 6f20 6672 6f6d 205b  linked to from [
+00001460: 7468 6973 2072 6570 6f73 6974 6f72 795d  this repository]
+00001470: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001480: 636f 6d2f 6661 6562 7279 6b2f 6661 6562  com/faebryk/faeb
+00001490: 7279 6b29 2e0a 4966 2079 6f75 2068 6176  ryk)..If you hav
+000014a0: 6520 616e 7920 7175 6573 7469 6f6e 7320  e any questions 
+000014b0: 796f 7520 6361 6e20 6173 6b20 7468 656d  you can ask them
+000014c0: 206f 6e20 6f75 7220 5b44 6973 636f 7264   on our [Discord
+000014d0: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
+000014e0: 642e 6767 2f39 356a 5975 506d 6e55 5729  d.gg/95jYuPmnUW)
+000014f0: 2e0a 466f 7220 7075 6c6c 2072 6571 7565  ..For pull reque
+00001500: 7374 7320 616e 6420 6275 672d 7265 706f  sts and bug-repo
+00001510: 7274 732c 2073 6565 206f 7572 205b 636f  rts, see our [co
+00001520: 6e74 7269 6275 7469 6e67 2067 7569 6465  ntributing guide
+00001530: 6c69 6e65 735d 2864 6f63 732f 434f 4e54  lines](docs/CONT
+00001540: 5249 4255 5449 4e47 2e6d 6429 2e0a 0a2d  RIBUTING.md)...-
+00001550: 2d2d 0a0a 2323 2044 6576 656c 6f70 6d65  --..## Developme
+00001560: 6e74 0a0a 2323 2320 496e 7374 616c 6c69  nt..### Installi
+00001570: 6e67 2066 726f 6d20 736f 7572 6365 0a53  ng from source.S
+00001580: 6574 7570 0a0a 6060 6062 6173 680a 3e20  etup..```bash.> 
+00001590: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
+000015a0: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6165  //github.com/fae
+000015b0: 6272 796b 2f66 6165 6272 796b 2e67 6974  bryk/faebryk.git
+000015c0: 0a3e 2063 6420 6661 6562 7279 6b0a 3e0a  .> cd faebryk.>.
+000015d0: 3e20 706f 6574 7279 2069 6e73 7461 6c6c  > poetry install
+000015e0: 0a60 6060 0a0a 5275 6e6e 696e 6720 6578  .```..Running ex
+000015f0: 616d 706c 6573 0a0a 6060 6062 6173 680a  amples..```bash.
+00001600: 3e20 706f 6574 7279 2073 6865 6c6c 0a3e  > poetry shell.>
+00001610: 2070 7974 686f 6e20 2e2f 6578 616d 706c   python ./exampl
+00001620: 6573 2f3c 7361 6d70 6c65 5f6e 616d 653e  es/<sample_name>
+00001630: 2e70 790a 6060 600a 0a23 2323 2056 6572  .py.```..### Ver
+00001640: 7369 6f6e 696e 670a 0a66 6165 6272 796b  sioning..faebryk
+00001650: 2075 7365 7320 5b73 656d 616e 7469 6320   uses [semantic 
+00001660: 7665 7273 696f 6e69 6e67 5d28 6874 7470  versioning](http
+00001670: 733a 2f2f 7365 6d76 6572 2e6f 7267 2f29  s://semver.org/)
+00001680: 2069 6e20 7468 6520 5b72 656c 6561 7365   in the [release
+00001690: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+000016a0: 622e 636f 6d2f 6661 6562 7279 6b2f 6661  b.com/faebryk/fa
+000016b0: 6562 7279 6b2f 7265 6c65 6173 6573 292e  ebryk/releases).
+000016c0: 0a0a 4173 2066 6561 6272 796b 2069 7320  ..As feabryk is 
+000016d0: 7374 696c 6c20 696e 2074 6865 2065 6172  still in the ear
+000016e0: 6c79 2073 7461 6765 7320 6f66 2064 6576  ly stages of dev
+000016f0: 656c 6f70 6d65 6e74 206e 6577 2072 656c  elopment new rel
+00001700: 6561 7365 7320 7769 6c6c 2068 6176 6520  eases will have 
+00001710: 6120 6c6f 7420 6f66 2028 6272 6561 6b69  a lot of (breaki
+00001720: 6e67 2920 6368 616e 6765 7320 696e 2074  ng) changes in t
+00001730: 6865 6d2e 0a4f 7572 205b 726f 6164 6d61  hem..Our [roadma
+00001740: 705d 2823 7665 7273 696f 6e69 6e67 2928  p](#versioning)(
+00001750: 544f 444f 2920 7769 6c6c 2073 686f 7720  TODO) will show 
+00001760: 796f 7520 7768 6572 6520 7468 6520 7072  you where the pr
+00001770: 6f6a 6563 7420 6973 2067 6f69 6e67 2074  oject is going t
+00001780: 6f20 616e 6420 7768 6174 2079 6f75 2063  o and what you c
+00001790: 616e 2065 7870 6563 7420 696e 2066 7574  an expect in fut
+000017a0: 7572 6520 7265 6c65 6173 6573 2e0a 0a23  ure releases...#
+000017b0: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+000017c0: 0a53 6565 205b 434f 4e54 5249 4255 5449  .See [CONTRIBUTI
+000017d0: 4e47 2e6d 645d 2864 6f63 732f 434f 4e54  NG.md](docs/CONT
+000017e0: 5249 4255 5449 4e47 2e6d 6429 0a0a 546f  RIBUTING.md)..To
+000017f0: 2067 6574 2069 6e73 7069 7261 7469 6f6e   get inspiration
+00001800: 206f 6e20 7468 696e 6773 2074 6f20 776f   on things to wo
+00001810: 726b 206f 6e20 6368 6563 6b20 6f75 7420  rk on check out 
+00001820: 7468 6520 6973 7375 6573 2e0a 0a23 2323  the issues...###
+00001830: 2320 5275 6e6e 696e 6720 796f 7572 206f  # Running your o
+00001840: 776e 2065 7870 6572 696d 656e 7473 2f4d  wn experiments/M
+00001850: 616b 696e 6720 7361 6d70 6c65 730a 0a46  aking samples..F
+00001860: 6972 7374 2066 6f6c 6c6f 7720 7468 6520  irst follow the 
+00001870: 7374 6570 7320 696e 2067 6574 2072 756e  steps in get run
+00001880: 6e69 6e67 2066 726f 6d20 736f 7572 6365  ning from source
+00001890: 2e0a 5468 656e 2061 6464 2061 2066 696c  ..Then add a fil
+000018a0: 6520 696e 2065 7861 6d70 6c65 732f 2028  e in examples/ (
+000018b0: 796f 7520 6361 6e20 7573 6520 6f6e 6520  you can use one 
+000018c0: 6f66 2074 6865 2065 7861 6d70 6c65 7320  of the examples 
+000018d0: 6173 2074 656d 706c 6174 6529 2e0a 4361  as template)..Ca
+000018e0: 6c6c 2079 6f75 7220 6669 6c65 2077 6974  ll your file wit
+000018f0: 6820 6070 7974 686f 6e33 2065 7861 6d70  h `python3 examp
+00001900: 6c65 732f 3c79 6f75 7266 696c 653e 2e70  les/<yourfile>.p
+00001910: 7960 2e0a 0a23 2323 2320 5275 6e6e 696e  y`...#### Runnin
+00001920: 6720 7465 7374 730a 0a52 756e 0a0a 6060  g tests..Run..``
+00001930: 6062 6173 680a 3e20 7079 7465 7374 2074  `bash.> pytest t
+00001940: 6573 740a 6060 600a 0a23 2320 436f 6d6d  est.```..## Comm
+00001950: 756e 6974 7920 5375 7070 6f72 740a 0a43  unity Support..C
+00001960: 6f6d 6d75 6e69 7479 2073 7570 706f 7274  ommunity support
+00001970: 2069 7320 7072 6f76 6964 6564 2076 6961   is provided via
+00001980: 2044 6973 636f 7264 3b20 7365 6520 7468   Discord; see th
+00001990: 6520 5265 736f 7572 6365 7320 6265 6c6f  e Resources belo
+000019a0: 7720 666f 7220 6465 7461 696c 732e 0a0a  w for details...
+000019b0: 2323 2320 5265 736f 7572 6365 730a 0a2d  ### Resources..-
+000019c0: 2053 6f75 7263 6520 436f 6465 3a20 3c68   Source Code: <h
+000019d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000019e0: 6d2f 6661 6562 7279 6b2f 6661 6562 7279  m/faebryk/faebry
+000019f0: 6b3e 0a2d 2043 6861 743a 2052 6561 6c2d  k>.- Chat: Real-
+00001a00: 7469 6d65 2063 6861 7420 6861 7070 656e  time chat happen
+00001a10: 7320 696e 2066 6165 6272 796b 2773 2044  s in faebryk's D
+00001a20: 6973 636f 7264 2053 6572 7665 722e 2055  iscord Server. U
+00001a30: 7365 2074 6869 7320 4469 7363 6f72 6420  se this Discord 
+00001a40: 5b49 6e76 6974 655d 2868 7474 7073 3a2f  [Invite](https:/
+00001a50: 2f64 6973 636f 7264 2e67 672f 3935 6a59  /discord.gg/95jY
+00001a60: 7550 6d6e 5557 2920 746f 2072 6567 6973  uPmnUW) to regis
+00001a70: 7465 720a 2d20 4973 7375 6573 3a20 3c68  ter.- Issues: <h
+00001a80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001a90: 6d2f 6661 6562 7279 6b2f 6661 6562 7279  m/faebryk/faebry
+00001aa0: 6b2f 6973 7375 6573 3e0a                 k/issues>.
```

