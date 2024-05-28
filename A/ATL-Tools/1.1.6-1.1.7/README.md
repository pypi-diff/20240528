# Comparing `tmp/atl_tools-1.1.6.tar.gz` & `tmp/atl_tools-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atl_tools-1.1.6.tar", last modified: Mon May 20 07:29:50 2024, max compression
+gzip compressed data, was "atl_tools-1.1.7.tar", last modified: Tue May 28 01:33:37 2024, max compression
```

## Comparing `atl_tools-1.1.6.tar` & `atl_tools-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-20 07:29:50.667467 atl_tools-1.1.6/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-20 07:29:50.667467 atl_tools-1.1.6/ATL_Tools/
--rw-rw-r--   0 atl       (1002) atl       (1002)    33181 2024-05-20 07:19:50.000000 atl_tools-1.1.6/ATL_Tools/ATL_gdal.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.6/ATL_Tools/ATL_path.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     2844 2024-05-20 07:20:13.000000 atl_tools-1.1.6/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-20 07:29:50.667467 atl_tools-1.1.6/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     5272 2024-05-20 07:29:50.000000 atl_tools-1.1.6/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-05-20 07:29:50.000000 atl_tools-1.1.6/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-05-20 07:29:50.000000 atl_tools-1.1.6/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-05-20 07:29:50.000000 atl_tools-1.1.6/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     5272 2024-05-20 07:29:50.667467 atl_tools-1.1.6/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)     4973 2024-05-20 07:27:23.000000 atl_tools-1.1.6/README.md
--rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-05-20 07:23:25.000000 atl_tools-1.1.6/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-05-20 07:29:50.667467 atl_tools-1.1.6/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-28 01:33:37.064577 atl_tools-1.1.7/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-28 01:33:37.060577 atl_tools-1.1.7/ATL_Tools/
+-rw-rw-r--   0 atl       (1002) atl       (1002)    38081 2024-05-28 01:28:47.000000 atl_tools-1.1.7/ATL_Tools/ATL_gdal.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.7/ATL_Tools/ATL_path.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     2836 2024-05-28 01:29:06.000000 atl_tools-1.1.7/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-28 01:33:37.060577 atl_tools-1.1.7/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     5493 2024-05-28 01:33:37.000000 atl_tools-1.1.7/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-05-28 01:33:37.000000 atl_tools-1.1.7/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-05-28 01:33:37.000000 atl_tools-1.1.7/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-05-28 01:33:37.000000 atl_tools-1.1.7/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     5493 2024-05-28 01:33:37.064577 atl_tools-1.1.7/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)     5194 2024-05-28 01:31:47.000000 atl_tools-1.1.7/README.md
+-rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-05-28 01:32:10.000000 atl_tools-1.1.7/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-05-28 01:33:37.064577 atl_tools-1.1.7/setup.cfg
```

### Comparing `atl_tools-1.1.6/ATL_Tools/ATL_gdal.py` & `atl_tools-1.1.7/ATL_Tools/ATL_gdal.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # coding: utf-8
 
 from osgeo import gdal, ogr
 import os
 import glob
 import numpy as np
 import math
-from typing import Dict, List, Optional, Sequence
+from typing import Dict, List, Optional, Sequence, Union
 from .ATL_path import mkdir_or_exist, find_data_list
 from tqdm import tqdm 
 import json
 import cv2
 
 def read_img_to_array_with_info(filename: str, 
              convert_HWC: Optional[bool] = False) -> np.ndarray:   
@@ -592,33 +592,66 @@
     ds2w = None
     ds1c = gdal.Translate('', ds1, format='MEM', projWin=[min_x, max_y, max_x, min_y], 
     outputSRS=projection)
     ds1 = None
 
     return ds1c,ds2c
 
-def crop_tif_with_json_zero(img_path: str,
-                       output_path: str,
-                       geojson_path: str):
+def crop_tif_with_json_zero(img_path: Union[str, gdal.Dataset],
+                            output_path: str,
+                            geojson_path: str):
     '''✔将带有坐标的图像按照json矢量进行裁切,矢量外无数据区域为0,适合训练
+        也可以裁切mask标签。
 
     Args:
-        img_path (str): 输入图像的路径
+        img_path (str or gdal.Dataset): 输入图像的路径 or GDAL dataset
         output_path (str): 输出图像的路径
         geojson_path (str): Geojson文件的路径
         
     Returns: 
         保存裁切后的图像至本地
+
+    Example:
+        >>> from ATL_Tools import mkdir_or_exist, find_data_list
+        >>> from ATL_Tools.ATL_gdal import crop_tif_with_json_zero
+        >>> from tqdm import tqdm
+        >>> import os 
+        >>> from osgeo import gdal
+
+        >>> label_path_all = '/opt/AI-Tianlong/Datasets/ATL-ATLNongYe/ATL推理大图/大庆/推理结果-24类/推理结果-24-mask'
+        >>> output_path_all = '/opt/AI-Tianlong/Datasets/ATL-ATLNongYe/ATL推理大图/大庆/推理结果-24类/推理结果-24-mask-crop'
+        >>> img_path_all = '/opt/AI-Tianlong/Datasets/ATL-ATLNongYe/ATL推理大图/大庆/要推理的images-矢量裁切'
+        >>> json_path_all = '../要推理的json/'
+        >>> mkdir_or_exist(output_path_all)
+        >>> label_list = find_data_list(label_path_all, suffix='.png')
+
+        >>> for label_path in tqdm(label_list, colour='Green'):
+        >>>     # 添加坐标
+        >>>     IMG_file_path = os.path.join(img_path_all, os.path.basename(label_path).replace('.png', '.tif'))
+        >>>     IMG_gdal = gdal.Open(IMG_file_path, gdal.GA_ReadOnly)
+        >>>     assert  IMG_gdal is not None, f"无法打开 {IMG_file_path}"
+        >>>     trans = IMG_gdal.GetGeoTransform()
+        >>>     proj = IMG_gdal.GetProjection()
+        >>>     label_gdal = gdal.Open(label_path, gdal.GA_ReadOnly)
+        >>>     label_gdal.SetGeoTransform(trans)
+        >>>     # 裁切
+        >>>     label_output_path = os.path.join(output_path_all, os.path.basename(label_path).replace('.png', '.tif'))
+        >>>     json_path = os.path.join(json_path_all, os.path.basename(label_path).split('_')[-1].replace('.png', '.json'))
+        >>>     print(f'正在裁切: {label_output_path},json: {json_path}')
+        >>>     crop_tif_with_json_zero(label_gdal, label_output_path, json_path)
     '''
     if os.path.exists(output_path):
         print(f"存在{output_path}, 已覆盖")
         os.remove(output_path)
 
     # 打开栅格文件
-    raster_ds = gdal.Open(img_path)
+    if isinstance(img_path, str):
+        raster_ds = gdal.Open(img_path)
+    elif isinstance(img_path, gdal.Dataset):
+        raster_ds = img_path
     assert raster_ds!=None, f'打开 {raster_ds} 失败'
 
     # 打开GeoJSON文件
     geojson_ds = ogr.Open(geojson_path)
     geojson_layer = geojson_ds.GetLayer()
 
     # 获取GeoJSON文件的范围
@@ -634,36 +667,40 @@
     gdal.Warp(output_path, raster_ds, options=warp_options)
 
     # 关闭数据源
     raster_ds = None
     geojson_ds = None
     print(f'根据矢量裁切{img_path}完成！无数据区域为0')
 
-def crop_tif_with_json_nan(img_path: str,
+def crop_tif_with_json_nan(img_path: Union[str, gdal.Dataset],
                            output_path: str,
                            geojson_path: str,
                            add_alpha_chan: bool = False) -> None:
     '''✔将带有坐标的图像按照json矢量进行裁切
     使无数据区域的值为nan,优先使用这个, 矢量外无数据区域为nan
 
     Args:
-        img_path (str): 输入图像的路径
+        img_path (str or gdal.Dataset): 输入图像的路径 or GDAL dataset
         output_path (str): 输出图像的路径
         geojson_path (str): Geojson文件的路径
         add_alpha_chan (bool): 是否给RGB添加alpha通道
         
     Returns: 
         保存裁切后的图像至本地
     '''
 
     if os.path.exists(output_path):
         print(f"存在{output_path}, 已覆盖")
         os.remove(output_path)
+        
     # 打开栅格文件
-    raster_ds = gdal.Open(img_path)
+    if isinstance(img_path, str):
+        raster_ds = gdal.Open(img_path)
+    elif isinstance(img_path, gdal.Dataset):
+        raster_ds = img_path
     assert raster_ds!=None, f'打开 {raster_ds} 失败'
 
     # 打开GeoJSON文件
     geojson_ds = ogr.Open(geojson_path)
     geojson_layer = geojson_ds.GetLayer()
 
     # 获取GeoJSON文件的范围
@@ -804,71 +841,122 @@
         output_geojson,    # 输出文件路径
         input_shp   # 输入Shapefile文件路径
     ]
 
     # 调用ogr2ogr工具执行转换
     subprocess.run(ogr2ogr_cmd)
 
-def cut_image_with_overlap(input_file, output_dir, tile_size=5000, overlap=500):
-    """将大图裁切成小图，以供GPU可以进行推理
+def clip_big_image(image_path: str, 
+                   save_path: str, 
+                   crop_size: int = 5000):
+    """把大图裁切成指定尺寸的小图，以供 GPU 可以进行推理（不带坐标）
+    
     Args:
-        input_file (str): 输入图像路径
-        output_dir (str): 输出图像路径
-        tile_size (int): 图像块的大小，默认为5000
-        overlap (int): 图像块的重叠大小，默认为500
+        image_path (str): 输入的大图路径
+        save_path (str): 输出的小图路径
+        crop_size (int): 裁切的尺寸，默认为5000
+    
+    Returns:
+        None, 保存小图至指定的文件夹
 
-    Returns: 
-        None, 保存裁切后的图像至指定目录。
+    Examples:
+       完整的使用示例见：
+       裁切：
+       https://github.com/AI-Tianlong/Useful-Tools/blob/main/code/0-Sentinel-2-%E5%A4%84%E7%90%86%E4%BB%A3%E7%A0%81/8-%E5%9B%BE%E7%89%87%E5%A4%AA%E5%A4%A7%E7%88%86%E6%98%BE%E5%AD%98-%E8%A3%81%E5%88%87%E6%88%905000%E5%B0%8F%E5%9B%BE%E6%8E%A8%E7%90%86.py
+       推理之后合并:
+       https://github.com/AI-Tianlong/Useful-Tools/blob/main/code/0-Sentinel-2-%E5%A4%84%E7%90%86%E4%BB%A3%E7%A0%81/9-%E9%87%8D%E6%96%B0%E5%B0%86%E6%AD%A5%E9%AA%A48%E7%9A%84%E5%B0%8F%E5%9B%BE%E5%90%88%E5%B9%B6%E6%88%90%E5%A4%A7%E5%9B%BE.py
+   
     """
-    # 打开输入图像
-    dataset = gdal.Open(input_file)
-    if not dataset:
-        raise FileNotFoundError(f"Unable to open {input_file}")
-
-    # 获取图像尺寸
-    width = dataset.RasterXSize
-    height = dataset.RasterYSize
-
-    # 获取投影和地理变换信息
-    projection = dataset.GetProjection()
-    geotransform = dataset.GetGeoTransform()
-
-    # 计算图像块的步长（减去重叠部分）
-    step_size = tile_size - overlap
-
-    # 计算图像块的数量
-    x_tiles = (width + step_size - 1) // step_size
-    y_tiles = (height + step_size - 1) // step_size
-    print(f'正在裁切 {input_file} ...')
-    print(f'该图像将被裁切为 {x_tiles*y_tiles} 个 {tile_size}x{tile_size} 的小图....')
-
-    for i in range(x_tiles):
-        for j in range(y_tiles):
-            # 计算图像块的像素范围
-            x_offset = i * step_size
-            y_offset = j * step_size
-
-            # 计算实际读取的像素范围
-            x_size = min(tile_size, width - x_offset)
-            y_size = min(tile_size, height - y_offset)
-
-            # 计算输出的地理范围
-            minx = geotransform[0] + x_offset * geotransform[1] + y_offset * geotransform[2]
-            maxy = geotransform[3] + x_offset * geotransform[4] + y_offset * geotransform[5]
-            maxx = minx + x_size * geotransform[1] + y_size * geotransform[2]
-            miny = maxy + x_size * geotransform[4] + y_size * geotransform[5]
-
-            # 裁切图像块
-            output_img_path = os.path.join(output_dir,f'{os.path.basename(input_file).split(".")[0]}_{i}_{j}.tif')
-            gdal.Translate(
-                output_img_path,
-                dataset,
-                srcWin=[x_offset, y_offset, x_size, y_size],
-                format='GTiff',
-                outputSRS=projection,
-                outputBounds=[minx, miny, maxx, maxy]
-            )
-    print(f"{input_file} 已经裁切完成")
 
 
 
+    img_gdal = gdal.Open(image_path)
+    img_bit = img_gdal.GetRasterBand(1).DataType
+
+    img_basename = os.path.basename(image_path).split('.')[0] #nangangqu.tif
+    
+    # 对图像进行裁切,分为8000*8000的地方和512*512的地方
+    image_gdal = gdal.Open(image_path)
+    img = image_gdal.ReadAsArray()
+    img = img.transpose((1,2,0))
+
+    h, w, c = img.shape
+    rows, cols, bands = img.shape
+
+    if h < crop_size or w < crop_size:
+        print(f'--- 当前 {img_basename} 图像尺寸小于 {crop_size}，不进行裁切')
+
+        out_path = os.path.join(save_path, os.path.basename(image_path))
+        Driver = gdal.GetDriverByName("Gtiff")
+        new_img = Driver.Create(out_path, w,h,c, img_bit)
+        for band_num in range(bands):
+            band = new_img.GetRasterBand(band_num+1)
+            band.WriteArray(img[:, :, band_num])
+        return None
+    
+    else:
+    
+        hang = h - (h//crop_size)*crop_size
+        lie =  w - (w//crop_size)*crop_size
+        print(f'图像尺寸：{img.shape}')
+        print(f'可裁成{h//crop_size+1}行...{hang}')
+        print(f'可裁成{w//crop_size+1}列...{lie}')
+        print(f'共{crop_size}：{((h//crop_size+1)*(w//crop_size+1))+1}张')
+
+        # 8000的部分 xxxxx._0_0_8000.tif
+        for i in range(h//crop_size):
+            for j in range(w//crop_size):
+                out_path = os.path.join(save_path, img_basename+'_'+str(i)+'_'+str(j)+'_'+str(crop_size)+'.tif')
+                Driver = gdal.GetDriverByName("Gtiff")
+
+                new_512 = np.zeros((crop_size,crop_size, c),dtype=np.uint8)
+                new_img = Driver.Create(out_path, crop_size, crop_size, c, img_bit)
+            
+                new_512 = img[i*crop_size:i*crop_size+crop_size,j*crop_size:j*crop_size+crop_size,:]   #横着来       
+
+                for band_num in range(bands):
+                    band = new_img.GetRasterBand(band_num + 1)
+                    band.WriteArray(new_512[:, :, band_num])
+
+        #以外的部分
+
+        # 下边的 xxxxx._xia_0_8000.tif
+        for j in range(w//crop_size):
+            new_512 = np.zeros((crop_size,crop_size, c),dtype=np.uint8)
+            new_512 = img[h-crop_size:h, j*crop_size:j*crop_size+crop_size, :]   #横着来
+            
+            out_path = os.path.join(save_path, img_basename+'_'+str('xia')+'_'+str(j)+'_'+str(crop_size)+'.tif')
+            # cv2.imwrite(out_path,new_512)
+            Driver = gdal.GetDriverByName("Gtiff")
+            new_img = Driver.Create(out_path, crop_size,crop_size, c, img_bit)
+            for band_num in range(bands):
+                band = new_img.GetRasterBand(band_num+1)
+                band.WriteArray(new_512[:, :, band_num])
+
+        #右边的 xxxxx._you_0_8000.tif
+        for j in range(h//crop_size):
+            new_512 = np.zeros((crop_size,crop_size, c),dtype=np.uint8)
+            new_512 = img[j*crop_size:j*crop_size+crop_size, w-crop_size:w, :]   #横着来
+            
+            out_path = os.path.join(save_path,img_basename+'_'+str('you')+'_'+str(j)+'_'+str(crop_size)+'.tif')
+            # cv2.imwrite(out_path,new_512)
+            Driver = gdal.GetDriverByName("Gtiff")
+            new_img = Driver.Create(out_path, crop_size,crop_size, c, img_bit)
+            for band_num in range(bands):
+                band = new_img.GetRasterBand(band_num+1)
+                band.WriteArray(new_512[:, :, band_num])
+
+        #右下角的
+        new_512 = np.zeros((crop_size,crop_size, c),dtype=np.uint8)
+        new_512 = img[h-crop_size:h, w-crop_size:w, :]   #横着来
+        out_path = os.path.join(save_path, img_basename+'_'+str('youxia')+'_'+str(crop_size)+'.tif')
+        # cv2.imwrite(out_path,new_512)
+        Driver = gdal.GetDriverByName("Gtiff")
+        new_img = Driver.Create(out_path, crop_size,crop_size, c, img_bit)
+        for band_num in range(bands):
+            band = new_img.GetRasterBand(band_num+1)
+            band.WriteArray(new_512[:, :, band_num])
+
+    print(f'--- 当前 {img_basename} 图像裁切完成')
+
+
```

### Comparing `atl_tools-1.1.6/ATL_Tools/ATL_path.py` & `atl_tools-1.1.7/ATL_Tools/ATL_path.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.1.6/ATL_Tools/__init__.py` & `atl_tools-1.1.7/ATL_Tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
             raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
             crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
             crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
             Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
             resample_image,      # ✔使用GDAL对图像进行重采样
             shp_to_geojson,      # ✔将shp文件转为geojson文件
-            cut_image_with_overlap, # 将大图裁切为小图，支持重叠
+            clip_big_image, # 将大图裁切为小图，支持重叠
         )
 
 ---
 示例程序：
 ----       
 示例1-根据json批量裁切影像根据矢量批量裁切影像
```

### Comparing `atl_tools-1.1.6/ATL_Tools.egg-info/PKG-INFO` & `atl_tools-1.1.7/ATL_Tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.6
+Version: 1.1.7
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 最新版本 v1.1.6
@@ -91,7 +91,8 @@
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
 - 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
 - 2024-05-20 v1.1.6 ATL_gdal 中 增加 `cut_image_with_overlap()`支持将大图裁切成指定尺寸的小图，并带有坐标。
+- 2024-05-28 v1.1.7 ATL_gdal 中 修改 v1.1.6 中新增函数 为`clip_big_image()`。ATL_gdal中`crop_tif_with_json_zero()`和`crop_tif_with_json_nan()`支持传入参数 `img_path(str)` 或 `img_path(gdal.Dataset)`。
```

### Comparing `atl_tools-1.1.6/PKG-INFO` & `atl_tools-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.6
+Version: 1.1.7
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 最新版本 v1.1.6
@@ -91,7 +91,8 @@
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
 - 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
 - 2024-05-20 v1.1.6 ATL_gdal 中 增加 `cut_image_with_overlap()`支持将大图裁切成指定尺寸的小图，并带有坐标。
+- 2024-05-28 v1.1.7 ATL_gdal 中 修改 v1.1.6 中新增函数 为`clip_big_image()`。ATL_gdal中`crop_tif_with_json_zero()`和`crop_tif_with_json_nan()`支持传入参数 `img_path(str)` 或 `img_path(gdal.Dataset)`。
```

### Comparing `atl_tools-1.1.6/README.md` & `atl_tools-1.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,8 +82,9 @@
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
 - 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
-- 2024-05-20 v1.1.6 ATL_gdal 中 增加 `cut_image_with_overlap()`支持将大图裁切成指定尺寸的小图，并带有坐标。
+- 2024-05-20 v1.1.6 ATL_gdal 中 增加 `cut_image_with_overlap()`支持将大图裁切成指定尺寸的小图，并带有坐标。
+- 2024-05-28 v1.1.7 ATL_gdal 中 修改 v1.1.6 中新增函数 为`clip_big_image()`。ATL_gdal中`crop_tif_with_json_zero()`和`crop_tif_with_json_nan()`支持传入参数 `img_path(str)` 或 `img_path(gdal.Dataset)`。
```

