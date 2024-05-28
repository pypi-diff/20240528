# Comparing `tmp/movoid_robotframework-1.4.8.tar.gz` & `tmp/movoid_robotframework-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework-1.4.8.tar", last modified: Fri May 10 20:23:08 2024, max compression
+gzip compressed data, was "movoid_robotframework-1.4.9.tar", last modified: Thu May 16 16:34:23 2024, max compression
```

## Comparing `movoid_robotframework-1.4.8.tar` & `movoid_robotframework-1.4.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 20:23:08.847076 movoid_robotframework-1.4.8/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2024-05-10 20:23:08.846077 movoid_robotframework-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 20:23:08.833090 movoid_robotframework-1.4.8/RobotFrameworkBasic/
--rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:23:08.837077 movoid_robotframework-1.4.8/RobotFrameworkBasic/action/
--rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/action/__init__.py
--rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/action/calculate.py
--rw-rw-rw-   0        0        0     9917 2024-05-10 20:17:13.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/action/config.py
--rw-rw-rw-   0        0        0     8155 2024-05-10 20:17:13.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/common.py
--rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/decorator.py
--rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/error.py
--rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/main.py
--rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/version.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:23:08.845050 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/
--rw-rw-rw-   0        0        0      290 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 20:23:08.847076 movoid_robotframework-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-05-10 20:22:31.000000 movoid_robotframework-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:34:23.525874 movoid_robotframework-1.4.9/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2024-05-16 16:34:23.524866 movoid_robotframework-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:34:23.513416 movoid_robotframework-1.4.9/RobotFrameworkBasic/
+-rw-rw-rw-   0        0        0      470 2024-05-16 16:33:18.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:34:23.517646 movoid_robotframework-1.4.9/RobotFrameworkBasic/action/
+-rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/action/__init__.py
+-rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/action/calculate.py
+-rw-rw-rw-   0        0        0     9945 2024-05-16 16:33:18.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/action/config.py
+-rw-rw-rw-   0        0        0     8155 2024-05-10 20:17:13.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/common.py
+-rw-rw-rw-   0        0        0    20079 2024-05-16 16:33:18.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/decorator.py
+-rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/error.py
+-rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/main.py
+-rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.9/RobotFrameworkBasic/version.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:34:23.523864 movoid_robotframework-1.4.9/movoid_robotframework.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-05-16 16:34:23.000000 movoid_robotframework-1.4.9/movoid_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-16 16:34:23.000000 movoid_robotframework-1.4.9/movoid_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:34:23.000000 movoid_robotframework-1.4.9/movoid_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-16 16:34:23.000000 movoid_robotframework-1.4.9/movoid_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-16 16:34:23.000000 movoid_robotframework-1.4.9/movoid_robotframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:34:23.525874 movoid_robotframework-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      558 2024-05-16 16:33:59.000000 movoid_robotframework-1.4.9/setup.py
```

### Comparing `movoid_robotframework-1.4.8/RobotFrameworkBasic/action/calculate.py` & `movoid_robotframework-1.4.9/RobotFrameworkBasic/action/calculate.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.8/RobotFrameworkBasic/action/config.py` & `movoid_robotframework-1.4.9/RobotFrameworkBasic/action/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
     @robot_log_keyword
     def config_init(self, json_file: str = None):
         """
         初始化json文件，相当于重新选择json文件并读取生效
         :param json_file: json文件的路径，可以绝对可以相对，没有该文件的情况下保存会新建一个
         """
         self.config.init(json_file)
+        return self.config
 
     @robot_log_keyword
     def config_use_label(self, *labels: str, override: bool = True, clear: bool = False):
         """
         选择相应的label生效
         :param labels: 待选择的label，必须是json文件里的
         :param override: 如果某个key已经存在，那么新数据是否覆盖就数据，默认覆盖
```

### Comparing `movoid_robotframework-1.4.8/RobotFrameworkBasic/common.py` & `movoid_robotframework-1.4.9/RobotFrameworkBasic/common.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.8/RobotFrameworkBasic/decorator.py` & `movoid_robotframework-1.4.9/RobotFrameworkBasic/decorator.py`

 * *Files 19% similar despite different names*

```diff
@@ -208,14 +208,111 @@
                     return False
 
         return wrapper
 
     return dec
 
 
+def wait_until_stable(check_function, timeout=30, init_check=True, init_check_function=None, init_sleep=0, stable_time=3, check_interval=0.2, error=True):
+    """
+    通过操作某个函数，达成某个最终的目的。如果检查未通过，那么会循环进行操作
+    这是一个装饰器，需要套在一个空函数上（仅函数名会被继承）
+        当然了，你也可以套在一个有价值的函数上，但是这个函数的所有痕迹都会被抹除
+    :param check_function:检查函数，返回值必须是一个bool值，或者返回值会被强制转换为bool
+    :param timeout:限时。只有在这个时长范围内一直通过，才算成功.
+    :param init_check:是否进行初始检查，如果为True，那j么会在操作前进行检查，如果通过，那么会跳过操作，直接结束
+    :param init_check_function:初始检查函数，返回值必须是一个bool值，或者返回值会被强制转换为bool，如果存在。那么初始检查会考虑使用这个。这个函数的参数必须和check_function完全一致，否则会报错
+    :param init_sleep:初始的等待时间，在初始检查前进行的等待，不计入整体timeout时间，一般配合初始检查init_check=True使用
+    :param stable_time:需要达到的稳定状态的持续时间，只有一直判定正确超过这个时间，才能算过
+    :param check_interval:连续两次检查之间的时间间隔，默认值为0.2，如果想要进行更细致的循环检查，可以将这个数值设置得更小
+    :param error:当检查失败后，是否raise一个error。默认为True，会raise。
+    :return: 返回是否判定成功，但是当error=True时，失败了会raise AssertionError，那也就不会有返回值了
+    """
+    _timeout = 3 if timeout is None else float(timeout)  # type:float
+    _init_check = True if init_check is None else bool(init_check)  # type:bool
+    init_check_function = check_function if init_check_function is None else init_check_function
+    _init_sleep = 0 if init_sleep is None else float(init_sleep)  # type:float
+    _stable_time = 3 if stable_time is None else float(stable_time)  # type:float
+    _check_interval = 0.2 if check_interval is None else float(check_interval)  # type:float
+    _error = True if error is None else bool(error)  # type:bool
+
+    def dec(func):
+        @wraps_func(func, check_function)
+        def wrapper(self,
+                    do_kwargs,
+                    check_kwargs,
+                    timeout=_timeout,  # noqa
+                    init_check=_init_check,  # noqa
+                    init_sleep=_init_sleep,  # noqa
+                    stable_time=_stable_time,  # noqa
+                    check_interval=_check_interval,  # noqa
+                    error=_error):  # noqa
+            fail_print = []
+            check_text = f'check {check_function.__name__}{check_kwargs}'
+            if init_check:
+                try:
+                    check_bool = init_check_function(**check_kwargs)
+                    if check_bool:
+                        print_text = f'init {check_text} pass.'
+                    else:
+                        print_text = f'init {check_text} fail.'
+                    self.print(print_text)
+                except Exception as err:
+                    print_text = f'init {check_text} error:{err}'
+                    self.print(print_text)
+                    fail_print.append(print_text + '\n' + traceback.format_exc())
+            time.sleep(init_sleep)
+            total_time = 0
+            start_time_point = time.time()
+            loop_time = 0
+            pass_time = 0
+            while total_time < timeout:
+                total_interval_time_point = time.time()
+                loop_time += 1
+                try:
+                    check_bool = check_function(**check_kwargs)
+                    if check_bool:
+                        print_text = '{:.3f} second {} time {} pass.'.format(time.time() - start_time_point, loop_time, check_text)
+                        if pass_time == 0:
+                            pass_time = time.time()
+                            now_stable_time = 0
+                        else:
+                            now_stable_time = time.time() - pass_time
+                        print_text += ' it has been stable for {:.3f} seconds.'.format(now_stable_time)
+                        self.print(print_text)
+                        if now_stable_time > stable_time:
+                            return True
+                    else:
+                        print_text = '{:.3f} second {} time {} fail.'.format(time.time() - start_time_point, loop_time, check_text)
+                        pass_time = 0
+                        self.print(print_text)
+                except Exception as err:
+                    print_text = '{:.3f} second {} time {} error:{}'.format(time.time() - start_time_point, loop_time, check_text, err)
+                    self.print(print_text)
+                    fail_print.append(print_text + '\n' + traceback.format_exc())
+                    pass_time = 0
+                total_interval_time = time.time() - total_interval_time_point
+                if total_interval_time < check_interval:
+                    time.sleep(check_interval - total_interval_time)
+                total_time = time.time() - start_time_point
+            else:
+                total_time = time.time() - start_time_point
+                print_text = '{:.3f} second {} time {} all fail/error.do_until_check fail.'.format(total_time, loop_time, check_text)
+                self.print(*fail_print, sep='\n')
+                if error:
+                    raise AssertionError(print_text)
+                else:
+                    self.print(print_text)
+                    return False
+
+        return wrapper
+
+    return dec
+
+
 def do_when_error(error_function):
     def dec(func):
         @wraps_func(func, error_function)
         def wrapper(kwargs, error_kwargs):
             try:
                 re_value = func(**kwargs)
             except Exception as err:
```

### Comparing `movoid_robotframework-1.4.8/RobotFrameworkBasic/version.py` & `movoid_robotframework-1.4.9/RobotFrameworkBasic/version.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.8/movoid_robotframework.egg-info/SOURCES.txt` & `movoid_robotframework-1.4.9/movoid_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.8/setup.py` & `movoid_robotframework-1.4.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework',
-    version='1.4.8',
+    version='1.4.9',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

