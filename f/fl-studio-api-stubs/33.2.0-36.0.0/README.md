# Comparing `tmp/fl_studio_api_stubs-33.2.0.tar.gz` & `tmp/fl_studio_api_stubs-36.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl_studio_api_stubs-33.2.0.tar", max compression
+gzip compressed data, was "fl_studio_api_stubs-36.0.0.tar", max compression
```

## Comparing `fl_studio_api_stubs-33.2.0.tar` & `fl_studio_api_stubs-36.0.0.tar`

### file list

```diff
@@ -1,109 +1,4 @@
--rw-r--r--   0        0        0     7642 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/LICENSE.md
--rwxr-xr-x   0        0        0     2519 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/README.md
--rw-r--r--   0        0        0     2945 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/pyproject.toml
--rw-r--r--   0        0        0     3020 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/arrangement/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/arrangement/py.typed
--rw-r--r--   0        0        0     2345 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/channels/__init__.py
--rw-r--r--   0        0        0     1821 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/channels/__notes.py
--rw-r--r--   0        0        0    24796 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/channels/__properties.py
--rw-r--r--   0        0        0     6865 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/channels/__sequencer.py
--rw-r--r--   0        0        0     4050 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/channels/__ui.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/channels/py.typed
--rw-r--r--   0        0        0     7058 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/device/__device.py
--rw-r--r--   0        0        0     3300 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/device/__dispatch.py
--rw-r--r--   0        0        0     5249 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/device/__fl.py
--rw-r--r--   0        0        0     1757 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/device/__init__.py
--rw-r--r--   0        0        0     1902 2024-01-21 12:02:43.947190 fl_studio_api_stubs-33.2.0/src/device/__util.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/device/py.typed
--rw-r--r--   0        0        0      713 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/enveditor/__init__.py
--rw-r--r--   0        0        0     7538 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/enveditor/__sample.py
--rw-r--r--   0        0        0     3336 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/enveditor/__script_dialog.py
--rw-r--r--   0        0        0     1172 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/enveditor/__utils.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/enveditor/py.typed
--rw-r--r--   0        0        0       42 2024-01-21 12:02:44.315187 fl_studio_api_stubs-33.2.0/src/fl_classes/.git
--rw-r--r--   0        0        0     1366 2024-01-21 12:02:44.323187 fl_studio_api_stubs-33.2.0/src/fl_classes/.gitignore
--rw-r--r--   0        0        0     7642 2024-01-21 12:02:44.323187 fl_studio_api_stubs-33.2.0/src/fl_classes/LICENSE.md
--rw-r--r--   0        0        0      283 2024-01-21 12:02:44.323187 fl_studio_api_stubs-33.2.0/src/fl_classes/README.md
--rw-r--r--   0        0        0    20163 2024-01-21 12:02:44.323187 fl_studio_api_stubs-33.2.0/src/fl_classes/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:44.323187 fl_studio_api_stubs-33.2.0/src/fl_classes/py.typed
--rw-r--r--   0        0        0      739 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/__init__.py
--rw-r--r--   0        0        0     8350 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/channels.py
--rw-r--r--   0        0        0      444 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/configuration/__init__.py
--rw-r--r--   0        0        0      665 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/configuration/config_typings.py
--rw-r--r--   0        0        0      170 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/configuration/default.json
--rw-r--r--   0        0        0     1383 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/configuration/load_data.py
--rw-r--r--   0        0        0     1463 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/configuration/schema.json
--rw-r--r--   0        0        0      775 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/configuration/target_version.py
--rw-r--r--   0        0        0     5535 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/consts.py
--rw-r--r--   0        0        0     2930 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/decorators.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/device.py
--rw-r--r--   0        0        0     6524 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/emulation.py
--rw-r--r--   0        0        0     2683 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/exceptions.py
--rw-r--r--   0        0        0       40 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/helpers/__init__.py
--rw-r--r--   0        0        0     1114 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/helpers/file_from_here.py
--rw-r--r--   0        0        0     1331 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/__init__.py
--rw-r--r--   0        0        0     1746 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/channels.py
--rw-r--r--   0        0        0      604 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/device.py
--rw-r--r--   0        0        0     2406 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/general.py
--rw-r--r--   0        0        0     1633 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/mixer.py
--rw-r--r--   0        0        0     2688 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/pattern.py
--rw-r--r--   0        0        0      532 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/plugin.py
--rw-r--r--   0        0        0      618 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/transport.py
--rw-r--r--   0        0        0     1178 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/models/ui.py
--rw-r--r--   0        0        0     1407 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/patterns.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/py.typed
--rw-r--r--   0        0        0     1928 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/state.py
--rw-r--r--   0        0        0      337 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/fl_model/util.py
--rw-r--r--   0        0        0      663 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/flpianoroll/__init__.py
--rw-r--r--   0        0        0     3026 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/flpianoroll/__marker.py
--rw-r--r--   0        0        0     4416 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/flpianoroll/__note.py
--rw-r--r--   0        0        0     3997 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/flpianoroll/__score.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/flpianoroll/py.typed
--rw-r--r--   0        0        0     4501 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/general/__fl_state.py
--rw-r--r--   0        0        0     1096 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/general/__init__.py
--rw-r--r--   0        0        0     6966 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/general/__undo.py
--rw-r--r--   0        0        0     2730 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/general/__undo_proposed.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/general/py.typed
--rw-r--r--   0        0        0      853 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/launchMapPages/__init__.py
--rw-r--r--   0        0        0     3437 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/launchMapPages/__launchMapPages.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/launchMapPages/py.typed
--rw-r--r--   0        0        0      462 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/midi/__encode.py
--rw-r--r--   0        0        0    17402 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/midi/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/midi/py.typed
--rw-r--r--   0        0        0     3898 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/mixer/__events.py
--rw-r--r--   0        0        0     2871 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/mixer/__init__.py
--rw-r--r--   0        0        0     3890 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/mixer/__properties.py
--rw-r--r--   0        0        0     2085 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/mixer/__selection.py
--rw-r--r--   0        0        0    15818 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/mixer/__tracks.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/mixer/py.typed
--rw-r--r--   0        0        0     1446 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/patterns/__groups.py
--rw-r--r--   0        0        0      318 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/patterns/__helpers.py
--rw-r--r--   0        0        0     1504 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/patterns/__init__.py
--rw-r--r--   0        0        0     1107 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/patterns/__performance.py
--rw-r--r--   0        0        0    10333 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/patterns/__properties.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/patterns/py.typed
--rw-r--r--   0        0        0     2146 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/playlist/__init__.py
--rw-r--r--   0        0        0    11758 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/playlist/__performance.py
--rw-r--r--   0        0        0     7165 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/playlist/__tracks.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/playlist/py.typed
--rw-r--r--   0        0        0     2454 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/plugins/__init__.py
--rw-r--r--   0        0        0    13076 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/plugins/__plugins.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/plugins/py.typed
--rw-r--r--   0        0        0     4001 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/screen/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/screen/py.typed
--rw-r--r--   0        0        0      922 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/transport/__init__.py
--rw-r--r--   0        0        0     3088 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/transport/__position.py
--rw-r--r--   0        0        0     9383 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/transport/__state.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/transport/py.typed
--rw-r--r--   0        0        0     3889 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/__browser.py
--rw-r--r--   0        0        0     1547 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/__editors.py
--rw-r--r--   0        0        0     7228 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/__fl_state.py
--rw-r--r--   0        0        0     2986 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/__init__.py
--rw-r--r--   0        0        0     2872 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/__keyboard.py
--rw-r--r--   0        0        0     3688 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/__navigation.py
--rw-r--r--   0        0        0     2557 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/__overlays.py
--rw-r--r--   0        0        0     5685 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/__windows.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/ui/py.typed
--rw-r--r--   0        0        0    11401 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 12:02:43.951190 fl_studio_api_stubs-33.2.0/src/utils/py.typed
--rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 fl_studio_api_stubs-33.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7642 2024-05-28 10:53:31.153757 fl_studio_api_stubs-36.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3962 2024-05-28 13:46:50.769735 fl_studio_api_stubs-36.0.0/README.md
+-rw-r--r--   0        0        0     3893 2024-05-28 14:06:25.260400 fl_studio_api_stubs-36.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 fl_studio_api_stubs-36.0.0/PKG-INFO
```

### Comparing `fl_studio_api_stubs-33.2.0/LICENSE.md` & `fl_studio_api_stubs-36.0.0/LICENSE.md`

 * *Files identical despite different names*

