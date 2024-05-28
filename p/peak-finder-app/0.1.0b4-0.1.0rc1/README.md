# Comparing `tmp/peak_finder_app-0.1.0b4.tar.gz` & `tmp/peak_finder_app-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peak_finder_app-0.1.0b4.tar", max compression
+gzip compressed data, was "peak_finder_app-0.1.0rc1.tar", max compression
```

## Comparing `peak_finder_app-0.1.0b4.tar` & `peak_finder_app-0.1.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 peak_finder_app-0.1.0b4/LICENSE
--rw-r--r--   0        0        0      970 2024-05-06 01:50:01.813417 peak_finder_app-0.1.0b4/peak_finder/__init__.py
--rw-r--r--   0        0        0      866 2024-04-23 22:39:24.314550 peak_finder_app-0.1.0b4/peak_finder/anomaly.py
--rw-r--r--   0        0        0     8372 2024-04-23 22:39:24.314612 peak_finder_app-0.1.0b4/peak_finder/anomaly_group.py
--rw-r--r--   0        0        0    78823 2024-04-23 22:39:24.315729 peak_finder_app-0.1.0b4/peak_finder/application.py
--rw-r--r--   0        0        0     1785 2024-04-23 22:39:24.315729 peak_finder_app-0.1.0b4/peak_finder/constants.py
--rw-r--r--   0        0        0    15078 2024-04-23 22:39:24.316280 peak_finder_app-0.1.0b4/peak_finder/driver.py
--rw-r--r--   0        0        0   356591 2024-04-23 22:39:24.319046 peak_finder_app-0.1.0b4/peak_finder/images/peak_finder_app.png
--rw-r--r--   0        0        0    15808 2024-04-23 22:39:24.319046 peak_finder_app-0.1.0b4/peak_finder/layout.py
--rw-r--r--   0        0        0    10882 2024-04-23 22:39:24.319593 peak_finder_app-0.1.0b4/peak_finder/line_anomaly.py
--rw-r--r--   0        0        0    11584 2024-04-23 22:39:24.320130 peak_finder_app-0.1.0b4/peak_finder/line_data.py
--rw-r--r--   0        0        0    11849 2024-04-23 22:39:24.320197 peak_finder_app-0.1.0b4/peak_finder/line_group.py
--rw-r--r--   0        0        0    11812 2024-04-23 22:39:24.320728 peak_finder_app-0.1.0b4/peak_finder/line_position.py
--rw-r--r--   0        0        0    13241 2024-04-23 22:39:24.321386 peak_finder_app-0.1.0b4/peak_finder/params.py
--rw-r--r--   0        0        0     1106 2024-04-23 22:39:24.321970 peak_finder_app-0.1.0b4/peak_finder/utils.py
--rw-r--r--   0        0        0      117 2024-04-23 22:39:24.312898 peak_finder_app-0.1.0b4/peak_finder-assets/__init__.py
--rw-r--r--   0        0        0  1983716 2024-04-23 22:39:24.854255 peak_finder_app-0.1.0b4/peak_finder-assets/FlinFlon_tem_aoi.geoh5
--rw-r--r--   0        0        0     6446 2024-05-02 04:28:11.322688 peak_finder_app-0.1.0b4/peak_finder-assets/uijson/peak_finder.ui.json
--rw-r--r--   0        0        0     5684 2024-05-06 01:48:12.028817 peak_finder_app-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0     6280 2024-04-28 20:57:34.791039 peak_finder_app-0.1.0b4/README.rst
--rw-r--r--   0        0        0     6573 2024-04-23 22:39:23.613401 peak_finder_app-0.1.0b4/THIRD_PARTY_SOFTWARE.rst
--rw-r--r--   0        0        0     8283 1970-01-01 00:00:00.000000 peak_finder_app-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-05-21 17:35:01.387711 peak_finder_app-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0      968 2024-05-28 16:28:24.872918 peak_finder_app-0.1.0rc1/peak_finder/__init__.py
+-rw-r--r--   0        0        0      866 2024-05-21 17:35:02.069892 peak_finder_app-0.1.0rc1/peak_finder/anomaly.py
+-rw-r--r--   0        0        0     4488 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder/anomaly_group.py
+-rw-r--r--   0        0        0    79833 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder/application.py
+-rw-r--r--   0        0        0     1785 2024-05-21 17:35:02.071000 peak_finder_app-0.1.0rc1/peak_finder/constants.py
+-rw-r--r--   0        0        0    15164 2024-05-28 16:44:35.319139 peak_finder_app-0.1.0rc1/peak_finder/driver.py
+-rw-r--r--   0        0        0   356591 2024-05-21 17:35:02.072980 peak_finder_app-0.1.0rc1/peak_finder/images/peak_finder_app.png
+-rw-r--r--   0        0        0    15847 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder/layout.py
+-rw-r--r--   0        0        0    10584 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder/line_anomaly.py
+-rw-r--r--   0        0        0    11835 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder/line_data.py
+-rw-r--r--   0        0        0    11735 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder/line_group.py
+-rw-r--r--   0        0        0     9757 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder/line_position.py
+-rw-r--r--   0        0        0    13769 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder/params.py
+-rw-r--r--   0        0        0     1106 2024-05-21 17:35:02.074134 peak_finder_app-0.1.0rc1/peak_finder/utils.py
+-rw-r--r--   0        0        0      117 2024-05-21 17:35:02.069298 peak_finder_app-0.1.0rc1/peak_finder-assets/__init__.py
+-rw-r--r--   0        0        0  1983716 2024-05-21 17:35:02.598544 peak_finder_app-0.1.0rc1/peak_finder-assets/FlinFlon_tem_aoi.geoh5
+-rw-r--r--   0        0        0     6546 2024-05-21 17:35:54.192132 peak_finder_app-0.1.0rc1/peak_finder-assets/uijson/peak_finder.ui.json
+-rw-r--r--   0        0        0     5682 2024-05-28 16:29:35.334551 peak_finder_app-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7236 2024-05-21 19:53:38.927852 peak_finder_app-0.1.0rc1/README.rst
+-rw-r--r--   0        0        0     6573 2024-05-21 17:35:01.387711 peak_finder_app-0.1.0rc1/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     9214 1970-01-01 00:00:00.000000 peak_finder_app-0.1.0rc1/PKG-INFO
```

### Comparing `peak_finder_app-0.1.0b4/LICENSE` & `peak_finder_app-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b4/peak_finder/__init__.py` & `peak_finder_app-0.1.0rc1/peak_finder/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of peak-finder-app project.
 #
 #  All rights reserved.
 #
 
-__version__ = "0.1.0-beta.4"
+__version__ = "0.1.0-rc.1"
 import os
 import warnings
 from pathlib import Path
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/anomaly.py` & `peak_finder_app-0.1.0rc1/peak_finder/anomaly.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b4/peak_finder/application.py` & `peak_finder_app-0.1.0rc1/peak_finder/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from geoh5py.shared.utils import fetch_active_workspace, is_uuid
 from geoh5py.ui_json import InputFile
 from tqdm import tqdm
 
 from peak_finder.anomaly_group import AnomalyGroup
 from peak_finder.driver import PeakFinderDriver
 from peak_finder.layout import peak_finder_layout
+from peak_finder.line_position import LinePosition
 from peak_finder.params import PeakFinderParams
 from peak_finder.utils import get_ordered_survey_lines
 
 
 class PeakFinder(
     BaseDashApplication
 ):  # pylint: disable=too-many-public-methods, too-many-instance-attributes
@@ -60,17 +61,18 @@
 
         :param ui_json: ui.json file to load.
         :param ui_json_data: Data from ui.json file.
         :param params: Peak finder params.
         """
         self._active_channels: dict | None = None
         self._figure = None
+        self._line_field: ReferencedData | None = None
         self._line_indices = None
         self._computed_lines = None
-        self._survey = None
+        self._survey: Curve | None = None
         self._property_groups = None
         self._ordered_survey_lines: dict | None = None
 
         super().__init__(ui_json, ui_json_data, params)
 
         self._app = None
 
@@ -307,15 +309,21 @@
         Line labels for survey.
         """
         return self._line_field
 
     @line_field.setter
     def line_field(self, value):
         if is_uuid(value):
-            self._line_field = self.workspace.get_entity(uuid.UUID(value))
+            data = self.workspace.get_entity(uuid.UUID(value))[0]
+
+            if not isinstance(data, ReferencedData):
+                raise TypeError("Line field must be of type ReferencedData.")
+
+            self._line_field = data
+
         elif isinstance(value, ReferencedData):
             self._line_field = value
         else:
             self._line_field = None
 
     @property
     def computed_lines(self) -> dict | None:
@@ -333,18 +341,15 @@
         """
         Current survey object.
         """
         if self._survey is None:
             self.workspace: Workspace = Workspace()
             with fetch_active_workspace(self.params.geoh5):
                 self._survey = self.params.objects.copy(parent=self.workspace)
-                line_field = self.workspace.get_entity(self.params.line_field.uid)[0]
-
-                if isinstance(line_field, ReferencedData):
-                    self._line_field = line_field
+                self._line_field = self.params.get_line_field(self._survey)
 
             self._active_channels = None
             self._ordered_survey_lines = None
 
         return self._survey
 
     @property
@@ -391,36 +396,38 @@
 
         self.property_groups = property_groups
 
         self.app.layout.children += [
             dcc.Store(id="trace_map", data=trace_map),
         ]
 
-        # Line dropdown options
-        selected_line_options = [
-            {"label": label, "value": id}
-            for id, label in self.ordered_survey_lines.items()
-        ]
-        # Initial line
-        selected_line = None
-        if len(selected_line_options) > 0:
-            selected_line = selected_line_options[0]["value"]
-
-        specify_values = {
-            "selected_line": [
-                {"property": "options", "value": selected_line_options},
-                {"property": "value", "value": selected_line},
-            ],
-            "group_name": [
-                {
-                    "property": "options",
-                    "value": list(self.property_groups.keys()),
-                }
-            ],
-        }
+        specify_values = {}
+        if self.ordered_survey_lines is not None and self.property_groups is not None:
+            # Line dropdown options
+            selected_line_options = [
+                {"label": label, "value": id}
+                for id, label in self.ordered_survey_lines.items()
+            ]
+            # Initial line
+            selected_line = None
+            if len(selected_line_options) > 0:
+                selected_line = selected_line_options[0]["value"]
+
+            specify_values = {
+                "selected_line": [
+                    {"property": "options", "value": selected_line_options},
+                    {"property": "value", "value": selected_line},
+                ],
+                "group_name": [
+                    {
+                        "property": "options",
+                        "value": list(self.property_groups.keys()),
+                    }
+                ],
+            }
 
         BaseDashApplication.init_vals(
             self.app.layout.children, self._ui_json_data, kwargs=specify_values
         )
 
     @staticmethod
     def update_plot_visibility(plot_selection: list[str]) -> tuple:
@@ -704,43 +711,45 @@
             for key in entries_to_remove:
                 self.computed_lines.pop(key, None)
         else:
             self.computed_lines = {}
 
         # Add new lines
         for line_anomaly in tqdm(results):
-            # Add anomalies to self.lines
+
+            if "n_lines" in triggers and line_anomaly.line_id in self.computed_lines:
+                continue
+
             line_groups = line_anomaly.anomalies
             line_anomalies: list[AnomalyGroup] = []
             if line_groups is not None:
                 for line_group in line_groups:
                     line_anomalies += line_group.groups
+
             if line_anomaly.line_id not in self.computed_lines:
                 self.computed_lines[line_anomaly.line_id] = {
                     "position": [],
                     "anomalies": [],
                     "plot_line_start": np.inf,
                 }
 
-            if not line_anomalies:
-                continue
-
-            self.computed_lines[line_anomaly.line_id]["anomalies"].append(
-                line_anomalies
-            )
             # Add position to self.lines
             self.computed_lines[line_anomaly.line_id]["position"].append(
                 line_anomaly.position
             )
 
             self.computed_lines[line_anomaly.line_id]["plot_line_start"] = min(
                 np.min(line_anomaly.position.locations_resampled),
                 self.computed_lines[line_anomaly.line_id]["plot_line_start"],
             )
 
+            self.computed_lines[line_anomaly.line_id]["anomalies"].append(
+                line_anomalies
+            )
+
         return lines_computation_trigger + 1
 
     def update_selected_line_figure(self, *args) -> go.Figure | None:
         """
         :param args: Triggers for updating the figure.
 
         :return: Updated figure.
@@ -791,15 +800,15 @@
         sign = 1
         if flip_sign:
             sign *= -1
 
         y_min, y_max = np.inf, -np.inf
         log = y_scale == "symlog"
         threshold = np.float_power(10, linear_threshold)
-        all_values = []
+        values_list = []
 
         trace_dict: dict[str, dict[str, dict]] = {
             "lines": {
                 "lines": {
                     "x": [None],
                     "y": [None],
                 }
@@ -823,15 +832,15 @@
                 locs = position.locations_resampled
 
                 if position.line_indices.sum() < 2 or locs is None:
                     continue
 
                 values = full_values[position.line_indices]
                 values, _ = position.resample_values(values)
-                all_values += list(values.flatten())
+                values_list += list(values.flatten())
 
                 if log:
                     sym_values = symlog(values, threshold)
                 else:
                     sym_values = values
 
                 y_min = np.nanmin([sym_values.min(), y_min])
@@ -869,15 +878,15 @@
                             trace_dict["property_groups"][group_name][
                                 "customdata"
                             ] += list(values[start:end]) + [None]
 
         if np.isinf(y_min) or self.property_groups is None:
             return no_update, None, None, None
 
-        all_values = np.array(all_values)
+        all_values = np.array(values_list)
         _, y_label, y_tickvals, y_ticktext = format_axis(
             channel="Data",
             axis=all_values,
             log=log,
             threshold=threshold,
         )
 
@@ -915,16 +924,17 @@
         # Update figure layout
         self.update_figure_layout(
             y_label,
             y_tickvals,
             y_ticktext,
             y_min,
             y_max,
-            min_value,
+            symlog(min_value, threshold),
             x_label,
+            self.computed_lines[selected_line]["position"],
         )
         return (
             figure_lines_trigger + 1,
             thresh_min,
             thresh_max,
             thresh_ticks,
         )
@@ -1513,14 +1523,15 @@
         y_label: str | None,
         y_tickvals: np.ndarray | None,
         y_ticktext: list[str] | None,
         y_min: float | None,
         y_max: float | None,
         min_value: float,
         x_label: str,
+        line_position: LinePosition,
     ):
         """
         Update the figure layout.
 
         :param y_label: Label for y-axis.
         :param y_tickvals: Y-axis tick values.
         :param y_ticktext: Y-axis tick text.
@@ -1955,14 +1966,15 @@
         with fetch_active_workspace(self.params.geoh5) as workspace:
             param_dict = self.get_params_dict(locals())
             param_dict.update(
                 {
                     "geoh5": workspace,
                     "objects": self.params.objects,
                     "line_field": self.params.line_field,
+                    "monitoring_directory": self.params.monitoring_directory,
                 }
             )
 
             if masking_data == "None":
                 param_dict["masking_data"] = None
 
             if self.property_groups is not None:
@@ -1983,14 +1995,30 @@
         )
 
         driver = PeakFinderDriver(new_params)
         driver.run()
 
         return ["Saved to " + str(workspace.h5file)]
 
+    @property
+    def params(self) -> PeakFinderParams:
+        """
+        Application parameters
+        """
+        return self._params
+
+    @params.setter
+    def params(self, params: PeakFinderParams):
+        if not isinstance(params, PeakFinderParams):
+            raise TypeError(
+                f"Input parameters must be an instance of {PeakFinderParams}"
+            )
+
+        self._params = params
+
 
 if __name__ == "__main__":
     print("Loading geoh5 file . . .")
     FILE = sys.argv[1]
     ifile = InputFile.read_ui_json(FILE)
     if ifile.data["launch_dash"]:
         ifile.workspace.open("r")
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/constants.py` & `peak_finder_app-0.1.0rc1/peak_finder/constants.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b4/peak_finder/driver.py` & `peak_finder_app-0.1.0rc1/peak_finder/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from curve_apps.trend_lines.params import Parameters
 from dask import compute
 from dask.diagnostics import ProgressBar
 from geoapps_utils.conversions import hex_to_rgb
 from geoapps_utils.driver.driver import BaseDriver
 from geoapps_utils.formatters import string_name
 from geoh5py import Workspace
-from geoh5py.data import Data
+from geoh5py.data import ReferencedData
 from geoh5py.groups import ContainerGroup, PropertyGroup
 from geoh5py.objects import Curve, Points
 from geoh5py.shared.utils import fetch_active_workspace
 from scipy.spatial import KDTree
 from tqdm import tqdm
 
 from peak_finder.constants import validations
@@ -101,31 +101,30 @@
                 anomalies += [line_class]
 
         return anomalies
 
     @staticmethod
     def get_line_indices(  # pylint: disable=too-many-locals
         survey_obj: Curve,
-        line_field_obj: Data,
+        line_field_obj: ReferencedData,
         line_ids: list[int],
-    ) -> dict | None:
+    ) -> dict:
         """
         Get line indices for plotting.
 
         :param survey_obj: Survey object.
         :param line_field_obj: Line field object.
         :param line_ids: Line IDs.
 
         :return: Line indices for each line ID given.
         """
         if (
             not isinstance(survey_obj, Curve)
             or survey_obj.vertices is None
-            or not hasattr(line_field_obj, "values")
-            or not isinstance(line_field_obj.values, np.ndarray | list)
+            or line_field_obj.values is None
         ):
             return {}
 
         line_length = len(line_field_obj.values)
 
         indices_dict: dict = {}
         for line_id in line_ids:
@@ -167,14 +166,17 @@
 
         return indices_dict
 
     def run(self):  # noqa  # pylint: disable=R0912, R0914, too-many-statements
         with fetch_active_workspace(self.params.geoh5, mode="r+"):
             survey = self.params.objects
 
+            if survey is None:
+                raise ValueError("Survey object not found.")
+
             output_group = ContainerGroup.create(
                 self.params.geoh5, name=string_name(self.params.ga_group_name)
             )
 
             channel_groups = self.params.get_property_groups()
 
             active_channels = {}
@@ -191,33 +193,38 @@
 
             print("Submitting parallel jobs:")
             property_groups = [
                 survey.find_or_create_property_group(name=name)
                 for name in channel_groups
             ]
 
-            survey_obj = self.params.objects
+            line_field_obj = self.params.get_line_field(survey)
+
             if self.params.masking_data is not None:
                 masking_array = self.params.masking_data.values
 
                 workspace = Workspace()
-                survey_obj = survey_obj.copy(parent=workspace)
+                survey = survey.copy(parent=workspace)
 
                 if False in masking_array:
-                    survey_obj.remove_vertices(~masking_array)
-                line_field_obj = survey_obj.get_data(self.params.line_field.uid)[0]
-            else:
-                line_field_obj = self.params.line_field
+                    survey.remove_vertices(~masking_array)
+
+                line_obj = survey.get_data(line_field_obj.uid)[0]
+
+                if not isinstance(line_obj, ReferencedData):
+                    raise ValueError("Line field not found.")
+
+                line_field_obj = line_obj
 
             line_ids = line_field_obj.value_map.map.keys()
             indices_dict = PeakFinderDriver.get_line_indices(
-                survey_obj, line_field_obj, line_ids
+                survey, line_field_obj, line_ids
             )
             anomalies = PeakFinderDriver.compute_lines(
-                survey=survey_obj,
+                survey=survey,
                 line_indices_dict=indices_dict,
                 line_ids=line_ids,
                 property_groups=property_groups,
                 smoothing=self.params.smoothing,
                 min_amplitude=self.params.min_amplitude,
                 min_value=self.params.min_value,
                 min_width=self.params.min_width,
@@ -273,38 +280,31 @@
                             anom_start.append(inds_map[anom.start])
                             anom_end.append(inds_map[anom.end])
                             peaks.append(inds_map[anom.peak])
 
             print("Exporting . . .")
             group_points = None
             if group_center:
-                channel_group = np.hstack(channel_group)  # Start count at 1
-
                 # Create reference values and color_map
                 group_map, color_map = {0: "Unknown"}, [[0, 0, 0, 0, 0]]
                 for ind, (name, group) in enumerate(channel_groups.items()):
                     group_map[ind + 1] = name
                     color_map += [[ind + 1] + hex_to_rgb(group["color"]) + [0]]
 
-                color_map = np.core.records.fromarrays(
-                    np.vstack(color_map).T,
-                    names=["Value", "Red", "Green", "Blue", "Alpha"],
-                )
                 group_points = Points.create(
                     self.params.geoh5,
                     name="Anomaly Groups",
                     vertices=np.vstack(group_center),
                     parent=output_group,
                 )
 
                 group_points.entity_type.name = self.params.ga_group_name
-                amplitude = np.hstack(amplitude)
                 group_points.add_data(
                     {
-                        "amplitude": {"values": amplitude},
+                        "amplitude": {"values": np.asarray(amplitude)},
                         "start": {
                             "values": np.vstack(group_start).flatten().astype(np.int32)
                         },
                         "end": {
                             "values": np.vstack(group_end).flatten().astype(np.int32)
                         },
                     }
@@ -314,27 +314,41 @@
                         "channel_group": {
                             "type": "referenced",
                             "values": np.hstack(channel_group),
                             "value_map": group_map,
                         }
                     }
                 )
-                channel_group_data.entity_type.color_map = {
-                    "name": "Time Groups",
-                    "values": color_map,
-                }
+                channel_group_data.entity_type.color_map = np.vstack(color_map)
                 line_id_data = group_points.add_data(
                     {
                         line_field_obj.name: {
                             "values": np.hstack(line_ids).astype(np.int32),
                             "entity_type": line_field_obj.entity_type,
                         }
                     }
                 )
 
+                if self.params.trend_lines:
+                    inputs = {
+                        "geoh5": self.params.geoh5,
+                        "entity": group_points,
+                        "data": channel_group_data,
+                        "parts": line_id_data,
+                        "export_as": "Trend Lines",
+                        "damping": 1,
+                    }
+
+                    params = Parameters.build(inputs)
+                    driver = TrendLinesDriver(params)
+                    out_trend = driver.create_output("Trend Lines", parent=output_group)
+
+                    if out_trend is not None:
+                        driver.add_ui_json(out_trend)
+
             if anom_locs:
                 anom_points = Points.create(
                     self.params.geoh5,
                     name="Anomalies",
                     vertices=np.vstack(anom_locs),
                     parent=output_group,
                 )
@@ -351,31 +365,25 @@
                         },
                         "downward inflection": {
                             "values": np.vstack(inflect_down).flatten().astype(np.int32)
                         },
                     }
                 )
 
-            if group_points is not None and self.params.trend_lines:
-                inputs = {
-                    "geoh5": self.params.geoh5,
-                    "entity": group_points,
-                    "data": channel_group_data,
-                    "parts": line_id_data,
-                    "export_as": "Trend Lines",
-                    "damping": 1,
-                }
-
-                params = Parameters.build(inputs)
-                driver = TrendLinesDriver(params)
-                out_trend = driver.create_output("Trend Lines", parent=output_group)
-
-                if out_trend is not None:
-                    driver.add_ui_json(out_trend)
-
         with self.params.geoh5.open(mode="r+"):
             self.update_monitoring_directory(output_group)
 
+    @property
+    def params(self) -> PeakFinderParams:
+        """Application parameters."""
+        return self._params
+
+    @params.setter
+    def params(self, val: PeakFinderParams):
+        if not isinstance(val, PeakFinderParams):
+            raise TypeError("Parameters must be of type BaseParams.")
+        self._params = val
+
 
 if __name__ == "__main__":
     FILE = sys.argv[1]
     PeakFinderDriver.start(FILE)
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/images/peak_finder_app.png` & `peak_finder_app-0.1.0rc1/peak_finder/images/peak_finder_app.png`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b4/peak_finder/layout.py` & `peak_finder_app-0.1.0rc1/peak_finder/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,36 +89,14 @@
 
 visual_params_layout = html.Div(
     id="visual_params",
     children=[
         html.Div(
             [
                 dcc.Markdown(
-                    children="Select Line",
-                    style={
-                        "width": "30%",
-                        "display": "inline-block",
-                        "vertical-align": "middle",
-                    },
-                ),
-                dcc.Dropdown(
-                    id="selected_line",
-                    options=[],
-                    style={
-                        "width": "70%",
-                        "display": "inline-block",
-                        "vertical-align": "middle",
-                    },
-                ),
-            ],
-            style={"margin-bottom": "20px"},
-        ),
-        html.Div(
-            [
-                dcc.Markdown(
                     children="N outward lines",
                     style={
                         "width": "30%",
                         "display": "inline-block",
                     },
                 ),
                 dcc.Input(
@@ -231,14 +209,36 @@
 
 detection_params_layout = html.Div(
     id="detection_params",
     children=[
         html.Div(
             [
                 dcc.Markdown(
+                    children="Select Line",
+                    style={
+                        "width": "30%",
+                        "display": "inline-block",
+                        "vertical-align": "middle",
+                    },
+                ),
+                dcc.Dropdown(
+                    id="selected_line",
+                    options=[],
+                    style={
+                        "width": "70%",
+                        "display": "inline-block",
+                        "vertical-align": "middle",
+                    },
+                ),
+            ],
+            style={"margin-bottom": "20px"},
+        ),
+        html.Div(
+            [
+                dcc.Markdown(
                     children="Masking Data",
                     style={
                         "width": "30%",
                         "display": "inline-block",
                         "vertical-align": "middle",
                     },
                 ),
@@ -426,14 +426,15 @@
                         "display": "inline-block",
                     },
                 ),
                 dcc.Input(
                     id="max_separation",
                     value=100,
                     type="number",
+                    debounce=True,
                     style={
                         "width": "70%",
                         "display": "inline-block",
                     },
                 ),
                 dcc.Checklist(
                     id="flip_sign",
@@ -485,19 +486,19 @@
                     ],
                     style={"width": "70%", "display": "inline-block"},
                 ),
                 html.Div(
                     [
                         dcc.Dropdown(
                             options=[
-                                "Visual parameters",
                                 "Detection parameters",
+                                "Visual parameters",
                             ],
                             id="widget_selection",
-                            value="Visual parameters",
+                            value="Detection parameters",
                             style={"width": "70%", "margin-bottom": "20px"},
                         ),
                         visual_params_layout,
                         detection_params_layout,
                     ],
                     style={"width": "30%", "display": "inline-block"},
                 ),
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/line_anomaly.py` & `peak_finder_app-0.1.0rc1/peak_finder/line_anomaly.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,34 +20,20 @@
 class LineAnomaly:  # pylint: disable=R0902, duplicate-code
     """
     Main class for finding anomalies.
 
     Contains list of LineGroup objects.
     """
 
-    _entity: Curve
-    _line_id: int
-    _line_indices: list[int] | np.ndarray
-    _line_start: list[int]
-    _max_migration: float
-    _minimal_output: bool
-    _min_amplitude: int
-    _min_channels: int
-    _min_value: float
-    _min_width: float
-    _property_groups: list[PropertyGroup]
-    _smoothing: int
-    _use_residual: bool
-
     def __init__(  # pylint: disable=R0913, R0914
         self,
         entity,
         line_id,
-        line_indices,
-        line_start,
+        line_indices: np.ndarray,
+        line_start: np.ndarray,
         property_groups,
         max_migration=50.0,
         minimal_output=False,
         min_amplitude=25,
         min_channels=3,
         min_value=-np.inf,
         min_width=200.0,
@@ -113,29 +99,29 @@
         return self._line_id
 
     @line_id.setter
     def line_id(self, value: int):
         self._line_id = value
 
     @property
-    def line_indices(self) -> list[int] | None:
+    def line_indices(self) -> np.ndarray:
         """
         Indices of vertices for line profile.
         """
         return self._line_indices
 
     @line_indices.setter
-    def line_indices(self, value):
+    def line_indices(self, value: np.ndarray):
         if not isinstance(value, np.ndarray):
             raise TypeError("Line indices must be a numpy array.")
 
         self._line_indices = value
 
     @property
-    def line_start(self) -> list[int] | None:
+    def line_start(self) -> np.ndarray:
         """
         Index for start of the line.
         """
         return self._line_start
 
     @line_start.setter
     def line_start(self, value):
@@ -161,14 +147,17 @@
             isinstance(item, PropertyGroup) for item in value
         ):
             raise TypeError("Property groups must be a list of PropertyGroups.")
 
         self._property_groups = value
         channels = []
         for group in self._property_groups:
+            if group.properties is None:
+                continue
+
             channels += [self.entity.get_entity(uid)[0] for uid in group.properties]
 
         self._channels = list(set(channels))
 
     @property
     def smoothing(self) -> int:
         """
@@ -317,18 +306,18 @@
 
             if active_cells.size == 0:
                 return None
 
             sorting = np.concatenate((active_cells[:, 0], [active_cells[-1, 1]]))
 
             self._position = LinePosition(
-                locations=self.locations,
-                line_indices=self.line_indices,
-                line_start=self.line_start,
-                sorting=sorting,
+                self.locations,
+                self.line_indices,
+                self.line_start,
+                sorting,
                 smoothing=self.smoothing,
                 residual=self.use_residual,
             )
         return self._position
 
     def find_anomalies(  # pylint: disable=R0914
         self,
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/line_data.py` & `peak_finder_app-0.1.0rc1/peak_finder/line_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,46 +10,45 @@
 import numpy as np
 from geoh5py.data import FloatData
 
 from peak_finder.anomaly import Anomaly
 from peak_finder.line_position import LinePosition
 
 
-class LineData:
+class LineData:  # pylint: disable=too-many-instance-attributes
     """
     Contains full list of Anomaly objects and line data values.
     """
 
-    def __init__(  # pylint: disable=R0913
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         data: FloatData,
         position: LinePosition,
         min_amplitude: int,
         min_width: float,
         max_migration: float,
         min_value: float = -np.inf,
     ):
-        self._data_entity = data
-        self._position = position
-        self._min_amplitude = min_amplitude
-        self._min_width = min_width
-        self._max_migration = max_migration
-        self._min_value = min_value
-        self._min_value = min_value
-        self._values = None
-        self._peaks = None
-        self._lows = None
-        self._inflect_up = None
-        self._inflect_down = None
-        self._values_resampled_raw = None
-        self._values_resampled = None
+        self.data_entity = data
+        self.position: LinePosition = position
+        self.min_amplitude = min_amplitude
+        self.min_width = min_width
+        self.max_migration = max_migration
+        self.min_value = min_value
+        self.min_value = min_value
+        self._values: np.ndarray | None = None
+        self._peaks: np.ndarray | None = None
+        self._lows: np.ndarray | None = None
+        self._inflect_up: np.ndarray | None = None
+        self._inflect_down: np.ndarray | None = None
+        self._values_resampled: np.ndarray | None = None
         self._anomalies: list[Anomaly] | None = None
 
     @property
-    def values(self) -> np.ndarray:
+    def values(self) -> np.ndarray | None:
         """
         Original values sorted along line.
         """
         if self._values is None:
             if self.data_entity is not None and self.position.sorting is not None:
                 self._values = self.data_entity.values[  # type: ignore
                     self.position.sorting
@@ -68,37 +67,42 @@
     @property
     def data_entity(self) -> FloatData:
         """
         Data entity.
         """
         return self._data_entity
 
+    @data_entity.setter
+    def data_entity(self, data):
+        """
+        Data entity.
+        """
+        if getattr(self, "_data_entity", None) is not None:
+            raise ValueError("Data entity is already set.")
+
+        if not isinstance(data, FloatData):
+            raise TypeError("Data entity must be of type geoh5py.data.FloatData.")
+
+        self._data_entity = data
+
     @property
     def values_resampled(self) -> np.ndarray:
         """
         Values re-sampled on a regular interval.
         """
         if self._values_resampled is None:
             (
                 self._values_resampled,
-                self._values_resampled_raw,
+                _,
             ) = self.position.resample_values(self.values)
         return self._values_resampled
 
     @values_resampled.setter
     def values_resampled(self, values):
         self._values_resampled = values
-        self._values_resampled_raw = None
-
-    @property
-    def values_resampled_raw(self) -> np.ndarray:
-        """
-        Resampled values prior to smoothing.
-        """
-        return self._values_resampled_raw
 
     @property
     def min_amplitude(self) -> int:
         """
         Minimum amplitude of anomaly.
         """
         return self._min_amplitude
@@ -153,16 +157,15 @@
 
     @property
     def anomalies(self) -> list[Anomaly]:
         """
         Full list of anomalies.
         """
         if self._anomalies is None:
-            anomalies = self.compute()
-            self._anomalies = np.array(anomalies)
+            self._anomalies = self.compute()
         return self._anomalies
 
     @property
     def peaks(self) -> np.ndarray | None:
         """
         Find peak indices.
         """
@@ -192,15 +195,15 @@
             dx = self.derivative(order=1)  # pylint: disable=C0103
             ddx = self.derivative(order=2)
 
             lows = np.where(
                 (np.diff(np.sign(dx)) != 0)
                 & (ddx[1:] > 0)
                 & (
-                    values[:-1] > self.min_value
+                    values[:-1] >= self.min_value
                 )  # pylint: disable=unsubscriptable-object
             )[0]
             self._lows = np.r_[0, lows, self.position.locations_resampled.shape[0] - 1]
         return self._lows
 
     @property
     def inflect_up(self) -> np.ndarray | None:
@@ -213,15 +216,15 @@
             dx = self.derivative(order=1)  # pylint: disable=C0103
             ddx = self.derivative(order=2)
 
             self._inflect_up = np.where(
                 (np.diff(np.sign(ddx)) != 0)
                 & (dx[1:] > 0)
                 & (
-                    values[:-1] > self.min_value
+                    values[:-1] >= self.min_value
                 )  # pylint: disable=unsubscriptable-object
             )[0]
         return self._inflect_up
 
     @property
     def inflect_down(self) -> np.ndarray | None:
         """
@@ -233,15 +236,15 @@
             dx = self.derivative(order=1)  # pylint: disable=C0103
             ddx = self.derivative(order=2)
 
             self._inflect_down = np.where(
                 (np.diff(np.sign(ddx)) != 0)
                 & (dx[1:] < 0)
                 & (
-                    values[:-1] > self.min_value
+                    values[:-1] >= self.min_value
                 )  # pylint: disable=unsubscriptable-object
             )[0]
         return self._inflect_down
 
     def get_list_attr(self, attr: str) -> list | np.ndarray:
         """
         Get list of anomaly attributes.
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/line_group.py` & `peak_finder_app-0.1.0rc1/peak_finder/line_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -210,126 +210,144 @@
             peak values, and channel groups.
         """
         locs = self.position.locations_resampled
 
         full_anomalies = []
         full_channels = []
         full_peak_positions = []
-        full_peak_values = []
+
         for ind, line_data in enumerate(line_data_subset):
-            values = line_data.values_resampled
             for anom in line_data.anomalies:
                 full_anomalies.append(anom)
                 full_channels.append(ind)
                 full_peak_positions.append(locs[anom.peak])
-                full_peak_values.append(values[anom.peak])
-        full_channels = np.array(full_channels)
-        full_peak_positions = np.array(full_peak_positions)
+
         return (
             full_anomalies,
-            full_channels,
-            full_peak_positions,
-            full_peak_values,
+            np.array(full_channels),
+            np.array(full_peak_positions),
         )
 
-    def group_n_groups(  # pylint: disable=R0914
-        self, groups: list[AnomalyGroup]
-    ) -> list[AnomalyGroup]:
+    @staticmethod
+    def accumulate_groups(
+        path: np.ndarray, neighbourhood: np.ndarray, max_length: int
+    ) -> list[np.ndarray]:
+        """
+        Accumulate neighbouring groups.
+
+        :param path: Current path made up of coupled anomaly indices.
+        :param neighbourhood: Array of all neighbouring couple indices.
+        :param max_length: Maximum number of anomalies in a path.
+
+        :return: List of all possible paths.
+        """
+        if len(np.unique(path)) == max_length:
+            return [path]
+
+        next_neighbours = np.where(path[-1, 1] == neighbourhood[:, 0])[0]
+
+        if len(next_neighbours) == 0:
+            return [path]
+
+        branches = []
+        for next_neighbour in next_neighbours:
+            current = np.vstack([path, neighbourhood[next_neighbour]])
+            paths = LineGroup.accumulate_groups(current, neighbourhood, max_length)
+
+            for branch in paths:
+                branches.append(branch)
+
+        return branches
+
+    @staticmethod
+    def find_neighbour_groups(groups: list[AnomalyGroup], max_separation: int) -> list:
+        """
+        Loop through all anomaly groups and find neighbours within the
+        maximum separation.
+
+        :param groups: List of anomaly groups.
+        :param max_separation: Maximum number of indices separating anomalies to form a group.
+
+        :return: List of indices for all group pairs.
+        """
+        all_starts = np.asarray([group.start for group in groups])
+        all_ends = np.asarray([group.end for group in groups])
+
+        neighbours_list = []
+        for cur, end in enumerate(all_ends):
+            dist = np.abs(all_starts - end)
+            next_neighbour = np.where(dist < max_separation)[0]
+            neighbours_list += [[cur, nn] for nn in next_neighbour if nn != cur]
+
+        return neighbours_list
+
+    def group_n_groups(self, groups: list[AnomalyGroup]) -> list[AnomalyGroup]:
         """
         Merge consecutive peaks into groups of n_groups.
 
         :param groups: List of anomaly groups.
 
         :return: List of merged anomaly groups.
         """
         if self.position.sampling is None or self.channels is None:
             return groups
 
-        for _ in range(self.n_groups):
-            # Sort groups by their starts
-            all_starts = [group.start for group in groups]
-            sort_inds = np.argsort([group.start for group in groups])
-            groups = list(np.array(groups)[sort_inds])
-
-            all_starts = np.array(all_starts)[sort_inds]
-            all_ends = [group.end for group in groups]
-
-            merged = []
-            for group in groups:
-                # Get indices of consecutive peaks within max_separation
-                delta_ind = self.max_separation / self.position.sampling
+        return_groups: list[AnomalyGroup] = []
+        all_starts = np.array([group.start for group in groups])
+        sort_inds = np.argsort(all_starts)
+        sorted_groups: list[AnomalyGroup] = list(np.array(groups)[sort_inds])
+
+        max_separation = np.ceil(self.max_separation / self.position.sampling)
+        neighbours_list = self.find_neighbour_groups(sorted_groups, max_separation)
+
+        if len(neighbours_list) == 0:
+            return return_groups
+
+        neighbourhood = np.vstack(neighbours_list)
+
+        for couple in neighbourhood:
+            branches = self.accumulate_groups(
+                couple[np.newaxis, :], neighbourhood, self.n_groups
+            )
 
-                start_ind = np.searchsorted(
-                    all_ends, group.start - delta_ind, side="left"  # type: ignore
-                )
-                end_ind = (
-                    np.searchsorted(
-                        all_starts, group.end + delta_ind, side="right"  # type: ignore
-                    )
-                    - 1
-                )
-                in_range = np.arange(start_ind, end_ind + 1)
+            for branch in branches:
 
-                # Loop over peaks in range and create groups for all possibilities
-                for i in in_range:
-                    if groups[i].subgroups.intersection(group.subgroups):
-                        continue
-                    n_groups = len(group.subgroups) + len(groups[i].subgroups)
-                    if n_groups <= self.n_groups:
-                        new_group = AnomalyGroup(
-                            position=self.position,
-                            anomalies=np.concatenate(
-                                (group.anomalies, groups[i].anomalies)
-                            ),
-                            property_group=self.property_group,
-                            full_azimuth=np.concatenate(
-                                (group.full_azimuth, groups[i].full_azimuth)
-                            ),
-                            channels=self.channels,
-                            full_peak_values=np.concatenate(
-                                (group.full_peak_values, groups[i].full_peak_values)
-                            ),
-                            subgroups=group.subgroups.union(groups[i].subgroups),
-                        )
-                        merged.append(new_group)
-            groups += merged
-
-        return_groups = []
-        unique_groups = []
-        for group in groups:
-            if (
-                len(group.subgroups) == self.n_groups
-                and group.subgroups not in unique_groups
-            ):
-                unique_groups.append(group.subgroups)
-                return_groups.append(group)
+                indices = np.unique(branch)
+
+                if len(indices) < self.n_groups:
+                    continue
+
+                new_group = AnomalyGroup(
+                    np.concatenate([sorted_groups[ind].anomalies for ind in indices]),
+                    self.property_group,
+                    subgroups={sorted_groups[ind] for ind in indices},
+                )
+                return_groups.append(new_group)
 
         return return_groups
 
     def compute(  # pylint: disable=R0913, R0914
         self,
     ) -> list[AnomalyGroup] | list:
         """
         Group anomalies.
 
         :return: List of groups of anomalies.
         """
         groups: list = []
         group_id = -1
-        azimuth = self.position.compute_azimuth()
 
         if self.channels is None or self.n_groups is None:
             return groups
 
         # Get full lists of anomaly attributes
         (
             full_anomalies,
             full_channels,
             full_peak_positions,
-            full_peak_values,
         ) = self.get_anomaly_attributes(list(self.channels.values()))
 
         full_group_ids = np.ones(len(full_anomalies), dtype="bool") * -1
         for ind, _ in enumerate(full_anomalies):
             # Skip if already labeled
             if full_group_ids[ind] != -1:
                 continue
@@ -349,23 +367,18 @@
             ):
                 continue
 
             full_group_ids[near] = group_id
 
             # Make AnomalyGroup
             near_anomalies = np.array(full_anomalies)[near]
-            near_values = np.array(full_peak_values)[near]
 
             group = AnomalyGroup(
-                self.position,
                 near_anomalies,
                 self.property_group,
-                azimuth,
-                self.channels,
-                near_values,
                 set(),
             )
             groups += [group]
 
         if self.n_groups > 1:
             groups = self.group_n_groups(groups)
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/line_position.py` & `peak_finder_app-0.1.0rc1/peak_finder/line_position.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,164 +17,134 @@
     Compute and store the derivatives of inline data values. The values are re-sampled at a constant
     interval, padded then transformed to the Fourier domain using the :obj:`numpy.fft` package.
 
     :param locations: An array of data locations, either as distance along line or 3D coordinates.
         For 3D coordinates, the locations are automatically converted and sorted as distance from
         the origin.
     :param values: Data values used to compute derivatives over, shape(locations.shape[0],).
-    :param epsilon: Adjustable constant used in :obj:`scipy.interpolate.Rbf`. Defaults to 20x the
-        average sampling
-    :param interpolation: Type on interpolation accepted by the :obj:`scipy.interpolate.Rbf`
-        routine: 'multiquadric', 'inverse', 'gaussian', 'linear', 'cubic', 'quintic', 'thin_plate'
     :param smoothing: Number of neighbours used by the :obj:`geoapps.utils.running_mean` routine.
     :param residual: Use the residual between the values and the running mean to compute
         derivatives.
     :param sampling: Sampling interval length (m) used in the FFT. Defaults to the mean data
         separation.
     """
 
     def __init__(  # pylint: disable=R0913
         self,
-        locations: np.ndarray | None = None,
-        line_indices: np.ndarray | None = None,
-        line_start: list[int] | None = None,
-        sorting: np.ndarray | None = None,
-        epsilon: float | None = None,
-        interpolation: str = "gaussian",
+        locations: np.ndarray,
+        line_indices: np.ndarray,
+        line_start: np.ndarray,
+        sorting: np.ndarray,
         smoothing: int = 0,
         residual: bool = False,
-        sampling: float | None = None,
         **kwargs,
     ):
-        self._locations_resampled = None
-        self.x_locations = None
-        self.y_locations = None
-        self.z_locations = None
+        self._locations: np.ndarray
+        self._locations_resampled: np.ndarray
+        self._sampling: float
+        self._sampling_width: int
         self._map_locations = None
         self.line_indices = line_indices
         self.line_start = line_start
         self.sorting = sorting
         self.locations = locations
-        self._epsilon = epsilon
-        self._interpolation = interpolation
         self._smoothing = smoothing
         self._residual = residual
-        self._sampling = sampling
-        self.Fx = None  # pylint: disable=C0103
-        self.Fy = None  # pylint: disable=C0103
-        self.Fz = None  # pylint: disable=C0103
+        self._x_interp: interp1d | None = None
+        self._y_interp: interp1d | None = None
+        self._z_interp: interp1d | None = None
 
         for key, value in kwargs.items():
             if getattr(self, key, None) is not None:
                 setattr(self, key, value)
 
     @property
-    def epsilon(self) -> float | None:
-        """
-        Adjustable constant used by :obj:`scipy.interpolate.Rbf`
-        """
-        if getattr(self, "_epsilon", None) is None and self.locations is not None:
-            width = self.locations[-1] - self.locations[0]
-            self._epsilon = width / 5.0
-
-        return self._epsilon
-
-    @property
-    def sampling_width(self) -> int:
-        """
-        Number of padding cells added for the FFT
-        """
-        if (
-            getattr(self, "_sampling_width", None) is None
-            and self.locations_resampled is not None
-        ):
-            self._sampling_width = int(np.floor(len(self.locations_resampled)))
-
-        return self._sampling_width
-
-    @property
     def locations(self) -> np.ndarray:
         """
         Position of values along line.
         """
         return self._locations
 
     @locations.setter
-    def locations(self, locations):
-        self._locations = None
-        self.x_locations = None
+    def locations(self, locations: np.ndarray):
         self.y_locations = None
         self.z_locations = None
-        self._locations_resampled = None
-        self._map_locations = None
-
-        if locations is not None and len(locations) > 0:
-            if locations.ndim > 1:
-                self.x_locations = locations[self.sorting, 0]
-                self.y_locations = locations[self.sorting, 1]
-                if locations.shape[1] == 3:
-                    self.z_locations = locations[self.sorting, 2]
-
-                distances = np.linalg.norm(
-                    np.c_[
-                        self.line_start[0] - locations[self.sorting, 0],
-                        self.line_start[1] - locations[self.sorting, 1],
-                    ],
-                    axis=1,
-                )
-            else:
-                self.x_locations = locations
-                distances = locations[self.sorting]
 
-            self._locations = distances
+        if locations is None or len(locations) < 2:
+            raise ValueError("Locations must be an array of at least 2 points.")
 
-            if self._locations[0] == self._locations[-1]:
-                return
-
-            dx = np.mean(  # pylint: disable=C0103
-                np.abs(self.locations[1:] - self.locations[:-1])
-            )
-            self._sampling_width = np.abs(
-                np.ceil((self._locations[-1] - self._locations[0]) / dx).astype(int)
-            )
-            self._locations_resampled = np.linspace(
-                self._locations[0], self._locations[-1], self.sampling_width
-            )
+        if locations.ndim > 1:
+            self.x_locations = locations[self.sorting, 0]
+            self.y_locations = locations[self.sorting, 1]
+
+            if locations.shape[1] == 3:
+                self.z_locations = locations[self.sorting, 2]
+
+            xy_locations = self.line_start[None, :2] - locations[self.sorting, :2]
+
+            distances = np.linalg.norm(xy_locations, axis=1)
+        else:
+            self.x_locations = locations
+            distances = locations[self.sorting]
+
+        self._locations = distances
+
+        if self._locations[0] == self._locations[-1]:
+            raise ValueError("Locations must be unique.")
+
+        dx = np.mean(  # pylint: disable=C0103
+            np.abs(self.locations[1:] - self.locations[:-1])
+        )
+        self._sampling_width = np.abs(
+            np.ceil((self._locations[-1] - self._locations[0]) / dx).astype(int)
+        )
+        self._locations_resampled = np.linspace(
+            distances[0], distances[-1], self._sampling_width
+        )
+        self._sampling = np.mean(
+            np.abs(self.locations_resampled[1:] - self.locations_resampled[:-1])
+        )
 
     @property
     def line_indices(self) -> np.ndarray:
         """
         Indices for current line
         """
         return self._line_indices
 
     @line_indices.setter
     def line_indices(self, value):
         self._line_indices = value
 
     @property
-    def line_start(self) -> list[int] | None:
+    def line_start(self) -> np.ndarray:
         """
         Start index for current line
         """
         return self._line_start
 
     @line_start.setter
-    def line_start(self, value):
-        self._line_start = value
+    def line_start(self, value: np.ndarray):
+        if len(value) < 2:
+            raise ValueError("Line start must be an array of at least two values.")
+
+        self._line_start = np.asarray(value)
 
     @property
     def sorting(self) -> np.ndarray:
         """
         Locations sorting order.
         """
         return self._sorting
 
     @sorting.setter
     def sorting(self, value):
+        if not isinstance(value, np.ndarray):
+            raise ValueError("Sorting must be a numpy array.")
+
         self._sorting = value
 
     @property
     def map_locations(self) -> np.ndarray:
         """
         A list where the indices are the resampled locations indices and the values are the
         original locations indices.
@@ -190,51 +160,32 @@
     def locations_resampled(self) -> np.ndarray:
         """
         Position of values resampled on a fix interval.
         """
         return self._locations_resampled
 
     @property
-    def sampling(self) -> float | None:
+    def sampling(self) -> float:
         """
         Discrete interval length (m)
         """
-        if (
-            getattr(self, "_sampling", None) is None
-            and self.locations_resampled is not None
-        ):
-            self._sampling = np.mean(
-                np.abs(self.locations_resampled[1:] - self.locations_resampled[:-1])
-            )
         return self._sampling
 
     @property
-    def interpolation(self) -> str:
-        """
-        Method of interpolation: 'linear', 'nearest', 'slinear', 'quadratic' or 'cubic'
-        """
-        return self._interpolation
-
-    @interpolation.setter
-    def interpolation(self, method):
-        methods = ["linear", "nearest", "slinear", "quadratic", "cubic"]
-        assert method in methods, f"Method on interpolation must be one of {methods}"
-
-    @property
     def residual(self) -> bool:
         """
         Use the residual of the smoothing data.
         """
         return self._residual
 
     @residual.setter
     def residual(self, value):
         assert isinstance(value, bool), "Residual must be a bool"
-        if value != self._residual:
-            self._residual = value
+
+        self._residual = value
 
     @property
     def smoothing(self) -> int:
         """
         Smoothing factor in terms of number of nearest neighbours used
         in a running mean averaging of the signal.
         """
@@ -244,89 +195,93 @@
     def smoothing(self, value):
         assert (
             isinstance(value, int) and value >= 0
         ), "Smoothing parameter must be an integer >0"
         if value != self._smoothing:
             self._smoothing = value
 
-    def resample_values(self, values) -> np.ndarray:
+    def resample_values(self, values) -> tuple[np.ndarray, np.ndarray]:
         """
         Values re-sampled on a regular interval.
         """
-        values_resampled = None
-        values_resampled_raw = None
-        if self.locations is not None:
-            interp = interp1d(self.locations, values, fill_value="extrapolate")
-            values_resampled = interp(self._locations_resampled)
-            if values_resampled is not None:
-                values_resampled_raw = values_resampled.copy()
-            if self._smoothing > 0:
-                mean_values = running_mean(
-                    values_resampled,
-                    width=self._smoothing,
-                    method="centered",
-                )
-
-                if self.residual:
-                    values_resampled = values_resampled - mean_values
-                else:
-                    values_resampled = mean_values
+        interp = interp1d(self.locations, values, fill_value="extrapolate")
+        values_resampled = interp(self._locations_resampled)
 
-        return values_resampled, values_resampled_raw
+        if self._smoothing > 0:
+            mean_values = running_mean(
+                values_resampled,
+                width=self._smoothing,
+                method="centered",
+            )
+
+            if self.residual:
+                return values_resampled - mean_values, values_resampled
+
+            return mean_values, values_resampled
+
+        return values_resampled, values_resampled
 
-    def interp_x(self, distance: float) -> float:
+    def interp_x(self, distance: np.ndarray) -> np.ndarray:
         """
         Get the x-coordinate from the inline distance.
 
         :param distance: Inline distance.
 
         :return: x-coordinate.
         """
-        if getattr(self, "Fx", None) is None:
-            self.Fx = interp1d(
+        if self._x_interp is None:
+            self._x_interp = interp1d(
                 self.locations,
                 self.x_locations,
                 bounds_error=False,
                 fill_value="extrapolate",
             )
-        return self.Fx(distance)  # type: ignore
+        return self._x_interp(distance)
 
-    def interp_y(self, distance: float) -> float:
+    def interp_y(self, distance: np.ndarray) -> np.ndarray | None:
         """
         Get the y-coordinate from the inline distance.
 
         :param distance: Inline distance.
 
         :return: y-coordinate.
         """
-        if getattr(self, "Fy", None) is None:
-            self.Fy = interp1d(
+        if self._y_interp is None and self.y_locations is not None:
+            self._y_interp = interp1d(
                 self.locations,
                 self.y_locations,
                 bounds_error=False,
                 fill_value="extrapolate",
             )
-        return self.Fy(distance)  # type: ignore
 
-    def interp_z(self, distance: float) -> float:
+        if self._y_interp is None:
+            return None
+
+        return self._y_interp(distance)
+
+    def interp_z(self, distance: float) -> float | None:
         """
         Get the z-coordinate from the inline distance.
 
         :param distance: Inline distance.
 
         :return: z-coordinate.
         """
-        if getattr(self, "Fz", None) is None:
-            self.Fz = interp1d(
+        if self._z_interp is None and self.z_locations is not None:
+            self._z_interp = interp1d(
                 self.locations,
                 self.z_locations,
                 bounds_error=False,
                 fill_value="extrapolate",
             )
-        return self.Fz(distance)  # type: ignore
+
+        if self._z_interp is None:
+            return None
+
+        return self._z_interp(distance)
 
     def interpolate_array(self, inds: np.ndarray) -> np.ndarray:
         """
         Interpolate the locations of the line profile at the given indices.
 
         :param inds: Indices of locations to interpolate.
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/params.py` & `peak_finder_app-0.1.0rc1/peak_finder/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 #
 
 from __future__ import annotations
 
 import string
 from copy import deepcopy
 
+import numpy as np
 from geoapps_utils.driver.params import BaseParams
-from geoh5py.data import Data
+from geoh5py.data import Data, ReferencedData
 from geoh5py.groups import PropertyGroup
-from geoh5py.objects import ObjectBase
+from geoh5py.objects import Curve
 from geoh5py.ui_json import InputFile
 
 from peak_finder.constants import default_ui_json, defaults, validations
 
 
 class PeakFinderParams(BaseParams):  # pylint: disable=R0902, R0904
     """
@@ -26,26 +27,26 @@
 
     def __init__(self, input_file: InputFile | None = None, **kwargs):
         self._default_ui_json: dict | None = deepcopy(default_ui_json)
         self._defaults: dict | None = deepcopy(defaults)
         self._free_parameter_keys: list = ["data", "color"]
         self._free_parameter_identifier: str = "group"
         self._validations: dict | None = validations
-        self._objects: ObjectBase | None = None
-        self._flip_sign: bool | None = None
-        self._line_field: Data | None = None
+        self._objects: Curve
+        self._flip_sign: bool = False
+        self._line_field: ReferencedData
         self._masking_data: Data | None = None
-        self._smoothing: int | None = None
-        self._min_amplitude: int | None = None
-        self._min_value: float | None = None
-        self._min_width: float | None = None
-        self._max_migration: float | None = None
-        self._min_channels: int | None = None
-        self._n_groups: int | None = None
-        self._max_separation: float | None = None
+        self._smoothing: int = 0
+        self._min_amplitude: int = 1
+        self._min_value: float = -np.inf
+        self._min_width: float = 0.0
+        self._max_migration: float = np.inf
+        self._min_channels: int = 1
+        self._n_groups: int = 1
+        self._max_separation: float = np.inf
         self._ga_group_name: str | None = None
         self._structural_markers: bool | None = None
         self._trend_lines: bool | None = None
         self._line_id: int | None = None
         self._group_a_data: PropertyGroup | None = None
         self._group_a_color: str | None = None
         self._group_b_data: PropertyGroup | None = None
@@ -86,15 +87,15 @@
         return self._conda_environment_boolean
 
     @conda_environment_boolean.setter
     def conda_environment_boolean(self, val):
         self.setter_validator("conda_environment_boolean", val)
 
     @property
-    def flip_sign(self) -> bool | None:
+    def flip_sign(self) -> bool:
         """
         Flip sign of data.
         """
         return self._flip_sign
 
     @flip_sign.setter
     def flip_sign(self, val):
@@ -108,15 +109,15 @@
         return self._ga_group_name
 
     @ga_group_name.setter
     def ga_group_name(self, val):
         self.setter_validator("ga_group_name", val)
 
     @property
-    def line_field(self) -> Data | None:
+    def line_field(self) -> ReferencedData:
         """
         Object containing line ids and associated names.
         """
         return self._line_field
 
     @line_field.setter
     def line_field(self, val):
@@ -141,60 +142,60 @@
         return self._line_id
 
     @line_id.setter
     def line_id(self, val):
         self.setter_validator("line_id", val)
 
     @property
-    def max_migration(self) -> float | None:
+    def max_migration(self) -> float:
         """
         Threshold on the lateral shift (m) of peaks within a grouping of anomalies.
         """
         return self._max_migration
 
     @max_migration.setter
     def max_migration(self, val):
         self.setter_validator("max_migration", val)
 
     @property
-    def min_amplitude(self) -> int | None:
+    def min_amplitude(self) -> int:
         """
         Threshold on the minimum amplitude of the anomaly, expressed as
         a percent of the height scaled by the minimum value.
         """
         return self._min_amplitude
 
     @min_amplitude.setter
     def min_amplitude(self, val):
         self.setter_validator("min_amplitude", val)
 
     @property
-    def min_channels(self) -> int | None:
+    def min_channels(self) -> int:
         """
         Minimum number of data channels required to form a group.
         """
         return self._min_channels
 
     @min_channels.setter
     def min_channels(self, val):
         self.setter_validator("min_channels", val)
 
     @property
-    def min_value(self) -> float | None:
+    def min_value(self) -> float:
         """
         Minimum absolute data value to be considered for anomaly detection.
         """
         return self._min_value
 
     @min_value.setter
     def min_value(self, val):
         self.setter_validator("min_value", val)
 
     @property
-    def min_width(self) -> float | None:
+    def min_width(self) -> float:
         """
         Minimum anomaly width (m) measured between start and end of bounding minima.
         """
         return self._min_width
 
     @min_width.setter
     def min_width(self, val):
@@ -208,15 +209,15 @@
         return self._monitoring_directory
 
     @monitoring_directory.setter
     def monitoring_directory(self, val):
         self.setter_validator("monitoring_directory", val)
 
     @property
-    def objects(self) -> ObjectBase | None:
+    def objects(self) -> Curve:
         """
         Objects to use for line profile.
         """
         return self._objects
 
     @objects.setter
     def objects(self, val):
@@ -227,15 +228,15 @@
         return self._plot_result
 
     @plot_result.setter
     def plot_result(self, val):
         self._plot_result = val
 
     @property
-    def smoothing(self) -> int | None:
+    def smoothing(self) -> int:
         """
         Number of neighbors used in running mean smoothing.
         """
         return self._smoothing
 
     @smoothing.setter
     def smoothing(self, val):
@@ -249,26 +250,26 @@
         return self._trend_lines
 
     @trend_lines.setter
     def trend_lines(self, val):
         self.setter_validator("trend_lines", val)
 
     @property
-    def n_groups(self) -> int | None:
+    def n_groups(self) -> int:
         """
         Number of consecutive peaks to merge into a single anomaly.
         """
         return self._n_groups
 
     @n_groups.setter
     def n_groups(self, val):
         self.setter_validator("n_groups", val)
 
     @property
-    def max_separation(self) -> float | None:
+    def max_separation(self) -> float:
         """
         Maximum separation between peaks to merge into single anomaly.
         """
         return self._max_separation
 
     @max_separation.setter
     def max_separation(self, val):
@@ -455,7 +456,26 @@
                     "param": name,
                     "data": prop_group.uid,
                     "color": getattr(self, f"group_{name}_color", None),
                     "label": [count],
                     "properties": prop_group.properties,
                 }
         return property_groups
+
+    def get_line_field(self, survey: Curve) -> ReferencedData:
+        """
+        Get the line field object.
+        """
+        line_field_obj = self.line_field
+
+        if line_field_obj is None:
+            unique_parts = np.unique(survey.parts.astype(int)) + 1
+            line_field_obj = survey.add_data(
+                {
+                    "Line ID": {
+                        "values": survey.parts.astype(int) + 1,
+                        "value_map": {ind: f"Line {ind}" for ind in unique_parts},
+                        "type": "referenced",
+                    }
+                }
+            )
+        return line_field_obj
```

### Comparing `peak_finder_app-0.1.0b4/peak_finder/utils.py` & `peak_finder_app-0.1.0rc1/peak_finder/utils.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b4/peak_finder-assets/FlinFlon_tem_aoi.geoh5` & `peak_finder_app-0.1.0rc1/peak_finder-assets/FlinFlon_tem_aoi.geoh5`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b4/peak_finder-assets/uijson/peak_finder.ui.json` & `peak_finder_app-0.1.0rc1/peak_finder-assets/uijson/peak_finder.ui.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9572472848788637%*

 * *Differences: {"'ga_group_name'": "{'main': True, 'group': '3 - Python run preferences'}",*

 * * "'group_a_color'": "{'group': '2- Group A'}",*

 * * "'group_a_data'": "{'group': '2- Group A'}",*

 * * "'line_field'": "{'group': '1 - Data', 'optional': True, 'enabled': False}",*

 * * "'objects'": "{'group': '1 - Data'}",*

 * * "'structural_markers'": "{'main': True, 'group': '3 - Python run preferences'}",*

 * * "'trend_lines'": "{'group': '3 - Python run preferences'}",*

 * * 'delete': "['workspace']"}*

```diff
@@ -5,31 +5,31 @@
         "group": "Detection Parameters",
         "label": "Flip sign",
         "main": false,
         "value": false
     },
     "ga_group_name": {
         "enabled": true,
-        "group": "Python run preferences",
+        "group": "3 - Python run preferences",
         "label": "Save As",
-        "main": false,
+        "main": true,
         "value": "peak_finder"
     },
     "geoh5": "",
     "group_a_color": {
         "dataType": "Text",
-        "group": "Group A",
+        "group": "2- Group A",
         "label": "Color",
         "main": true,
         "value": "#0000FF"
     },
     "group_a_data": {
         "association": "Vertex",
         "dataGroupType": "Multi-element",
-        "group": "Group A",
+        "group": "2- Group A",
         "label": "Property Group",
         "main": true,
         "parent": "objects",
         "value": ""
     },
     "group_b_color": {
         "dataType": "Text",
@@ -135,17 +135,19 @@
         "label": "Run interactive app",
         "main": true,
         "value": true
     },
     "line_field": {
         "association": "Vertex",
         "dataType": "Referenced",
-        "group": "Data",
+        "enabled": false,
+        "group": "1 - Data",
         "label": "Line Field",
         "main": true,
+        "optional": true,
         "parent": "objects",
         "value": ""
     },
     "line_id": "",
     "masking_data": {
         "association": "Vertex",
         "dataType": "Boolean",
@@ -197,15 +199,15 @@
     "n_groups": {
         "group": "Detection Parameters",
         "label": "Merge # Peaks",
         "main": false,
         "value": 1
     },
     "objects": {
-        "group": "Data",
+        "group": "1 - Data",
         "label": "Object",
         "main": true,
         "meshType": [
             "{6a057fdc-b355-11e3-95be-fd84a7ffcb88}",
             "{19730589-fd28-4649-9de0-ad47249d9aba}"
         ],
         "value": ""
@@ -220,21 +222,21 @@
     "smoothing": {
         "group": "Detection Parameters",
         "label": "Smoothing window",
         "main": false,
         "value": 6
     },
     "structural_markers": {
-        "group": "Python run preferences",
+        "group": "3 - Python run preferences",
         "label": "Export all markers",
-        "main": false,
+        "main": true,
         "value": false
     },
     "title": "Peak Finder Parameters",
     "trend_lines": {
+        "group": "3 - Python run preferences",
         "label": "Create trend lines",
         "main": true,
         "value": false
     },
-    "version": "0.1.0",
-    "workspace": ""
+    "version": "0.1.0"
 }
```

### Comparing `peak_finder_app-0.1.0b4/pyproject.toml` & `peak_finder_app-0.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peak-finder-app"
-version = "0.1.0-beta.4"
+version = "0.1.0-rc.1"
 license = "MIT"
 description = "Peak Finder App"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = ["Dominique Fournier <dominiquef@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/peak-finder-app"
 documentation = "https://mirageoscience-peak-finder-app.readthedocs-hosted.com/"
 homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
@@ -47,19 +47,19 @@
 numpy = "~1.23.5"  # also in geoapps-utils, geoh5py
 plotly = "~5.19.0"
 scipy = "~1.10.1"
 tqdm = "^4.66.1"
 
 ## Pip dependencies from Git repositories
 #----------------------------------------
-geoh5py = {version = "~0.9.0rc1", source = "pypi", allow-prereleases = true}  # also in geoapps-utils
+geoh5py = {version = "~0.9.0rc3", source = "pypi", allow-prereleases = true}  # also in geoapps-utils
 #geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
 #geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
 
-geoapps-utils = {version = "~0.3.0rc1", source = "pypi", allow-prereleases = true}
+geoapps-utils = {version = "~0.3.0rc4", source = "pypi", allow-prereleases = true}
 #geoapps-utils = { url = "https://github.com/MiraGeoscience/geoapps-utils/archive/refs/heads/release/0.3.0.zip#sha256=" }
 #geoapps-utils = {url = "http://localhost:8888/geoapps-utils.tar.gz#sha256="}
 
 curve-apps = {version = "~0.1.0rc2", source = "pypi", allow-prereleases = true}
 #curve-apps = {url = "https://github.com/MiraGeoscience/curve-apps/archive/refs/heads/release/0.1.0.zip#sha256="}
 #curve-apps = {url = "http://localhost:8888/curve-apps.tar.gz#sha256="}
```

### Comparing `peak_finder_app-0.1.0b4/README.rst` & `peak_finder_app-0.1.0rc1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -55,79 +55,101 @@
 
 To install **peak-finder-app**, you need to install **Conda** first.
 
 We recommend to install **Conda** using `miniforge`_.
 
 .. _miniforge: https://github.com/conda-forge/miniforge
 
-Within a conda environment
---------------------------
+Quick installation
+-------------------
 
-You can install (or update) a conda environment with all the requires packages to run **peak-finder-app**.
-To do so you can directly run the **Install_or_Update.bat** file by double left clicking on it.
+To install (or re-install) a conda environment to run **peak-finder-app**, simply execute the **install.bat** file.
 
-Install with conda
-------------------
+To install in editable mode, so that changes in the source code are immediately reflected in the
+running application, execute with the ``-e`` option: ``install.bat -e``
+(in editable mode, the source folder must not be moved or deleted after installation).
 
-You can install the package using ``conda`` and the ``.lock`` files from a conda prompt:
 
-.. code-block:: bash
+Manual installation
+-------------------
 
-  conda env create -n my-env -f environments/[the_desired_env].lock.yml
+You should not install the package directly with ``pip``, as the app requires conda packages to run.
 
-Install with PyPI
------------------
+First create a Conda environment with all the required dependencies,
+then activate it and install the package in this environment using
+``pip install --no-deps ...``
 
-You should not install the package from PyPI, as the app requires conda packages to run.
-Still, you can install it in a conda environment without its dependencies (``--no-deps``).
+See instructions below for more details and options.
+
+Prepare a Conda environment with dependencies
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+You can create a Conda environment with all the required dependencies ``conda`` and the ``.lock``
+files from a conda prompt::
+
+    $ conda env create --solver libmamba -n my-env -f environments/[the_desired_env].lock.yml
+
+.. note::
+    The package itself is not install yet in the Conda environment. See following instructions.
+
+.. warning::
+    All the following ``pip`` commands are meant to be executed in the Conda environment you just created.
+    Activate it with::
+
+    $ conda activate my-env
 
 From PyPI
 ~~~~~~~~~
 
-To install the **peak-finder-app** package published on PyPI:
-
-.. code-block:: bash
+To install the **peak-finder-app** package published on PyPI::
 
-    pip install -U --no-deps peak-finder-app
+    $ pip install --no-deps -U peak-finder-app
 
 From a Git tag or branch
 ~~~~~~~~~~~~~~~~~~~~~~~~
-If the package is not on PiPY yet, you can install it from a Git tag:
+If the revision of the package is not on PyPI yet, you can install it from a Git tag::
 
-.. code-block:: bash
+    $ pip install --no-deps -U --force-reinstall https://github.com/MiraGeoscience/peak-finder-app/archive/refs/tags/TAG.zip
 
-    pip install -U --no-deps --force-reinstall https://github.com/MiraGeoscience/peak-finder-app/archive/refs/tags/TAG.zip
+Or to install the latest changes available on a given Git branch::
 
-Or to install the latest changes available on a given Git branch:
-
-.. code-block:: bash
-
-    pip install -U --no-deps --force-reinstall https://github.com/MiraGeoscience/peak-finder-app/archive/refs/heads/BRANCH.zip
+    $ pip install --no-deps -U --force-reinstall https://github.com/MiraGeoscience/peak-finder-app/archive/refs/heads/BRANCH.zip
 
 .. note::
     The ``--force-reinstall`` option is used to make sure the updated version
     of the sources is installed, and not the cached version, even if the version number
-    did not change. The ``-U`` or ``--upgrade`` option is used to make sure to get the latest version,
-    on not merely reinstall the same version. As the package is aimed to be in a **Conda environment**, the option ``--no-deps`` is used to avoid installing the dependencies with pip, as they will be installed with conda.
+    did not change.
+
+    The ``-U`` or ``--upgrade`` option is used to make sure to get the latest version,
+    on not merely reinstall the same version.
+
+    The option ``--no-deps`` is used to avoid installing the dependencies with pip,
+    as they have dependencies are already installed within the **Conda environment**.
 
 From a local copy of the sources
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-If you have a git clone of the package sources locally,
-you can install **peak-finder-app** from the local copy of the sources with:
+If you have a git clone of the package sources locally, you can install **peak-finder-app** from the
+local copy of the sources. At the root of the sources, you will find a ``pyproject.toml`` file.
 
-.. code-block:: bash
+Change directory to the root of the sources::
 
-    pip install -U --force-reinstall path/to/project_folder_with_pyproject_toml
+    $ cd path/to/project_folder_with_pyproject_toml
 
-Or in **editable mode**, so that you can edit the sources and see the effect immediately at runtime:
+Then run::
 
-.. code-block:: bash
+    $ pip install --no-deps -U --force-reinstall .
 
-    pip install -e -U --force-reinstall path/to/project_folder_with_pyproject_toml
+Or in **editable mode**, so that you can edit the sources and see the effect immediately at runtime::
 
+    $ pip install --no-deps -U --force-reinstall -e .
+
+Setup for development
+^^^^^^^^^^^^^^^^^^^^^
+To configure the development environment and tools, please see `README-dev.rst`_.
+
+.. _README-dev.rst: README-dev.rst
 
 License
 ^^^^^^^
 MIT License
 
 Copyright (c) 2024 Mira Geoscience
 
@@ -155,7 +177,11 @@
 The peak-finder-app Software may provide links to third party libraries or code (collectively “Third Party Software”)
 to implement various functions. Third Party Software does not comprise part of the Software.
 The use of Third Party Software is governed by the terms of such software license(s).
 Third Party Software notices and/or additional terms and conditions are located in the
 `THIRD_PARTY_SOFTWARE.rst`_ file.
 
 .. _THIRD_PARTY_SOFTWARE.rst: THIRD_PARTY_SOFTWARE.rst
+
+Copyright
+^^^^^^^^^
+Copyright (c) 2024 Mira Geoscience Ltd.
```

### Comparing `peak_finder_app-0.1.0b4/THIRD_PARTY_SOFTWARE.rst` & `peak_finder_app-0.1.0rc1/THIRD_PARTY_SOFTWARE.rst`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b4/PKG-INFO` & `peak_finder_app-0.1.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-finder-app
-Version: 0.1.0b4
+Version: 0.1.0rc1
 Summary: Peak Finder App
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Dominique Fournier
 Maintainer-email: dominiquef@mirageoscience.com
@@ -26,16 +26,16 @@
 Requires-Dist: Pillow (>=10.1.0,<10.2.0)
 Requires-Dist: curve-apps (>=0.1.0rc2,<0.2.0)
 Requires-Dist: dash (>=2.12,<3.0) ; extra == "dash"
 Requires-Dist: dash-daq (>=0.5.0,<0.6.0) ; extra == "dash"
 Requires-Dist: dask[distributed] (==2022.10.*)
 Requires-Dist: distributed (==2022.10.*)
 Requires-Dist: flask (>=3.0.3,<4.0.0) ; extra == "dash"
-Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
-Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
+Requires-Dist: geoapps-utils (>=0.3.0rc4,<0.4.0)
+Requires-Dist: geoh5py (>=0.9.0rc3,<0.10.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: plotly (>=5.19.0,<5.20.0)
 Requires-Dist: pydantic (>=2.5.2,<2.6.0)
 Requires-Dist: pyqt5-qt5 (==5.15.2) ; extra == "dash"
 Requires-Dist: pyqtwebengine (>=5.15.2,<5.15.7) ; extra == "dash"
 Requires-Dist: pyqtwebengine-qt5 (==5.15.2) ; extra == "dash"
@@ -104,79 +104,101 @@
 
 To install **peak-finder-app**, you need to install **Conda** first.
 
 We recommend to install **Conda** using `miniforge`_.
 
 .. _miniforge: https://github.com/conda-forge/miniforge
 
-Within a conda environment
---------------------------
+Quick installation
+-------------------
 
-You can install (or update) a conda environment with all the requires packages to run **peak-finder-app**.
-To do so you can directly run the **Install_or_Update.bat** file by double left clicking on it.
+To install (or re-install) a conda environment to run **peak-finder-app**, simply execute the **install.bat** file.
 
-Install with conda
-------------------
+To install in editable mode, so that changes in the source code are immediately reflected in the
+running application, execute with the ``-e`` option: ``install.bat -e``
+(in editable mode, the source folder must not be moved or deleted after installation).
 
-You can install the package using ``conda`` and the ``.lock`` files from a conda prompt:
 
-.. code-block:: bash
+Manual installation
+-------------------
 
-  conda env create -n my-env -f environments/[the_desired_env].lock.yml
+You should not install the package directly with ``pip``, as the app requires conda packages to run.
 
-Install with PyPI
------------------
+First create a Conda environment with all the required dependencies,
+then activate it and install the package in this environment using
+``pip install --no-deps ...``
 
-You should not install the package from PyPI, as the app requires conda packages to run.
-Still, you can install it in a conda environment without its dependencies (``--no-deps``).
+See instructions below for more details and options.
+
+Prepare a Conda environment with dependencies
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+You can create a Conda environment with all the required dependencies ``conda`` and the ``.lock``
+files from a conda prompt::
+
+    $ conda env create --solver libmamba -n my-env -f environments/[the_desired_env].lock.yml
+
+.. note::
+    The package itself is not install yet in the Conda environment. See following instructions.
+
+.. warning::
+    All the following ``pip`` commands are meant to be executed in the Conda environment you just created.
+    Activate it with::
+
+    $ conda activate my-env
 
 From PyPI
 ~~~~~~~~~
 
-To install the **peak-finder-app** package published on PyPI:
-
-.. code-block:: bash
+To install the **peak-finder-app** package published on PyPI::
 
-    pip install -U --no-deps peak-finder-app
+    $ pip install --no-deps -U peak-finder-app
 
 From a Git tag or branch
 ~~~~~~~~~~~~~~~~~~~~~~~~
-If the package is not on PiPY yet, you can install it from a Git tag:
+If the revision of the package is not on PyPI yet, you can install it from a Git tag::
 
-.. code-block:: bash
+    $ pip install --no-deps -U --force-reinstall https://github.com/MiraGeoscience/peak-finder-app/archive/refs/tags/TAG.zip
 
-    pip install -U --no-deps --force-reinstall https://github.com/MiraGeoscience/peak-finder-app/archive/refs/tags/TAG.zip
+Or to install the latest changes available on a given Git branch::
 
-Or to install the latest changes available on a given Git branch:
-
-.. code-block:: bash
-
-    pip install -U --no-deps --force-reinstall https://github.com/MiraGeoscience/peak-finder-app/archive/refs/heads/BRANCH.zip
+    $ pip install --no-deps -U --force-reinstall https://github.com/MiraGeoscience/peak-finder-app/archive/refs/heads/BRANCH.zip
 
 .. note::
     The ``--force-reinstall`` option is used to make sure the updated version
     of the sources is installed, and not the cached version, even if the version number
-    did not change. The ``-U`` or ``--upgrade`` option is used to make sure to get the latest version,
-    on not merely reinstall the same version. As the package is aimed to be in a **Conda environment**, the option ``--no-deps`` is used to avoid installing the dependencies with pip, as they will be installed with conda.
+    did not change.
+
+    The ``-U`` or ``--upgrade`` option is used to make sure to get the latest version,
+    on not merely reinstall the same version.
+
+    The option ``--no-deps`` is used to avoid installing the dependencies with pip,
+    as they have dependencies are already installed within the **Conda environment**.
 
 From a local copy of the sources
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-If you have a git clone of the package sources locally,
-you can install **peak-finder-app** from the local copy of the sources with:
+If you have a git clone of the package sources locally, you can install **peak-finder-app** from the
+local copy of the sources. At the root of the sources, you will find a ``pyproject.toml`` file.
 
-.. code-block:: bash
+Change directory to the root of the sources::
 
-    pip install -U --force-reinstall path/to/project_folder_with_pyproject_toml
+    $ cd path/to/project_folder_with_pyproject_toml
 
-Or in **editable mode**, so that you can edit the sources and see the effect immediately at runtime:
+Then run::
 
-.. code-block:: bash
+    $ pip install --no-deps -U --force-reinstall .
 
-    pip install -e -U --force-reinstall path/to/project_folder_with_pyproject_toml
+Or in **editable mode**, so that you can edit the sources and see the effect immediately at runtime::
 
+    $ pip install --no-deps -U --force-reinstall -e .
+
+Setup for development
+^^^^^^^^^^^^^^^^^^^^^
+To configure the development environment and tools, please see `README-dev.rst`_.
+
+.. _README-dev.rst: README-dev.rst
 
 License
 ^^^^^^^
 MIT License
 
 Copyright (c) 2024 Mira Geoscience
 
@@ -205,7 +227,11 @@
 to implement various functions. Third Party Software does not comprise part of the Software.
 The use of Third Party Software is governed by the terms of such software license(s).
 Third Party Software notices and/or additional terms and conditions are located in the
 `THIRD_PARTY_SOFTWARE.rst`_ file.
 
 .. _THIRD_PARTY_SOFTWARE.rst: THIRD_PARTY_SOFTWARE.rst
 
+Copyright
+^^^^^^^^^
+Copyright (c) 2024 Mira Geoscience Ltd.
+
```

