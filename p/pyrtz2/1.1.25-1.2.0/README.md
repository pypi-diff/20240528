# Comparing `tmp/pyrtz2-1.1.25.tar.gz` & `tmp/pyrtz2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.1.25.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.1.25.tar` & `pyrtz2-1.2.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.25/.gitattributes
--rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.25/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.25/LICENSE
--rw-r--r--   0        0        0      771 2024-04-19 14:18:48.509303 pyrtz2-1.1.25/README.md
--rw-r--r--   0        0        0   108501 2024-04-12 19:08:16.330771 pyrtz2-1.1.25/example/con050.PNG
--rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell37m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell37m0001.tif
--rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell38m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell38m0001.tif
--rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell39m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell39m0001.tif
--rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell40m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell40m0001.tif
--rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell42m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.25/example/con050/jasYcon050cell42m0001.tif
--rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.25/example/con050_cp_annotations.json
--rw-r--r--   0        0        0   216499 2024-04-09 18:08:42.337499 pyrtz2-1.1.25/example/con050_curves.pdf
--rw-r--r--   0        0        0     1245 2024-04-09 18:08:23.807163 pyrtz2-1.1.25/example/con050_fits.csv
--rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.25/example/con050_vd_annotations.json
--rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.25/example/test.py
--rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.25/pyproject.toml
--rw-r--r--   0        0        0       62 2024-05-12 14:31:31.060598 pyrtz2-1.1.25/pyrtz2/__init__.py
--rw-r--r--   0        0        0     2905 2024-05-12 14:31:18.502112 pyrtz2-1.1.25/pyrtz2/afm.py
--rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.25/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.25/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     5108 2024-05-09 16:24:06.292616 pyrtz2-1.1.25/pyrtz2/asylum.py
--rw-r--r--   0        0        0    17635 2024-05-09 16:12:23.316799 pyrtz2-1.1.25/pyrtz2/curves.py
--rw-r--r--   0        0        0     4451 2024-05-12 13:36:33.665861 pyrtz2-1.1.25/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.25/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.25/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.25/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.25/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.1.25/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     2826 2024-04-06 15:45:15.625467 pyrtz2-1.1.25/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     2874 2024-04-06 15:44:47.448540 pyrtz2-1.1.25/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.25/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1186 2024-04-06 15:49:10.935231 pyrtz2-1.1.25/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     1718 2024-05-11 14:17:25.543113 pyrtz2-1.1.25/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1707 2024-04-06 15:49:56.149071 pyrtz2-1.1.25/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3230 2024-04-06 15:49:27.361168 pyrtz2-1.1.25/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.25/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.25/pyrtz2/src/data/__init__.py
--rw-r--r--   0        0        0     3275 2024-04-06 15:49:11.334196 pyrtz2-1.1.25/pyrtz2/src/data/downloader.py
--rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.25/pyrtz2/src/data/experiment_loader.py
--rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.25/pyrtz2/src/data/image_loader.py
--rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.25/pyrtz2/src/data/processor.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.25/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.25/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 pyrtz2-1.1.25/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.2.0/.gitattributes
+-rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.2.0/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.2.0/LICENSE
+-rw-r--r--   0        0        0      771 2024-04-19 14:18:48.509303 pyrtz2-1.2.0/README.md
+-rw-r--r--   0        0        0   108501 2024-04-12 19:08:16.330771 pyrtz2-1.2.0/example/con050.PNG
+-rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell37m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell37m0001.tif
+-rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell38m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell38m0001.tif
+-rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell39m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell39m0001.tif
+-rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell40m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell40m0001.tif
+-rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell42m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell42m0001.tif
+-rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.2.0/example/con050_cp_annotations.json
+-rw-r--r--   0        0        0   216499 2024-04-09 18:08:42.337499 pyrtz2-1.2.0/example/con050_curves.pdf
+-rw-r--r--   0        0        0     1245 2024-04-09 18:08:23.807163 pyrtz2-1.2.0/example/con050_fits.csv
+-rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.2.0/example/con050_vd_annotations.json
+-rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.2.0/example/test.py
+-rw-r--r--   0        0        0      837 2024-05-22 01:14:58.847887 pyrtz2-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-28 05:05:16.395659 pyrtz2-1.2.0/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     2905 2024-05-12 14:31:18.502112 pyrtz2-1.2.0/pyrtz2/afm.py
+-rw-r--r--   0        0        0      334 2024-05-23 04:49:31.358304 pyrtz2-1.2.0/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.2.0/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     5108 2024-05-23 04:03:31.968397 pyrtz2-1.2.0/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    18167 2024-05-26 21:26:32.180350 pyrtz2-1.2.0/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4446 2024-05-23 21:11:51.382633 pyrtz2-1.2.0/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.2.0/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.0/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     2461 2024-05-22 13:02:06.518745 pyrtz2-1.2.0/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     4851 2024-05-22 12:50:02.290868 pyrtz2-1.2.0/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.2.0/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     6326 2024-05-28 05:05:42.387835 pyrtz2-1.2.0/pyrtz2/src/components/downloader.py
+-rw-r--r--   0        0        0     1796 2024-05-26 12:23:11.462175 pyrtz2-1.2.0/pyrtz2/src/components/experiment_loader.py
+-rw-r--r--   0        0        0     3520 2024-05-26 21:30:53.840715 pyrtz2-1.2.0/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     3251 2024-05-26 21:23:53.868511 pyrtz2-1.2.0/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2192 2024-05-24 00:21:12.997723 pyrtz2-1.2.0/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1294 2024-05-28 04:32:50.442531 pyrtz2-1.2.0/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     8188 2024-05-28 04:30:53.580503 pyrtz2-1.2.0/pyrtz2/src/components/image.py
+-rw-r--r--   0        0        0     3530 2024-05-28 04:32:50.846663 pyrtz2-1.2.0/pyrtz2/src/components/image_controls.py
+-rw-r--r--   0        0        0     2929 2024-05-28 04:27:34.233541 pyrtz2-1.2.0/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1102 2024-05-26 18:40:42.770898 pyrtz2-1.2.0/pyrtz2/src/components/image_loader.py
+-rw-r--r--   0        0        0     1509 2024-05-22 12:41:39.698771 pyrtz2-1.2.0/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3214 2024-05-23 03:44:27.840596 pyrtz2-1.2.0/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1211 2024-05-23 03:57:00.269489 pyrtz2-1.2.0/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.0/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2242 2024-05-28 05:00:03.989827 pyrtz2-1.2.0/pyrtz2/src/utils/processor.py
+-rw-r--r--   0        0        0     2905 2024-05-27 16:39:21.314177 pyrtz2-1.2.0/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0     1558 1970-01-01 00:00:00.000000 pyrtz2-1.2.0/PKG-INFO
```

### Comparing `pyrtz2-1.1.25/LICENSE` & `pyrtz2-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/README.md` & `pyrtz2-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050.PNG` & `pyrtz2-1.2.0/example/con050.PNG`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell37m0000.ibw` & `pyrtz2-1.2.0/example/con050/jasYcon050cell37m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell37m0001.tif` & `pyrtz2-1.2.0/example/con050/jasYcon050cell37m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell38m0000.ibw` & `pyrtz2-1.2.0/example/con050/jasYcon050cell38m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell38m0001.tif` & `pyrtz2-1.2.0/example/con050/jasYcon050cell38m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell39m0000.ibw` & `pyrtz2-1.2.0/example/con050/jasYcon050cell39m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell39m0001.tif` & `pyrtz2-1.2.0/example/con050/jasYcon050cell39m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell40m0000.ibw` & `pyrtz2-1.2.0/example/con050/jasYcon050cell40m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell40m0001.tif` & `pyrtz2-1.2.0/example/con050/jasYcon050cell40m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell42m0000.ibw` & `pyrtz2-1.2.0/example/con050/jasYcon050cell42m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050/jasYcon050cell42m0001.tif` & `pyrtz2-1.2.0/example/con050/jasYcon050cell42m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050_curves.pdf` & `pyrtz2-1.2.0/example/con050_curves.pdf`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/example/con050_fits.csv` & `pyrtz2-1.2.0/example/con050_fits.csv`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/pyproject.toml` & `pyrtz2-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     'numpy',
     'pandas',
     'pillow',
     'plotly',
     'PyPDF2',
     'scikit-learn',
     'scipy',
+    'scikit-image',
+    'opencv-python',
     'tqdm',
 ]
 
 [project.urls]
 Documentation = "https://www.youtube.com/@hoseynamiri"
 Source = "https://github.com/HoseynAAmiri/pyrtz2"
 Home = "https://github.com/HoseynAAmiri"
```

### Comparing `pyrtz2-1.1.25/pyrtz2/afm.py` & `pyrtz2-1.2.0/pyrtz2/afm.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/pyrtz2/assets/style.css` & `pyrtz2-1.2.0/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/pyrtz2/asylum.py` & `pyrtz2-1.2.0/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/pyrtz2/curves.py` & `pyrtz2-1.2.0/pyrtz2/curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import pickle
 import pandas as pd
 import numpy as np
 import json
 import ast
 import io
 from tqdm import tqdm
-from typing import Any, Iterable
+from typing import Any, Iterable, overload
 from time import sleep
 
 from .fit import lin_fit, poly_fit, hertzian_fit, biexponential_fit
-from .src.components.fig import make_fig
+from .src.components.fig import make
 
 
 def read_json_file(file: str) -> dict[tuple, bool | int]:
     with open(file, 'rt') as cf:
         anno_str_dict = json.load(cf)
 
     anno_tuple_dict = {}
@@ -101,20 +101,23 @@
         return self.get_data_between(0, self.contact_index)
 
     def get_indent(self) -> pd.DataFrame:
         return self.get_data_between(self.contact_index, self.dwell_range[0])
 
     def get_indent_until(self, ind: float) -> pd.DataFrame:
         indent = self.get_indent()
-        ind_index = (np.abs(indent['ind'].to_numpy() - ind)).argmin()
+        indentation = indent['ind'].to_numpy()
+        indentation = indentation - indentation[0]
+        ind_index = np.argmin(np.abs(indentation - ind))
         return indent.iloc[:ind_index+1].reset_index(drop=True)
 
     def get_indent_between(self, first: float, last: float) -> pd.DataFrame:
         indent = self.get_indent()
         f = indent['f'].to_numpy()
+        f = f - f[0]
         first_index = np.argmin(np.abs(f - f[-1] * first))
         last_index = np.argmin(np.abs(f - f[-1] * last))
         return indent.iloc[first_index:last_index+1].reset_index(drop=True)
 
     def get_dwell(self) -> pd.DataFrame:
         return self.get_data_between(self.dwell_range[0], self.dwell_range[1])
 
@@ -203,15 +206,15 @@
 
         self.figs_data = {
             'approach': (approach['ind'].to_numpy(), approach['f'].to_numpy()),
             'dwell': (dwell['t'].to_numpy(), dwell['f'].to_numpy())
         }
 
     def get_contact_fig_plot(self) -> go.Figure:
-        fig = make_fig(
+        fig = make(
             title=fr"$\text{{Selected Contact Point: {self.contact_index}}}$",
             xaxis=r"$Indentation \text{ (m)}$"
         )
 
         x, y = self.figs_data['approach']
         hover_texts = [f'Index: {i}' for i in range(len(x))]
         trace = go.Scattergl(
@@ -231,15 +234,15 @@
         y_line = y[self.contact_index]
         fig.add_vline(x=x_line, line=dict(color='red', width=1.2))
         fig.add_hline(y=y_line, line=dict(color='red', width=1.2))
         self.contact_fig = fig
         return fig
 
     def get_dwell_fig_plot(self) -> go.Figure:
-        fig = make_fig(
+        fig = make(
             title=r"$\text{Dwell}$",
             xaxis=r"$Time \text{ (s)}$"
         )
 
         x, y = self.figs_data['dwell']
         trace = go.Scattergl(
             x=x,
@@ -250,21 +253,28 @@
         )
 
         fig.add_trace(trace)
 
         self.dwell_fig = fig
         return fig
 
+    @overload
+    def get_fits_data(self, probe_diameter: float, ind: float) -> None: ...
+
+    @overload
+    def get_fits_data(self, probe_diameter: float,
+                      ind: list[float]) -> None: ...
+
     def get_fits_data(self, probe_diameter: float, ind: float | list[float]) -> None:
         indent = self.get_indent()
         indent_x_pred = indent['ind'].to_numpy()
         self.indent_param, self.indent_R2, indent_y_pred = self.fit_indent()
 
-        self.max_ind = max(indent['ind'])
-        self.max_f = max(indent['f'])
+        self.max_ind = np.max(indent['ind'])
+        self.max_f = np.max(indent['f'])
 
         if isinstance(ind, float):
             self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_until(
                 probe_diameter, ind)
             hertzian_x_pred = self.get_indent_until(ind)['ind'].to_numpy()
         elif isinstance(ind, list) and len(ind) == 2:
             self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_between(
@@ -276,64 +286,65 @@
         dwell_x_pred = dwell['t'].to_numpy()
         self.dwell_param, self.dwell_R2, dwell_y_pred = self.fit_dwell()
 
         self.fits_data = {
             'indent': (indent_x_pred, indent_y_pred),
             'hertzian': (hertzian_x_pred, hertzian_y_pred),
             'dwell': (dwell_x_pred, dwell_y_pred),
-
         }
 
     def add_contact_fit(self) -> go.Figure:
-        x, y = self.fits_data['indent']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            name='PolyFit',
-            mode='lines',
-            line={'color': 'red'},
-        )
-        self.contact_fig.add_trace(trace)
+        if hasattr(self, 'fits_data'):
+            x, y = self.fits_data['indent']
+            trace = go.Scattergl(
+                x=x,
+                y=y,
+                name='PolyFit',
+                mode='lines',
+                line={'color': 'red'},
+            )
+            self.contact_fig.add_trace(trace)
 
-        x, y = self.fits_data['hertzian']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            name='HertzianFit',
-            mode='lines',
-            line={
-                'color': 'green',
-                'width': 3,
-            },
-        )
-        self.contact_fig.add_trace(trace)
+            x, y = self.fits_data['hertzian']
+            trace = go.Scattergl(
+                x=x,
+                y=y,
+                name='HertzianFit',
+                mode='lines',
+                line={
+                    'color': 'green',
+                    'width': 3,
+                },
+            )
+            self.contact_fig.add_trace(trace)
 
         return self.contact_fig
 
     def add_dwell_fit(self) -> go.Figure:
-        x, y = self.fits_data['dwell']
+        if hasattr(self, 'fits_data'):
+            x, y = self.fits_data['dwell']
 
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            name='DwellFit',
-            mode='lines',
-            line={
-                'color': 'green',
-                'width': 3,
-            },
-        )
-        self.dwell_fig.add_trace(trace)
+            trace = go.Scattergl(
+                x=x,
+                y=y,
+                name='DwellFit',
+                mode='lines',
+                line={
+                    'color': 'green',
+                    'width': 3,
+                },
+            )
+            self.dwell_fig.add_trace(trace)
 
         return self.dwell_fig
 
     def get_contact_fig_pdf(self) -> go.Figure:
         title = fr"$\text{{Selected Contact Point: {self.contact_index}}}$"
         xaxis = r"$Indentation \text{ (m)}$"
-        fig = make_fig(title, xaxis)
+        fig = make(title, xaxis)
 
         x, y = self.figs_data['approach']
         trace = go.Scatter(x=x, y=y, name='Approach', marker={'color': 'blue'})
         fig.add_trace(trace)
 
         x_line = x[self.contact_index]
         y_line = y[self.contact_index]
@@ -354,15 +365,15 @@
         fig.update_layout(width=480, height=400)
         sleep(1)
         return fig
 
     def get_dwell_fig_pdf(self) -> go.Figure:
         title = r"$\text{Dwell}$"
         xaxis = r"$Time \text{ (s)}$"
-        fig = make_fig(title, xaxis)
+        fig = make(title, xaxis)
 
         x, y = self.figs_data['dwell']
         trace = go.Scatter(x=x, y=y, name='Dwell',
                            marker_color='red')
         fig.add_trace(trace)
 
         if hasattr(self, 'fits_data'):
```

### Comparing `pyrtz2-1.1.25/pyrtz2/fit.py` & `pyrtz2-1.2.0/pyrtz2/fit.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,54 +34,53 @@
     y_pred = np.poly1d(popt)(x)
     r2_score = r2(y, y_pred)
     return popt, r2_score, y_pred
 
 
 def powerlaw_fit(x, y):
     x_min = min(x)
-    x_max = max(x)
     y_min = min(y)
+    x = (x - x_min)
+    x_max = max(x)
+    x = x / x_max
+    y = (y - y_min)
     y_max = max(y)
-    x = (x - x_min) / x_max
-    y = (y - y_min) / y_max
+    y = y / y_max
     bounds = ([0, 0], [np.inf, np.inf])
     popt, _ = curve_fit(powerlaw, x, y, bounds=bounds)
     y_pred = powerlaw(x, *popt)
     r2_score = r2(y, y_pred)
     return popt, r2_score, y_pred * y_max + y_min
 
 
 def poly_fit(x, y):
     x_min = min(x)
-    x_max = max(x)
     y_min = min(y)
+    x = (x - x_min)
+    x_max = max(x)
+    x = x / x_max
+    y = (y - y_min)
     y_max = max(y)
-    x = (x - x_min) / x_max
-    y = (y - y_min) / y_max
-    bounds = ([0, 0,  0], [np.inf, np.inf, np.inf])
-    popt, _ = curve_fit(poly, x, y, bounds=bounds)
+    y = y / y_max
+    bounds = ([0, 0, 0], [np.inf, np.inf, np.inf])
+    p0 = [1, 1, 1]
+    popt, _ = curve_fit(poly, x, y, bounds=bounds, p0=p0, jac='3-point')
     y_pred = poly(x, *popt)
     r2_score = r2(y, y_pred)
     return popt, r2_score, y_pred * y_max + y_min
 
 
 def hertzian_fit(x, y, diameter):
     def wrapper(ind, e_star):
         return hertzian(ind, diameter, e_star)
 
-    x_min = min(x)
-    y_min = min(y)
-    x = x - x_min
-    y = y - y_min
-
     popt, _ = curve_fit(wrapper, x, y)
-
     y_pred = hertzian(x, diameter, *popt)
     r2_score = r2(y, y_pred)
-    return popt, r2_score, y_pred + y_min
+    return popt, r2_score, y_pred
 
 
 def exponential_fit(x, y, bound=False):
     if bound:
         def bnd_wrapper(t, tau):
             return exponential(t, y[0], tau, y[-1])
```

### Comparing `pyrtz2-1.1.25/pyrtz2/src/components/annotator.py` & `pyrtz2-1.2.0/pyrtz2/src/components/annotator.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,42 +8,50 @@
 from ..utils.utils import load_json, update_annotations
 
 
 def render(app: Dash) -> html.Div:
     @app.callback(
         [Output(ids.CP_ANNOTATIONS, 'data', allow_duplicate=True),
          Output(ids.VD_ANNOTATIONS, 'data', allow_duplicate=True),
+         Output(ids.IM_ANNOTATIONS, 'data', allow_duplicate=True),
          Output(ids.UPLOAD_ANNOTATIONS, 'contents')],
         [Input(ids.UPLOAD_ANNOTATIONS, 'contents')],
         [State(ids.CP_ANNOTATIONS, 'data'),
-         State(ids.VD_ANNOTATIONS, 'data')],
+         State(ids.VD_ANNOTATIONS, 'data'),
+         State(ids.IM_ANNOTATIONS, 'data')],
         prevent_initial_call=True
     )
-    def load_annotations(encoded_contents, cp_data, vd_data):
-        if not encoded_contents or not cp_data or not vd_data:
+    def load_annotations(encoded_contents, cp_data, vd_data, im_data):
+        if not encoded_contents or not cp_data or not vd_data or not im_data:
             raise PreventUpdate
 
         content_type, content_string = encoded_contents.split(',')
         loaded_annotations = load_json(content_string)
         first_value = next(iter(loaded_annotations.values()))
         if isinstance(first_value, bool):
             vd_annotations = json.loads(vd_data)
             vd_annotations = update_annotations(
                 vd_annotations, loaded_annotations)
-            return no_update, json.dumps(vd_annotations), None
+            return no_update, json.dumps(vd_annotations), no_update, None
         elif isinstance(first_value, int):
             cp_annotations = json.loads(cp_data)
             cp_annotations = update_annotations(
                 cp_annotations, loaded_annotations)
-            return json.dumps(cp_annotations), no_update, None
+            return json.dumps(cp_annotations), no_update, no_update, None
+        elif isinstance(first_value, dict):
+            im_annotations = json.loads(im_data)
+            im_annotations = update_annotations(
+                im_annotations, loaded_annotations)
+            return no_update, no_update, json.dumps(im_annotations), None
 
     return html.Div(
         children=[
             dcc.Store(id=ids.CP_ANNOTATIONS),
             dcc.Store(id=ids.VD_ANNOTATIONS),
+            dcc.Store(id=ids.IM_ANNOTATIONS),
             dcc.Upload(
                 className='drag-drop',
                 children=html.Div(
                     ['Drag and Drop or ', html.A('Select Annotation File'), ' to Load']),
                 id=ids.UPLOAD_ANNOTATIONS,
                 multiple=False
             ),
```

### Comparing `pyrtz2-1.1.25/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.2.0/pyrtz2/src/components/contact_controls.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,21 +123,15 @@
                         ),
                     ],
                     style={
                         'display': 'flex',
                         'gap': '5px',
                     },
                 ),
-            ),
-            html.Button(
-                children="Download Annotations",
-                id=ids.DOWNLOAD_ANNOTATIONS,
-                n_clicks=0,
-                className="dash-button"
-            ),
+            )
         ],
         style={
             'display': 'flex',
             'flex-direction': 'column',
             'gap': '5px',
             'align-items': 'start'
         }
```

### Comparing `pyrtz2-1.1.25/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.2.0/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.25/pyrtz2/src/components/ids.py` & `pyrtz2-1.2.0/pyrtz2/src/components/ids.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,33 +8,37 @@
 
 CURVE_DROPDOWN = "curve-dropdown"
 CURVE_DATA = "curve-data"
 LOAD_ANIMATION = "load-animation"
 BUTTON_BACK = "button-back"
 BUTTON_FORWARD = "button-forward"
 
-IMAGE_FRAME = "image-frame"
-LOADIMAGE_ANIMATION = "loadimage-animation"
+IMAGE_HOLDER = "image-holder"
+CLIP_LIMIT = "cliplimit-input"
+SQUARE_VALUE = "square-value"
+PIXEL_SIZE = "conversion-factor"
+IM_DROPDOWN = "image-dropdown"
 
 UPLOAD_ANNOTATIONS = "upload-annotations"
 CP_ANNOTATIONS = "cp-annotations"
 VD_ANNOTATIONS = "vd-annotations"
+IM_ANNOTATIONS = "img-annotations"
 
 VD_CHECKLIST = "vd-checklist"
 ADJUST_CHECKLIST = "adjust-checklist"
 LOADCONTACT_ANIMATION = "loadcontact-animation"
 DETECT_CONTACT = "detect-contact"
 RESET_CONTACT = "reset-contact"
 FIT_CHECKLIST = "fit-checklist"
 INDENTATION = "indentation"
 
 DOWNLOAD_ANNOTATIONS = "download-annotations"
-DOWNLOAD_IMAGEDATA = "download-imagedata"
 DOWNLOAD_FITS = "download-fits"
 DOWNLOAD_CURVES = "download-curves"
 DOWNLOAD_EXPERIMENT = "download-experiment"
+DOWNLOAD_IMAGES = "download-images"
 DOWNLOAD_ANIMATION = "download-animation"
-DOWNLOAD = 'download'
+DOWNLOAD = "download"
 
 FIG_HOLDER = "fig-holder"
 CONTACT_FIG = "contact-fig"
-FORCETIME_FIG = "forcetime-fig"
+DWELL_FIG = "dwell-fig"
```

### Comparing `pyrtz2-1.1.25/pyrtz2/src/components/layout.py` & `pyrtz2-1.2.0/pyrtz2/src/components/layout.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,19 +32,15 @@
             html.Hr(),
             html.Div(
                 className='dashboard',
                 children=[
                     html.Div(
                         children=[
                             curve_dropdown.render(app),
-                            dcc.Loading(
-                                id=ids.LOADIMAGE_ANIMATION,
-                                type="default",
-                                children=[image_frame.render(app)]
-                            ),
+                            image_frame.render(app),
                         ],
                         style={
                             'width': '50%',
                         },
                     ),
                     toolbox.render(app),
                 ],
```

### Comparing `pyrtz2-1.1.25/pyrtz2/src/components/loader.py` & `pyrtz2-1.2.0/pyrtz2/src/components/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from dash import Dash, dcc, html
 from dash.dependencies import Input, Output, State
 
 import os
 
-from . import ids
-from ..data import (
+from . import (
+    ids,
     experiment_loader,
     image_loader
 )
 
 
 def render(app: Dash) -> html.Div:
-
     @app.callback(
         Output(ids.LOG, 'children'),
         Input(ids.LOAD_EXPERIMENT, 'n_clicks'),
         [State(ids.EXPERIMENT_PATH, 'value'),
          State(ids.EXPERIMENT_LABELS, 'value'),
          State(ids.PROBE_DIAMETER, 'value')],
         prevent_initial_call=True
```

### Comparing `pyrtz2-1.1.25/pyrtz2/src/data/experiment_loader.py` & `pyrtz2-1.2.0/pyrtz2/src/components/experiment_loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 from ...afm import AFM
 from ..components import ids
 from ..utils.utils import dump, make_json
 
 
 def render(app: Dash) -> dcc.Store:
     @app.callback(
-        [Output(ids.EXPERIMENT, 'data', allow_duplicate=True),Output(ids.CP_ANNOTATIONS, 'data', allow_duplicate=True),
-         Output(ids.VD_ANNOTATIONS, 'data', allow_duplicate=True)],
+        [Output(ids.EXPERIMENT, 'data', allow_duplicate=True),
+         Output(ids.CP_ANNOTATIONS, 'data', allow_duplicate=True),
+         Output(ids.VD_ANNOTATIONS, 'data', allow_duplicate=True),
+         Output(ids.IM_ANNOTATIONS, 'data', allow_duplicate=True)],
         [Input(ids.LOAD_EXPERIMENT, 'n_clicks')],
         [State(ids.EXPERIMENT_PATH, 'value'),
          State(ids.EXPERIMENT_LABELS, 'value'),
          State(ids.PROBE_DIAMETER, 'value')],
         prevent_initial_call=True
     )
     def store_experiment_info(_, experiment_path, labels, probe_diameter):
@@ -28,10 +30,12 @@
         exp_name = os.path.basename(os.path.normpath(experiment_path))
         path = os.path.dirname(os.path.normpath(experiment_path))
         label_list = [label.strip() for label in labels.split(';')]
         experiment = AFM(path, exp_name, label_list, float(probe_diameter))
         experiment.experiment.reduce_data()
         cp_data = make_json(experiment.curve_keys, 0)
         vd_data = make_json(experiment.curve_keys, False)
-        return dump(experiment), cp_data, vd_data
+        im_data = make_json(experiment.curve_keys, {'selection': 'exclude',
+                                                    'clickData': []})
+        return dump(experiment), cp_data, vd_data, im_data
 
     return dcc.Store(id=ids.EXPERIMENT)
```

### Comparing `pyrtz2-1.1.25/pyrtz2/src/data/image_loader.py` & `pyrtz2-1.2.0/pyrtz2/src/components/image_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,17 @@
          State(ids.EXPERIMENT_LABELS, 'value')],
         prevent_initial_call=True
     )
     def store_images(_, experiment_path, labels):
         label_list = [label.strip() for label in labels.split(';')]
 
         images = {}
-        all_images_dict = {}
+        all_images = {}
         for tif_path in glob.glob(os.path.join(experiment_path, '*.tif')):
             curve_name = os.path.basename(tif_path).split('.')[0]
             curve_key = extract_keys(curve_name, label_list)
-            all_images_dict[curve_key] = os.path.join(experiment_path, tif_path)
-            images = group_values_by_keys(all_images_dict)
+            all_images[curve_key] = os.path.join(experiment_path, tif_path)
+            images = group_values_by_keys(all_images)
 
         return dump(images)
 
     return dcc.Store(id=ids.IMAGES)
```

### Comparing `pyrtz2-1.1.25/pyrtz2/src/utils/utils.py` & `pyrtz2-1.2.0/pyrtz2/src/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,13 +78,28 @@
         new_key = key[:-1]
         if new_key not in new_dict:
             new_dict[new_key] = [value]
         else:
             new_dict[new_key].append(value)
     return new_dict
 
-def load_image(image_path:str) -> str:
+
+def load_image(image_path: str) -> str:
     img = Image.open(image_path)
     buffer = io.BytesIO()
     img.save(buffer, format="JPEG")  # can be changed to "PNG"
     encoded_image = base64.b64encode(buffer.getvalue()).decode()
-    return f"data:image/jpeg;base64,{encoded_image}"
+    return f"data:image/jpeg;base64,{encoded_image}"
+
+
+def parse_path(shape_path: str) -> list[list[list[int]]]:
+    shape_path = shape_path.replace('M', 'L').replace('Z', 'L')
+    path_parts = shape_path.split('L')
+
+    coordinates = []
+    for part in path_parts:
+        if part.strip():
+            coord_str = part.strip()
+            coord = [int(round(float(x))) for x in coord_str.split(',')]
+            coordinates.append(coord)
+
+    return [coordinates]
```

### Comparing `pyrtz2-1.1.25/PKG-INFO` & `pyrtz2-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.1.25
+Version: 1.2.0
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
@@ -13,14 +13,16 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pillow
 Requires-Dist: plotly
 Requires-Dist: PyPDF2
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
+Requires-Dist: scikit-image
+Requires-Dist: opencv-python
 Requires-Dist: tqdm
 Project-URL: Documentation, https://www.youtube.com/@hoseynamiri
 Project-URL: Home, https://github.com/HoseynAAmiri
 Project-URL: Source, https://github.com/HoseynAAmiri/pyrtz2
 
 # pyrtz2
```

