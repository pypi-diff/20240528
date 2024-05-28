# Comparing `tmp/easyidp-2.0.0.dev3.tar.gz` & `tmp/easyidp-2.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyidp-2.0.0.dev3.tar", last modified: Fri Sep  2 08:34:34 2022, max compression
+gzip compressed data, was "easyidp-2.0.0.dev4.tar", last modified: Wed Jan 25 10:02:11 2023, max compression
```

## Comparing `easyidp-2.0.0.dev3.tar` & `easyidp-2.0.0.dev4.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-09-02 08:34:34.294764 easyidp-2.0.0.dev3/
--rw-rw-rw-   0        0        0     1103 2021-03-09 06:14:06.000000 easyidp-2.0.0.dev3/LICENSE
--rw-rw-rw-   0        0        0     9336 2022-09-02 08:34:34.294764 easyidp-2.0.0.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     7996 2022-07-28 11:21:49.000000 easyidp-2.0.0.dev3/README.md
-drwxrwxrwx   0        0        0        0 2022-09-02 08:34:34.242092 easyidp-2.0.0.dev3/easyidp/
--rw-rw-rw-   0        0        0     4682 2022-09-02 03:47:11.000000 easyidp-2.0.0.dev3/easyidp/__init__.py
--rw-rw-rw-   0        0        0     8360 2022-09-02 03:30:30.000000 easyidp-2.0.0.dev3/easyidp/cvtools.py
--rw-rw-rw-   0        0        0    18700 2022-08-04 12:25:37.000000 easyidp-2.0.0.dev3/easyidp/data.py
--rw-rw-rw-   0        0        0    40312 2022-08-04 13:10:07.000000 easyidp-2.0.0.dev3/easyidp/geotiff.py
--rw-rw-rw-   0        0        0     8170 2022-09-02 03:30:23.000000 easyidp-2.0.0.dev3/easyidp/jsonfile.py
--rw-rw-rw-   0        0        0    40126 2022-09-02 08:13:15.000000 easyidp-2.0.0.dev3/easyidp/metashape.py
--rw-rw-rw-   0        0        0    35530 2022-09-02 08:13:23.000000 easyidp-2.0.0.dev3/easyidp/pix4d.py
--rw-rw-rw-   0        0        0    18179 2022-08-04 12:09:01.000000 easyidp-2.0.0.dev3/easyidp/pointcloud.py
--rw-rw-rw-   0        0        0    14952 2022-08-04 13:10:51.000000 easyidp-2.0.0.dev3/easyidp/reconstruct.py
--rw-rw-rw-   0        0        0    17223 2022-08-04 12:03:05.000000 easyidp-2.0.0.dev3/easyidp/roi.py
--rw-rw-rw-   0        0        0    16349 2022-08-06 07:30:28.000000 easyidp-2.0.0.dev3/easyidp/shp.py
--rw-rw-rw-   0        0        0     3199 2022-07-15 08:23:41.000000 easyidp-2.0.0.dev3/easyidp/visualize.py
-drwxrwxrwx   0        0        0        0 2022-09-02 08:34:34.257658 easyidp-2.0.0.dev3/easyidp.egg-info/
--rw-rw-rw-   0        0        0     9336 2022-09-02 08:34:34.000000 easyidp-2.0.0.dev3/easyidp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2022-09-02 08:34:34.000000 easyidp-2.0.0.dev3/easyidp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-02 08:34:34.000000 easyidp-2.0.0.dev3/easyidp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      373 2022-09-02 08:34:34.000000 easyidp-2.0.0.dev3/easyidp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-09-02 08:34:34.000000 easyidp-2.0.0.dev3/easyidp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       81 2022-09-02 08:34:34.298794 easyidp-2.0.0.dev3/setup.cfg
--rw-rw-rw-   0        0        0     2493 2022-09-02 08:33:01.000000 easyidp-2.0.0.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-02 08:34:34.293759 easyidp-2.0.0.dev3/tests/
--rw-rw-rw-   0        0        0      348 2022-08-04 13:24:52.000000 easyidp-2.0.0.dev3/tests/__init__.py
--rw-rw-rw-   0        0        0     6553 2022-08-20 16:15:27.000000 easyidp-2.0.0.dev3/tests/test_cvtools.py
--rw-rw-rw-   0        0        0      753 2022-08-04 12:40:27.000000 easyidp-2.0.0.dev3/tests/test_data.py
--rw-rw-rw-   0        0        0    20513 2022-08-04 12:33:52.000000 easyidp-2.0.0.dev3/tests/test_geotiff.py
--rw-rw-rw-   0        0        0     1415 2022-09-02 03:30:23.000000 easyidp-2.0.0.dev3/tests/test_jsonfile.py
--rw-rw-rw-   0        0        0    14474 2022-09-02 08:11:07.000000 easyidp-2.0.0.dev3/tests/test_metashape.py
--rw-rw-rw-   0        0        0     1406 2022-07-26 08:56:27.000000 easyidp-2.0.0.dev3/tests/test_pathtools.py
--rw-rw-rw-   0        0        0     9566 2022-09-02 07:58:10.000000 easyidp-2.0.0.dev3/tests/test_pix4d.py
--rw-rw-rw-   0        0        0    18731 2022-08-04 10:56:15.000000 easyidp-2.0.0.dev3/tests/test_pointcloud.py
--rw-rw-rw-   0        0        0     5580 2022-08-04 13:25:23.000000 easyidp-2.0.0.dev3/tests/test_reconstruct.py
--rw-rw-rw-   0        0        0     8852 2022-08-04 11:56:48.000000 easyidp-2.0.0.dev3/tests/test_roi.py
--rw-rw-rw-   0        0        0     8283 2022-08-04 10:20:34.000000 easyidp-2.0.0.dev3/tests/test_shp.py
+drwxrwxrwx   0        0        0        0 2023-01-25 10:02:11.096249 easyidp-2.0.0.dev4/
+-rw-rw-rw-   0        0        0     1103 2022-10-24 08:31:27.000000 easyidp-2.0.0.dev4/LICENSE
+-rw-rw-rw-   0        0        0     6783 2023-01-25 10:02:11.097250 easyidp-2.0.0.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     5408 2023-01-12 11:47:25.000000 easyidp-2.0.0.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-01-25 10:02:10.961685 easyidp-2.0.0.dev4/easyidp/
+-rw-rw-rw-   0        0        0     7451 2023-01-25 04:48:18.000000 easyidp-2.0.0.dev4/easyidp/__init__.py
+-rw-rw-rw-   0        0        0    14103 2023-01-12 11:47:25.000000 easyidp-2.0.0.dev4/easyidp/cvtools.py
+-rw-rw-rw-   0        0        0    22526 2023-01-25 08:15:54.000000 easyidp-2.0.0.dev4/easyidp/data.py
+-rw-rw-rw-   0        0        0    60552 2023-01-19 06:50:36.000000 easyidp-2.0.0.dev4/easyidp/geotiff.py
+-rw-rw-rw-   0        0        0     7366 2023-01-19 07:02:31.000000 easyidp-2.0.0.dev4/easyidp/geotools.py
+-rw-rw-rw-   0        0        0     8557 2023-01-12 11:47:25.000000 easyidp-2.0.0.dev4/easyidp/jsonfile.py
+-rw-rw-rw-   0        0        0    64092 2023-01-25 08:54:33.000000 easyidp-2.0.0.dev4/easyidp/metashape.py
+-rw-rw-rw-   0        0        0    67648 2023-01-25 08:54:22.000000 easyidp-2.0.0.dev4/easyidp/pix4d.py
+-rw-rw-rw-   0        0        0    51066 2023-01-20 07:30:20.000000 easyidp-2.0.0.dev4/easyidp/pointcloud.py
+-rw-rw-rw-   0        0        0    27955 2023-01-25 08:49:29.000000 easyidp-2.0.0.dev4/easyidp/reconstruct.py
+-rw-rw-rw-   0        0        0    43385 2023-01-25 09:12:08.000000 easyidp-2.0.0.dev4/easyidp/roi.py
+-rw-rw-rw-   0        0        0    16343 2023-01-19 06:16:26.000000 easyidp-2.0.0.dev4/easyidp/shp.py
+-rw-rw-rw-   0        0        0    11593 2023-01-25 05:15:00.000000 easyidp-2.0.0.dev4/easyidp/visualize.py
+drwxrwxrwx   0        0        0        0 2023-01-25 10:02:10.972699 easyidp-2.0.0.dev4/easyidp.egg-info/
+-rw-rw-rw-   0        0        0     6783 2023-01-25 10:02:10.000000 easyidp-2.0.0.dev4/easyidp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-01-25 10:02:10.000000 easyidp-2.0.0.dev4/easyidp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-25 10:02:10.000000 easyidp-2.0.0.dev4/easyidp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      432 2023-01-25 10:02:10.000000 easyidp-2.0.0.dev4/easyidp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-01-25 10:02:10.000000 easyidp-2.0.0.dev4/easyidp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       81 2023-01-25 10:02:11.097250 easyidp-2.0.0.dev4/setup.cfg
+-rw-rw-rw-   0        0        0     2702 2022-10-24 23:02:38.000000 easyidp-2.0.0.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-25 10:02:11.096249 easyidp-2.0.0.dev4/tests/
+-rw-rw-rw-   0        0        0      365 2023-01-25 08:14:37.000000 easyidp-2.0.0.dev4/tests/__init__.py
+-rw-rw-rw-   0        0        0    15021 2023-01-12 11:47:25.000000 easyidp-2.0.0.dev4/tests/test_cvtools.py
+-rw-rw-rw-   0        0        0     1024 2023-01-20 01:47:05.000000 easyidp-2.0.0.dev4/tests/test_data.py
+-rw-rw-rw-   0        0        0    24066 2023-01-19 06:49:17.000000 easyidp-2.0.0.dev4/tests/test_geotiff.py
+-rw-rw-rw-   0        0        0     4481 2023-01-12 11:47:26.000000 easyidp-2.0.0.dev4/tests/test_init_class_func.py
+-rw-rw-rw-   0        0        0     1415 2022-09-02 03:30:23.000000 easyidp-2.0.0.dev4/tests/test_jsonfile.py
+-rw-rw-rw-   0        0        0    20399 2023-01-24 07:33:17.000000 easyidp-2.0.0.dev4/tests/test_metashape.py
+-rw-rw-rw-   0        0        0    10914 2023-01-25 04:49:40.000000 easyidp-2.0.0.dev4/tests/test_pix4d.py
+-rw-rw-rw-   0        0        0    18758 2022-12-26 09:47:44.000000 easyidp-2.0.0.dev4/tests/test_pointcloud.py
+-rw-rw-rw-   0        0        0     9749 2023-01-25 09:46:56.000000 easyidp-2.0.0.dev4/tests/test_reconstruct.py
+-rw-rw-rw-   0        0        0    11400 2023-01-12 11:47:26.000000 easyidp-2.0.0.dev4/tests/test_roi.py
+-rw-rw-rw-   0        0        0     8413 2023-01-19 06:16:26.000000 easyidp-2.0.0.dev4/tests/test_shp.py
+-rw-rw-rw-   0        0        0     4219 2023-01-25 09:46:01.000000 easyidp-2.0.0.dev4/tests/test_visualize.py
```

### Comparing `easyidp-2.0.0.dev3/LICENSE` & `easyidp-2.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `easyidp-2.0.0.dev3/easyidp/data.py` & `easyidp-2.0.0.dev4/easyidp/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         os.mkdir(str(add_usr))
 
     return add_usr / file_name
 
 def show_data_dir():
     """open the cached data files in cross-platform system default viewer.
 
+    Notes
+    -----
     It modified from this [1]_ webpage.
 
     References
     ----------
     .. [1] Python: Opening a folder in Explorer/Nautilus/Finder https://stackoverflow.com/questions/6631299/python-opening-a-folder-in-explorer-nautilus-finder
 
     """
@@ -114,14 +116,16 @@
     """
     lotus = Lotus()
     gd = GDownTest()
     test = TestData()
 
 
 class EasyidpDataSet():
+    """The base class for Dataset
+    """
 
     def __init__(self, name="", url_list=[], size="",):
         """The dataset has the following properties (almost in string type)
 
         name
             The dataset name
         url_list
@@ -168,52 +172,14 @@
         self.zip_file = user_data_dir(self.name + ".zip")
 
         self.pix4d = self.ReconsProj()
         self.metashape = self.ReconsProj()
 
     def load_data(self):
         r"""Download dataset from Google Drive to user AppData folder
-
-        Caution
-        -------
-        For users in China mainland, please either find a way to access google drive,
-        or download from `CowTransfer Link <https://cowtransfer.com/s/4cc3d3f199824b>`_ 
-
-        Save and extract all \*.zip file to folder ``idp.data.show_data_dir()``.
-
-        The data structure should like this:
-
-        
-        .. tab:: Windows
-
-            .. code-block:: text
-
-                . C:\Users\<user>\AppData\Local\easyidp.data
-                |-- 2017_tanashi_lotus
-                |-- gdown_test
-                |-- ...
-
-        .. tab:: MacOS
-
-            .. code-block:: text
-
-                . ~/Library/Application Support/easyidp.data
-                |-- 2017_tanashi_lotus
-                |-- gdown_test
-                |-- ...
-
-        .. tab:: Linux/BSD
-
-            .. code-block:: text
-
-                . ~/.local/share/easyidp.data   # or in $XDG_DATA_HOME, if defined
-                |-- 2017_tanashi_lotus
-                |-- gdown_test
-                |-- ...
-
         """
 
         if not os.path.exists(self.data_dir):
             out = self._download_data()
 
             if os.path.exists(self.zip_file):
                 print("Successfully downloaded, start unzipping ...")
@@ -282,21 +248,70 @@
             self.param = ""
             self.dom = ""
             self.dsm = ""
             self.pcd = ""
 
 
 class Lotus(EasyidpDataSet):
+    """The dataset for lotus plot in Tanashi, Tokyo.
+
+    .. image:: ../../_static/images/data/2017_tanashi_lotus.png 
+        :width: 600
+        :alt: 2017_tanashi_lotus.png 
+
+    - **Crop** : lotus
+    - **Location** : Tanashi, Nishi-Tokyo, Japan
+    - **Flight date** : May 31, 2017
+    - **UAV model** : DJI Inspire 1
+    - **Flight height** : 30m
+    - **Image number** :142
+    - **Image size** : 4608 x 3456
+    - **Software** : Pix4D, Metashape
+    - **Outputs** : DOM, DSM, PCD
+    """
+
+    url_list = [
+        "https://drive.google.com/file/d/1SJmp-bG5SZrwdeJL-RnnljM2XmMNMF0j/view?usp=sharing",
+        "https://fieldphenomics.cowtransfer.com/s/9a87698f8d3242"
+    ]
+    name = "2017_tanashi_lotus"
+    size = "3.3GB"
 
     def __init__(self):
-        url_list = [
-            "https://drive.google.com/file/d/1SJmp-bG5SZrwdeJL-RnnljM2XmMNMF0j/view?usp=sharing",
-            "https://cowtransfer.com/s/03355b0b684442"
-        ]
-        super().__init__(name="2017_tanashi_lotus", url_list=url_list, size="3.6GB")
+        """
+        Containts the following arguments, you can access by:
+
+        .. code-block:: python
+
+            >>> lotus = idp.data.Lotus()
+            >>> lotus.photo
+            'C:\\Users\\<user>\\AppData\\Local\\easyidp.data\\2017_tanashi_lotus\\20170531\\photos'
+
+        - ``.photo`` : the folder containts raw images
+        - ``.shp`` : the plot roi shapefile
+        - ``.pix4d.project`` : the pix4d project folder
+        - ``.pix4d.param`` : the pix4d project parameter folder
+        - ``.pix4d.dom`` : the pix4d produced orthomosaic
+        - ``.pix4d.dsm`` : the pix4d produced digial surface del
+        - ``.pix4d.pcd`` : the pix4d produced point cloud
+        - ``.metashape.project`` : the metashape project file
+        - ``.metashape.param`` : the metashape project folder
+        - ``.metashape.dom`` : the metashape produced orthomosaic
+        - ``.metashape.pcd`` : the metashape produced point cloud
+        - ``.metashape.dsm`` : the metashape produced digial surface model
+
+        See also
+        --------
+        EasyidpDataSet
+        """
+        self.data_dir = user_data_dir(self.name)
+        self.zip_file = user_data_dir(self.name + ".zip")
+
+        self.pix4d = self.ReconsProj()
+        self.metashape = self.ReconsProj()
 
         super().load_data()
 
         self.photo = self.data_dir / "20170531" / "photos"
         self.shp = self.data_dir / "plots.shp"
 
         self.pix4d.project = self.data_dir / "20170531"
@@ -308,47 +323,144 @@
 
         self.metashape.project = self.data_dir / "170531.Lotus.psx"
         self.metashape.param = self.data_dir / "170531.Lotus.files"
         self.metashape.dom = self.data_dir / "170531.Lotus.outputs" / "170531.Lotus_dom.tif"
         self.metashape.dsm = self.data_dir / "170531.Lotus.outputs" / "170531.Lotus_dsm.tif"
         self.metashape.pcd = self.data_dir / "170531.Lotus.outputs" / "170531.Lotus.laz"
 
-    def load_data(self):
-        return super().load_data()
-
         
 class GDownTest(EasyidpDataSet):
 
+    url_list = [
+        "https://drive.google.com/file/d/1yWvIOYJ1ML-UGleh3gT5b7dxXzBuSPgQ/view?usp=sharing",
+        "https://fieldphenomics.cowtransfer.com/s/b5a469fab5dc48"
+    ]
+
     def __init__(self):
-        url_list = [
-            "https://drive.google.com/file/d/1yWvIOYJ1ML-UGleh3gT5b7dxXzBuSPgQ/view?usp=sharing",
-            "https://cowtransfer.com/s/20fe3984fb9a47"
-        ]
-        super().__init__("gdown_test", url_list, "0.2KB")
+
+        super().__init__("gdown_test", self.url_list, "0.2KB")
         super().load_data()
 
         self.pix4d.proj = self.data_dir / "file1.txt"
         self.metashape.param = self.data_dir / "folder1"
 
-    def load_data(self):
-        return super().load_data()
-
 
 
 class TestData(EasyidpDataSet):
+    """The data for developer and package testing.
+    """
+
+    url_list = [
+        "https://drive.google.com/file/d/17b_17CofqIuCVOWMnD67_wOnWMtwF8bw/view?usp=sharing",
+        "https://fieldphenomics.cowtransfer.com/s/edaf0826b02548"
+    ]
+    
+    name = "data_for_tests"
+    size = "344MB"
 
     def __init__(self, test_out="./tests/out"):
-        url_list = [
-            "https://drive.google.com/file/d/17b_17CofqIuCVOWMnD67_wOnWMtwF8bw/view?usp=sharing",
-            "https://cowtransfer.com/s/9d60d394cbd448"
-        ]
+        """
+        Containts the following arguments, you can access by:
+        
+        **json test module** 
 
-        self.name = "data_for_tests"
-        self.url_list = url_list
-        self.size = "344MB"
+        * ``.json.for_read_json``
+        * ``.json.labelme_demo``
+        * ``.json.labelme_warn``
+        * ``.json.labelme_err``
+
+        **shp test module** 
+
+        * ``.shp.lotus_shp`` 
+        * ``.shp.lotus_prj`` 
+        * ``.shp.complex_shp``
+        * ``.shp.complex_prj``
+        * ``.shp.lonlat_shp``
+        * ``.shp.utm53n_shp``
+        * ``.shp.utm53n_prj``
+        * ``.shp.rice_shp``
+        * ``.shp.rice_prj``
+        * ``.shp.roi_shp``
+        * ``.shp.roi_prj``
+        * ``.shp.testutm_shp``
+        * ``.shp.testutm_prj``
+
+        **pcd test module** 
+
+        * ``.pcd.lotus_las``
+        * ``.pcd.lotus_laz``
+        * ``.pcd.lotus_pcd``
+        * ``.pcd.lotus_las13``
+        * ``.pcd.lotus_laz13``
+        * ``.pcd.lotus_ply_asc``
+        * ``.pcd.lotus_ply_bin``
+        * ``.pcd.maize_las``
+        * ``.pcd.maize_laz``
+        * ``.pcd.maize_ply``
+
+        **roi test module** 
+
+        * ``.roi.dxf``
+        * ``.roi.lxyz_txt``
+        * ``.roi.xyz_txt``
+
+        **geotiff test module**
+
+        * ``.tiff.soyweed_part``
+        * ``.tiff.out``
+
+        **metashape test module** 
+
+        * ``.metashape.goya_psx``
+        * ``.metashape.goya_param``
+        * ``.metashape.lotus_psx``
+        * ``.metashape.lotus_param``
+        * ``.metashape.lotus_dsm``
+        * ``.metashape.wheat_psx``
+        * ``.metashape.wheat_param``
+        * ``.metashape.multichunk_psx``
+        * ``.metashape.multichunk_param``
+
+
+        **pix4d test module** 
+
+        * ``.pix4d.lotus_folder``
+        * ``.pix4d.lotus_param``
+        * ``.pix4d.lotus_photos``
+        * ``.pix4d.lotus_dom``
+        * ``.pix4d.lotus_dsm``
+        * ``.pix4d.lotus_pcd``
+        * ``.pix4d.lotus_dom_part``
+        * ``.pix4d.lotus_dsm_part``
+        * ``.pix4d.lotus_pcd_part``
+        * ``.pix4d.maize_folder``
+        * ``.pix4d.maize_dom``
+        * ``.pix4d.maize_dsm``
+        * ``.pix4d.maize_noparam``
+        * ``.pix4d.maize_empty``
+        * ``.pix4d.maize_noout``
+
+        **cvtools test module** 
+
+        * ``.cv.out``
+        
+        **visualize test module** 
+
+        * ``.vis.out``
+
+
+        Parameters
+        ----------
+        test_out : str, optional
+            The folder for saving temporary outputs, by default "./tests/out"
+
+        See also
+        --------
+        EasyidpDataSet
+        """
         self.data_dir = user_data_dir(self.name)
         self.zip_file = user_data_dir(self.name + ".zip")
 
         super().load_data()
 
         self.json = self.JsonDataset(self.data_dir, test_out)
         self.metashape = self.MetashapeDataset(self.data_dir, test_out)
@@ -356,14 +468,15 @@
         self.shp = self.ShapefileDataset(self.data_dir, test_out)
         self.pcd = self.PointCloudDataset(self.data_dir, test_out)
         self.roi = self.ROIDataset(self.data_dir)
         self.tiff = self.TiffDataSet(self.data_dir, test_out)
 
         self.cv = self.CVDataset(self.data_dir, test_out)
         self.vis = self.VisualDataset(self.data_dir, test_out)
+        self.b2r = self.Back2rawDataset(self.data_dir, test_out)
 
 
     class MetashapeDataset():
 
         def __init__(self, data_dir, test_out):
             if isinstance(test_out, str):
                 test_out = Path(test_out)
@@ -374,14 +487,17 @@
             self.lotus_psx   = data_dir / "metashape" / "Lotus.psx"
             self.lotus_param = data_dir / "metashape" / "Lotus.files"
             self.lotus_dsm   = data_dir / "metashape" / "Lotus.files" / "170531.Lotus_dsm.tif"
 
             self.wheat_psx   = data_dir / "metashape" / "wheat_tanashi.psx"
             self.wheat_param = data_dir / "metashape" / "wheat_tanashi.files"
 
+            self.multichunk_psx   = data_dir / "metashape" / "multichunk.psx"
+            self.multichunk_param = data_dir / "metashape" / "multichunk.files"
+
 
     class Pix4Dataset():
 
         def __init__(self, data_dir):
 
             # here is reorgainzed pix4d project
             self.lotus_folder   = data_dir / "pix4d" / "lotus_tanashi_full"
@@ -527,7 +643,21 @@
 
             if isinstance(test_out, str):
                 test_out = Path(test_out)
             self.out = test_out / "visual_test"
 
         def __truediv__(self, other):
             return self.data_dir / "visual_test" / other
+        
+
+
+    class Back2rawDataset():
+
+        def __init__(self, data_dir, test_out):
+            self.data_dir = data_dir
+
+            if isinstance(test_out, str):
+                test_out = Path(test_out)
+            self.out = test_out / "back2raw_test"
+
+        def __truediv__(self, other):
+            return self.data_dir / "back2raw_test" / other
```

### Comparing `easyidp-2.0.0.dev3/easyidp/jsonfile.py` & `easyidp-2.0.0.dev4/easyidp/jsonfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,268 +1,273 @@
-import json
-import os
-import numpy as np
-
-class MyEncoder(json.JSONEncoder):
-    # The original json package doesn't compatible to numpy object, add this compatible encoder to it.
-    # usage: json.dump(..., cls=MyEncoder)
-    # references: https://stackoverflow.com/questions/27050108/convert-numpy-type-to-python
-    
-    def default(self, obj):
-        if isinstance(obj, np.integer):
-            return int(obj)
-        elif isinstance(obj, np.floating):
-            return float(obj)
-        elif isinstance(obj, np.ndarray):
-            return obj.tolist()
-        else:
-            return super(MyEncoder, self).default(obj)
-
-def read_json(json_path):
-    """Read json file to python dict.
-
-    Parameters
-    ----------
-    json_path : str
-        The path to json file
-
-    Returns
-    -------
-    dict
-    """
-    if os.path.exists(json_path):
-        with open(json_path) as json_file:
-            data = json.load(json_file)
-            return data
-    else:
-        raise FileNotFoundError(f"Could not locate the given json file [{json_path}]")
-
-def dict2json(data_dict, json_path, indent=None, encoding='utf-8'):
-    """Convert dict to the same structure json file
-    
-    Parameters
-    ----------
-    data_dict : dict
-        the dict object want to save as json file
-    json_path : str
-        the path including json file name to save the json file
-        e.g. ``D:/xxx/xxxx/save.json`` 
-    indent : int | None
-        whether save "readable" json with indent, default 0 without indent
-    encoding : str
-        the encoding type of output file
-
-    Notes
-    -----
-    **indient example**
-
-    .. code-block:: python
-
-        >>> print(json.dumps(data), indent=0)
-        {"age": 4, "name": "niuniuche", "attribute": "toy"}
-        >>> print(json.dumps(data,indent=4))
-        {
-            "age": 4,
-            "name": "niuniuche",
-            "attribute": "toy"
-        }
-
-    See also
-    --------
-    easyidp.jsonfile.write_json, easyidp.jsonfile.save_json
-    """
-    json_path = str(json_path)
-    if isinstance(json_path, str) and json_path[-5:] == '.json':
-        with open(json_path, 'w', encoding=encoding) as result_file:
-            json.dump(data_dict, result_file, ensure_ascii=False, cls=MyEncoder, indent=indent)
-
-            # print(f'Save Json file -> {os.path.abspath(json_path)}')
-
-
-def write_json(data_dict, json_path, indent=0, encoding='utf-8'):
-    """Save dict to the same structure json file
-    
-    Parameters
-    ----------
-    data_dict : dict
-        the dict object want to save as json file
-    json_path : str
-        the path including json file name to save the json file
-        e.g. ``D:/xxx/xxxx/save.json``
-    indent : int | None
-        whether save "readable" json with indent, default 0 without indent
-    encoding : str
-        the encoding type of output file
-
-    Notes
-    -----
-    **indient example**
-
-    .. code-block:: python
-
-        >>> print(json.dumps(data), indent=0)
-        {"age": 4, "name": "niuniuche", "attribute": "toy"}
-        >>> print(json.dumps(data,indent=4))
-        {
-            "age": 4,
-            "name": "niuniuche",
-            "attribute": "toy"
-        }
-
-    See also
-    --------
-    easyidp.jsonfile.dict2json, easyidp.jsonfile.save_json
-
-    """
-    dict2json(data_dict, json_path, indent, encoding)
-
-
-def save_json(data_dict, json_path, indent=0, encoding='utf-8'):
-    """Save dict to the same structure json file
-    
-    Parameters
-    ----------
-    data_dict : dict
-        the dict object want to save as json file
-    json_path : str
-        the path including json file name to save the json file
-        e.g. ``D:/xxx/xxxx/save.json``
-    indent : int | None
-        whether save "readable" json with indent, default 0 without indent
-    encoding : str
-        the encoding type of output file
-
-    Notes
-    -----
-    **indient example**
-
-    .. code-block:: python
-
-        >>> print(json.dumps(data), indent=0)
-        {"age": 4, "name": "niuniuche", "attribute": "toy"}
-        >>> print(json.dumps(data,indent=4))
-        {
-            "age": 4,
-            "name": "niuniuche",
-            "attribute": "toy"
-        }
-
-    See also
-    --------
-    easyidp.jsonfile.dict2json, easyidp.jsonfile.save_json
-
-    """
-    dict2json(data_dict, json_path, indent, encoding)
-
-# just copied from previous `caas_lite.py`, haven't modified yet
-def _to_labelme_json(grid_tagged, json_folder, minimize=True):
-    """Save the tagged shp polygon crop result to json file, for deeplearing use
-
-    Parameters
-    ----------
-    grid_tagged : pandas.DataFrame
-        the output of self.dataframe_add_shp_tags()
-        The 4 column dataframe shows in this function introduction, sorted by "grid_name"
-    json_folder : str
-        the folder or path to save those json files
-    minimize : bool
-        whether create a json without space
-
-    Notes
-    -----
-    The labelme json file has the following structure:
-
-    .. code-block:: json
-
-        {
-            "version": "4.5.6",  # the Labelme.exe version, optional
-            "flags": {},
-            "imagePath": "xxxx.tiff",
-            "imageHeight": 1000,
-            "imageWidth": 1000,
-            "imageData": null,
-            "shapes": [{ }, { }, { }]
-        }      
-
-    for each ``{}`` items in "shapes":
-
-    .. code-block:: json
-
-        {
-            "label": "field",
-            "group_id": null,
-            "shape_type": "polygon",
-            "flags": {},
-            "points": [[x1, y1], [x2, y2], [x3, y3]]  # with or without the first point
-        }
-
-    Example of ``grid_tagged`` 
-
-    +------------------+----------+---------------------+-------+
-    |     grid_name    | dict_key |    polygon_list     |  tag  |
-    +==================+==========+=====================+=======+
-    | 'grid_x1_y1.tif' | 'key1'   | [poly1, poly2, ...] | field |
-    +------------------+----------+---------------------+-------+
-    | 'grid_x1_y1.tif' | 'key2'   | [poly1, poly2, ...] | crops |
-    +------------------+----------+---------------------+-------+
-    | 'grid_x1_y2.tif' | 'key1'   | [poly1, poly2, ...] | field |
-    +------------------+----------+---------------------+-------+
-    | 'grid_x2_y1.tif' | 'key1'   | [poly1, poly2, ...] | field |
-    +------------------+----------+---------------------+-------+
-    | 'grid_x3_y2.tif' | 'key2'   | [poly1, poly2, ...] | crops |
-    +------------------+----------+---------------------+-------+
-    |      ...         |   ...    |         ...         |  ...  | 
-    +------------------+----------+---------------------+-------+
-
-    Example of ``minimize``
-
-    - True
-
-      .. code-block:: json
-
-        {"name":"lucy","sex":"boy"}
-    
-    - False
-
-      .. code-block:: json
-
-        {
-            "name":"lucy",
-            "sex":"boy"
-        } 
-
-    """
-    total_dict = {}
-    for i in range(len(grid_tagged)):
-        # todo modify here
-        img_name = grid_tagged.loc[i]['grid_name']
-        poly = grid_tagged.loc[i]['polygon_list']
-        tag = grid_tagged.loc[i]['tag']
-        
-        if img_name not in total_dict.keys():
-            single_dict = {"version": "4.5.6", 
-                            "flags": {},
-                            "imagePath": img_name,
-                            "imageHeight": 1000,
-                            "imageWidth": 1000,
-                            "imageData": None,
-                            "shapes": []}
-        else:
-            single_dict = total_dict[img_name]
-            
-        for item in poly:
-            single_item = {"label": tag,
-                            "group_id": None,   # json null = python None
-                            "shape_type": "polygon",
-                            "flags": {},
-                            "points": item.tolist()}
-            single_dict['shapes'].append(single_item)
-            
-        total_dict[img_name] = single_dict
-        
-    # after iter all items
-    for k, d in total_dict.items():
-        json_name = k.replace('.tif', '.json')
-        if minimize:
-            dict2json(d, os.path.join(json_folder, json_name))
-        else:
+import json
+import os
+import numpy as np
+
+class MyEncoder(json.JSONEncoder):
+    # The original json package doesn't compatible to numpy object, add this compatible encoder to it.
+    # usage: json.dump(..., cls=MyEncoder)
+    # references: https://stackoverflow.com/questions/27050108/convert-numpy-type-to-python
+    
+    def default(self, obj):
+        if isinstance(obj, np.integer):
+            return int(obj)
+        elif isinstance(obj, np.floating):
+            return float(obj)
+        elif isinstance(obj, np.ndarray):
+            return obj.tolist()
+        else:
+            return super(MyEncoder, self).default(obj)
+
+def read_json(json_path):
+    """Read json file to python dict.
+
+    Parameters
+    ----------
+    json_path : str
+        The path to json file
+
+    Returns
+    -------
+    dict
+
+    Example
+    -------
+
+    Data prepare:
+
+    .. code-block:: python
+
+        >>> import easyidp as idp
+        >>> test_data = idp.data.TestData()
+
+    Use this function:
+
+    .. code-block:: python
+
+        >>> out = idp.jsonfile.read_json(test_data.json.for_read_json)
+        >>> out
+        {'test': {'rua': [[12, 34], [45, 56]]}, 'hua': [34, 34.567]}
+
+    """
+    if os.path.exists(json_path):
+        with open(json_path) as json_file:
+            data = json.load(json_file)
+            return data
+    else:
+        raise FileNotFoundError(f"Could not locate the given json file [{json_path}]")
+
+def dict2json(data_dict, json_path, indent=None, encoding='utf-8'):
+    """Save dict object to the same structure json file
+    
+    Parameters
+    ----------
+    data_dict : dict
+        the dict object want to save as json file
+    json_path : str
+        the path including json file name to save the json file
+        e.g. ``D:/xxx/xxxx/save.json`` 
+    indent : int | None
+        whether save "readable" json with indent, default 0 without indent
+    encoding : str
+        the encoding type of output file
+
+    Example
+    -------
+
+    .. code-block:: python
+
+        >>> import easyidp as idp
+        >>> a = {"test": {"rua": np.asarray([[12, 34], [45, 56]])}, "hua":[np.int32(34), np.float64(34.567)]}
+        >>> idp.jsonfile.dict2json(a, "/path/to/save/json_file.json")
+
+    .. note:: 
+
+        Dict without indient:
+
+        .. code-block:: python
+
+            >>> print(json.dumps(data), indent=0)
+            {"age": 4, "name": "niuniuche", "attribute": "toy"}
+
+        Dict with 4 space as indient:
+
+        .. code-block:: python
+
+            >>> print(json.dumps(data,indent=4))
+            {
+                "age": 4,
+                "name": "niuniuche",
+                "attribute": "toy"
+            }
+
+    See also
+    --------
+    easyidp.jsonfile.write_json, easyidp.jsonfile.save_json
+    
+    """
+    json_path = str(json_path)
+    if isinstance(json_path, str) and json_path[-5:] == '.json':
+        with open(json_path, 'w', encoding=encoding) as result_file:
+            json.dump(data_dict, result_file, ensure_ascii=False, cls=MyEncoder, indent=indent)
+
+            # print(f'Save Json file -> {os.path.abspath(json_path)}')
+
+
+def write_json(data_dict, json_path, indent=0, encoding='utf-8'):
+    """Save dict to the same structure json file, a function wrapper for :func:`dict2json`
+    
+    Parameters
+    ----------
+    data_dict : dict
+        the dict object want to save as json file
+    json_path : str
+        the path including json file name to save the json file
+        e.g. ``D:/xxx/xxxx/save.json``
+    indent : int | None
+        whether save "readable" json with indent, default 0 without indent
+    encoding : str
+        the encoding type of output file
+
+
+    See also
+    --------
+    easyidp.jsonfile.dict2json
+
+    """
+    dict2json(data_dict, json_path, indent, encoding)
+
+
+def save_json(data_dict, json_path, indent=0, encoding='utf-8'):
+    """Save dict to the same structure json file, a function wrapper for :func:`dict2json`
+    
+    Parameters
+    ----------
+    data_dict : dict
+        the dict object want to save as json file
+    json_path : str
+        the path including json file name to save the json file
+        e.g. ``D:/xxx/xxxx/save.json``
+    indent : int | None
+        whether save "readable" json with indent, default 0 without indent
+    encoding : str
+        the encoding type of output file
+
+    See also
+    --------
+    easyidp.jsonfile.dict2json
+
+    """
+    dict2json(data_dict, json_path, indent, encoding)
+
+# just copied from previous `caas_lite.py`, haven't modified yet
+def _to_labelme_json(grid_tagged, json_folder, minimize=True):
+    """Save the tagged shp polygon crop result to json file, for deeplearing use
+
+    Parameters
+    ----------
+    grid_tagged : pandas.DataFrame
+        the output of self.dataframe_add_shp_tags()
+        The 4 column dataframe shows in this function introduction, sorted by "grid_name"
+    json_folder : str
+        the folder or path to save those json files
+    minimize : bool
+        whether create a json without space
+
+    Notes
+    -----
+    The labelme json file has the following structure:
+
+    .. code-block:: json
+
+        {
+            "version": "4.5.6",  # the Labelme.exe version, optional
+            "flags": {},
+            "imagePath": "xxxx.tiff",
+            "imageHeight": 1000,
+            "imageWidth": 1000,
+            "imageData": null,
+            "shapes": [{ }, { }, { }]
+        }      
+
+    for each ``{}`` items in "shapes":
+
+    .. code-block:: json
+
+        {
+            "label": "field",
+            "group_id": null,
+            "shape_type": "polygon",
+            "flags": {},
+            "points": [[x1, y1], [x2, y2], [x3, y3]]  # with or without the first point
+        }
+
+    Example of ``grid_tagged`` 
+
+    +------------------+----------+---------------------+-------+
+    |     grid_name    | dict_key |    polygon_list     |  tag  |
+    +==================+==========+=====================+=======+
+    | 'grid_x1_y1.tif' | 'key1'   | [poly1, poly2, ...] | field |
+    +------------------+----------+---------------------+-------+
+    | 'grid_x1_y1.tif' | 'key2'   | [poly1, poly2, ...] | crops |
+    +------------------+----------+---------------------+-------+
+    | 'grid_x1_y2.tif' | 'key1'   | [poly1, poly2, ...] | field |
+    +------------------+----------+---------------------+-------+
+    | 'grid_x2_y1.tif' | 'key1'   | [poly1, poly2, ...] | field |
+    +------------------+----------+---------------------+-------+
+    | 'grid_x3_y2.tif' | 'key2'   | [poly1, poly2, ...] | crops |
+    +------------------+----------+---------------------+-------+
+    |      ...         |   ...    |         ...         |  ...  | 
+    +------------------+----------+---------------------+-------+
+
+    Example of ``minimize``
+
+    - True
+
+      .. code-block:: json
+
+        {"name":"lucy","sex":"boy"}
+    
+    - False
+
+      .. code-block:: json
+
+        {
+            "name":"lucy",
+            "sex":"boy"
+        } 
+
+    """
+    total_dict = {}
+    for i in range(len(grid_tagged)):
+        # todo modify here
+        img_name = grid_tagged.loc[i]['grid_name']
+        poly = grid_tagged.loc[i]['polygon_list']
+        tag = grid_tagged.loc[i]['tag']
+        
+        if img_name not in total_dict.keys():
+            single_dict = {"version": "4.5.6", 
+                            "flags": {},
+                            "imagePath": img_name,
+                            "imageHeight": 1000,
+                            "imageWidth": 1000,
+                            "imageData": None,
+                            "shapes": []}
+        else:
+            single_dict = total_dict[img_name]
+            
+        for item in poly:
+            single_item = {"label": tag,
+                            "group_id": None,   # json null = python None
+                            "shape_type": "polygon",
+                            "flags": {},
+                            "points": item.tolist()}
+            single_dict['shapes'].append(single_item)
+            
+        total_dict[img_name] = single_dict
+        
+    # after iter all items
+    for k, d in total_dict.items():
+        json_name = k.replace('.tif', '.json')
+        if minimize:
+            dict2json(d, os.path.join(json_folder, json_name))
+        else:
             dict2json(d, os.path.join(json_folder, json_name), indent=2)
```

### Comparing `easyidp-2.0.0.dev3/easyidp/metashape.py` & `easyidp-2.0.0.dev4/easyidp/metashape.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,352 @@
 import os
 import pyproj
 import zipfile
 import numpy as np
 import warnings
+from tabulate import tabulate
 from xml.etree import ElementTree
 import xml.dom.minidom as minidom
+from tqdm import tqdm
 from copy import copy as ccopy
 
 import easyidp as idp
 
 
 class Metashape(idp.reconstruct.Recons):
-    # the object for each chunk in Metashape project
+    """the object for each chunk in Metashape 3D reconstruction project"""
 
     def __init__(self, project_path=None, chunk_id=None):
+        """The method to initialize the Metashape class
+
+        Parameters
+        ----------
+        project_path : str, optional
+            The metashape project file to open, like "xxxx.psx",, by default None, means create an empty class
+        chunk_id : int or str, optional
+            The chunk id or name(label) want to open, by default None, open the first chunk.
+
+        Example
+        -------
+
+        .. code-block:: python
+
+            >>> import easyidp as idp
+            >>> test_data = idp.data.TestData()
+
+        Then open the demo Metashape project:
+
+        .. code-block:: python
+
+            >>> ms = idp.Metashape(test_data.metashape.lotus_psx)
+            <'Lotus.psx' easyidp.Metashape object with 1 active chunks>
+
+              id  label
+            ----  -------
+            -> 0  Chunk 1
+
+        Or you can create an empty class and then open project:
+
+        .. code-block:: python
+
+            >>> ms = idp.Metashape()
+            >>> ms.open_project(test_data.metashape.lotus_psx)
+            <'Lotus.psx' easyidp.Metashape object with 1 active chunks>
+
+            id  label
+            ----  -------
+            -> 0  Chunk 1
+
+        .. caution::
+
+            One metashape project may have several chunks, and each ``easyidp.Metashape`` project could only handle with only one chunk at once. 
+
+            The arrow before ID shows which chunk has been opened
+
+            .. code-block:: text
+
+                <'multichunk.psx' easyidp.Metashape object with 2 active chunks>
+
+                  id  label
+                ----  ------------
+                -> 1  multiple_bbb
+                   2  miltiple_aaa
+
+        """
         super().__init__()
         self.software = "metashape"
         self.transform = idp.reconstruct.ChunkTransform()
 
-        # the whole metashape project (parent) info
+        # store the whole metashape project (parent) meta info:
+        #: the folder contains the metashape project (.psx) files
         self.project_folder = None
+        #: the metashape project (file) name.
         self.project_name = None
-        self.project_chunks_dict = None
-        self.crs = None
-        self.reference_crs = pyproj.CRS.from_epsg(4326)
+        #: the chunk that be picked as for easyidp (this class, only deal with one chunk in metashape project)
+        self.chunk_id = chunk_id
 
-        if project_path is not None:
-            self._open_whole_project(project_path)
-            if chunk_id is not None:
-                self.open_chunk(chunk_id)
-        else:
-            if chunk_id is not None:
-                raise LookupError(
-                    f"Could not load chunk_id [{chunk_id}] for project_path [{project_path}]")
-        
+        # hidden attributes
+        self._project_chunks_dict = None
+        self._chunk_id2label = {}   # for project_chunks
+        self._label2chunk_id = {}   # for project_chunks
+        self._reference_crs = pyproj.CRS.from_epsg(4326)
+
+        ########################################
+        # mute attributes warning for auto doc #
+        ########################################
+        #: project / chunk name
+        self.label = self.label
+        #: project meta information
+        self.meta = self.meta
+        #: whether this project is activated, (often for Metashape), ``<class 'bool'>``
+        self.enabled = self.enabled
+        #: the container for all sensors in this project (camera model), ``<class 'easyidp.Container'>``
+        self.sensors = self.sensors
+        #: the container for all photos used in this project (images), ``<class 'easyidp.Container'>``
+        self.photos = self.photos
+
+        self.open_project(project_path, chunk_id)
+
+    def __repr__(self) -> str:
+        return self._show_chunk()
+
+    def __str__(self) -> str:
+        return self._show_chunk()
 
     ###############
     # zip/xml I/O #
     ###############
 
+    def _show_chunk(self, return_table_only=False):
+        if self.project_folder is None \
+            or self.project_name is None \
+            or self._project_chunks_dict is None \
+            or len(self._chunk_id2label) == 0 \
+            or len(self._label2chunk_id) == 0:
+            return "<Empty easyidp.Metashape object>"
+        else:
+            show_str = f"<'{self.project_name}.psx' easyidp.Metashape object with {len(self._project_chunks_dict)} active chunks>\n\n"
+
+            head = ["id", "label"]
+            data = []
+            for idx, label in self._chunk_id2label.items():
+                if idx == str(self.chunk_id) or label == str(self.chunk_id):
+                    idx = '-> ' + idx
+                data.append([idx, label])
+
+            table_str = tabulate(data, headers=head, tablefmt='simple', colalign=["right", "left"])
+
+            if return_table_only:
+                return table_str
+            else:
+                return show_str + table_str
+            
+    def open_project(self, project_path, chunk_id=None):
+        """Open a new 3D reconstructin project to overwritting current project.
+
+        Parameters
+        ----------
+        project_path : str, optional
+            The pix4d project file to open, like "xxxx.psx", or "xxxx" without suffix.
+        chunk_id : int or str, optional
+            The chunk id or name(label) want to open, by default None, open the first chunk.
+
+        Example
+        --------
+
+        .. code-block:: python
+
+            >>> import easyidp as idp
+            >>> test_data = idp.data.TestData()
+
+            >>> ms = idp.Metashape()
+            <Empty easyidp.Metashape object>
+
+            >>> ms.open_project(test_data.metashape.lotus_psx)
+            <'Lotus.psx' easyidp.Metashape object with 1 active chunks>
+
+              id  label
+            ----  -------
+            -> 0  Chunk 1
+
+        """
+        if project_path is not None:
+            self._open_whole_project(project_path)
+            self.open_chunk(self.chunk_id)
+        else:
+            if chunk_id is not None:
+                warnings.warn(
+                    f"Unable to open chunk_id [{chunk_id}] for empty project with project_path={project_path}")
+
     def open_chunk(self, chunk_id, project_path=None):
+        """switch to the other chunk, or chunk in a new project
+
+        Parameters
+        ----------
+        chunk_id : int or str
+            The chunk id or name(label) want to open
+        project_path : str, optional
+            The new metashape project file to open, like "xxxx.psx",, by default None, means swtich inside current metashape project
+
+
+        Example
+        --------
+
+        Data prepare
+
+        .. code-block:: python
+
+            >>> import easyidp as idp
+            >>> test_data = idp.data.TestData()
+
+            >>> ms = idp.Metashape(test_data.metashape.multichunk_psx)
+            <'multichunk.psx' easyidp.Metashape object with 4 active chunks>
+
+              id  label
+            ----  --------------
+            -> 1  multiple_bbb
+               2  multiple_aaa
+               3  multiple_aaa_1
+               4  multiple_aaa_2
+
+        Then switch from chunk 1 to chunk 4, by id or by label:
+
+        .. code-block:: python
+
+            >>> ms.open_chunk('4')
+            # or
+            >>> ms.open_chunk('multiple_aaa_2')
+
+            >>> ms
+            <'multichunk.psx' easyidp.Metashape object with 4 active chunks>
+            
+              id  label
+            ----  --------------
+               1  multiple_bbb
+               2  multiple_aaa
+               3  multiple_aaa_1
+            -> 4  multiple_aaa_2
+        
+        """
         # given new project path, switch project
         if project_path is not None:  
             self._open_whole_project(project_path)
         else:
             # not given metashape project path when init this class
-            if self.project_chunks_dict is None:
+            if self._project_chunks_dict is None:
                 raise FileNotFoundError(
                     f"Not specify Metashape project (project_path="
                     f"'{os.path.join(self.project_folder, self.project_name)}')"
                     f"Please specify `project_path` to this function"
                 )
         
         if isinstance(chunk_id, int):
             chunk_id = str(chunk_id)
 
-        if chunk_id in self.project_chunks_dict.keys():
+        if chunk_id in self._project_chunks_dict.keys():
             chunk_content_dict = read_chunk_zip(
                 self.project_folder, 
                 self.project_name, 
                 chunk_id=chunk_id, skip_disabled=False)
             self._chunk_dict_to_object(chunk_content_dict)
+        elif chunk_id in self._label2chunk_id.keys():
+            chunk_content_dict = read_chunk_zip(
+                self.project_folder, 
+                self.project_name, 
+                chunk_id=self._label2chunk_id[chunk_id], skip_disabled=False)
+            self._chunk_dict_to_object(chunk_content_dict)
         else:
             raise KeyError(
-                f"Could not find chunk_id [{chunk_id}] in "
-                f"{list(self.project_chunks_dict.keys())}")
+                f"Could not find chunk_id [{chunk_id}] in {self._chunk_id2label}")
+        
+        self.chunk_id = chunk_id
 
     def _open_whole_project(self, project_path):
         _check_is_software(project_path)
         folder_path, project_name, ext = _split_project_path(project_path)
 
         # chunk_dict.keys() = [1,2,3,4,5] int id
         project_dict = read_project_zip(folder_path, project_name)
 
+        chunk_id2label = {}
+        label2chunk_id = {}
+        for chunk_id in project_dict.keys():
+            chunk_dict = read_chunk_zip(folder_path, project_name, chunk_id, return_label_only=True)
+
+            if chunk_dict['enabled']:
+                lb = chunk_dict['label']
+                lb_len = len(lb)
+                # judge if two chunks have the same label
+                while lb in label2chunk_id.keys():
+                    # extract '_1' from 'chunk_name_1' if have
+                    suffix = lb[lb_len:][1:]
+                    # do not have 
+                    if suffix == '':
+                        lb = lb[:lb_len] + '_1'
+                    else:
+                        lb = lb[:lb_len] + '_' + str(int(suffix) + 1)
+
+                chunk_id2label[chunk_id] = lb
+                label2chunk_id[lb] = chunk_id
+            else:   # ignore the disabled chunk.
+                project_dict.pop(chunk_id)
+
+        # open the first chunk if chunk_id not given.
+        first_chunk_id = list(project_dict.keys())[0]
+        if len(project_dict) == 1:  # only has one chunk, open directly
+            if str(self.chunk_id) not in chunk_id2label.keys() and self.chunk_id not in chunk_id2label.values():
+                warnings.warn(
+                    f"This project only has one chunk named "
+                    f"[{first_chunk_id}] '{chunk_id2label[first_chunk_id]}', "
+                    f"ignore the wrong chunk_id [{self.chunk_id}] specified by user.")
+            self.chunk_id = first_chunk_id
+        else:   # has multiple chunks
+            if self.chunk_id is None:
+                warnings.warn(
+                    f"The project has [{len(project_dict)}] chunks, however no chunk_id has been specified, "
+                    f"open the first chunk [{first_chunk_id}] '{chunk_id2label[first_chunk_id]}' by default.")
+                self.chunk_id = first_chunk_id
+
+        # save to project parameters
         self.project_folder = folder_path
         self.project_name = project_name
-        self.project_chunks_dict = project_dict
+        self._project_chunks_dict = project_dict
+        self._chunk_id2label = chunk_id2label
+        self._label2chunk_id = label2chunk_id
+
 
     def _chunk_dict_to_object(self, chunk_dict):
         self.label = chunk_dict["label"]
         self.enabled = chunk_dict["enabled"]
-        self.transform = chunk_dict["transform"]
+
+        self._reference_crs = chunk_dict["crs"]
+
+        # adapt for empty chunk without any information
+        missing_pool = []
+
+        if "transform" in chunk_dict.keys():
+            self.transform = chunk_dict["transform"]
+        else:
+            self.enabled = False
+            missing_pool.append('transform')
+
         self.sensors = chunk_dict["sensors"]
+        if len(chunk_dict["sensors"]) == 0:
+            self.enabled = False
+            missing_pool.append('sensors')
+
         self.photos = chunk_dict["photos"]
-        self.reference_crs = chunk_dict["crs"]
+        if len(chunk_dict["photos"]) == 0:
+            self.enabled = False
+            missing_pool.append('photos')
+
+        # show warning for emtpy tasks
+        if not self.enabled:
+            warnings.warn(f"Current chunk missing required {missing_pool} information "
+                "(is it an empty chunk without finishing SfM tasks?) and unable to do further analysis.")
 
     
     #######################
     # backward projection #
     #######################
 
     def _local2world(self, points_np):
@@ -97,23 +356,23 @@
         if self.transform.matrix_inv is None:
             self.transform.matrix_inv = np.linalg.inv(self.transform.matrix)
 
         return apply_transform_matrix(points_np, self.transform.matrix_inv)
 
     def _world2crs(self, points_np):
         if self.crs is None:
-            return convert_proj3d(points_np, self.world_crs, self.reference_crs)
+            return idp.geotools.convert_proj3d(points_np, self._world_crs, self._reference_crs)
         else:
-            return convert_proj3d(points_np, self.world_crs, self.crs)
+            return idp.geotools.convert_proj3d(points_np, self._world_crs, self.crs)
 
     def _crs2world(self, points_np):
         if self.crs is None:
-            return convert_proj3d(points_np, self.reference_crs, self.world_crs)
+            return idp.geotools.convert_proj3d(points_np, self._reference_crs, self._world_crs)
         else:
-            return convert_proj3d(points_np, self.crs, self.world_crs)
+            return idp.geotools.convert_proj3d(points_np, self.crs, self._world_crs)
 
     def _back2raw_one2one(self, points_np, photo_id, distortion_correct=True):
         """Project one ROI(polygon) on one given photo
 
         Parameters
         ----------
         points_np : ndarray (nx3)
@@ -143,15 +402,15 @@
 
         if not camera_i.enabled:
             return None
 
         t = camera_i.transform[0:3, 3]
         r = camera_i.transform[0:3, 0:3]
 
-        points_np, is_single = _is_single_point(points_np)
+        points_np, is_single = idp.geotools.is_single_point(points_np)
 
         xyz = (points_np - t).dot(r)
 
         xh = xyz[:, 0] / xyz[:, 2]
         yh = xyz[:, 1] / xyz[:, 2]
 
         # without distortion
@@ -179,51 +438,94 @@
             out = ppix[:, 0:2]
 
         if is_single:
             return out[0, :]
         else:
             return out
 
-    def back2raw_crs(self, points_xyz, distortion_correct=True, save_folder=None, ignore=None, log=False):
+    def back2raw_crs(self, points_xyz, ignore=None, log=False):
         """Projs one GIS coordintates ROI (polygon) to all images
 
         Parameters
         ----------
         points_hv : ndarray (nx3)
             The 3D coordinates of polygon vertexm, in CRS coordinates
-        distortion_correct : bool, optional
-            Whether do distortion correction, by default True (back to raw image);
-            If back to software corrected images without len distortion, set it to True. 
-            Pix4D support do this operation, seems metashape not supported yet.
         ignore : str | None, optional
-            None: strickly in image area;
-            'x': only y (vertical) in image area, x can outside image;
-            'y': only x (horizontal) in image area, y can outside image.
+            Whether tolerate small parts outside image, check 
+            :func:`easyidp.reconstruct.Sensor.in_img_boundary` for more details.
+
+            - ``None``: strickly in image area;
+            - ``x``: only y (vertical) in image area, x can outside image;
+            - ``y``: only x (horizontal) in image area, y can outside image.
+
         log : bool, optional
             whether print log for debugging, by default False
 
         Returns
         -------
         dict,
             a dictionary that key = img_name and values= pixel coordinate
+
+        Example
+        -------
+
+        Data preparation
+
+        .. code-block:: python
+
+            >>> import easyidp as idp
+
+            >>> ms = idp.Metashape(test_data.metashape.lotus_psx)
+            >>> dsm = idp.GeoTiff(test_data.metashape.lotus_dsm)
+            >>> ms.crs = dsm.crs
+
+            >>> plot =  np.array([   # N1E1 plot geo coordinate
+            ...     [ 368020.2974959 , 3955511.61264302,      97.56272272],
+            ...     [ 368022.24288365, 3955512.02973983,      97.56272272],
+            ...     [ 368022.65361232, 3955510.07798313,      97.56272272],
+            ...     [ 368020.69867274, 3955509.66725421,      97.56272272],
+            ...     [ 368020.2974959 , 3955511.61264302,      97.56272272]
+            ... ])
+
+        ..caution:: specifying the CRS of metashape project (``ms.crs = dsm.crs``) is required before doing backward projection calculation
+
+        Then use this function to find the previous ROI positions on the raw images:
+
+        .. code-block:: python
+
+            >>> out_dict = ms.back2raw_crs(plot)
+
+            >>> out_dict["DJI_0478"]
+            array([[   2.03352333, 1474.90817792],
+                   [  25.04572582, 1197.08827224],
+                   [ 311.99971438, 1214.81701547],
+                   [ 288.88669685, 1492.59824542],
+                   [   2.03352333, 1474.90817792]])
+
         """
+        if not self.enabled:
+            raise TypeError("Unable to process disabled chunk (.enabled=False)")
+        
+        if self.crs is None:
+            warnings.warn("Have not specify the CRS of output DOM/DSM/PCD, may get wrong backward projection results, please specify it by `ms.crs=dom.crs` or `ms.crs=pyproj.CRS.from_epsg(...)` ")
+        
         local_coord = self._world2local(self._crs2world(points_xyz))
 
         # for each raw image in the project / flight
         out_dict = {}
         for photo_name, photo in self.photos.items():
             # skip not enabled photos
             if not photo.enabled:
                 continue
             # reverse projection to given raw images
             projected_coord = self._back2raw_one2one(local_coord, photo, distortion_correct=True)
 
             # find out those correct images
             if log:
-                print(f'[Calculator][Judge]{photo.label}w:{photo.w}h:{photo.h}->', end='')
+                print(f'[Calculator][Judge]{photo.label}w:{photo.sensor.width}h:{photo.sensor.height}->', end='')
 
             coords = photo.sensor.in_img_boundary(projected_coord, ignore=ignore, log=log)
             if coords is not None:
                 out_dict[photo_name] = coords
 
         return out_dict
 
@@ -232,144 +534,514 @@
         """Projects several GIS coordintates ROIs (polygons) to all images
 
         Parameters
         ----------
         roi : easyidp.ROI | dict
             the <ROI> object created by easyidp.ROI() or dictionary
         save_folder : str, optional
-            the folder to save projected preview images and json files, by default ""
-        distortion_correct : bool, optional
-            Whether do distortion correction, by default True (back to raw image);
-            If back to software corrected images without len distortion, set it to True. 
-            Pix4D support do this operation, seems metashape not supported yet.
+            the folder to save json files and parts of ROI on raw images, by default None
         ignore : str | None, optional
-            None: strickly in image area;
-            'x': only y (vertical) in image area, x can outside image;
-            'y': only x (horizontal) in image area, y can outside image.
+            Whether tolerate small parts outside image, check 
+            :func:`easyidp.reconstruct.Sensor.in_img_boundary` for more details.
+
+            - ``None``: strickly in image area;
+            - ``x``: only y (vertical) in image area, x can outside image;
+            - ``y``: only x (horizontal) in image area, y can outside image.
+
         log : bool, optional
             whether print log for debugging, by default False
+
+
+        Example
+        -------
+
+        Data prepare
+
+        .. code-block:: python
+
+            >>> import easyidp as idp
+
+            >>> lotus = idp.data.Lotus()
+
+            >>> ms = idp.Metashape(project_path=lotus.metashape.project)
+
+            >>> roi = idp.ROI(lotus.shp, name_field=0)
+            [shp][proj] Use projection [WGS 84] for loaded shapefile [plots.shp]
+            Read shapefile [plots.shp]: 100%|███████████████| 112/112 [00:00<00:00, 2481.77it/s]
+            >>> roi = roi[0:2]
+
+            >>> roi.get_z_from_dsm(lotus.pix4d.dsm)
+
+
+        Then using this function to do backward projection:
+
+        .. code-block:: python
+
+            >>> out_all = ms.back2raw(roi)
+            {
+                'N1W1': {
+                    'DJI_0478.JPG': 
+                        array([[  14.96726711, 1843.13937997],
+                               [  38.0361733 , 1568.36113526],
+                               [ 320.25420037, 1584.28772847],
+                               [ 297.16110119, 1859.05913936],
+                               [  14.96726711, 1843.13937997]])
+                    'DJI_0479':
+                        array([...])
+                    ...
+                }
+                'N1W2': {...}   # output of `back2raw_crs()`
+            }
+
         """
+        if not self.enabled:
+            raise TypeError("Unable to process disabled chunk (.enabled=False)")
+        
+        if self.crs is None and roi.crs is None:
+            warnings.warn("Have not specify the CRS of output DOM/DSM/PCD, may get wrong backward projection results, please specify it by either `ms.crs=...` or `roi.crs=...` ")
+        
         out_dict = {}
+
+        before_crs = ccopy(self.crs)
         self.crs = ccopy(roi.crs)
-        for k, points_xyz in roi.items():
+
+        pbar = tqdm(roi.items(), desc=f"Backward roi to raw images")
+        for k, points_xyz in pbar:
             if isinstance(save_folder, str) and os.path.isdir(save_folder):
                 save_path = os.path.join(save_folder, k)
             else:
                 save_path = None
 
-            one_roi_dict= self.back2raw_crs(points_xyz, save_folder=save_path, **kwargs)
+            if points_xyz.shape[1] != 3:
+                raise ValueError(f"The back2raw function requires 3D roi with shape=(n, 3), but [{k}] is {points_xyz.shape}")
+
+            one_roi_dict= self.back2raw_crs(points_xyz, **kwargs)
 
             out_dict[k] = one_roi_dict
 
+        self.crs = before_crs
+
+        if save_folder is not None:
+            idp.reconstruct.save_back2raw_json_and_png(self, out_dict, save_folder)
+
         return out_dict
 
-    def get_photo_position(self, to_crs=None):
+    def get_photo_position(self, to_crs=None, refresh=False):
         """Get all photos' center geo position (on given CRS)
 
         Parameters
         ----------
         to_crs : pyproj.CRS, optional
             Transformed to another geo coordinate, by default None, the project.crs
+        refresh : bool, optional
+            
+            - ``False`` : Use cached results (if have), by default
+            - ``True`` : recalculate the photo position
 
         Returns
         -------
         dict
             The dictionary contains "photo.label": [x, y, z] coordinates
+
+        Example
+        -------
+
+        Data prepare
+
+        .. code-block:: python
+        
+            >>> import numpy as np
+            >>> np.set_printoptions(suppress=True)
+
+            >>> import easyidp as idp
+
+            >>> lotus = idp.data.Lotus()
+            >>> ms = idp.Metashape(project_path=lotus.metashape.project)
+
+        Then use this function to get the photo position in 3D world:
+
+        .. code-block:: python
+
+            >>> out = ms.get_photo_position()
+            {
+                'DJI_0422': array([139.54053245,  35.73458169, 130.09433649]), 
+                'DJI_0423': array([139.54053337,  35.73458315, 129.93437641]),
+                ...
+            }
+
+        .. caution:: by default, if not specifying the CRS of metashape project, it will return in default CRS (epsg: 4326) -> (lon, lat, height), if need turn to the same coordinate like DOM/DSM, please specify the CRS first
+
+        .. code-block:: python
+
+            >>> dom = idp.GeoTiff(lotus.metashape.dom)
+            >>> ms.crs = dom.crs
+
+            >>> out = ms.get_photo_position()
+            {
+                'DJI_0422': array([ 368017.73174354, 3955492.1925972 ,     130.09433649]), 
+                'DJI_0423': array([ 368017.81717717, 3955492.35300323,     129.93437641]),
+                ...
+            }
+
         """
+        if not self.enabled:
+            raise TypeError("Unable to process disabled chunk (.enabled=False)")
+    
+        if self._photo_position_cache is not None and not refresh:
+            return self._photo_position_cache.copy()
+        else:
+            # change the out crs
+            before_crs = ccopy(self.crs)
+            if isinstance(to_crs, pyproj.CRS) and not to_crs.equals(self.crs):
+                self.crs = ccopy(to_crs)
+
+            out = {}
+            pbar = tqdm(self.photos, desc=f"Getting photo positions")
+            for p in pbar:
+                if p.enabled:
+                    # the metashape logic, did the convertion based on self.crs in the following functions
+                    # this is different with the pix4d project, check Pix4D.get_photo_position() for more info
+                    pos = self._world2crs(self._local2world(p.transform[0:3, 3]))
 
-        # change the out crs
-        before_crs = ccopy(self.crs)
-        if isinstance(to_crs, pyproj.CRS) and not to_crs.equals(self.crs):
-            self.crs = ccopy(to_crs)
+                    out[p.label] = pos
+                    p.position = pos
 
-        out = {}
-        for p in self.photos:
-            if p.enabled:
-                pos = self._world2crs(self._local2world(p.transform[0:3, 3]))
-                out[p.label] = pos
+            self.crs = before_crs
 
-        self.crs = before_crs
+            # cache the photo position results for later use
+            self._photo_position_cache = out
+
+            return out
+
+
+    def sort_img_by_distance(self, img_dict_all, roi, distance_thresh=None, num=None, save_folder=None):
+        """Advanced wrapper of sorting back2raw img_dict results by distance from photo to roi
+
+        Parameters
+        ----------
+        img_dict_all : dict
+            All output dict of roi.back2raw(...)
+            e.g. img_dict = roi.back2raw(...) -> img_dict
+        roi: idp.ROI
+            Your roi variable
+        num : None or int
+            Keep the closest {x} images
+        distance_thresh : None or float
+            Keep the images closer than this distance to ROI.
+        save_folder : str, optional
+            the folder to save json files and parts of ROI on raw images, by default None
+
+        Returns
+        -------
+        dict
+            the same structure as output of roi.back2raw(...)
+
+        Example
+        -------
+
+        In the previous :func:`back2raw` results :
+
+        .. code-block:: python
+
+            >>> out_all = ms.back2raw(roi)
+            {
+                'N1W1': {
+                    'DJI_0478.JPG': 
+                        array([[  14.96726711, 1843.13937997],
+                               [  38.0361733 , 1568.36113526],
+                               [ 320.25420037, 1584.28772847],
+                               [ 297.16110119, 1859.05913936],
+                               [  14.96726711, 1843.13937997]])
+                    'DJI_0479':
+                        array([...])
+                    ...
+                }
+                'N1W2': {...}   # output of `back2raw_crs()`
+            }
+
+        The image are in chaos order, in most application cases, probable only 1-3 closest images 
+        (to ROI in real world) are required, so this function is provided to sort/filter out.
+
+        In the following example, it filtered 3 images whose distance from camera to ROI in real 
+        world smaller than 10m:
+
+        .. code-block:: python
+
+            >>> img_dict_sort = ms.sort_img_by_distance(
+            ...     out_all, roi,
+            ...     distance_thresh=10,  # distance threshold is 10m
+            ...     num=3   # only keep 3 closest images
+            ... )
+
+            >>> img_dict_sort
+            {
+                'N1W1': {
+                    'DJI_0500': array([[1931.09279469, 2191.59919979],
+                                       [1939.92139124, 1930.65101348],
+                                       [2199.9439422 , 1939.32128527],
+                                       [2191.19230849, 2200.557026  ],
+                                       [1931.09279469, 2191.59919979]]), 
+                    'DJI_0517': array([[2870.94915401, 2143.3570243 ],
+                                       [2596.8790503 , 2161.04730612],
+                                       [2578.87033498, 1886.89058023],
+                                       [2853.13891851, 1869.99769984],
+                                       [2870.94915401, 2143.3570243 ]]), 
+                    'DJI_0518': array([[3129.43264924, 1984.91814896],
+                                       [2856.71879306, 2002.03817639],
+                                       [2838.71418138, 1730.00287388],
+                                       [3111.73360179, 1713.76233134],
+                                       [3129.43264924, 1984.91814896]])
+                }, 
+                'N1W2': {
+                    'DJI_0500': array([[2214.36789052, 2200.35979344],
+                                       [2221.8996575 , 1940.70687713],
+                                       [2479.9825464 , 1949.3909589 ],
+                                       [2472.52171907, 2209.40355333],
+                                       [2214.36789052, 2200.35979344]]), 
+                    'DJI_0517': array([[2849.82108263, 1845.6733702 ],
+                                       [2577.37309441, 1863.60741328],
+                                       [2559.80046778, 1592.07656949],
+                                       [2832.52942622, 1574.92640413],
+                                       [2849.82108263, 1845.6733702 ]]), 
+                    'DJI_0516': array([[2891.61686486, 2542.98979632],
+                                       [2616.06780032, 2559.41601014],
+                                       [2598.43900454, 2282.36641612],
+                                       [2874.23023492, 2266.71552931],
+                                       [2891.61686486, 2542.98979632]])
+                }
+            }
+
+        Or pick the closest one image:
 
-        return out
+        .. code-block:: python
+
+            >>> img_dict_sort = ms.sort_img_by_distance(
+            ...     out_all, roi,
+            ...     num=1   # only keep the closest images
+            ... )
+
+            >>> img_dict_sort
+            {
+                'N1W1': {
+                    'DJI_0500': array([[1931.09279469, 2191.59919979],
+                                       [1939.92139124, 1930.65101348],
+                                       [2199.9439422 , 1939.32128527],
+                                       [2191.19230849, 2200.557026  ],
+                                       [1931.09279469, 2191.59919979]])
+                }, 
+                'N1W2': {
+                    'DJI_0500': array([[2214.36789052, 2200.35979344],
+                                       [2221.8996575 , 1940.70687713],
+                                       [2479.9825464 , 1949.3909589 ],
+                                       [2472.52171907, 2209.40355333],
+                                       [2214.36789052, 2200.35979344]])
+                }
+            }
+
+        You can use ``list(dict.keys())[0]`` to get the image name automatically to iterate each plot:
+
+        .. code-block:: python
+
+            for plot_name, plot_value in img_dict_sort.items():
+                img_name = list(plot_value.key())[0]
+
+                coord = plot_value[img_name]
+                # or
+                coord = img_dict_sort[plot_name][img_name]
+
+        """
+        if not self.enabled:
+            raise TypeError("Unable to process disabled chunk (.enabled=False)")
+        
+        return idp.reconstruct.sort_img_by_distance(self, img_dict_all, roi, distance_thresh, num, save_folder)
+    
+    def show_roi_on_img(self, img_dict, roi_name, img_name=None, **kwargs):
+        """Visualize the specific backward projection results for given roi on the given image.
+
+        Parameters
+        ----------
+        img_dict : dict
+            The backward results from back2raw()
+        roi_name : str
+            The roi name to show
+        img_name : str
+            the image file name, by default None, plotting all available images
+        corrected_poly_coord : np.ndarray, optional
+            the corrected 2D polygon pixel coordiante on the image (if have), by default None
+        title : str, optional
+            The image title displayed on the top, by default None -> ``ROI [roi_name] on [img_name]``
+        save_as : str, optional
+            file path to save the output figure, by default None
+        show : bool, optional
+            whether display (in jupyter notebook) or popup (in command line) the figure, by default False
+        color : str, optional
+            the polygon line color, by default 'red'
+        alpha : float, optional
+            the polygon transparency, by default 0.5
+        dpi : int, optional
+            the dpi of produced figure, by default 72
+
+        Example
+        -------
+
+        .. code-block:: python
+
+            >>> img_dict_ms = roi.back2raw(ms)
+
+        Check the "N1W1" ROI on image "DJI_0479.JPG":
+
+        .. code-block:: python
+
+            >>> ms.show_roi_on_img(img_dict_ms, "N1W1", "DJI_0479")
+            
+        Check the "N1W1" ROI on all available images:
+
+            >>> ms.show_roi_on_img(img_dict_ms, "N1W1")
+
+        For more details, please check in :ref:`this example <show-one-roi-on-img-demo>`
+
+        See also
+        --------
+        easyidp.visualize.draw_polygon_on_img, easyidp.visualize.draw_backward_one_roi
+        """
+        # check if given has values
+        if roi_name not in img_dict.keys() or \
+                (img_name is not None and \
+                    img_name not in img_dict[roi_name].keys()):
+            raise IndexError(f"Could not find backward results of plot [{roi_name}] on image [{img_name}]")
+        
+        if img_name is not None and img_name not in self.photos.keys():
+            raise FileNotFoundError(f"Could not find the image file [{img_name}] in the Metashape project")
+        
+        if 'title' not in kwargs:
+            kwargs['title'] = f"ROI [{roi_name}] on [{img_name}]"
+
+        if 'show' not in kwargs:
+            kwargs['show'] = True
+    
+        if img_name is not None:
+            idp.visualize.draw_polygon_on_img(
+                img_name, 
+                img_path=self.photos[img_name].path, 
+                poly_coord=img_dict[roi_name][img_name], 
+                **kwargs
+                )
+        else:
+            idp.visualize.draw_backward_one_roi(
+                self, img_dict[roi_name], 
+                **kwargs
+            )
 
 ###############
 # zip/xml I/O #
 ###############
 
 def read_project_zip(project_folder, project_name):
-    """
-    [inner function] read project.zip xml files to string
-    project path = "/root/to/metashape/test_proj.psx"
-    -->  project_folder = "/root/to/metashape/"
-    -->  project_name = "test_proj"
+    """parse xml in the ``project.zip`` file, and get the chunk id and path
 
     Parameters
     ----------
     project_folder: str
     project_name: str
 
     Returns
     -------
     project_dict: dict
         key = chunk_id, value = chunk_path
 
     Notes
     -----
-    xml_str example:
+    If one project path look likes: ``/root/to/metashape/test_proj.psx``, 
+    then the input parameter should be:
+    
+    - ``project_folder = "/root/to/metashape/"``
+    - ``project_name = "test_proj"``
+
+    And obtained xml_str example:
+
+    .. code-block:: xml
 
         <document version="1.2.0">
           <chunks next_id="2">
             <chunk id="0" path="0/chunk.zip"/>
           </chunks>
           <meta>
             <property name="Info/LastSavedDateTime" value="2020:06:22 02:23:20"/>
             <property name="Info/LastSavedSoftwareVersion" value="1.6.2.10247"/>
             <property name="Info/OriginalDateTime" value="2020:06:22 02:20:16"/>
             <property name="Info/OriginalSoftwareName" value="Agisoft Metashape"/>
             <property name="Info/OriginalSoftwareVendor" value="Agisoft"/>
             <property name="Info/OriginalSoftwareVersion" value="1.6.2.10247"/>
           </meta>
         </document>
+
+    Example
+    --------
+
+    Data prepare
+
+    .. code-block:: python
+
+        >>> import easyidp as idp
+        >>> test_data = idp.data.TestData()
+
+        >>> project_folder = test_data.metashape.lotus_psx.parents[0]
+        PosixPath('/Users/<user>/Library/Application Support/easyidp.data/data_for_tests/metashape')
+        >>> project_name = 'Lotus'
+
+    Then use this function to 
+
+    .. code-block:: python
+
+        >>> idp.metashape.read_project_zip(project_folder, project_name)
+        {'0': '0/chunk.zip'}
+
     """
     project_dict = {}
 
     zip_file = f"{project_folder}/{project_name}.files/project.zip"
     xml_str = _get_xml_str_from_zip_file(zip_file, "doc.xml")
     xml_tree = ElementTree.fromstring(xml_str)
 
     for chunk in xml_tree[0]:   # tree[0] -> <chunks>
         project_dict[chunk.attrib['id']] = chunk.attrib['path']
 
     return project_dict
 
 
-def read_chunk_zip(project_folder, project_name, chunk_id, skip_disabled=False):
-    """[inner function] read chunk.zip xml file in given chunk
-    project path = "/root/to/metashape/test_proj.psx"
-    -->  project_folder = "/root/to/metashape/"
-    -->  project_name = "test_proj"
+def read_chunk_zip(project_folder, project_name, chunk_id, skip_disabled=False, return_label_only=False):
+    """parse xml in the given ``chunk.zip`` file.
 
     Parameters
     ----------
     project_folder: str
     project_name: str
     chunk_id: int or str
         the chunk id start from 0 of chunk.zip
     skip_disabled: bool
-        return None if chunk enabled == False
-
+        return None if chunk enabled is False in metashape project
+    return_label_only: bool
+        Only parse chunk.label, by default False
 
     Returns
     -------
     chunk_dict or None
 
     Notes
     -----
+    If one project path look likes: ``/root/to/metashape/test_proj.psx``, 
+    then the input parameter should be:
+    
+    - ``project_folder = "/root/to/metashape/"``
+    - ``project_name = "test_proj"``
+
     Example for xml_str:
 
+    .. code-block:: xml
+
         <chunk version="1.2.0" label="170525" enabled="true">
         <sensors next_id="1">
             <sensor id="0" label="FC550, DJI MFT 15mm F1.7 ASPH (15mm)" type="frame">
             ...  -> _decode_sensor_tag()
             </sensor>
             ...  -> for loop in this function
         </sensors>
@@ -392,27 +1064,85 @@
         <transform>
 
         <region>
             <center>-8.1800672545192263e+00 -2.6103071594817338e+00 -1.0706980639382815e+01</center>
             <size>3.3381093645095824e+01 2.3577857828140260e+01 7.2410767078399658e+00</size>
             <R>-9.8317886026354417e-01 ...  9.9841729020145376e-01</R>   // 9 numbers
         </region>
+
+    Example
+    --------
+
+    Data prepare
+
+    .. code-block:: python
+
+        >>> import easyidp as idp
+        >>> test_data = idp.data.TestData()
+
+        >>> project_folder = test_data.metashape.lotus_psx.parents[0]
+        PosixPath('/Users/<user>/Library/Application Support/easyidp.data/data_for_tests/metashape')
+        >>> project_name = 'Lotus'
+
+    Then parse the chunk:
+
+    .. code-block:: python
+
+        >>> idp.metashape.read_chunk_zip(project_folder, project_name, chunk_id=0)
+        {
+            'label': 'Chunk 1', 
+
+            'enabled': True, 
+
+            'transform': <easyidp.reconstruct.ChunkTransform object at 0x7fe2b81bf370>,
+
+            'sensors': <easyidp.Container> with 1 items
+                       [0]     FC550, DJI MFT 15mm F1.7 ASPH (15mm)
+                       <easyidp.reconstruct.Sensor object at 0x7fe2a873a040>, 
+
+            'photos': <easyidp.Container> with 151 items
+                      [0]     DJI_0422
+                      <easyidp.reconstruct.Photo object at 0x7fe2a873a9a0>
+                      [1]     DJI_0423
+                      <easyidp.reconstruct.Photo object at 0x7fe2a873a130>
+                      ...
+                      [149]   DJI_0571
+                      <easyidp.reconstruct.Photo object at 0x7fe298e82820>
+                      [150]   DJI_0572
+                      <easyidp.reconstruct.Photo object at 0x7fe298e82850>, 
+            
+            'crs': <Geographic 2D CRS: EPSG:4326>
+                   Name: WGS 84
+                   Axis Info [ellipsoidal]:
+                   - Lat[north]: Geodetic latitude (degree)
+                   - Lon[east]: Geodetic longitude (degree)
+                   Area of Use:
+                   - name: World.
+                   - bounds: (-180.0, -90.0, 180.0, 90.0)
+                   Datum: World Geodetic System 1984 ensemble
+                   - Ellipsoid: WGS 84
+                   - Prime Meridian: Greenwich
+        }
+
     """
     frame_zip_file = f"{project_folder}/{project_name}.files/{chunk_id}/chunk.zip"
     xml_str = _get_xml_str_from_zip_file(frame_zip_file, "doc.xml")
     xml_tree = ElementTree.fromstring(xml_str)
 
     chunk_dict = {}
 
     chunk_dict["label"] = xml_tree.attrib["label"]
     chunk_dict["enabled"] = bool(xml_tree.attrib["enabled"])
 
     if skip_disabled and not chunk_dict["enabled"]:
         return None
 
+    if return_label_only:
+        return chunk_dict
+
     # metashape chunk.transform.matrix
     transform_tags = xml_tree.findall("./transform")
     if len(transform_tags) == 1:
         chunk_dict["transform"] = _decode_chunk_transform_tag(transform_tags[0])
 
     sensors = idp.Container()
     for sensor_tag in xml_tree.findall("./sensors/sensor"):
@@ -458,16 +1188,15 @@
 
     chunk_dict["crs"] = _decode_chunk_reference_tag(xml_tree.findall("./reference"))
 
     return chunk_dict
 
 
 def _split_project_path(path: str):
-    """
-    [inner_function] Get project name, current folder, extension, etc. from given project path.
+    """Get project name, current folder, extension, etc. from given project path.
 
     Parameters
     ----------
     path: str
         e.g. proj_path="/root/to/metashape/test_proj.psx"
 
     Returns
@@ -482,16 +1211,15 @@
     folder_path, file_name = os.path.split(path)
     project_name, ext = os.path.splitext(file_name)
 
     return folder_path, project_name, ext
 
 
 def _check_is_software(path: str):
-    """
-    [inner function] Check if given path is metashape project structure
+    """Check if given path is metashape project structure
 
     Parameters
     ----------
     path: str
         e.g. proj_path="/root/to/metashape/test_proj.psx"
 
     Returns
@@ -505,16 +1233,15 @@
     data_folder = os.path.join(folder_path, project_name + ".files")
 
     if not os.path.exists(data_folder):
         raise FileNotFoundError(f"Could not find Metashape project file [{data_folder}]")
 
 
 def _get_xml_str_from_zip_file(zip_file, xml_file):
-    """
-    [inner function] read xml file in zip file
+    """read xml file in zip file
 
     Parameters
     ----------
     zip_file: str
         the path to zip file, e.g. "data/metashape/goya_test.files/project.zip"
     xml_file: str
         the file name in zip file, e.g. "doc.xml" in previous zip file
@@ -985,150 +1712,53 @@
 
 
 ###############
 # calculation #
 ###############
 
 def apply_transform_matrix(points_xyz, matrix):
-    """
-    Transforms a point or points in homogeneous coordinates.
+    """Transforms a point or points in homogeneous coordinates.
     equal to Metashape.Matrix.mulp() or Metashape.Matrix.mulv()
 
     Parameters
     ----------
     matrix: np.ndarray
         4x4 transform numpy array
     points_df: np.ndarray
-        # 1x3 single point
-        >>> np.array([1,2,3])
-           x  y  z
-        0  1  2  3
-
-        # nx3 points
-        >>> np.array([[1,2,3], [4,5,6], ...])
-           x  y  z
-        0  1  2  3
-        1  4  5  6
-        ...
-
-    Returns
-    -------
-    out: pd.DataFrame
-        same size as input points_np
-           x  y  z
-        0  1  2  3
-        1  4  5  6
-    """
-    points_xyz, is_single = _is_single_point(points_xyz)
-
-    point_ext = np.insert(points_xyz, 3, 1, axis=1)
-    dot_matrix = point_ext.dot(matrix.T)
-    dot_points = dot_matrix[:, 0:3] / dot_matrix[:, 3][:, np.newaxis]
-
-    if is_single:
-        return dot_points[0,:]
-    else:
-        return dot_points
+        For example:
 
+        .. code-block:: python
 
-def convert_proj3d(points_np, crs_origin, crs_target, is_xyz=True):
-    """
-    Transform a point or points from one CRS to another CRS, by pyproj.CRS.Transformer function
+            # 1x3 single point
+            >>> np.array([1,2,3])
+               x  y  z
+            0  1  2  3
 
-    Parameters
-    ----------
-    points_np : np.ndarray
-        the nx3 3D coordinate points
-    crs_origin : pyproj.CRS object
-        the CRS of points_np
-    crs_target : pyproj.CRS object
-        the CRS of target
-    is_xyz: bool, default false
-        The format of points_np; 
-        True: x, y, z; False: lon, lat, alt
+            # nx3 points
+            >>> np.array([[1,2,3], [4,5,6], ...])
+               x  y  z
+            0  1  2  3
+            1  4  5  6
+            ...
 
     Returns
     -------
-    np.ndarray
-
-    Notes
-    -----
-    ``point_np`` and ``fmt`` parameters
-
-    .. tab:: is_xyz = True
-
-        points_np in this format:
+    out: pd.DataFrame
+        same size as input points_np:
 
         .. code-block:: text
 
                x  y  z
             0  1  2  3
-
-    .. tab:: is_xyz = False
-
-        points_np in this format:
-
-        .. code-block:: text
-
-                lon  lat  alt
-            0    1    2    3
-            1    4    5    6
-
-    .. caution::
-
-        pyproj.CRS order: (lat, lon, alt)
-        points order in EasyIDP are commonly (lon, lat, alt)
-
-        But if is xyz format, no need to change order
+            1  4  5  6
 
     """
-    ts = pyproj.Transformer.from_crs(crs_origin, crs_target)
-
-    points_np, is_single = _is_single_point(points_np)
+    points_xyz, is_single = idp.geotools.is_single_point(points_xyz)
 
-    # check unit to know if is (lon, lat, lat) -> degrees or (x, y, z) -> meters
-    x_unit = crs_origin.coordinate_system.axis_list[0].unit_name
-    y_unit = crs_origin.coordinate_system.axis_list[1].unit_name
-    if x_unit == "degree" and y_unit == "degree": 
-        is_xyz = False
-    else:
-        is_xyz = True
+    point_ext = np.insert(points_xyz, 3, 1, axis=1)
+    dot_matrix = point_ext.dot(matrix.T)
+    dot_points = dot_matrix[:, 0:3] / dot_matrix[:, 3][:, np.newaxis]
 
-    if is_xyz:
-        if crs_target.is_geocentric:
-            x, y, z = ts.transform(*points_np.T)
-            out =  np.vstack([x, y, z]).T
-        elif crs_target.is_geographic:
-            lat, lon, alt = ts.transform(*points_np.T)
-            # the pyproj output order is reversed
-            out = np.vstack([lon, lat, alt]).T
-        elif crs_target.is_projected:
-            lat_m, lon_m, alt_m = ts.transform(*points_np.T)
-            out = np.vstack([lat_m, lon_m, alt_m]).T
-        else:
-            raise TypeError(f"Given crs is neither `crs.is_geocentric=True` nor `crs.is_geographic` nor `crs.is_projected`")
-    else:   
-        lon, lat, alt = points_np[:,0], points_np[:,1], points_np[:,2]
-        
-        if crs_target.is_geocentric:
-            x, y, z = ts.transform(lat, lon, alt)
-            out = np.vstack([x, y, z]).T
-        elif crs_target.is_geographic:
-            lat, lon, alt = ts.transform(lat, lon, alt)
-            out = np.vstack([lon, lat, alt]).T
-        elif crs_target.is_projected and crs_target.is_derived:
-            lat_m, lon_m, alt_m = ts.transform(lat, lon, alt)
-            out = np.vstack([lat_m, lon_m, alt_m]).T
-        else:
-            raise TypeError(f"Given crs is neither `crs.is_geocentric=True` nor `crs.is_geographic` nor `crs.is_projected`")
     if is_single:
-        return out[0, :]
-    else:
-        return out
-
-def _is_single_point(points_np):
-    # check if only contains one point
-    if points_np.shape == (3,):
-        # with only single point
-        return np.array([points_np]), True
+        return dot_points[0,:]
     else:
-        return points_np, False
+        return dot_points
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `easyidp-2.0.0.dev3/easyidp/shp.py` & `easyidp-2.0.0.dev4/easyidp/shp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,58 @@
 import os
 import pyproj
 import shapefile
 import numpy as np
+import warnings
 from tabulate import tabulate
 from tqdm import tqdm
 from pathlib import Path
 
 import easyidp as idp
 
+
 def read_proj(prj_path):
     """read \*.prj file to pyproj object
     
     Parameters
     ----------
     prj_path : str
         the file path of shp \*.prj
     
     Returns
     -------
-    proj : the pyproj object
+    <pyproj.CRS> object
+
+    Example
+    -------
+
+    .. code-block:: python
+
+        >>> import easyidp as idp
+        >>> test_data = idp.data.TestData()
+
+        >>> prj_path = test_data.shp.roi_prj
+        PosixPath('/Users/<user>/Library/Application Support/easyidp.data/data_for_tests/shp_test/roi.prj')
+        
+        >>> out_proj = idp.shp.read_proj(prj_path)
+        >>> out_proj
+        <Derived Projected CRS: EPSG:32654>
+        Name: WGS 84 / UTM zone 54N
+        Axis Info [cartesian]:
+        - E[east]: Easting (metre)
+        - N[north]: Northing (metre)
+        Area of Use:
+        - undefined
+        Coordinate Operation:
+        - name: UTM zone 54N
+        - method: Transverse Mercator
+        Datum: World Geodetic System 1984
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+
     """
     with open(str(prj_path), 'r') as f:
         wkt_string = f.readline()
 
     proj = pyproj.CRS.from_wkt(wkt_string)
     
     if proj.name == 'WGS 84':
@@ -37,14 +67,45 @@
     
     Parameters
     ----------
     shp_path : str
         the file path of \*.shp
     encoding : str
         default is 'utf-8', however, or some chinese characters, 'gbk' is required
+
+    Example
+    -------
+
+    .. code-block:: python
+
+        >>> import easyidp as idp
+        >>> test_data = idp.data.TestData()
+
+        >>> idp.shp.show_shp_fields(test_data.shp.complex_shp, encoding="GBK") 
+          [-1]            [0] ID                [1] MASSIFID       [2] CROPTYPE    [3] CROPDATE    [4] CROPAREA    [5] ATTID
+        ------  ---------------------------  -------------------  --------------  --------------  --------------  -----------
+             0  230104112201809010000000000  2301041120000000000       小麦         2018-09-01     61525.26302
+             1  230104112201809010000000012  2301041120000000012       蔬菜         2018-09-01      2802.33512
+             2  230104112201809010000000014  2301041120000000014       玉米         2018-09-01      6960.7745
+           ...              ...                      ...               ...             ...             ...            ...
+           320  230104112201809010000000583  2301041120000000583       大豆         2018-09-01      380.41704
+           321  230104112201809010000000584  2301041120000000584       其它         2018-09-01      9133.25998
+           322  230104112201809010000000585  2301041120000000585       其它         2018-09-01      1704.27193
+    
+        >>> idp.shp.show_shp_fields(test_data.shp.lotus_shp)
+          [-1]   [0] plot_id
+        ------  -------------
+             0      N1W1
+             1      N1W2
+             2      N1W3
+           ...       ...
+           109      S4E5
+           110      S4E6
+           111      S4E7
+    
     """
     shp = shapefile.Reader(str(shp_path), encoding=encoding)
 
     # read shp file fields
     shp_fields = _get_field_key(shp)
 
     head = ["[-1]"] + [f"[{v}] {k}" for k, v in shp_fields.items()]
@@ -102,16 +163,16 @@
         .. code-block:: python
 
             {'id1': np.array([[x1,y1],[x2,y2],...]),
              'id2': np.array([[x1,y1],[x2,y2],...]),...}
     pyproj.CRS, optional
         once set return_proj=True
 
-    Examples
-    --------
+    Example
+    -------
 
     The example shp file has the following columns:
 
     +--------------+--------------+----------------+----------------+----------------+-------------+
     | [0] ID       | [1] MASSIFID | [2] CROPTYPE   | [3] CROPDATE   | [4] CROPAREA   | [5] ATTID   |
     +==============+==============+================+================+================+=============+
     | 23010...0000 | 23010...0000 | 小麦           | 2018-09-01     | 61525.26302    |             |
@@ -138,15 +199,16 @@
     +--------------+--------------+----------------+----------------+----------------+-------------+
 
     First, prepare data
 
     .. code-block:: python
 
         >>> import easyidp as idp
-        >>> data_path = "./tests/data/shp_test/complex_shp_review.shp"
+        >>> testdata = idp.data.TestData()
+        >>> data_path = testdata.shp.complex_shp
 
     Then using the second column ``MASSIFID`` as shape keys:
 
     .. code-block:: python
 
         >>> out = idp.shp.read_shp(data_path, name_field="MASSIFID", encoding='gbk')
         >>> # or 
@@ -175,14 +237,15 @@
     And you can also add column_names to id by ``include_title=True`` :
 
     .. code-block:: python
 
         >>> out = idp.shp.read_shp(data_path, name_field=["CROPTYPE", "MASSIFID"], include_title=True, encoding='gbk') 
         >>> out.keys()
         dict_keys(['CROPTYPE_小麦_MASSIFID_23010...0000', 'CROPTYPE_蔬菜_MASSIFID_23010...0012', ... ])
+
     """
     #####################################
     # check projection coordinate first #
     #####################################
     if shp_proj is None:
         prj_path = Path(shp_path).with_suffix('.prj')
 
@@ -214,15 +277,15 @@
 
     ### do not put it into the following loop, save calculation time.
     if isinstance(name_field, list):
         field_id = [_find_name_related_int_id(shp_fields, nf) for nf in name_field]
     else:
         field_id = _find_name_related_int_id(shp_fields, name_field)
 
-    pbar = tqdm(shp.shapes(), desc=f"[shp] read shp [{os.path.basename(shp_path)}]")
+    pbar = tqdm(shp.shapes(), desc=f"Read shapefile [{os.path.basename(shp_path)}]")
     for i, shape in enumerate(pbar):
         # convert dict_key name string by given name_field
         if isinstance(field_id, list):
             plot_name = ""
             for j, fid in enumerate(field_id):
                 if include_title:
                     plot_name += f"{idp._find_key(shp_fields, fid)}_{shp.records()[i][fid]}"
@@ -251,90 +314,26 @@
         ##################################
         coord_np = np.asarray(shape.points)
         # check if the last point == first point
         if (coord_np[0, :] != coord_np[-1, :]).all():
             # otherwise duplicate first point to last point to fit the polygon definition
             coord_np = np.append(coord_np, coord_np[0,:][None,:], axis = 0)
 
-        # if unit is degrees, exchange x and y
-        x_unit = shp_proj.coordinate_system.axis_list[0].unit_name
-        y_unit = shp_proj.coordinate_system.axis_list[1].unit_name
-        if x_unit == "degree" and y_unit == "degree": 
-            coord_np = np.flip(coord_np, axis=1)
-        # ----------- Notes --------------
-        # when shp unit is (degrees) latitiude and longitude
-        #     the default order is (lon, lat) --> (y, x)
-        # in easyidp, numpy, and pyproj coordiate system, needs (lat, lon), so need to revert
-        #   
-        #   ↑                 y         
-        #   N   O------------->  
-        #       |  ________      
-        #       | |        |     
-        #       | |  img   |     
-        #       | |________|     
-        #     x v                
-        #
-        # however, if unit is meter (e.g. UTM Zone), the order doesn't need to be changed
-        # ---------------------------------
-
         # check if has duplicated key, otherwise will cause override
         if plot_name in shp_dict.keys():
             raise KeyError(f"Meet with duplicated key [{plot_name}] for current shapefile, please specify another `name_field` from {shp_fields} or simple leave it blank `name_field=None`")
 
         shp_dict[plot_name] = coord_np
 
     if return_proj:
         return shp_dict, shp_proj
     else:
         return shp_dict
 
 
-def convert_proj(shp_dict, origin_proj, target_proj):
-    """ 
-    Provide the geo coordinate transfrom based on pyproj package
-
-    Parameters
-    ----------
-    shp_dict : dict
-        the output of read_shp() function
-    shp_proj : pyproj object
-        the hidden output of read_shp(..., return_proj=True)
-    target_proj : str | pyproj object
-        Examples:
-        [1] pyproj.CRS.from_epsg(4326)  
-        [2] r'path/to/{shp_name}.prj',
-    """
-    transformer = pyproj.Transformer.from_proj(origin_proj, target_proj)
-    trans_dict = {}
-    for k, coord_np in shp_dict.items():
-        if len(coord_np.shape) == 1:
-            transformed = transformer.transform(coord_np[0], coord_np[1])
-        elif len(coord_np.shape) == 2:
-            transformed = transformer.transform(coord_np[:, 0], coord_np[:, 1])
-        else:
-            raise IndexError(
-                f"The input coord should be either [x, y, z] -> shape=(3,) "
-                f"or [[x,y,z], [x,y,z], ...] -> shape=(n, 3)"
-                f"not current {coord_np.shape}")
-        coord_np = np.asarray(transformed).T
-
-        # judge if has inf value, means convert fail
-        if True in np.isinf(coord_np):
-            raise ValueError(
-                f'Fail to convert points from "{origin_proj.name}" to '
-                f'"{target_proj.name}", '
-                f'this may caused by the uncertainty of .prj file strings, '
-                f'please check the coordinate manually via QGIS Layer Infomation, '
-                f'get the EPGS code, and specify the function argument'
-                f'read_shp2d(..., given_proj=pyproj.CRS.from_epsg(xxxx))')
-        trans_dict[k] = coord_np
-
-    return trans_dict
-
-
 def _get_field_key(shp):
     """
     Convert shapefile header {"Column": int_id}
 
     Parameters
     ----------
     shp : shapefile.Reader object
@@ -393,14 +392,17 @@
             0
             >>> c = ["ID", "CROPTYPE"]
             >>> _find_name_related_int_id(a, b)
             [0, 2]
     """
     if name_field is None:
         field_id = None
+        warnings.warn(
+            "Not specifying parameter 'name_field', will using the row id (from 0 to end) as the index for each polygon."\
+            "Please using idp.shp.show_shp_field(shp_path) to display the full available indexs")
     elif isinstance(name_field, int):
         if name_field >= len(shp_fields):
             raise IndexError(f'Int key [{name_field}] is outside the number of fields {shp_fields}')
         field_id = name_field
     elif isinstance(name_field, str):
         if name_field not in shp_fields.keys():
             raise KeyError(f'Can not find key {name_field} in {shp_fields}')
```

### Comparing `easyidp-2.0.0.dev3/easyidp.egg-info/SOURCES.txt` & `easyidp-2.0.0.dev4/easyidp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 easyidp/__init__.py
 easyidp/cvtools.py
 easyidp/data.py
 easyidp/geotiff.py
+easyidp/geotools.py
 easyidp/jsonfile.py
 easyidp/metashape.py
 easyidp/pix4d.py
 easyidp/pointcloud.py
 easyidp/reconstruct.py
 easyidp/roi.py
 easyidp/shp.py
@@ -19,15 +20,16 @@
 easyidp.egg-info/dependency_links.txt
 easyidp.egg-info/requires.txt
 easyidp.egg-info/top_level.txt
 tests/__init__.py
 tests/test_cvtools.py
 tests/test_data.py
 tests/test_geotiff.py
+tests/test_init_class_func.py
 tests/test_jsonfile.py
 tests/test_metashape.py
-tests/test_pathtools.py
 tests/test_pix4d.py
 tests/test_pointcloud.py
 tests/test_reconstruct.py
 tests/test_roi.py
-tests/test_shp.py
+tests/test_shp.py
+tests/test_visualize.py
```

### Comparing `easyidp-2.0.0.dev3/setup.py` & `easyidp-2.0.0.dev4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,169 @@
-00000000: 696d 706f 7274 2070 6174 686c 6962 0a66  import pathlib.f
-00000010: 726f 6d20 7365 7475 7074 6f6f 6c73 2069  rom setuptools i
-00000020: 6d70 6f72 7420 7365 7475 702c 2066 696e  mport setup, fin
-00000030: 645f 7061 636b 6167 6573 0a0a 6865 7265  d_packages..here
-00000040: 203d 2070 6174 686c 6962 2e50 6174 6828   = pathlib.Path(
-00000050: 5f5f 6669 6c65 5f5f 292e 7061 7265 6e74  __file__).parent
-00000060: 2e72 6573 6f6c 7665 2829 0a6c 6f6e 675f  .resolve().long_
-00000070: 6465 7363 7269 7074 696f 6e20 3d20 2868  description = (h
-00000080: 6572 6520 2f20 2252 4541 444d 452e 6d64  ere / "README.md
-00000090: 2229 2e72 6561 645f 7465 7874 2865 6e63  ").read_text(enc
-000000a0: 6f64 696e 673d 2275 7466 2d38 2229 0a0a  oding="utf-8")..
-000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000c0: 203d 206c 6f6e 675f 6465 7363 7269 7074   = long_descript
-000000d0: 696f 6e2e 7265 706c 6163 6528 273c 6120  ion.replace('<a 
-000000e0: 6872 6566 3d22 5245 4144 4d45 5f43 4e2e  href="README_CN.
-000000f0: 6d64 223e e4b8 ade6 9687 3c2f 613e 5c6e  md">......</a>\n
-00000100: 5c6e 272c 2022 2229 0a0a 7769 7468 206f  \n', "")..with o
-00000110: 7065 6e28 2765 6173 7969 6470 2f5f 5f69  pen('easyidp/__i
-00000120: 6e69 745f 5f2e 7079 272c 2065 6e63 6f64  nit__.py', encod
-00000130: 696e 673d 2775 7466 2d38 2729 2061 7320  ing='utf-8') as 
-00000140: 6669 643a 0a20 2020 2066 6f72 206c 696e  fid:.    for lin
-00000150: 6520 696e 2066 6964 3a0a 2020 2020 2020  e in fid:.      
-00000160: 2020 6966 206c 696e 652e 7374 6172 7473    if line.starts
-00000170: 7769 7468 2827 5f5f 7665 7273 696f 6e5f  with('__version_
-00000180: 5f27 293a 0a20 2020 2020 2020 2020 2020  _'):.           
-00000190: 2056 4552 5349 4f4e 203d 206c 696e 652e   VERSION = line.
-000001a0: 7374 7269 7028 292e 7370 6c69 7428 295b  strip().split()[
-000001b0: 2d31 5d5b 313a 2d31 5d0a 2020 2020 2020  -1][1:-1].      
-000001c0: 2020 2020 2020 6272 6561 6b0a 0a0a 6465        break...de
-000001d0: 6620 7061 7273 655f 7265 7175 6972 656d  f parse_requirem
-000001e0: 656e 7473 5f66 696c 6528 6669 6c65 6e61  ents_file(filena
-000001f0: 6d65 293a 0a20 2020 2077 6974 6820 6f70  me):.    with op
-00000200: 656e 2866 696c 656e 616d 652c 2065 6e63  en(filename, enc
-00000210: 6f64 696e 673d 2775 7466 2d38 2729 2061  oding='utf-8') a
-00000220: 7320 6669 643a 0a20 2020 2020 2020 2072  s fid:.        r
-00000230: 6571 7569 7265 7320 3d20 5b6c 696e 652e  equires = [line.
-00000240: 7374 7269 7028 2920 666f 7220 6c69 6e65  strip() for line
-00000250: 2069 6e20 6669 642e 7265 6164 6c69 6e65   in fid.readline
-00000260: 7328 2920 6966 206c 696e 655d 0a0a 2020  s() if line]..  
-00000270: 2020 7265 7475 726e 2072 6571 7569 7265    return require
-00000280: 730a 0a0a 494e 5354 414c 4c5f 5245 5155  s...INSTALL_REQU
-00000290: 4952 4553 203d 2070 6172 7365 5f72 6571  IRES = parse_req
-000002a0: 7569 7265 6d65 6e74 735f 6669 6c65 2827  uirements_file('
-000002b0: 7265 7175 6972 656d 656e 7473 2f64 6566  requirements/def
-000002c0: 6175 6c74 2e74 7874 2729 0a23 2054 6865  ault.txt').# The
-000002d0: 2060 7265 7175 6972 656d 656e 7473 2f65   `requirements/e
-000002e0: 7874 7261 732e 7478 7460 2066 696c 6520  xtras.txt` file 
-000002f0: 6973 2065 7870 6c69 6369 7465 6c79 206f  is explicitely o
-00000300: 6d69 7474 6564 2062 6563 6175 7365 0a23  mitted because.#
-00000310: 2069 7420 636f 6e74 6169 6e73 2072 6571   it contains req
-00000320: 7569 7265 6d65 6e74 7320 7468 6174 2064  uirements that d
-00000330: 6f20 6e6f 7420 6861 7665 2077 6865 656c  o not have wheel
-00000340: 7320 7570 6c6f 6164 6564 2074 6f20 7069  s uploaded to pi
-00000350: 700a 2320 666f 7220 7468 6520 706c 6174  p.# for the plat
-00000360: 666f 726d 7320 7765 2077 6973 6820 746f  forms we wish to
-00000370: 2073 7570 706f 7274 2e0a 6578 7472 6173   support..extras
-00000380: 5f72 6571 7569 7265 203d 207b 0a20 2020  _require = {.   
-00000390: 2064 6570 3a20 7061 7273 655f 7265 7175   dep: parse_requ
-000003a0: 6972 656d 656e 7473 5f66 696c 6528 2772  irements_file('r
-000003b0: 6571 7569 7265 6d65 6e74 732f 2720 2b20  equirements/' + 
-000003c0: 6465 7020 2b20 272e 7478 7427 290a 2020  dep + '.txt').  
-000003d0: 2020 666f 7220 6465 7020 696e 205b 2764    for dep in ['d
-000003e0: 6f63 7327 2c20 2774 6573 7427 2c20 2762  ocs', 'test', 'b
-000003f0: 7569 6c64 275d 0a7d 0a0a 7365 7475 7028  uild'].}..setup(
-00000400: 0a20 2020 206e 616d 653d 2265 6173 7969  .    name="easyi
-00000410: 6470 222c 200a 2020 2020 7665 7273 696f  dp", .    versio
-00000420: 6e3d 5645 5253 494f 4e2c 0a20 2020 2061  n=VERSION,.    a
-00000430: 7574 686f 723d 2248 616f 7a68 6f75 2057  uthor="Haozhou W
-00000440: 616e 6722 2c20 0a20 2020 2061 7574 686f  ang", .    autho
-00000450: 725f 656d 6169 6c3d 2268 6f77 6361 6e6f  r_email="howcano
-00000460: 6577 616e 6740 676d 6169 6c2e 636f 6d22  ewang@gmail.com"
-00000470: 2c0a 2020 2020 6465 7363 7269 7074 696f  ,.    descriptio
-00000480: 6e3d 2241 2068 616e 6479 2074 6f6f 6c20  n="A handy tool 
-00000490: 666f 7220 6465 616c 696e 6720 7769 7468  for dealing with
-000004a0: 2072 6567 696f 6e20 6f66 2069 6e74 6572   region of inter
-000004b0: 6573 7420 2852 4f49 2920 6f6e 2074 6865  est (ROI) on the
-000004c0: 2069 6d61 6765 2072 6563 6f6e 7374 7275   image reconstru
-000004d0: 6374 696f 6e20 284d 6574 6173 6861 7065  ction (Metashape
-000004e0: 2026 2050 6978 3444 2920 6f75 7470 7574   & Pix4D) output
-000004f0: 732c 206d 6169 6e6c 7920 696e 2061 6772  s, mainly in agr
-00000500: 6963 756c 7475 7265 2061 7070 6c69 6361  iculture applica
-00000510: 7469 6f6e 7322 2c0a 2020 2020 6c6f 6e67  tions",.    long
-00000520: 5f64 6573 6372 6970 7469 6f6e 3d6c 6f6e  _description=lon
-00000530: 675f 6465 7363 7269 7074 696f 6e2c 0a20  g_description,. 
-00000540: 2020 206c 6f6e 675f 6465 7363 7269 7074     long_descript
-00000550: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000560: 3d22 7465 7874 2f6d 6172 6b64 6f77 6e22  ="text/markdown"
-00000570: 2c0a 2020 2020 7572 6c3d 2268 7474 7073  ,.    url="https
-00000580: 3a2f 2f67 6974 6875 622e 636f 6d2f 5554  ://github.com/UT
-00000590: 6f6b 796f 2d46 6965 6c64 5068 656e 6f6d  okyo-FieldPhenom
-000005a0: 6963 732d 4c61 622f 4561 7379 4944 5022  ics-Lab/EasyIDP"
-000005b0: 2c0a 2020 2020 7061 636b 6167 6573 3d66  ,.    packages=f
-000005c0: 696e 645f 7061 636b 6167 6573 2829 2c0a  ind_packages(),.
-000005d0: 2020 2020 696e 7374 616c 6c5f 7265 7175      install_requ
-000005e0: 6972 6573 3d49 4e53 5441 4c4c 5f52 4551  ires=INSTALL_REQ
-000005f0: 5549 5245 532c 0a20 2020 2065 7874 7261  UIRES,.    extra
-00000600: 735f 7265 7175 6972 653d 6578 7472 6173  s_require=extras
-00000610: 5f72 6571 7569 7265 2c0a 2020 2020 636c  _require,.    cl
-00000620: 6173 7369 6669 6572 733d 5b0a 2020 2020  assifiers=[.    
-00000630: 2020 2020 2244 6576 656c 6f70 6d65 6e74      "Development
-00000640: 2053 7461 7475 7320 3a3a 2034 202d 2042   Status :: 4 - B
-00000650: 6574 6122 2c0a 2020 2020 2020 2020 2249  eta",.        "I
-00000660: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-00000670: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
-00000680: 6172 6368 222c 0a20 2020 2020 2020 2022  arch",.        "
-00000690: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000006a0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-000006b0: 6963 656e 7365 222c 0a20 2020 2020 2020  icense",.       
-000006c0: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
-000006d0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000006e0: 6465 6e74 222c 0a20 2020 2020 2020 2022  dent",.        "
-000006f0: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-00000700: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
-00000710: 3a3a 2047 4953 222c 0a20 2020 2020 2020  :: GIS",.       
-00000720: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
-00000730: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000740: 203a 3a20 3322 2c0a 2020 2020 2020 2020   :: 3",.        
-00000750: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
-00000760: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000770: 3a3a 2033 2e37 222c 0a20 2020 2020 2020  :: 3.7",.       
-00000780: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
-00000790: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000007a0: 203a 3a20 332e 3822 2c0a 2020 2020 2020   :: 3.8",.      
-000007b0: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-000007c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000007d0: 6e20 3a3a 2033 2e39 222c 0a20 2020 2020  n :: 3.9",.     
-000007e0: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
-000007f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000800: 6f6e 203a 3a20 332e 3130 222c 0a20 2020  on :: 3.10",.   
-00000810: 2020 2020 2022 5072 6f67 7261 6d6d 696e       "Programmin
-00000820: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000830: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-00000840: 7922 2c0a 2020 2020 5d2c 0a20 2020 2070  y",.    ],.    p
-00000850: 7974 686f 6e5f 7265 7175 6972 6573 3d27  ython_requires='
-00000860: 3e3d 332e 362c 203c 3427 2c0a 2020 2020  >=3.6, <4',.    
-00000870: 7072 6f6a 6563 745f 7572 6c73 3d7b 0a20  project_urls={. 
-00000880: 2020 2020 2020 2027 446f 6375 6d65 6e74         'Document
-00000890: 6174 696f 6e27 3a20 2768 7474 7073 3a2f  ation': 'https:/
-000008a0: 2f65 6173 7969 6470 2e72 6561 6474 6865  /easyidp.readthe
-000008b0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-000008c0: 742f 272c 0a20 2020 2020 2020 2027 536f  t/',.        'So
-000008d0: 7572 6365 273a 2027 6874 7470 733a 2f2f  urce': 'https://
-000008e0: 6769 7468 7562 2e63 6f6d 2f55 546f 6b79  github.com/UToky
-000008f0: 6f2d 4669 656c 6450 6865 6e6f 6d69 6373  o-FieldPhenomics
-00000900: 2d4c 6162 2f45 6173 7949 4450 272c 0a20  -Lab/EasyIDP',. 
-00000910: 2020 2020 2020 2027 5472 6163 6b65 7227         'Tracker'
-00000920: 3a20 2768 7474 7073 3a2f 2f67 6974 6875  : 'https://githu
-00000930: 622e 636f 6d2f 5554 6f6b 796f 2d46 6965  b.com/UTokyo-Fie
-00000940: 6c64 5068 656e 6f6d 6963 732d 4c61 622f  ldPhenomics-Lab/
-00000950: 4561 7379 4944 502f 6973 7375 6573 272c  EasyIDP/issues',
-00000960: 0a20 2020 2020 2020 2027 666f 7275 6d27  .        'forum'
-00000970: 3a20 2768 7474 7073 3a2f 2f67 6974 6875  : 'https://githu
-00000980: 622e 636f 6d2f 5554 6f6b 796f 2d46 6965  b.com/UTokyo-Fie
-00000990: 6c64 5068 656e 6f6d 6963 732d 4c61 622f  ldPhenomics-Lab/
-000009a0: 4561 7379 4944 502f 6469 7363 7573 7369  EasyIDP/discussi
-000009b0: 6f6e 7327 0a20 2020 207d 2c0a 29         ons'.    },.)
+00000000: 696d 706f 7274 2070 6174 686c 6962 0d0a  import pathlib..
+00000010: 6672 6f6d 2073 6574 7570 746f 6f6c 7320  from setuptools 
+00000020: 696d 706f 7274 2073 6574 7570 2c20 6669  import setup, fi
+00000030: 6e64 5f70 6163 6b61 6765 730d 0a0d 0a68  nd_packages....h
+00000040: 6572 6520 3d20 7061 7468 6c69 622e 5061  ere = pathlib.Pa
+00000050: 7468 285f 5f66 696c 655f 5f29 2e70 6172  th(__file__).par
+00000060: 656e 742e 7265 736f 6c76 6528 290d 0a6c  ent.resolve()..l
+00000070: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+00000080: 3d20 2868 6572 6520 2f20 2252 4541 444d  = (here / "READM
+00000090: 452e 6d64 2229 2e72 6561 645f 7465 7874  E.md").read_text
+000000a0: 2865 6e63 6f64 696e 673d 2275 7466 2d38  (encoding="utf-8
+000000b0: 2229 0d0a 0d0a 6c6f 6e67 5f64 6573 6372  ")....long_descr
+000000c0: 6970 7469 6f6e 203d 206c 6f6e 675f 6465  iption = long_de
+000000d0: 7363 7269 7074 696f 6e2e 7265 706c 6163  scription.replac
+000000e0: 6528 273c 6120 6872 6566 3d22 6874 7470  e('<a href="http
+000000f0: 733a 2f2f 6561 7379 6964 702e 7265 6164  s://easyidp.read
+00000100: 7468 6564 6f63 732e 696f 2f7a 685f 434e  thedocs.io/zh_CN
+00000110: 2f6c 6174 6573 742f 2220 7461 7267 6574  /latest/" target
+00000120: 3d22 5f62 6c61 6e6b 223e e4b8 ade6 9687  ="_blank">......
+00000130: 3c2f 613e 207c 203c 6120 6872 6566 3d22  </a> | <a href="
+00000140: 6874 7470 733a 2f2f 6561 7379 6964 702e  https://easyidp.
+00000150: 7265 6164 7468 6564 6f63 732e 696f 2f6a  readthedocs.io/j
+00000160: 612f 6c61 7465 7374 2f22 2074 6172 6765  a/latest/" targe
+00000170: 743d 225f 626c 616e 6b22 3ee6 97a5 e69c  t="_blank">.....
+00000180: ace8 aa9e 28e7 bfbb e8a8 b3e5 8b9f e99b  ....(...........
+00000190: 8629 3c2f 613e 5c6e 5c6e 272c 2022 2229  .)</a>\n\n', "")
+000001a0: 0d0a 0d0a 7769 7468 206f 7065 6e28 2765  ....with open('e
+000001b0: 6173 7969 6470 2f5f 5f69 6e69 745f 5f2e  asyidp/__init__.
+000001c0: 7079 272c 2065 6e63 6f64 696e 673d 2775  py', encoding='u
+000001d0: 7466 2d38 2729 2061 7320 6669 643a 0d0a  tf-8') as fid:..
+000001e0: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
+000001f0: 6669 643a 0d0a 2020 2020 2020 2020 6966  fid:..        if
+00000200: 206c 696e 652e 7374 6172 7473 7769 7468   line.startswith
+00000210: 2827 5f5f 7665 7273 696f 6e5f 5f27 293a  ('__version__'):
+00000220: 0d0a 2020 2020 2020 2020 2020 2020 5645  ..            VE
+00000230: 5253 494f 4e20 3d20 6c69 6e65 2e73 7472  RSION = line.str
+00000240: 6970 2829 2e73 706c 6974 2829 5b2d 315d  ip().split()[-1]
+00000250: 5b31 3a2d 315d 0d0a 2020 2020 2020 2020  [1:-1]..        
+00000260: 2020 2020 6272 6561 6b0d 0a0d 0a0d 0a64      break......d
+00000270: 6566 2070 6172 7365 5f72 6571 7569 7265  ef parse_require
+00000280: 6d65 6e74 735f 6669 6c65 2866 696c 656e  ments_file(filen
+00000290: 616d 6529 3a0d 0a20 2020 2077 6974 6820  ame):..    with 
+000002a0: 6f70 656e 2866 696c 656e 616d 652c 2065  open(filename, e
+000002b0: 6e63 6f64 696e 673d 2775 7466 2d38 2729  ncoding='utf-8')
+000002c0: 2061 7320 6669 643a 0d0a 2020 2020 2020   as fid:..      
+000002d0: 2020 7265 7175 6972 6573 203d 205b 6c69    requires = [li
+000002e0: 6e65 2e73 7472 6970 2829 2066 6f72 206c  ne.strip() for l
+000002f0: 696e 6520 696e 2066 6964 2e72 6561 646c  ine in fid.readl
+00000300: 696e 6573 2829 2069 6620 6c69 6e65 5d0d  ines() if line].
+00000310: 0a0d 0a20 2020 2072 6574 7572 6e20 7265  ...    return re
+00000320: 7175 6972 6573 0d0a 0d0a 0d0a 494e 5354  quires......INST
+00000330: 414c 4c5f 5245 5155 4952 4553 203d 2070  ALL_REQUIRES = p
+00000340: 6172 7365 5f72 6571 7569 7265 6d65 6e74  arse_requirement
+00000350: 735f 6669 6c65 2827 7265 7175 6972 656d  s_file('requirem
+00000360: 656e 7473 2f64 6566 6175 6c74 2e74 7874  ents/default.txt
+00000370: 2729 0d0a 2320 5468 6520 6072 6571 7569  ')..# The `requi
+00000380: 7265 6d65 6e74 732f 6578 7472 6173 2e74  rements/extras.t
+00000390: 7874 6020 6669 6c65 2069 7320 6578 706c  xt` file is expl
+000003a0: 6963 6974 656c 7920 6f6d 6974 7465 6420  icitely omitted 
+000003b0: 6265 6361 7573 650d 0a23 2069 7420 636f  because..# it co
+000003c0: 6e74 6169 6e73 2072 6571 7569 7265 6d65  ntains requireme
+000003d0: 6e74 7320 7468 6174 2064 6f20 6e6f 7420  nts that do not 
+000003e0: 6861 7665 2077 6865 656c 7320 7570 6c6f  have wheels uplo
+000003f0: 6164 6564 2074 6f20 7069 700d 0a23 2066  aded to pip..# f
+00000400: 6f72 2074 6865 2070 6c61 7466 6f72 6d73  or the platforms
+00000410: 2077 6520 7769 7368 2074 6f20 7375 7070   we wish to supp
+00000420: 6f72 742e 0d0a 6578 7472 6173 5f72 6571  ort...extras_req
+00000430: 7569 7265 203d 207b 0d0a 2020 2020 6465  uire = {..    de
+00000440: 703a 2070 6172 7365 5f72 6571 7569 7265  p: parse_require
+00000450: 6d65 6e74 735f 6669 6c65 2827 7265 7175  ments_file('requ
+00000460: 6972 656d 656e 7473 2f27 202b 2064 6570  irements/' + dep
+00000470: 202b 2027 2e74 7874 2729 0d0a 2020 2020   + '.txt')..    
+00000480: 666f 7220 6465 7020 696e 205b 2764 6f63  for dep in ['doc
+00000490: 7327 2c20 2774 6573 7427 2c20 2762 7569  s', 'test', 'bui
+000004a0: 6c64 275d 0d0a 7d0d 0a0d 0a73 6574 7570  ld']..}....setup
+000004b0: 280d 0a20 2020 206e 616d 653d 2265 6173  (..    name="eas
+000004c0: 7969 6470 222c 200d 0a20 2020 2076 6572  yidp", ..    ver
+000004d0: 7369 6f6e 3d56 4552 5349 4f4e 2c0d 0a20  sion=VERSION,.. 
+000004e0: 2020 2061 7574 686f 723d 2248 616f 7a68     author="Haozh
+000004f0: 6f75 2057 616e 6722 2c20 0d0a 2020 2020  ou Wang", ..    
+00000500: 6175 7468 6f72 5f65 6d61 696c 3d22 686f  author_email="ho
+00000510: 7763 616e 6f65 7761 6e67 4067 6d61 696c  wcanoewang@gmail
+00000520: 2e63 6f6d 222c 0d0a 2020 2020 6465 7363  .com",..    desc
+00000530: 7269 7074 696f 6e3d 2241 2068 616e 6479  ription="A handy
+00000540: 2074 6f6f 6c20 666f 7220 6465 616c 696e   tool for dealin
+00000550: 6720 7769 7468 2072 6567 696f 6e20 6f66  g with region of
+00000560: 2069 6e74 6572 6573 7420 2852 4f49 2920   interest (ROI) 
+00000570: 6f6e 2074 6865 2069 6d61 6765 2072 6563  on the image rec
+00000580: 6f6e 7374 7275 6374 696f 6e20 284d 6574  onstruction (Met
+00000590: 6173 6861 7065 2026 2050 6978 3444 2920  ashape & Pix4D) 
+000005a0: 6f75 7470 7574 732c 206d 6169 6e6c 7920  outputs, mainly 
+000005b0: 696e 2061 6772 6963 756c 7475 7265 2061  in agriculture a
+000005c0: 7070 6c69 6361 7469 6f6e 7322 2c0d 0a20  pplications",.. 
+000005d0: 2020 206c 6f6e 675f 6465 7363 7269 7074     long_descript
+000005e0: 696f 6e3d 6c6f 6e67 5f64 6573 6372 6970  ion=long_descrip
+000005f0: 7469 6f6e 2c0d 0a20 2020 206c 6f6e 675f  tion,..    long_
+00000600: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+00000610: 656e 745f 7479 7065 3d22 7465 7874 2f6d  ent_type="text/m
+00000620: 6172 6b64 6f77 6e22 2c0d 0a20 2020 2075  arkdown",..    u
+00000630: 726c 3d22 6874 7470 733a 2f2f 6769 7468  rl="https://gith
+00000640: 7562 2e63 6f6d 2f55 546f 6b79 6f2d 4669  ub.com/UTokyo-Fi
+00000650: 656c 6450 6865 6e6f 6d69 6373 2d4c 6162  eldPhenomics-Lab
+00000660: 2f45 6173 7949 4450 222c 0d0a 2020 2020  /EasyIDP",..    
+00000670: 7061 636b 6167 6573 3d66 696e 645f 7061  packages=find_pa
+00000680: 636b 6167 6573 2829 2c0d 0a20 2020 2069  ckages(),..    i
+00000690: 6e73 7461 6c6c 5f72 6571 7569 7265 733d  nstall_requires=
+000006a0: 494e 5354 414c 4c5f 5245 5155 4952 4553  INSTALL_REQUIRES
+000006b0: 2c0d 0a20 2020 2065 7874 7261 735f 7265  ,..    extras_re
+000006c0: 7175 6972 653d 6578 7472 6173 5f72 6571  quire=extras_req
+000006d0: 7569 7265 2c0d 0a20 2020 2063 6c61 7373  uire,..    class
+000006e0: 6966 6965 7273 3d5b 0d0a 2020 2020 2020  ifiers=[..      
+000006f0: 2020 2244 6576 656c 6f70 6d65 6e74 2053    "Development S
+00000700: 7461 7475 7320 3a3a 2034 202d 2042 6574  tatus :: 4 - Bet
+00000710: 6122 2c0d 0a20 2020 2020 2020 2022 496e  a",..        "In
+00000720: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000730: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
+00000740: 7263 6822 2c0d 0a20 2020 2020 2020 2022  rch",..        "
+00000750: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000760: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000770: 6963 656e 7365 222c 0d0a 2020 2020 2020  icense",..      
+00000780: 2020 224f 7065 7261 7469 6e67 2053 7973    "Operating Sys
+00000790: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000007a0: 6e64 656e 7422 2c0d 0a20 2020 2020 2020  ndent",..       
+000007b0: 2022 546f 7069 6320 3a3a 2053 6369 656e   "Topic :: Scien
+000007c0: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+000007d0: 6720 3a3a 2047 4953 222c 0d0a 2020 2020  g :: GIS",..    
+000007e0: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
+000007f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000800: 686f 6e20 3a3a 2033 222c 0d0a 2020 2020  hon :: 3",..    
+00000810: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
+00000820: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000830: 686f 6e20 3a3a 2033 2e37 222c 0d0a 2020  hon :: 3.7",..  
+00000840: 2020 2020 2020 2250 726f 6772 616d 6d69        "Programmi
+00000850: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000860: 7974 686f 6e20 3a3a 2033 2e38 222c 0d0a  ython :: 3.8",..
+00000870: 2020 2020 2020 2020 2250 726f 6772 616d          "Program
+00000880: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000890: 2050 7974 686f 6e20 3a3a 2033 2e39 222c   Python :: 3.9",
+000008a0: 0d0a 2020 2020 2020 2020 2250 726f 6772  ..        "Progr
+000008b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000008c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000008d0: 3022 2c0d 0a20 2020 2020 2020 2022 5072  0",..        "Pr
+000008e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000008f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000900: 3320 3a3a 204f 6e6c 7922 2c0d 0a20 2020  3 :: Only",..   
+00000910: 205d 2c0d 0a20 2020 2070 7974 686f 6e5f   ],..    python_
+00000920: 7265 7175 6972 6573 3d27 3e3d 332e 362c  requires='>=3.6,
+00000930: 203c 3427 2c0d 0a20 2020 2070 726f 6a65   <4',..    proje
+00000940: 6374 5f75 726c 733d 7b0d 0a20 2020 2020  ct_urls={..     
+00000950: 2020 2027 446f 6375 6d65 6e74 6174 696f     'Documentatio
+00000960: 6e27 3a20 2768 7474 7073 3a2f 2f65 6173  n': 'https://eas
+00000970: 7969 6470 2e72 6561 6474 6865 646f 6373  yidp.readthedocs
+00000980: 2e69 6f2f 656e 2f6c 6174 6573 742f 272c  .io/en/latest/',
+00000990: 0d0a 2020 2020 2020 2020 2753 6f75 7263  ..        'Sourc
+000009a0: 6527 3a20 2768 7474 7073 3a2f 2f67 6974  e': 'https://git
+000009b0: 6875 622e 636f 6d2f 5554 6f6b 796f 2d46  hub.com/UTokyo-F
+000009c0: 6965 6c64 5068 656e 6f6d 6963 732d 4c61  ieldPhenomics-La
+000009d0: 622f 4561 7379 4944 5027 2c0d 0a20 2020  b/EasyIDP',..   
+000009e0: 2020 2020 2027 5472 6163 6b65 7227 3a20       'Tracker': 
+000009f0: 2768 7474 7073 3a2f 2f67 6974 6875 622e  'https://github.
+00000a00: 636f 6d2f 5554 6f6b 796f 2d46 6965 6c64  com/UTokyo-Field
+00000a10: 5068 656e 6f6d 6963 732d 4c61 622f 4561  Phenomics-Lab/Ea
+00000a20: 7379 4944 502f 6973 7375 6573 272c 0d0a  syIDP/issues',..
+00000a30: 2020 2020 2020 2020 2766 6f72 756d 273a          'forum':
+00000a40: 2027 6874 7470 733a 2f2f 6769 7468 7562   'https://github
+00000a50: 2e63 6f6d 2f55 546f 6b79 6f2d 4669 656c  .com/UTokyo-Fiel
+00000a60: 6450 6865 6e6f 6d69 6373 2d4c 6162 2f45  dPhenomics-Lab/E
+00000a70: 6173 7949 4450 2f64 6973 6375 7373 696f  asyIDP/discussio
+00000a80: 6e73 270d 0a20 2020 207d 2c0d 0a29       ns'..    },..)
```

### Comparing `easyidp-2.0.0.dev3/tests/test_data.py` & `easyidp-2.0.0.dev4/tests/test_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import shutil
 from pathlib import Path
 
 import easyidp as idp
 
+def test_get_download_url_without_download():
+
+    assert idp.data.Lotus.name == '2017_tanashi_lotus'
+    assert idp.data.TestData.name == 'data_for_tests'
+
+    url = idp.data.Lotus.url_list
+
+    assert isinstance(url, list)
+    assert isinstance(url[1], str)
+
 def test_usr_data_dir():
     root_dir = idp.data.user_data_dir("")
     assert "easyidp.data" in str(root_dir)
 
 def test_gdown():
     gd_dir = idp.data.user_data_dir("gdown_test")
```

### Comparing `easyidp-2.0.0.dev3/tests/test_geotiff.py` & `easyidp-2.0.0.dev4/tests/test_geotiff.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     assert maize_part_np.shape == (722, 836, 4)
 
     lh = idp.geotiff.get_header(test_data.pix4d.lotus_dom_part)
     lotus_part_np = idp.geotiff.get_imarray(test_data.pix4d.lotus_dom_part)
     assert lotus_part_np.shape == (lh["height"], lh["width"], lh["dim"])
 
 
-def test_def_geo2pixel2geo():
+def test_def_geo2pixel2geo_UTM():
     gis_coord = np.asarray([
         [ 484593.67474654, 3862259.42413431],
         [ 484593.41064743, 3862259.92582402],
         [ 484593.64841806, 3862260.06515117],
         [ 484593.93077419, 3862259.55455913],
         [ 484593.67474654, 3862259.42413431]])
 
@@ -65,15 +65,15 @@
     # please check v1.0 easyric.tests.test_io_geotiff.py line 114
     # > https://github.com/UTokyo-FieldPhenomics-Lab/EasyIDP/blob/a3420bc7b1e0f1013411565cf0e66dd2d2ba5371/easyric/tests/test_io_geotiff.py#L114
     # to get the full string of this header
     # here we just use the extracted results
     header = {'width': 19436, 'height': 31255, 'dim':4, 
               'scale': [0.001, 0.001], 'nodata': None,
               'tie_point': [484576.70205, 3862285.5109300003], 
-              'proj': pyproj.CRS.from_string("WGS 84 / UTM zone 53N")}
+              'crs': pyproj.CRS.from_string("WGS 84 / UTM zone 53N")}
 
     expected_pixel_idx = np.array([
         [16972, 26086],
         [16708, 25585],
         [16946, 25445],
         [17228, 25956],
         [16972, 26086]])
@@ -103,14 +103,46 @@
 
     # then convert back should have fewer precision loss
     # but seems still have some preoblem
     gis_revert_flt = idp.geotiff.pixel2geo(pixel_coord_idx, header)
     np.testing.assert_almost_equal(gis_revert_flt, gis_coord, decimal=3)
 
 
+def test_def_geo2pixel2geo_lonlat():
+    # using the source: https://github.com/UTokyo-FieldPhenomics-Lab/EasyIDP/discussions/44
+    gis_latlon_coord = np.array([
+        [-80.83957435, 25.78354364],
+        [-80.83947435, 25.78354364],
+        [-80.83947435, 25.78344364],
+        [-80.83957435, 25.78344364],
+        [-80.83957435, 25.78354364]])
+
+    header = {
+        'height': 8748, 'width': 7941, 'dim': 1, 'nodata': -32767.0, 
+        'scale': [3.49222000000852e-07, 3.1617399999982425e-07], 
+        'tie_point': [-80.84039234705898, 25.784493471936425], 
+        'crs': pyproj.CRS.from_epsg(4326)
+    }
+
+    expected_pixel = np.array([
+        [2342.34114395, 3004.14308711],
+        [2628.6919466 , 3004.14308711],
+        [2628.6919466 , 3320.42462829],
+        [2342.34114395, 3320.42462829],
+        [2342.34114395, 3004.14308711]])
+
+    out = idp.geotiff.geo2pixel(gis_latlon_coord, header)
+
+    np.testing.assert_almost_equal(out, expected_pixel)
+
+    back = idp.geotiff.pixel2geo(out, header)
+
+    np.testing.assert_almost_equal(back, gis_latlon_coord, decimal=3)
+
+
 def test_def_tifffile_crop():
     maize_part_np = idp.geotiff.get_imarray(test_data.pix4d.maize_dom)
     # untiled tiff but 2 row as a patch
     with tf.TiffFile(test_data.pix4d.maize_dom) as tif:
         page = tif.pages[0]
 
         # even start + even line number
@@ -321,55 +353,107 @@
     with pytest.raises(ValueError, match=re.escape("Current version only support DSM, RGB and RGBA images (band expect: 1,3,4; get [5], dtype=np.uint8; get [<class 'numpy.float32'>])")):
         idp.geotiff._is_empty_imarray(wrong_header1, np.zeros((4,4,5)))
 
     wrong_header2 = {"dim":3, "dtype": np.float32}
     with pytest.raises(IndexError, match=re.escape("The imarray dimention [4] does not match with header dimention [3]")):
         idp.geotiff._is_empty_imarray(wrong_header2, np.zeros((4,4,4)))
 
+def test_def_save_geotiff_and_extratag():
+    dom_test = idp.GeoTiff(test_data.tiff.soyweed_part)
+    dom_imarray = idp.geotiff.get_imarray(test_data.tiff.soyweed_part)
+
+    left_top_corner = [200, 200]
+
+    extratags = idp.geotiff._offset_geotiff_extratags(dom_test.header, left_top_corner)
+
+    for t in extratags:
+        if t[0] == 33922:
+            # the key of above function is calculate the correct 
+            # <tifffile.TiffTag 33922 ModelTiepointTag @190>
+            assert t[3] == (0, 0, 0, 484593.61105, 3862259.86493, 0)
+
+    # test file type error
+    with pytest.raises(TypeError, match=re.escape("only *.tif file name is supported")):
+        idp.geotiff.save_geotiff(dom_test.header, dom_imarray, left_top_corner, "random_name.tifx")
+
+    # test whether correctly saved
+    save_tiff = test_data.tiff.out / "def_save_geotiff_test.tif"
+    if save_tiff.exists():
+        save_tiff.unlink()
+
+    idp.geotiff.save_geotiff(dom_test.header, dom_imarray, left_top_corner, save_tiff)
+
+    assert save_tiff.exists()
+
+    # check if successfully offseted 20x20 pixels
+    # visually check the output and input DOM in QGIS no problem
+    # here use code to check
+    saved_dom = idp.GeoTiff(save_tiff)
+
+    assert saved_dom.header['tie_point'] == [484593.61105, 3862259.86493]
+    assert dom_test.header['tie_point'] == [484593.41105, 3862260.0649300003]
+
 
 # ==============
 # GeoTiff Class
 # ==============
 
-def test_class_check_hasfile_decorator():
-    obj = idp.GeoTiff()
-
-    with pytest.raises(FileNotFoundError, match=re.escape("Could not operate if not specify correct geotiff file")):
-        obj.save_geotiff(np.ones((3,3)), np.ones((1,2)), "wrong_path")
-
-    obj2 = idp.GeoTiff(test_data.pix4d.lotus_dom)
-    obj2.file_path = f"not/exists/path"
-    with pytest.raises(FileNotFoundError, match=re.escape("Could not operate if not specify correct geotiff file")):
-        obj2.save_geotiff(np.ones((3,3)), np.ones((1,2)), "wrong_path")
-
-    obj3 = idp.GeoTiff(test_data.pix4d.lotus_dom)
-    obj3.header = None
-    with pytest.raises(FileNotFoundError, match=re.escape("Could not operate if not specify correct geotiff file")):
-        obj3.save_geotiff(np.ones((3,3)), np.ones((1,2)), "wrong_path")
+# This should be activated after geotiff.save_geotiff() function totally finished
+# def test_class_check_hasfile_decorator():
+#     obj = idp.GeoTiff()
+
+#     with pytest.raises(FileNotFoundError, match=re.escape("Could not operate if not specify correct geotiff file")):
+#         obj.save_geotiff(np.ones((3,3)), np.ones((1,2)), "wrong_path")
+
+#     obj2 = idp.GeoTiff(test_data.pix4d.lotus_dom)
+#     obj2.file_path = f"not/exists/path"
+#     with pytest.raises(FileNotFoundError, match=re.escape("Could not operate if not specify correct geotiff file")):
+#         obj2.save_geotiff(np.ones((3,3)), np.ones((1,2)), "wrong_path")
+
+#     obj3 = idp.GeoTiff(test_data.pix4d.lotus_dom)
+#     obj3.header = None
+#     with pytest.raises(FileNotFoundError, match=re.escape("Could not operate if not specify correct geotiff file")):
+#         obj3.save_geotiff(np.ones((3,3)), np.ones((1,2)), "wrong_path")
 
 def test_class_init_with_path():
     obj = idp.GeoTiff(test_data.pix4d.lotus_dom)
 
     # convert rel path to abs path, ideally it should longer
     assert Path(obj.file_path).resolve() == test_data.pix4d.lotus_dom.resolve()
     assert obj.header is not None
 
+def test_class_header_sugar_property():
+    # test the crs sugar to replace geotiff.header['crs']
+    obj = idp.GeoTiff(test_data.pix4d.lotus_dom)
+    
+    assert obj.crs == obj.header['crs']
+    assert obj.height == obj.header['height']
+    assert obj.width == obj.header['width']
+    assert obj.dim == obj.header['dim']
+    assert obj.nodata == obj.header['nodata']
+    assert obj.scale == obj.header['scale']
+    assert obj.tie_point == obj.header['tie_point']
+
+    # test value setter
+    with pytest.raises(AttributeError, match=re.escape("can't set attribute")):
+        obj.crs = 'aaa'
+
 
 def test_class_read_geotiff():
     obj = idp.GeoTiff()
     obj.read_geotiff(test_data.pix4d.lotus_dom)
 
     assert Path(obj.file_path).resolve() == test_data.pix4d.lotus_dom.resolve()
     assert obj.header is not None
 
 def test_class_crop_polygon_save_geotiff():
     obj = idp.GeoTiff(test_data.pix4d.lotus_dom)
 
     plot, proj = idp.shp.read_shp(test_data.shp.lotus_shp, name_field=0, return_proj=True)
-    plot_t = idp.shp.convert_proj(plot, proj, obj.header["crs"])
+    plot_t = idp.geotools.convert_proj(plot, proj, obj.header["crs"])
 
     # test case 1
     #  polygon_hv = plot_t["N1W1"]
     # then do random choose
     plot_id, polygon_hv = random.choice(list(plot_t.items()))
 
     save_tiff = test_data.tiff.out / "crop_polygon.tif"
@@ -441,52 +525,52 @@
         f"into geotiff shape [0, 0, 5490, 5752]. ")):
         out2 = obj.crop_rectangle(
         left=368017.75187, top=3955511.49993, 
         w=2.3561161599936895, h=2.362485199701041, 
         is_geo=False)
 
 
-def test_class_math_polygon():
+def test_class_polygon_math():
     # test dsm results
     dsm = idp.GeoTiff(test_data.pix4d.lotus_dsm)
 
     # plot_t["N1W1"] -> 
     poly_geo = np.array([
         [ 368017.7565143 , 3955511.08102277],
         [ 368019.70190232, 3955511.49811902],
         [ 368020.11263046, 3955509.54636219],
         [ 368018.15769062, 3955509.13563382],
         [ 368017.7565143 , 3955511.08102277]])
 
-    dsm_mean   = dsm.math_polygon(poly_geo, is_geo=True, kernel="mean")
-    dsm_min    = dsm.math_polygon(poly_geo, is_geo=True, kernel="min")
-    dsm_max    = dsm.math_polygon(poly_geo, is_geo=True, kernel="max")
-    dsm_pmin5  = dsm.math_polygon(poly_geo, is_geo=True, kernel="pmin5")
-    dsm_pmin10 = dsm.math_polygon(poly_geo, is_geo=True, kernel="pmin10")
-    dsm_pmax5  = dsm.math_polygon(poly_geo, is_geo=True, kernel="pmax5")
-    dsm_pmax10 = dsm.math_polygon(poly_geo, is_geo=True, kernel="pmax10")
+    dsm_mean   = dsm.polygon_math(poly_geo, is_geo=True, kernel="mean")
+    dsm_min    = dsm.polygon_math(poly_geo, is_geo=True, kernel="min")
+    dsm_max    = dsm.polygon_math(poly_geo, is_geo=True, kernel="max")
+    dsm_pmin5  = dsm.polygon_math(poly_geo, is_geo=True, kernel="pmin5")
+    dsm_pmin10 = dsm.polygon_math(poly_geo, is_geo=True, kernel="pmin10")
+    dsm_pmax5  = dsm.polygon_math(poly_geo, is_geo=True, kernel="pmax5")
+    dsm_pmax10 = dsm.polygon_math(poly_geo, is_geo=True, kernel="pmax10")
 
     assert 97 < dsm_mean   and dsm_mean   < 98
     assert 97 < dsm_min    and dsm_min    < 98
     assert 97 < dsm_max    and dsm_max    < 98
     assert 97 < dsm_pmin5  and dsm_pmin5  < 98
     assert 97 < dsm_pmin10 and dsm_pmin10 < 98
     assert 97 < dsm_pmax5  and dsm_pmax5  < 98
     assert 97 < dsm_pmax10 and dsm_pmax10 < 98
 
     # test dom results
     dom = idp.GeoTiff(test_data.pix4d.lotus_dom)
 
-    dom_mean   = dom.math_polygon(poly_geo, is_geo=True, kernel="mean")
-    dom_min    = dom.math_polygon(poly_geo, is_geo=True, kernel="min")
-    dom_max    = dom.math_polygon(poly_geo, is_geo=True, kernel="max")
-    dom_pmin5  = dom.math_polygon(poly_geo, is_geo=True, kernel="pmin5")
-    dom_pmin10 = dom.math_polygon(poly_geo, is_geo=True, kernel="pmin10")
-    dom_pmax5  = dom.math_polygon(poly_geo, is_geo=True, kernel="pmax5")
-    dom_pmax10 = dom.math_polygon(poly_geo, is_geo=True, kernel="pmax10")
+    dom_mean   = dom.polygon_math(poly_geo, is_geo=True, kernel="mean")
+    dom_min    = dom.polygon_math(poly_geo, is_geo=True, kernel="min")
+    dom_max    = dom.polygon_math(poly_geo, is_geo=True, kernel="max")
+    dom_pmin5  = dom.polygon_math(poly_geo, is_geo=True, kernel="pmin5")
+    dom_pmin10 = dom.polygon_math(poly_geo, is_geo=True, kernel="pmin10")
+    dom_pmax5  = dom.polygon_math(poly_geo, is_geo=True, kernel="pmax5")
+    dom_pmax10 = dom.polygon_math(poly_geo, is_geo=True, kernel="pmax10")
 
     assert dom_mean  .shape == (4, )
     assert dom_min   .shape == (4, )
     assert dom_max   .shape == (4, )
     assert dom_pmin5 .shape == (4, )
     assert dom_pmin10.shape == (4, )
     assert dom_pmax5 .shape == (4, )
@@ -512,15 +596,15 @@
         [ 368017.7565143 , 3955511.08102277]])
 
     pt = obj.point_query(poly_geo, is_geo=True)
 
     assert pt.shape == (5,)
     assert np.all(97 < pt) and np.all(pt < 98)
 
-def test_class_crop():
+def test_class_crop_rois():
     obj = idp.GeoTiff(test_data.pix4d.lotus_dom)
 
     roi = idp.ROI(test_data.shp.lotus_shp, name_field=0)
 
     # only pick 3 plots as testing data
     key_list = list(roi.keys())
     for key in key_list:
@@ -530,12 +614,26 @@
     roi.get_z_from_dsm(test_data.pix4d.lotus_dsm, mode="point", kernel="mean", buffer=0, keep_crs=False)
 
     tif_out_folder = test_data.tiff.out / "class_crop"
     if tif_out_folder.exists():
         shutil.rmtree(tif_out_folder)
     tif_out_folder.mkdir()
 
-    out_dict = obj.crop(roi, save_folder=tif_out_folder)
+    out_dict = obj.crop_rois(roi, save_folder=tif_out_folder)
 
     assert len(out_dict) == 3
     assert (tif_out_folder / "N1W1.tif").exists()
-    assert out_dict["N2E2"].shape == (320, 320, 4)
+    assert out_dict["N2E2"].shape == (320, 320, 4)
+
+def test_class_geo2pixel2geo_executable():
+
+    roi = idp.ROI(test_data.shp.lotus_shp, name_field=0)
+    dom = idp.GeoTiff(test_data.pix4d.lotus_dom)
+    roi.change_crs(dom.header['crs'])
+
+    roi_test = roi[111]
+
+    roi_test_pixel = dom.geo2pixel(roi_test)
+
+    roi_test_back = dom.pixel2geo(roi_test_pixel)
+
+    np.testing.assert_almost_equal(roi_test, roi_test_back, decimal=5)
```

### Comparing `easyidp-2.0.0.dev3/tests/test_jsonfile.py` & `easyidp-2.0.0.dev4/tests/test_jsonfile.py`

 * *Files identical despite different names*

### Comparing `easyidp-2.0.0.dev3/tests/test_pix4d.py` & `easyidp-2.0.0.dev4/tests/test_pix4d.py`

 * *Files 17% similar despite different names*

```diff
@@ -162,15 +162,16 @@
 
     assert isinstance(p4d.sensors[0], idp.reconstruct.Sensor)
     assert p4d.sensors[0].label == "FC550_DJIMFT15mmF1.7ASPH_15.0_4608x3456"
 
     assert p4d.sensors[0].calibration.f == 3951.0935994102065
     assert p4d.sensors[0].focal_length == 15.005226206224117
 
-    assert p4d.photos[0].label == "DJI_0151.JPG"
+    # assert p4d.photos[0].label == "DJI_0151.JPG"
+    assert p4d.photos[0].label == "DJI_0151"
     assert p4d.photos[0].path == ''
     assert "photos" in str(p4d.photos["DJI_0174.JPG"].path)
     assert p4d.photos["DJI_0174.JPG"].cam_matrix.shape == (3,3)
     assert p4d.photos["DJI_0174.JPG"].rotation.shape == (3,3)
     assert p4d.photos["DJI_0174.JPG"].location.shape == (3,)
     assert p4d.photos["DJI_0174.JPG"].transform.shape == (3,4)
 
@@ -190,15 +191,15 @@
     # lotus example
     p4d = idp.Pix4D()
     param_folder = test_data.pix4d.lotus_param
     image_folder = test_data.pix4d.lotus_photos
     p4d.open_project(test_data.pix4d.lotus_folder, raw_img_folder=image_folder, param_folder=param_folder)
     
     #plot, proj = idp.shp.read_shp(r"./tests/data/pix4d/lotus_tanashi_full/plots.shp", name_field=0, return_proj=True)
-    #plot_t = idp.shp.convert_proj(plot, proj, p4d.crs)
+    #plot_t = idp.geotools.convert_proj(plot, proj, p4d.crs)
     plot =  np.array([   # N1E1
         [ 368020.2974959 , 3955511.61264302,      97.56272272],
         [ 368022.24288365, 3955512.02973983,      97.56272272],
         [ 368022.65361232, 3955510.07798313,      97.56272272],
         [ 368020.69867274, 3955509.66725421,      97.56272272],
         [ 368020.2974959 , 3955511.61264302,      97.56272272]
     ])
@@ -209,22 +210,15 @@
     px_0177 = np.array([
         [ 137.10982937, 2359.55887614],
         [ 133.56116243, 2107.13954299],
         [ 384.767746  , 2097.05639105],
         [ 388.10993307, 2350.41225998],
         [ 137.10982937, 2359.55887614]])
 
-    np.testing.assert_almost_equal(out_dict["DJI_0177.JPG"], px_0177)
-
-    # plot figures
-    img_name = "DJI_0198.JPG"
-    photo = p4d.photos[img_name]
-    idp.visualize.draw_polygon_on_img(
-        img_name, photo.path, out_dict[img_name], show=False, 
-        save_as="./tests/out/visual_test/p4d_back2raw_single_view.png")
+    np.testing.assert_almost_equal(out_dict["DJI_0177"], px_0177)
 
 def test_class_back2raw():
     lotus = idp.data.Lotus()
 
     p4d = idp.Pix4D(project_path=lotus.pix4d.project, 
                     raw_img_folder=lotus.photo,
                     param_folder=lotus.pix4d.param)
@@ -237,26 +231,68 @@
             del roi[key]
     roi.get_z_from_dsm(lotus.pix4d.dsm)
 
     out_all = p4d.back2raw(roi)
 
     assert len(out_all) == 2
 
+def test_class_back2raw_error():
+
+    p4d = idp.Pix4D(test_data.pix4d.lotus_folder, 
+                    test_data.pix4d.lotus_photos,
+                    test_data.pix4d.lotus_param)
+
+    roi = idp.ROI(test_data.shp.lotus_shp, name_field=0)
+
+    with pytest.raises(
+        ValueError, 
+        match=re.escape(
+            "The back2raw function requires 3D roi with shape=(n, 3), but [N1W1] is (5, 2)")):
+            p4d.back2raw(roi)
+
 
 def test_class_get_photo_position():
     lotus = idp.data.Lotus()
 
     p4d = idp.Pix4D(project_path=lotus.pix4d.project, 
                     raw_img_folder=lotus.photo,
                     param_folder=lotus.pix4d.param)
 
     out = p4d.get_photo_position()
 
     assert len(out) == 151
-    assert "DJI_0430.JPG" in out.keys()
-    np.testing.assert_almost_equal(out['DJI_0430.JPG'], np.array([ 368020.07181613, 3955477.75605109,     136.75217778]))
+    assert "DJI_0430" in out.keys()
+    np.testing.assert_almost_equal(out['DJI_0430'], np.array([ 368020.07181613, 3955477.75605109,     136.75217778]))
 
     # convert to another proj?
-    out_lonlat = p4d.get_photo_position(to_crs=pyproj.CRS.from_epsg(4326))
+    out_lonlat = p4d.get_photo_position(to_crs=pyproj.CRS.from_epsg(4326), refresh=True)
     assert len(out_lonlat) == 151
-    assert "DJI_0430.JPG" in out_lonlat.keys()
-    np.testing.assert_almost_equal(out_lonlat['DJI_0430.JPG'], np.array(np.array([139.5405607 ,  35.73445188, 136.75217778])))
+    assert "DJI_0430" in out_lonlat.keys()
+    np.testing.assert_almost_equal(out_lonlat['DJI_0430'], np.array([139.5405607 ,  35.73445188, 136.75217778]))
+
+    # change crs and refresh
+    p4d.crs = pyproj.CRS.from_epsg(4326)
+    assert p4d._photo_position_cache is None
+    out_utm = p4d.get_photo_position()
+    np.testing.assert_almost_equal(out_utm['DJI_0430'], np.array([139.5405607 ,  35.73445188, 136.75217778]))
+
+
+def test_class_init():
+
+    # test read folder & p4d file extention
+
+    # easyidp.data/data_for_tests/pix4d/maize_tanashi/maize_tanashi_3NA_20190729_Ins1Rgb_30m_pix4d
+    p4d = idp.Pix4D(test_data.pix4d.maize_folder)
+    assert p4d.label == 'maize_tanashi_3NA_20190729_Ins1Rgb_30m_pix4d'
+
+    # easyidp.data/data_for_tests/pix4d/maize_tanashi/maize_tanashi_3NA_20190729_Ins1Rgb_30m_pix4d.p4d
+    p4d = idp.Pix4D(str(test_data.pix4d.maize_folder) + '.p4d' )
+    assert p4d.label == 'maize_tanashi_3NA_20190729_Ins1Rgb_30m_pix4d'
+
+def test_class_photos_get_by_short_name():
+    p4d = idp.Pix4D()
+
+    param_folder = test_data.pix4d.lotus_param
+    image_folder = test_data.pix4d.lotus_photos
+    p4d.open_project(test_data.pix4d.lotus_folder, raw_img_folder=image_folder, param_folder=param_folder)
+
+    assert p4d.photos["DJI_0174"] == p4d.photos["DJI_0174.JPG"]
```

### Comparing `easyidp-2.0.0.dev3/tests/test_pointcloud.py` & `easyidp-2.0.0.dev4/tests/test_pointcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,19 +147,19 @@
     # with normals
     if out_npath_bin.exists():
         out_npath_bin.unlink()
     if out_npath_asc.exists():
         out_npath_asc.unlink()
     
     # without normals
-    idp.pointcloud.write_ply(write_points, write_colors, out_path_bin, binary=True)
-    idp.pointcloud.write_ply(write_points, write_colors, out_path_asc, binary=False)
+    idp.pointcloud.write_ply(out_path_bin,  write_points, write_colors, binary=True)
+    idp.pointcloud.write_ply(out_path_asc,  write_points, write_colors, binary=False)
     # with normals
-    idp.pointcloud.write_ply(write_points, write_colors, out_npath_bin, normals=write_normals, binary=True)
-    idp.pointcloud.write_ply(write_points, write_colors, out_npath_asc, normals=write_normals, binary=False)
+    idp.pointcloud.write_ply(out_npath_bin, write_points, write_colors, normals=write_normals, binary=True)
+    idp.pointcloud.write_ply(out_npath_asc, write_points, write_colors, normals=write_normals, binary=False)
 
     # test if file created
     assert out_path_bin.exists()
     assert out_path_asc.exists()
 
     assert out_npath_bin.exists()
     assert out_npath_asc.exists()
@@ -196,17 +196,17 @@
     if out_path_las.exists():
         out_path_las.unlink()
     # with normals
     if out_npath_las.exists():
         out_npath_las.unlink()
 
     # without normals
-    idp.pointcloud.write_las(write_points, write_colors, out_path_las)
+    idp.pointcloud.write_las(out_path_las,  write_points, write_colors)
     # with normals
-    idp.pointcloud.write_las(write_points, write_colors, out_npath_las, normals=write_normals)
+    idp.pointcloud.write_las(out_npath_las, write_points, write_colors, normals=write_normals)
 
     # test if file created
     assert out_path_las.exists()
     assert out_npath_las.exists()
 
     p, c, n = idp.pointcloud.read_las(out_path_las)
     # where will be a precision loss, wait for the feedback of https://github.com/laspy/laspy/issues/222
@@ -230,17 +230,17 @@
     if out_path_laz.exists():
         out_path_laz.unlink()
     # with normals
     if out_npath_laz.exists():
         out_npath_laz.unlink()
 
     # without normals
-    idp.pointcloud.write_laz(write_points, write_colors, out_path_laz)
+    idp.pointcloud.write_laz(out_path_laz,  write_points, write_colors)
     # with normals
-    idp.pointcloud.write_laz(write_points, write_colors, out_npath_laz, normals=write_normals)
+    idp.pointcloud.write_laz(out_npath_laz, write_points, write_colors, normals=write_normals)
 
     # test if file created
     assert out_path_laz.exists()
     assert out_npath_laz.exists()
 
     p, c, n = idp.pointcloud.read_laz(out_path_laz)
     # where will be a precision loss, wait for the feedback of https://github.com/laspy/laspy/issues/222
@@ -339,29 +339,29 @@
 
     pcd.points = pts1
 
     np.testing.assert_almost_equal(pcd.points, pts1)
     np.testing.assert_almost_equal(pcd._points, pts1)
 
     ## change offset value
-    pcd.set_offset(np.array([1,1,1]))
+    pcd.update_offset_value(np.array([1,1,1]))
     
     np.testing.assert_almost_equal(pcd.points, pts1)
     np.testing.assert_almost_equal(pcd._points, np.array([[0,1,2],[3,4,5]]))
 
     # check create with offset
     pcd = idp.PointCloud(offset=[10,10,10])
 
     pcd.points = pts1
 
     np.testing.assert_almost_equal(pcd.points, pts1)
     np.testing.assert_almost_equal(pcd._points, np.array([[-9, -8, -7],[-6, -5, -4]]))
 
     # then change offset
-    pcd.set_offset([0, 0, 0])
+    pcd.update_offset_value([0, 0, 0])
 
     np.testing.assert_almost_equal(pcd.points, pts1)
     np.testing.assert_almost_equal(pcd._points, pts1)
 
 def test_class_pointcloud_def_read_point_cloud_no_offset():
     # read pcd without offset
     pcd = idp.PointCloud(test_data.pcd.lotus_ply_bin)
@@ -512,15 +512,15 @@
 
     tif_out_folder = test_data.pcd.out / "class_crop"
     # clear temp output folder
     if tif_out_folder.exists():
         shutil.rmtree(tif_out_folder)
     tif_out_folder.mkdir()
 
-    out = p4d.pcd.crop(roi, save_folder=tif_out_folder)
+    out = p4d.pcd.crop_rois(roi, save_folder=tif_out_folder)
 
     assert len(out) == 3
     assert len(out["N1W1"]) == 15226
 
     assert (tif_out_folder / "N1W1.ply").exists()
 
     # also need check the offsets and points values
```

### Comparing `easyidp-2.0.0.dev3/tests/test_roi.py` & `easyidp-2.0.0.dev4/tests/test_roi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,250 +1,327 @@
-import re
-import pytest
-import numpy as np
-import pyproj
-
-import easyidp as idp
-
-test_data = idp.data.TestData(test_out="./tests/out")
-
-def test_read_cc_txt():
-    results = np.array([
-        [-18.42576599, -16.10819054,  -0.63814539],
-        [-18.00066757, -18.05295944,  -0.67380333],
-        [-16.05021095, -17.63488388,  -0.68102068],
-        [-16.46848488, -15.66774559,  -0.6401825 ],
-        [-18.42576599, -16.10819054,  -0.63814539]])
-
-    # xyz type:
-    xyz_fpath = test_data.roi.xyz_txt
-    xyz_np = idp.roi.read_cc_txt(xyz_fpath)
-
-    np.testing.assert_almost_equal(xyz_np, results)
-
-    # lxyz type
-    lxyz_fpath = test_data.roi.lxyz_txt
-    lxyz_np = idp.roi.read_cc_txt(lxyz_fpath)
-
-    np.testing.assert_almost_equal(lxyz_np, results)
-
-
-def test_class_roi_init():
-    roi = idp.ROI()
-
-    # specify values
-    roi["ddfge"] = np.array([[1,2],[4,5]])
-    assert len(roi) == 1
-    assert "ddfge" in roi.item_label.keys()
-
-def test_class_roi_read_shp():
-    roi = idp.ROI()
-
-    roi.read_shp(test_data.shp.roi_shp, name_field=0)
-
-    assert len(roi) == 3
-    assert roi.crs.name == 'WGS 84 / UTM zone 54N'
-
-    # also test overwrite read
-    roi = idp.ROI()
-    roi.read_shp(test_data.shp.lotus_shp, name_field=0)
-
-    assert roi.crs.name == "WGS 84"
-    assert "N1W1" in roi.keys()
-
-def test_class_read_labelme_json():
-    json_path = test_data.json.labelme_demo
-
-    roi = idp.ROI(json_path)
-
-    assert roi['1'][0,0] == 2447.239263803681
-
-    # test errors
-    with pytest.raises(TypeError, match=r"It seems \[.*for_read_json\.json\] is not a Labelme json file"):
-        # > It seems [C:\\Users\\hwang\\AppData\\Local\\easyidp.data\\data_for_tests\\json_test\\for_read_json.json] is not a Labelme json file.
-        roi = idp.ROI(test_data.json.labelme_err)
-        
-
-    # test warnings
-    with pytest.warns(UserWarning, match=re.escape("Only labelme [polygon] shape are accepted, not [points] of [1]")):
-        roi = idp.ROI(test_data.json.labelme_warn)
-
-        assert len(roi) == 0
-
-
-def test_class_roi_change_crs():
-    roi = idp.ROI(test_data.shp.lotus_shp)
-
-    obj = idp.GeoTiff(test_data.pix4d.lotus_dom)
-
-    roi.change_crs(obj.header["crs"])
-    assert roi.crs.name == obj.header["crs"].name
-
-def test_class_roi_get_z_from_dsm():
-    # only test whether works, not examine the value is true or not
-    roi = idp.ROI(test_data.shp.lotus_shp, name_field=0)
-    # have different CRS from shp file
-    lotus_full_dsm = test_data.pix4d.lotus_dsm
-
-    # only pick 3 plots as testing data
-    key_list = list(roi.keys())
-    for key in key_list:
-        if key not in ["N1W1", "N2E2", "S1W1"]:
-            del roi[key]
-            
-    assert len(roi) == 3
-
-    #######################
-    # test mode == points #
-    #######################
-    ht = 97.63990020751953
-    map_ht = 97.56273651123047
-    # var name -> roi_mode_kernel_buffer_keepcrs
-    roi_p_mean_0_f = roi.copy()
-    roi_p_mean_0_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=0, keep_crs=False)
-    assert roi_p_mean_0_f.crs.name == 'WGS 84 / UTM zone 54N'
-    assert roi_p_mean_0_f[0].shape == (5,3)
-    np.testing.assert_almost_equal(roi_p_mean_0_f[0][0,0], 368017.7565143015)
-    np.testing.assert_almost_equal(roi_p_mean_0_f[0][0,1], 3955511.081022765)
-    np.testing.assert_almost_equal(roi_p_mean_0_f[0][0,2], ht)
-
-    roi_p_mean_0_t = roi.copy()
-    roi_p_mean_0_t.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=0, keep_crs=True)
-    assert roi_p_mean_0_t.crs.name == "WGS 84"
-    assert roi_p_mean_0_t[0].shape == (5,3)
-    np.testing.assert_almost_equal(roi_p_mean_0_t[0][0,0], 35.73475194328632)  # latitude
-    np.testing.assert_almost_equal(roi_p_mean_0_t[0][0,1], 139.54052962153048)  # longitude
-    np.testing.assert_almost_equal(roi_p_mean_0_t[0][0,2], ht)
-
-    roi_p_mean_1_f = roi.copy()
-    roi_p_mean_1_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=1, keep_crs=False)
-    assert roi_p_mean_1_f[0].shape == (5,3)
-    assert roi_p_mean_1_f[0][0,1] != ht
-
-    roi_p_mean_1d0_f = roi.copy()
-    roi_p_mean_1d0_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=1.0, keep_crs=False)
-    assert roi_p_mean_1d0_f[0].shape == (5,3)
-    # buffer 1.0 and buffer 1 should be the same
-    assert roi_p_mean_1d0_f[0][0,2] == roi_p_mean_1_f[0][0,2]
-
-    # using full map as results
-    roi_p_mean_m1_f = roi.copy()
-    roi_p_mean_m1_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=-1, keep_crs=False)
-    # all the z values should be the same
-    assert all(np.all(i[:,2] == map_ht) for i in roi_p_mean_m1_f.values())
-
-    roi_p_mean_m1d0_f = roi.copy()
-    roi_p_mean_m1d0_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=-1.0, keep_crs=False)
-    # all the z values should be the same
-    assert all(np.all(i[:,2] == map_ht) for i in roi_p_mean_m1d0_f.values())
-
-    #####################
-    # test mode == face #
-    #####################
-    roi_f_mean_1_f = roi.copy()
-    roi_f_mean_1_f.get_z_from_dsm(lotus_full_dsm, mode="face", kernel="mean", buffer=1, keep_crs=False)
-    assert roi_f_mean_1_f[0].shape == (5,3)
-    np.testing.assert_almost_equal(roi_f_mean_1_f[0][0,0], 368017.7565143015)
-    np.testing.assert_almost_equal(roi_f_mean_1_f[0][0,1], 3955511.081022765)
-
-    roi_f_mean_0_f = roi.copy()
-    roi_f_mean_0_f.get_z_from_dsm(lotus_full_dsm, mode="face", kernel="mean", buffer=0, keep_crs=False)
-    assert roi_f_mean_0_f[0].shape == (5,3)
-    np.testing.assert_almost_equal(roi_f_mean_0_f[0][0,0], 368017.7565143015)
-    np.testing.assert_almost_equal(roi_f_mean_0_f[0][0,1], 3955511.081022765)
-
-def test_class_roi_get_z_from_dsm_errors():
-    roi = idp.ROI(test_data.shp.lotus_shp)
-    lotus_full_dsm = test_data.pix4d.lotus_dsm
-
-    with pytest.raises(KeyError, match=re.escape("The param 'mode' only accept 'point' or 'face', not 'abcde'")):
-        roi.get_z_from_dsm(lotus_full_dsm, mode="abcde")
-
-    with pytest.raises(KeyError, match=re.escape(
-        "The param 'kernal' only accept 'mean', 'min', 'max', 'pmin5', 'pmin10', 'pmax5', 'pmax10' not 'abcde'"
-        )):
-        roi.get_z_from_dsm(lotus_full_dsm, kernel="abcde")
-
-    with pytest.raises(TypeError, match=re.escape(
-        "Only 'int' and 'float' are acceptable for 'buffer', not <class 'str'> [abcde]"
-        )):
-        roi.get_z_from_dsm(lotus_full_dsm, buffer="abcde")
-
-    with pytest.raises(FileNotFoundError, match=re.escape("Could not find file")):
-        roi.get_z_from_dsm("seffed")
-
-    with pytest.raises(TypeError, match=re.escape("Only geotiff path <str> and <easyidp.GeoTiff> object")):
-        roi.get_z_from_dsm(23345)
-
-    with pytest.raises(TypeError, match=re.escape("Could not operate without CRS specified")):
-        roi.crs = None
-        roi.get_z_from_dsm(lotus_full_dsm, buffer="abcde")
-
-
-def test_class_roi_crop():
-    # just ensure it can run, the data examine please check corresponding modules' test
-
-    # data prepare
-    lotus_full_dsm = test_data.pix4d.lotus_dsm
-    lotus_full_pcd = test_data.pix4d.lotus_pcd 
-    lotus_full_dom = test_data.pix4d.lotus_dom 
-    lotus_full_shp = test_data.shp.lotus_shp 
-
-    roi = idp.ROI(lotus_full_shp, name_field=0)
-
-    # only pick 3 plots as testing data
-    key_list = list(roi.keys())
-    for key in key_list:
-        if key not in ["N1W1", "N2E2", "S1W1"]:
-            del roi[key]
-
-    roi.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=0, keep_crs=False)
-
-    # crop geotiff
-    out_dom = roi.crop(lotus_full_dom)
-    assert len(out_dom) == 3
-
-    out_dsm = roi.crop(lotus_full_dsm)
-    assert len(out_dsm) == 3
-
-    # crop point cloud
-    out_pcd = roi.crop(lotus_full_pcd)
-    assert len(out_pcd) == 3
-
-def test_class_roi_crop_error():
-    roi = idp.ROI()
-
-    with pytest.raises(TypeError, match=re.escape("Could not operate without CRS specified")):
-        roi.crop("aaa")
-
-    roi.crs = pyproj.CRS.from_epsg(4326)
-    with pytest.raises(TypeError, match=re.escape(
-        "Only file path <str> or <easyidp.GeoTiff> object or <easyidp.PointCloud>"
-        " object are accepted, not <class 'str'>")):
-        roi.crop("aaa")
-
-
-def test_class_roi_back2raw():
-    # single chunk:
-    lotus = idp.data.Lotus()
-
-    p4d = idp.Pix4D(project_path=lotus.pix4d.project, 
-                    raw_img_folder=lotus.photo,
-                    param_folder=lotus.pix4d.param)
-
-    ms = idp.Metashape(project_path=lotus.metashape.project, chunk_id=0)
-
-    roi = idp.ROI(lotus.shp, name_field=0)
-    # only pick 2 plots as testing data
-    key_list = list(roi.keys())
-    for key in key_list:
-        if key not in ["N1W1", "N1W2"]:
-            del roi[key]
-    roi.get_z_from_dsm(lotus.pix4d.dsm)
-
-    ms.crs = roi.crs
-
-    out_p4d = roi.back2raw(p4d)
-    out_ms = roi.back2raw(ms)
-
-    assert len(out_p4d) == 2
-    assert len(out_ms) == 2
+import re
+import pytest
+import numpy as np
+import pyproj
+
+import easyidp as idp
+
+test_data = idp.data.TestData(test_out="./tests/out")
+
+def test_read_cc_txt():
+    results = np.array([
+        [-18.42576599, -16.10819054,  -0.63814539],
+        [-18.00066757, -18.05295944,  -0.67380333],
+        [-16.05021095, -17.63488388,  -0.68102068],
+        [-16.46848488, -15.66774559,  -0.6401825 ],
+        [-18.42576599, -16.10819054,  -0.63814539]])
+
+    # xyz type:
+    xyz_fpath = test_data.roi.xyz_txt
+    xyz_np = idp.roi.read_cc_txt(xyz_fpath)
+
+    np.testing.assert_almost_equal(xyz_np, results)
+
+    # lxyz type
+    lxyz_fpath = test_data.roi.lxyz_txt
+    lxyz_np = idp.roi.read_cc_txt(lxyz_fpath)
+
+    np.testing.assert_almost_equal(lxyz_np, results)
+
+
+def test_class_roi_init():
+    roi = idp.ROI()
+
+    # specify values
+    roi["ddfge"] = np.array([[1,2],[4,5]])
+    assert len(roi) == 1
+    assert "ddfge" in roi.item_label.keys()
+
+def test_class_roi_slice():
+    # solve the issue 58
+    roi = idp.ROI()
+
+    roi.read_shp(test_data.shp.roi_shp, name_field=0)
+
+    assert len(roi) == 3
+
+    roi = roi[0:2]
+
+    assert len(roi) == 2
+
+    for func_name in ["crop", "back2raw", "get_z_from_dsm"]:
+        assert func_name in dir(roi)
+
+def test_class_roi_copy():
+    roi = idp.ROI()
+
+    roi.read_shp(test_data.shp.roi_shp, name_field=0)
+
+    roi_copy = roi.copy()
+
+    roi_copy[0][0, 0] = 368000
+
+    assert roi_copy[0][0, 0] == 368000
+    assert roi[0][0, 0] == 368101.05641086295
+
+    assert roi.crs == roi_copy.crs
+    assert roi.source == roi_copy.source
+
+def test_class_roi_read_shp():
+    roi = idp.ROI()
+
+    roi.read_shp(test_data.shp.roi_shp, name_field=0)
+
+    assert len(roi) == 3
+    assert roi.crs.name == 'WGS 84 / UTM zone 54N'
+
+    # also test overwrite read
+    roi = idp.ROI()
+    roi.read_shp(test_data.shp.lotus_shp, name_field=0)
+
+    assert roi.crs.name == "WGS 84"
+    assert "N1W1" in roi.keys()
+
+def test_class_read_labelme_json():
+    json_path = test_data.json.labelme_demo
+
+    roi = idp.ROI(json_path)
+
+    assert roi['1'][0,0] == 2447.239263803681
+
+    # test errors
+    with pytest.raises(TypeError, match=r"It seems \[.*for_read_json\.json\] is not a Labelme json file"):
+        # > It seems [C:\\Users\\hwang\\AppData\\Local\\easyidp.data\\data_for_tests\\json_test\\for_read_json.json] is not a Labelme json file.
+        roi = idp.ROI(test_data.json.labelme_err)
+        
+
+    # test warnings
+    with pytest.warns(UserWarning, match=re.escape("Only labelme [polygon] shape are accepted, not [points] of [1]")):
+        roi = idp.ROI(test_data.json.labelme_warn)
+
+        assert len(roi) == 0
+
+
+def test_class_roi_change_crs():
+    roi = idp.ROI(test_data.shp.lotus_shp)
+
+    obj = idp.GeoTiff(test_data.pix4d.lotus_dom)
+
+    roi.change_crs(obj.header["crs"])
+    assert roi.crs.name == obj.header["crs"].name
+
+def test_class_roi_get_z_from_dsm():
+    # only test whether works, not examine the value is true or not
+    roi = idp.ROI(test_data.shp.lotus_shp, name_field=0)
+    # have different CRS from shp file
+    lotus_full_dsm = test_data.pix4d.lotus_dsm
+
+    # only pick 3 plots as testing data
+    key_list = list(roi.keys())
+    for key in key_list:
+        if key not in ["N1W1", "N2E2", "S1W1"]:
+            del roi[key]
+            
+    assert len(roi) == 3
+
+    #######################
+    # test mode == points #
+    #######################
+    ht = 97.63990020751953
+    map_ht = 97.56273651123047
+    # var name -> roi_mode_kernel_buffer_keepcrs
+    roi_p_mean_0_f = roi.copy()
+    roi_p_mean_0_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=0, keep_crs=False)
+    assert roi_p_mean_0_f.crs.name == 'WGS 84 / UTM zone 54N'
+    assert roi_p_mean_0_f[0].shape == (5,3)
+    np.testing.assert_almost_equal(roi_p_mean_0_f[0][0,0], 368017.7565143015)
+    np.testing.assert_almost_equal(roi_p_mean_0_f[0][0,1], 3955511.081022765)
+    np.testing.assert_almost_equal(roi_p_mean_0_f[0][0,2], ht)
+
+    roi_p_mean_0_t = roi.copy()
+    roi_p_mean_0_t.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=0, keep_crs=True)
+    assert roi_p_mean_0_t.crs.name == "WGS 84"
+    assert roi_p_mean_0_t[0].shape == (5,3)
+    np.testing.assert_almost_equal(roi_p_mean_0_t[0][0,0], 139.54052962153048)  # longitude
+    np.testing.assert_almost_equal(roi_p_mean_0_t[0][0,1], 35.73475194328632)  # latitude
+    np.testing.assert_almost_equal(roi_p_mean_0_t[0][0,2], ht)
+
+    roi_p_mean_1_f = roi.copy()
+    roi_p_mean_1_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=1, keep_crs=False)
+    assert roi_p_mean_1_f[0].shape == (5,3)
+    assert roi_p_mean_1_f[0][0,1] != ht
+
+    roi_p_mean_1d0_f = roi.copy()
+    roi_p_mean_1d0_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=1.0, keep_crs=False)
+    assert roi_p_mean_1d0_f[0].shape == (5,3)
+    # buffer 1.0 and buffer 1 should be the same
+    assert roi_p_mean_1d0_f[0][0,2] == roi_p_mean_1_f[0][0,2]
+
+    # using full map as results
+    roi_p_mean_m1_f = roi.copy()
+    roi_p_mean_m1_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=-1, keep_crs=False)
+    # all the z values should be the same
+    assert all(np.all(i[:,2] == map_ht) for i in roi_p_mean_m1_f.values())
+
+    roi_p_mean_m1d0_f = roi.copy()
+    roi_p_mean_m1d0_f.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=-1.0, keep_crs=False)
+    # all the z values should be the same
+    assert all(np.all(i[:,2] == map_ht) for i in roi_p_mean_m1d0_f.values())
+
+    #####################
+    # test mode == face #
+    #####################
+    roi_f_mean_1_f = roi.copy()
+    roi_f_mean_1_f.get_z_from_dsm(lotus_full_dsm, mode="face", kernel="mean", buffer=1, keep_crs=False)
+    assert roi_f_mean_1_f[0].shape == (5,3)
+    np.testing.assert_almost_equal(roi_f_mean_1_f[0][0,0], 368017.7565143015)
+    np.testing.assert_almost_equal(roi_f_mean_1_f[0][0,1], 3955511.081022765)
+
+    roi_f_mean_0_f = roi.copy()
+    roi_f_mean_0_f.get_z_from_dsm(lotus_full_dsm, mode="face", kernel="mean", buffer=0, keep_crs=False)
+    assert roi_f_mean_0_f[0].shape == (5,3)
+    np.testing.assert_almost_equal(roi_f_mean_0_f[0][0,0], 368017.7565143015)
+    np.testing.assert_almost_equal(roi_f_mean_0_f[0][0,1], 3955511.081022765)
+
+
+def test_class_roi_get_z_from_dsm_warns():
+    # the ROI outside the DSM ranges and cause nan values for z
+    # bug report #69
+    roi = idp.ROI(test_data.shp.lotus_shp, name_field=0)
+    roi = roi[0:3]
+
+    roi[0] = roi[0] + np.array([0,  -0.00029697])  # offset 1 degree lon & lat
+
+    lotus_full_dsm = test_data.pix4d.lotus_dsm
+
+    with pytest.warns(UserWarning, match=re.escape("Z values contains empty attribute [-10000.0] for ['N1W1'], this may be caused by the")):
+        roi.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=0, keep_crs=False)
+        print(roi[0])
+
+def test_class_roi_get_z_from_dsm_errors():
+    roi = idp.ROI(test_data.shp.lotus_shp)
+    lotus_full_dsm = test_data.pix4d.lotus_dsm
+
+    with pytest.raises(KeyError, match=re.escape("The param 'mode' only accept 'point' or 'face', not 'abcde'")):
+        roi.get_z_from_dsm(lotus_full_dsm, mode="abcde")
+
+    with pytest.raises(KeyError, match=re.escape(
+        "The param 'kernal' only accept 'mean', 'min', 'max', 'pmin5', 'pmin10', 'pmax5', 'pmax10' not 'abcde'"
+        )):
+        roi.get_z_from_dsm(lotus_full_dsm, kernel="abcde")
+
+    with pytest.raises(TypeError, match=re.escape(
+        "Only 'int' and 'float' are acceptable for 'buffer', not <class 'str'> [abcde]"
+        )):
+        roi.get_z_from_dsm(lotus_full_dsm, buffer="abcde")
+
+    with pytest.raises(FileNotFoundError, match=re.escape("Could not find file")):
+        roi.get_z_from_dsm("seffed")
+
+    with pytest.raises(TypeError, match=re.escape("Only geotiff path <str> and <easyidp.GeoTiff> object")):
+        roi.get_z_from_dsm(23345)
+
+    with pytest.raises(TypeError, match=re.escape("Could not operate without CRS specified")):
+        roi.crs = None
+        roi.get_z_from_dsm(lotus_full_dsm, buffer="abcde")
+
+def test_func_insert_z_value_for_roi_error():
+    # test catching incorrest ROI.shape
+    with pytest.raises(ValueError, match=re.escape("The expected ROI shape should be (n, 3), not given (5, 4)")):
+        out = idp.roi._insert_z_value_for_roi(np.ones((5,4)), 3)
+
+
+def test_class_roi_get_z_from_dsm_duplicate_load():
+    # fix bug #60
+    roi = idp.ROI(test_data.shp.lotus_shp, name_field=0)
+    roi = roi[0:3]
+
+    lotus_full_dsm = test_data.pix4d.lotus_dsm
+
+    roi.get_z_from_dsm(lotus_full_dsm)
+
+    assert roi['N1W1'].shape == (5, 3)
+
+    roi.get_z_from_dsm(lotus_full_dsm)
+
+    assert roi['N1W1'].shape == (5, 3)
+
+def test_class_roi_crop():
+    # just ensure it can run, the data examine please check corresponding modules' test
+
+    # data prepare
+    lotus_full_dsm = test_data.pix4d.lotus_dsm
+    lotus_full_pcd = test_data.pix4d.lotus_pcd 
+    lotus_full_dom = test_data.pix4d.lotus_dom 
+    lotus_full_shp = test_data.shp.lotus_shp 
+
+    roi = idp.ROI(lotus_full_shp, name_field=0)
+
+    # only pick 3 plots as testing data
+    key_list = list(roi.keys())
+    for key in key_list:
+        if key not in ["N1W1", "N2E2", "S1W1"]:
+            del roi[key]
+
+    roi.get_z_from_dsm(lotus_full_dsm, mode="point", kernel="mean", buffer=0, keep_crs=False)
+
+    # crop geotiff
+    out_dom = roi.crop(lotus_full_dom)
+    assert len(out_dom) == 3
+
+    out_dsm = roi.crop(lotus_full_dsm)
+    assert len(out_dsm) == 3
+
+    # crop point cloud
+    out_pcd = roi.crop(lotus_full_pcd)
+    assert len(out_pcd) == 3
+
+def test_class_roi_crop_error():
+    roi = idp.ROI()
+
+    with pytest.raises(TypeError, match=re.escape("Could not operate without CRS specified")):
+        roi.crop("aaa")
+
+    roi.crs = pyproj.CRS.from_epsg(4326)
+    with pytest.raises(TypeError, match=re.escape(
+        "Only file path <str> or <easyidp.GeoTiff> object or <easyidp.PointCloud>"
+        " object are accepted, not <class 'str'>")):
+        roi.crop("aaa")
+
+
+def test_class_roi_back2raw():
+    # single chunk:
+    lotus = idp.data.Lotus()
+
+    p4d = idp.Pix4D(project_path=lotus.pix4d.project, 
+                    raw_img_folder=lotus.photo,
+                    param_folder=lotus.pix4d.param)
+
+    ms = idp.Metashape(project_path=lotus.metashape.project, chunk_id=0)
+
+    roi = idp.ROI(lotus.shp, name_field=0)
+    # only pick 2 plots as testing data
+    key_list = list(roi.keys())
+    for key in key_list:
+        if key not in ["N1W1", "N1W2"]:
+            del roi[key]
+    roi.get_z_from_dsm(lotus.pix4d.dsm)
+
+    ms.crs = roi.crs
+
+    out_p4d = roi.back2raw(p4d)
+    out_ms = roi.back2raw(ms)
+
+    assert len(out_p4d) == 2
+    assert len(out_ms) == 2
+
+def test_class_roi_back2raw_error():
+    ms = idp.Metashape(test_data.metashape.lotus_psx)
+
+    roi = idp.ROI(test_data.shp.lotus_shp, name_field=0)
+
+    # test ROI.back2raw error
+    with pytest.raises(
+        ValueError, 
+        match=re.escape(
+            "The back2raw function requires 3D roi with shape=(n, 3), but [N1W1] is (5, 2)")):
+        out_ms = roi.back2raw(ms)
```

### Comparing `easyidp-2.0.0.dev3/tests/test_shp.py` & `easyidp-2.0.0.dev4/tests/test_shp.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,20 +79,19 @@
 
     # will raise error if shp_proj not given
     with pytest.raises(ValueError, match=re.escape("Unable to find the proj coordinate info [")):
         lonlat_shp = idp.shp.read_shp(shp_path)
 
     # continue if shp_proj is given
     lonlat_shp = idp.shp.read_shp(shp_path, shp_proj=pyproj.CRS.from_epsg(4326))
-    # flipped for pyproj which input is (lat, lon)
-    wanted_np = np.asarray([[34.90284972, 134.8312376],
-                            [34.90285097, 134.8312399],
-                            [34.90285516, 134.8312371],
-                            [34.90285426, 134.8312349],
-                            [34.90284972, 134.8312376]])
+    wanted_np = np.asarray([[134.8312376, 34.90284972],
+                            [134.8312399, 34.90285097],
+                            [134.8312371, 34.90285516],
+                            [134.8312349, 34.90285426],
+                            [134.8312376, 34.90284972]])
 
     np.testing.assert_almost_equal(lonlat_shp['0'], wanted_np)
 
 def test_read_shp_proj_success_print(capfd):
     shp_path = test_data.shp.testutm_shp
     test_utm_shp = idp.shp.read_shp(shp_path)
     out, err = capfd.readouterr()
@@ -105,16 +104,18 @@
                             [ 484593.62443893, 3862259.85857523]])
 
     np.testing.assert_almost_equal(test_utm_shp['0'], wanted_np)
 
 def test_read_shp_key_names():
     shp_path = test_data.shp.utm53n_shp
 
-    str_no_name_field_title_false = idp.shp.read_shp(shp_path)
-    assert "1" in str_no_name_field_title_false.keys()
+    # show warning if not specifying 'name_field'
+    with pytest.warns(UserWarning, match=re.escape("Not specifying parameter 'name_field', will using the row id ")):
+        str_no_name_field_title_false = idp.shp.read_shp(shp_path)
+        assert "1" in str_no_name_field_title_false.keys()
 
     str_no_name_field_title_true= idp.shp.read_shp(shp_path, include_title=True)
     assert "line_1" in str_no_name_field_title_true.keys()
 
     str_name_field_title_false = idp.shp.read_shp(shp_path, name_field="Attr")
     assert "1_02" in str_name_field_title_false.keys()
 
@@ -176,15 +177,15 @@
     lonlat_path = test_data.shp.lonlat_shp
     utm_path = test_data.shp.utm53n_shp
 
     lonlat_shp, lonlat_proj = idp.shp.read_shp(lonlat_path, shp_proj=pyproj.CRS.from_epsg(4326), return_proj=True)
 
     utm_shp, utm_proj = idp.shp.read_shp(utm_path, return_proj=True)
 
-    utm_cvt_shp = idp.shp.convert_proj(lonlat_shp, lonlat_proj, utm_proj)
+    utm_cvt_shp = idp.geotools.convert_proj(lonlat_shp, lonlat_proj, utm_proj)
 
     a = utm_cvt_shp['0']
     b = utm_shp['0']
 
     #  A         B
     #   o-------o
     #   |       |
```

