# Comparing `tmp/nb_libs-1.1.tar.gz` & `tmp/nb_libs-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_libs-1.1.tar", last modified: Sat May 25 15:08:46 2024, max compression
+gzip compressed data, was "dist\nb_libs-1.2.tar", last modified: Tue May 28 06:33:22 2024, max compression
```

## Comparing `nb_libs-1.1.tar` & `nb_libs-1.2.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 15:08:46.255695 nb_libs-1.1/
--rw-rw-rw-   0        0        0       41 2024-05-24 14:51:14.000000 nb_libs-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      995 2024-05-25 15:08:46.253690 nb_libs-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-05-24 14:51:14.000000 nb_libs-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 15:08:46.180666 nb_libs-1.1/nb_libs/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/__init__.py
--rw-rw-rw-   0        0        0     3106 2024-04-09 14:11:27.000000 nb_libs-1.1/nb_libs/auto_git.py
--rw-rw-rw-   0        0        0     2041 2024-04-09 14:11:27.000000 nb_libs-1.1/nb_libs/code_line_statistics.py
--rw-rw-rw-   0        0        0      362 2023-10-22 05:45:27.000000 nb_libs-1.1/nb_libs/dict2json.py
--rw-rw-rw-   0        0        0      490 2023-10-22 05:47:50.000000 nb_libs-1.1/nb_libs/global_dict.py
--rw-rw-rw-   0        0        0      487 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/lazy_importer.py
--rw-rw-rw-   0        0        0     1650 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/markdown2pdf.py
--rw-rw-rw-   0        0        0     3186 2024-05-24 19:36:58.000000 nb_libs-1.1/nb_libs/memory_leak_analysis.py
--rw-rw-rw-   0        0        0       21 2024-04-09 14:11:27.000000 nb_libs-1.1/nb_libs/nb_time.py
--rw-rw-rw-   0        0        0     3311 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/path_helper.py
--rw-rw-rw-   0        0        0     3527 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/pydantic_helper.py
--rw-rw-rw-   0        0        0     1418 2023-10-22 05:28:25.000000 nb_libs-1.1/nb_libs/restart_programe_by_interval.py
--rw-rw-rw-   0        0        0     1605 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/sys_frame_uitils.py
-drwxrwxrwx   0        0        0        0 2024-05-25 15:08:46.202679 nb_libs-1.1/nb_libs.egg-info/
--rw-rw-rw-   0        0        0      995 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      656 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 15:08:46.255695 nb_libs-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1821 2024-05-25 14:55:30.000000 nb_libs-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 15:08:46.247691 nb_libs-1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-05-24 18:29:31.000000 nb_libs-1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      760 2024-05-24 19:32:57.000000 nb_libs-1.1/tests/t_mem_leak.py
--rw-rw-rw-   0        0        0      225 2024-05-24 18:55:50.000000 nb_libs-1.1/tests/t_mem_leak2.py
--rw-rw-rw-   0        0        0      379 2023-10-22 05:28:25.000000 nb_libs-1.1/tests/test_restart_programe_by_interval.py
--rw-rw-rw-   0        0        0      128 2024-05-24 14:51:14.000000 nb_libs-1.1/tests/testai.py
--rw-rw-rw-   0        0        0      934 2024-04-09 14:11:27.000000 nb_libs-1.1/tests/tests_time.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:33:22.000000 nb_libs-1.2/
+-rw-rw-rw-   0        0        0       41 2024-04-18 02:51:35.000000 nb_libs-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      995 2024-05-28 06:33:22.000000 nb_libs-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-04-18 03:00:48.000000 nb_libs-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 06:33:21.000000 nb_libs-1.2/nb_libs/
+-rw-rw-rw-   0        0        0        0 2024-04-18 02:55:05.000000 nb_libs-1.2/nb_libs/__init__.py
+-rw-rw-rw-   0        0        0     3106 2023-11-17 02:18:55.000000 nb_libs-1.2/nb_libs/auto_git.py
+-rw-rw-rw-   0        0        0     2041 2024-01-02 03:07:27.000000 nb_libs-1.2/nb_libs/code_line_statistics.py
+-rw-rw-rw-   0        0        0      362 2023-10-23 03:14:12.000000 nb_libs-1.2/nb_libs/dict2json.py
+-rw-rw-rw-   0        0        0     2624 2024-05-28 03:59:56.000000 nb_libs-1.2/nb_libs/github_git_clone.py
+-rw-rw-rw-   0        0        0      490 2023-10-23 03:14:12.000000 nb_libs-1.2/nb_libs/global_dict.py
+-rw-rw-rw-   0        0        0      487 2024-04-16 03:39:38.000000 nb_libs-1.2/nb_libs/lazy_importer.py
+-rw-rw-rw-   0        0        0     1650 2024-04-22 09:48:53.000000 nb_libs-1.2/nb_libs/markdown2pdf.py
+-rw-rw-rw-   0        0        0     3192 2024-05-27 07:41:18.000000 nb_libs-1.2/nb_libs/memory_leak_analysis.py
+-rw-rw-rw-   0        0        0       21 2024-03-20 10:00:54.000000 nb_libs-1.2/nb_libs/nb_time.py
+-rw-rw-rw-   0        0        0     3311 2024-04-19 01:40:21.000000 nb_libs-1.2/nb_libs/path_helper.py
+-rw-rw-rw-   0        0        0     3828 2024-04-23 10:58:03.000000 nb_libs-1.2/nb_libs/pydantic_helper.py
+-rw-rw-rw-   0        0        0     2156 2024-05-08 06:23:47.000000 nb_libs-1.2/nb_libs/redis_key.py
+-rw-rw-rw-   0        0        0     1418 2023-03-15 02:37:59.000000 nb_libs-1.2/nb_libs/restart_programe_by_interval.py
+-rw-rw-rw-   0        0        0     1662 2024-05-28 06:32:52.000000 nb_libs-1.2/nb_libs/sys_frame_uitils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:33:21.000000 nb_libs-1.2/nb_libs.egg-info/
+-rw-rw-rw-   0        0        0      995 2024-05-28 06:33:20.000000 nb_libs-1.2/nb_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      724 2024-05-28 06:33:21.000000 nb_libs-1.2/nb_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 06:33:20.000000 nb_libs-1.2/nb_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-28 06:33:20.000000 nb_libs-1.2/nb_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 06:33:20.000000 nb_libs-1.2/nb_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 06:33:22.000000 nb_libs-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1821 2024-05-28 06:32:52.000000 nb_libs-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:33:22.000000 nb_libs-1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-27 07:41:18.000000 nb_libs-1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      742 2024-05-27 07:41:18.000000 nb_libs-1.2/tests/t_mem_leak.py
+-rw-rw-rw-   0        0        0      303 2024-05-27 07:41:18.000000 nb_libs-1.2/tests/t_mem_leak2.py
+-rw-rw-rw-   0        0        0      379 2023-03-15 02:57:54.000000 nb_libs-1.2/tests/test_restart_programe_by_interval.py
+-rw-rw-rw-   0        0        0      136 2024-05-08 03:44:54.000000 nb_libs-1.2/tests/test_sifn.py
+-rw-rw-rw-   0        0        0      128 2024-04-22 07:16:53.000000 nb_libs-1.2/tests/testai.py
+-rw-rw-rw-   0        0        0      934 2024-02-29 11:16:03.000000 nb_libs-1.2/tests/tests_time.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nb_libs-1.1/PKG-INFO` & `nb_libs-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_libs
-Version: 1.1
+Version: 1.2
 Summary: nb_libs 不想分开分发很多个不同功能单独的包,各种小功能杂项放在一起,具体功能看代码.
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_libs-1.1/nb_libs/auto_git.py` & `nb_libs-1.2/nb_libs/auto_git.py`

 * *Files identical despite different names*

### Comparing `nb_libs-1.1/nb_libs/code_line_statistics.py` & `nb_libs-1.2/nb_libs/code_line_statistics.py`

 * *Files identical despite different names*

### Comparing `nb_libs-1.1/nb_libs/markdown2pdf.py` & `nb_libs-1.2/nb_libs/markdown2pdf.py`

 * *Files identical despite different names*

### Comparing `nb_libs-1.1/nb_libs/memory_leak_analysis.py` & `nb_libs-1.2/nb_libs/memory_leak_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,20 +64,20 @@
                         max_size_obj = obj
 
 
             type__max_size_map[typex] = {f'{self.mla_flag}max_len': max_len, f'{self.mla_flag}max_str_len': max_str_len,f'{self.mla_flag}max_size': max_size}
             type__max_obj_map[typex] = {f'{self.mla_flag}max_len_obj':max_len_obj,f'{self.mla_flag}max_str_len_obj':max_str_len_obj,f'{self.mla_flag}max_size_obj':max_size_obj}
 
         # self.logger.debug(type__max_size_map)
-        self.logger.debug(self._dict_sort(type__max_size_map,f'{self.mla_flag}max_size'))
+        # self.logger.debug(self._dict_sort(type__max_size_map,f'{self.mla_flag}max_size'))
         # self.logger.debug(self._dict_sort(type__max_size_map, f'{self.mla_flag}max_str_len_obj')['__name__'])
-        self.logger.debug(type__max_obj_map['dict'][f'{self.mla_flag}max_str_len_obj'])
-        # for ref in gc.get_referrers(type__max_obj_map['dict'][f'{self.mla_flag}max_size_obj']):
-        #     if self.mla_flag not in str(ref):
-        #         self.logger.debug(ref)
+        self.logger.debug(type__max_obj_map['dict'][f'{self.mla_flag}max_str_len_obj'].keys())
+        for ref in gc.get_referrers(type__max_obj_map['dict'][f'{self.mla_flag}max_str_len_obj']):
+            if self.mla_flag not in str(ref):
+                self.logger.debug(ref)
 
 
     def start(self):
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `nb_libs-1.1/nb_libs/path_helper.py` & `nb_libs-1.2/nb_libs/path_helper.py`

 * *Files identical despite different names*

### Comparing `nb_libs-1.1/nb_libs/pydantic_helper.py` & `nb_libs-1.2/nb_libs/pydantic_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,24 @@
                 setattr(model, k, v)
         return model
 
     def __str__(self):
         str1 =  self.__repr_str__(' ')
         return f'<{self.__class__.__name__} id:{id(self)} [{str1}]>'
 
+    @staticmethod
+    def init_by_another_model(model_type:typing.Type[BaseModel],modelx:BaseModel):
+        init_dict = {}
+        for k,v in modelx.dict().items():
+            if k in model_type.__fields__.keys():
+                init_dict[k] = v
+        return model_type(**init_dict)
+
+
+
 
 
 if __name__ == '__main__':
     import nb_log
 
 
     class Model1(BaseJsonAbleModel):
```

### Comparing `nb_libs-1.1/nb_libs/restart_programe_by_interval.py` & `nb_libs-1.2/nb_libs/restart_programe_by_interval.py`

 * *Files identical despite different names*

### Comparing `nb_libs-1.1/nb_libs/sys_frame_uitils.py` & `nb_libs-1.2/nb_libs/sys_frame_uitils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import inspect
 import sys
 
+'''
+此模块不要导入nb_log,避免互相引用
+'''
 
 def get_current_fun_name():
     """
     获取代码所在函数或方法的名字
     :return:
     """
     method_name = inspect.getframeinfo(inspect.currentframe().f_back).function  # 也可以 sys._getframe(0).f_code.co_name
@@ -43,15 +46,15 @@
         print(sys._getframe(1).f_code.co_filename)  # 文件
         print(sys._getframe(1).f_code.co_name)  # 函数
         print(sys._getframe(0).f_code.co_name)  # 函数
         print(dir(sys._getframe(1)))
         print(sys._getframe(1).f_lineno)  # 行
         print(sys._getframe(0).f_back.f_lineno)
 
-        ef = EasyFrame(0)
+        ef = EasyFrame()
         print(ef.filename, ef.lineno, ef.func_name, ef.get_jump_line(next_line=True))
 
         ef = EasyFrame(1)
         print(ef.filename, ef.lineno, ef.func_name, ef.get_jump_line(next_line=True))
 
 
     get_a()
```

### Comparing `nb_libs-1.1/nb_libs.egg-info/PKG-INFO` & `nb_libs-1.2/nb_libs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-libs
-Version: 1.1
+Version: 1.2
 Summary: nb_libs 不想分开分发很多个不同功能单独的包,各种小功能杂项放在一起,具体功能看代码.
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_libs-1.1/nb_libs.egg-info/SOURCES.txt` & `nb_libs-1.2/nb_libs.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 MANIFEST.in
 README.md
 setup.py
 nb_libs/__init__.py
 nb_libs/auto_git.py
 nb_libs/code_line_statistics.py
 nb_libs/dict2json.py
+nb_libs/github_git_clone.py
 nb_libs/global_dict.py
 nb_libs/lazy_importer.py
 nb_libs/markdown2pdf.py
 nb_libs/memory_leak_analysis.py
 nb_libs/nb_time.py
 nb_libs/path_helper.py
 nb_libs/pydantic_helper.py
+nb_libs/redis_key.py
 nb_libs/restart_programe_by_interval.py
 nb_libs/sys_frame_uitils.py
 nb_libs.egg-info/PKG-INFO
 nb_libs.egg-info/SOURCES.txt
 nb_libs.egg-info/dependency_links.txt
 nb_libs.egg-info/requires.txt
 nb_libs.egg-info/top_level.txt
 tests/__init__.py
 tests/t_mem_leak.py
 tests/t_mem_leak2.py
 tests/test_restart_programe_by_interval.py
+tests/test_sifn.py
 tests/testai.py
 tests/tests_time.py
```

### Comparing `nb_libs-1.1/setup.py` & `nb_libs-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 setup(
     name='nb_libs',  #
-    version="1.1",
+    version="1.2",
     description=('nb_libs 不想分开分发很多个不同功能单独的包,各种小功能杂项放在一起,具体功能看代码.'),
     keywords=["nb_libs",],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
     # data_files=[filepath],
     author='bfzs',
```

### Comparing `nb_libs-1.1/tests/t_mem_leak.py` & `nb_libs-1.2/tests/t_mem_leak.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pymysql
 
 
 import logging
 import win32con
 from nb_libs.memory_leak_analysis import MemoryLeakAnalysis
-from tests.t_mem_leak2 import long_list,long_dict
+from tests.t_mem_leak2 import a
 
 logging.captureWarnings(True)
 
 logging.getLogger().setLevel(logging.ERROR)
 
 # gc.set_debug(1)
```

### Comparing `nb_libs-1.1/tests/tests_time.py` & `nb_libs-1.2/tests/tests_time.py`

 * *Files identical despite different names*

