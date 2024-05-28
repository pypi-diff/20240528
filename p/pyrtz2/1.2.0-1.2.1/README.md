# Comparing `tmp/pyrtz2-1.2.0.tar.gz` & `tmp/pyrtz2-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.2.0.tar` & `pyrtz2-1.2.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.2.0/.gitattributes
--rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.2.0/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.2.0/LICENSE
--rw-r--r--   0        0        0      771 2024-04-19 14:18:48.509303 pyrtz2-1.2.0/README.md
--rw-r--r--   0        0        0   108501 2024-04-12 19:08:16.330771 pyrtz2-1.2.0/example/con050.PNG
--rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell37m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell37m0001.tif
--rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell38m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell38m0001.tif
--rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell39m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell39m0001.tif
--rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell40m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell40m0001.tif
--rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell42m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.2.0/example/con050/jasYcon050cell42m0001.tif
--rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.2.0/example/con050_cp_annotations.json
--rw-r--r--   0        0        0   216499 2024-04-09 18:08:42.337499 pyrtz2-1.2.0/example/con050_curves.pdf
--rw-r--r--   0        0        0     1245 2024-04-09 18:08:23.807163 pyrtz2-1.2.0/example/con050_fits.csv
--rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.2.0/example/con050_vd_annotations.json
--rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.2.0/example/test.py
--rw-r--r--   0        0        0      837 2024-05-22 01:14:58.847887 pyrtz2-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       61 2024-05-28 05:05:16.395659 pyrtz2-1.2.0/pyrtz2/__init__.py
--rw-r--r--   0        0        0     2905 2024-05-12 14:31:18.502112 pyrtz2-1.2.0/pyrtz2/afm.py
--rw-r--r--   0        0        0      334 2024-05-23 04:49:31.358304 pyrtz2-1.2.0/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.2.0/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     5108 2024-05-23 04:03:31.968397 pyrtz2-1.2.0/pyrtz2/asylum.py
--rw-r--r--   0        0        0    18167 2024-05-26 21:26:32.180350 pyrtz2-1.2.0/pyrtz2/curves.py
--rw-r--r--   0        0        0     4446 2024-05-23 21:11:51.382633 pyrtz2-1.2.0/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.2.0/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.0/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     2461 2024-05-22 13:02:06.518745 pyrtz2-1.2.0/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     4851 2024-05-22 12:50:02.290868 pyrtz2-1.2.0/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.2.0/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     6326 2024-05-28 05:05:42.387835 pyrtz2-1.2.0/pyrtz2/src/components/downloader.py
--rw-r--r--   0        0        0     1796 2024-05-26 12:23:11.462175 pyrtz2-1.2.0/pyrtz2/src/components/experiment_loader.py
--rw-r--r--   0        0        0     3520 2024-05-26 21:30:53.840715 pyrtz2-1.2.0/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     3251 2024-05-26 21:23:53.868511 pyrtz2-1.2.0/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2192 2024-05-24 00:21:12.997723 pyrtz2-1.2.0/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1294 2024-05-28 04:32:50.442531 pyrtz2-1.2.0/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     8188 2024-05-28 04:30:53.580503 pyrtz2-1.2.0/pyrtz2/src/components/image.py
--rw-r--r--   0        0        0     3530 2024-05-28 04:32:50.846663 pyrtz2-1.2.0/pyrtz2/src/components/image_controls.py
--rw-r--r--   0        0        0     2929 2024-05-28 04:27:34.233541 pyrtz2-1.2.0/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1102 2024-05-26 18:40:42.770898 pyrtz2-1.2.0/pyrtz2/src/components/image_loader.py
--rw-r--r--   0        0        0     1509 2024-05-22 12:41:39.698771 pyrtz2-1.2.0/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3214 2024-05-23 03:44:27.840596 pyrtz2-1.2.0/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1211 2024-05-23 03:57:00.269489 pyrtz2-1.2.0/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.0/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     2242 2024-05-28 05:00:03.989827 pyrtz2-1.2.0/pyrtz2/src/utils/processor.py
--rw-r--r--   0        0        0     2905 2024-05-27 16:39:21.314177 pyrtz2-1.2.0/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0     1558 1970-01-01 00:00:00.000000 pyrtz2-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.2.1/.gitattributes
+-rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.2.1/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.2.1/LICENSE
+-rw-r--r--   0        0        0      866 2024-05-28 05:21:35.919234 pyrtz2-1.2.1/README.md
+-rw-r--r--   0        0        0   143826 2024-05-28 05:18:47.718007 pyrtz2-1.2.1/example/con050.PNG
+-rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell37m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell37m0001.tif
+-rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell38m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell38m0001.tif
+-rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell39m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell39m0001.tif
+-rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell40m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell40m0001.tif
+-rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell42m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.2.1/example/con050/jasYcon050cell42m0001.tif
+-rw-r--r--   0        0        0      202 2024-05-28 04:49:07.012252 pyrtz2-1.2.1/example/con050_cp_annotations.json
+-rw-r--r--   0        0        0   337342 2024-05-28 05:18:15.173445 pyrtz2-1.2.1/example/con050_curves.pdf
+-rw-r--r--   0        0        0     2741 2024-05-28 05:00:39.789633 pyrtz2-1.2.1/example/con050_fits.csv
+-rw-r--r--   0        0        0     2814 2024-05-28 04:49:07.129790 pyrtz2-1.2.1/example/con050_im_annotations.json
+-rw-r--r--   0        0        0      203 2024-05-28 04:49:07.063912 pyrtz2-1.2.1/example/con050_vd_annotations.json
+-rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.2.1/example/test.py
+-rw-r--r--   0        0        0      837 2024-05-22 01:14:58.847887 pyrtz2-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-28 05:21:48.867345 pyrtz2-1.2.1/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     2905 2024-05-12 14:31:18.502112 pyrtz2-1.2.1/pyrtz2/afm.py
+-rw-r--r--   0        0        0      334 2024-05-23 04:49:31.358304 pyrtz2-1.2.1/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.2.1/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     5108 2024-05-23 04:03:31.968397 pyrtz2-1.2.1/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    18167 2024-05-26 21:26:32.180350 pyrtz2-1.2.1/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4446 2024-05-23 21:11:51.382633 pyrtz2-1.2.1/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.2.1/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.1/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     2461 2024-05-22 13:02:06.518745 pyrtz2-1.2.1/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     4851 2024-05-22 12:50:02.290868 pyrtz2-1.2.1/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.2.1/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     6326 2024-05-28 05:05:42.387835 pyrtz2-1.2.1/pyrtz2/src/components/downloader.py
+-rw-r--r--   0        0        0     1796 2024-05-26 12:23:11.462175 pyrtz2-1.2.1/pyrtz2/src/components/experiment_loader.py
+-rw-r--r--   0        0        0     3520 2024-05-26 21:30:53.840715 pyrtz2-1.2.1/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     3251 2024-05-26 21:23:53.868511 pyrtz2-1.2.1/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2192 2024-05-24 00:21:12.997723 pyrtz2-1.2.1/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1294 2024-05-28 04:32:50.442531 pyrtz2-1.2.1/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     8188 2024-05-28 04:30:53.580503 pyrtz2-1.2.1/pyrtz2/src/components/image.py
+-rw-r--r--   0        0        0     3530 2024-05-28 04:32:50.846663 pyrtz2-1.2.1/pyrtz2/src/components/image_controls.py
+-rw-r--r--   0        0        0     2929 2024-05-28 04:27:34.233541 pyrtz2-1.2.1/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1102 2024-05-26 18:40:42.770898 pyrtz2-1.2.1/pyrtz2/src/components/image_loader.py
+-rw-r--r--   0        0        0     1509 2024-05-22 12:41:39.698771 pyrtz2-1.2.1/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3214 2024-05-23 03:44:27.840596 pyrtz2-1.2.1/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1211 2024-05-23 03:57:00.269489 pyrtz2-1.2.1/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.2.1/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2242 2024-05-28 05:00:03.989827 pyrtz2-1.2.1/pyrtz2/src/utils/processor.py
+-rw-r--r--   0        0        0     2905 2024-05-27 16:39:21.314177 pyrtz2-1.2.1/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 pyrtz2-1.2.1/PKG-INFO
```

### Comparing `pyrtz2-1.2.0/LICENSE` & `pyrtz2-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/README.md` & `pyrtz2-1.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pyrtz2
 
-Analysis of AFM force curves in Python.
+Analysis of AFM force curves and images via Python.
 
 Developed at Georgia Institute of Technology
 
 # Installation
 pyrtz2 is on PyPI. Install using pip (Python version >= 3.10.0 is required)
 
 ```
@@ -15,15 +15,15 @@
 
 ```
 from pyrtz2 import app
 app.run()
 ```
 You should see this interface:
 
-![pyrtz2.app](./example/con050.PNG)
+![pyrtz2.app](https://github.com/HoseynAAmiri/pyrtz2/blob/7c8204bdfcfbe644dc39b43e675b25e689a1cdb9/example/con050.PNG)
 
 You can select the contact point interactively. It will perform fits for approach and dwell parts of the curves using Hertzian and biexponential equations. After downloading the `csv` of fits, you can download those curves in one `pdf` file.
 
 These options are under development:
 - Show Fits
 - Download Image Data
 - Download Experiment
```

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell37m0000.ibw` & `pyrtz2-1.2.1/example/con050/jasYcon050cell37m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell37m0001.tif` & `pyrtz2-1.2.1/example/con050/jasYcon050cell37m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell38m0000.ibw` & `pyrtz2-1.2.1/example/con050/jasYcon050cell38m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell38m0001.tif` & `pyrtz2-1.2.1/example/con050/jasYcon050cell38m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell39m0000.ibw` & `pyrtz2-1.2.1/example/con050/jasYcon050cell39m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell39m0001.tif` & `pyrtz2-1.2.1/example/con050/jasYcon050cell39m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell40m0000.ibw` & `pyrtz2-1.2.1/example/con050/jasYcon050cell40m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell40m0001.tif` & `pyrtz2-1.2.1/example/con050/jasYcon050cell40m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell42m0000.ibw` & `pyrtz2-1.2.1/example/con050/jasYcon050cell42m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/example/con050/jasYcon050cell42m0001.tif` & `pyrtz2-1.2.1/example/con050/jasYcon050cell42m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyproject.toml` & `pyrtz2-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/afm.py` & `pyrtz2-1.2.1/pyrtz2/afm.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/assets/style.css` & `pyrtz2-1.2.1/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/asylum.py` & `pyrtz2-1.2.1/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/curves.py` & `pyrtz2-1.2.1/pyrtz2/curves.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/fit.py` & `pyrtz2-1.2.1/pyrtz2/fit.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/annotator.py` & `pyrtz2-1.2.1/pyrtz2/src/components/annotator.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.2.1/pyrtz2/src/components/contact_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.2.1/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/downloader.py` & `pyrtz2-1.2.1/pyrtz2/src/components/downloader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/experiment_loader.py` & `pyrtz2-1.2.1/pyrtz2/src/components/experiment_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/fig.py` & `pyrtz2-1.2.1/pyrtz2/src/components/fig.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/fig_frame.py` & `pyrtz2-1.2.1/pyrtz2/src/components/fig_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/fitter.py` & `pyrtz2-1.2.1/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/ids.py` & `pyrtz2-1.2.1/pyrtz2/src/components/ids.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/image.py` & `pyrtz2-1.2.1/pyrtz2/src/components/image.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/image_controls.py` & `pyrtz2-1.2.1/pyrtz2/src/components/image_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.2.1/pyrtz2/src/components/image_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/image_loader.py` & `pyrtz2-1.2.1/pyrtz2/src/components/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/layout.py` & `pyrtz2-1.2.1/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/loader.py` & `pyrtz2-1.2.1/pyrtz2/src/components/loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.2.1/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/utils/processor.py` & `pyrtz2-1.2.1/pyrtz2/src/utils/processor.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/pyrtz2/src/utils/utils.py` & `pyrtz2-1.2.1/pyrtz2/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.2.0/PKG-INFO` & `pyrtz2-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.2.0
+Version: 1.2.1
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
@@ -22,15 +22,15 @@
 Requires-Dist: tqdm
 Project-URL: Documentation, https://www.youtube.com/@hoseynamiri
 Project-URL: Home, https://github.com/HoseynAAmiri
 Project-URL: Source, https://github.com/HoseynAAmiri/pyrtz2
 
 # pyrtz2
 
-Analysis of AFM force curves in Python.
+Analysis of AFM force curves and images via Python.
 
 Developed at Georgia Institute of Technology
 
 # Installation
 pyrtz2 is on PyPI. Install using pip (Python version >= 3.10.0 is required)
 
 ```
@@ -41,15 +41,15 @@
 
 ```
 from pyrtz2 import app
 app.run()
 ```
 You should see this interface:
 
-![pyrtz2.app](./example/con050.PNG)
+![pyrtz2.app](https://github.com/HoseynAAmiri/pyrtz2/blob/7c8204bdfcfbe644dc39b43e675b25e689a1cdb9/example/con050.PNG)
 
 You can select the contact point interactively. It will perform fits for approach and dwell parts of the curves using Hertzian and biexponential equations. After downloading the `csv` of fits, you can download those curves in one `pdf` file.
 
 These options are under development:
 - Show Fits
 - Download Image Data
 - Download Experiment
```

