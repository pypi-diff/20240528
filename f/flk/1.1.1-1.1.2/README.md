# Comparing `tmp/flk-1.1.1.tar.gz` & `tmp/flk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flk-1.1.1.tar", last modified: Mon May 27 11:32:54 2024, max compression
+gzip compressed data, was "flk-1.1.2.tar", last modified: Tue May 28 17:05:03 2024, max compression
```

## Comparing `flk-1.1.1.tar` & `flk-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 11:32:54.281546 flk-1.1.1/
--rw-rw-rw-   0        0        0    11558 2024-05-20 16:14:53.000000 flk-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4733 2024-05-27 11:32:54.280549 flk-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4368 2024-05-27 11:30:06.000000 flk-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 11:32:54.258561 flk-1.1.1/flk/
--rw-rw-rw-   0        0        0       31 2024-05-21 08:15:15.000000 flk-1.1.1/flk/__init__.py
--rw-rw-rw-   0        0        0     1199 2024-05-21 08:11:02.000000 flk-1.1.1/flk/__main__.py
--rw-rw-rw-   0        0        0    16958 2024-05-27 11:27:54.000000 flk-1.1.1/flk/parser.py
--rw-rw-rw-   0        0        0     1919 2024-05-24 10:32:33.000000 flk-1.1.1/flk/variable.py
-drwxrwxrwx   0        0        0        0 2024-05-27 11:32:54.278550 flk-1.1.1/flk.egg-info/
--rw-rw-rw-   0        0        0     4733 2024-05-27 11:32:53.000000 flk-1.1.1/flk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-05-27 11:32:54.000000 flk-1.1.1/flk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 11:32:53.000000 flk-1.1.1/flk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-27 11:32:54.000000 flk-1.1.1/flk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 11:32:54.282543 flk-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      576 2024-05-27 11:32:52.000000 flk-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:05:03.068797 flk-1.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-20 16:14:53.000000 flk-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4733 2024-05-28 17:05:03.067781 flk-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4368 2024-05-27 11:30:06.000000 flk-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 17:05:03.050118 flk-1.1.2/flk/
+-rw-rw-rw-   0        0        0       31 2024-05-21 08:15:15.000000 flk-1.1.2/flk/__init__.py
+-rw-rw-rw-   0        0        0     1199 2024-05-21 08:11:02.000000 flk-1.1.2/flk/__main__.py
+-rw-rw-rw-   0        0        0    16638 2024-05-28 16:58:25.000000 flk-1.1.2/flk/parser.py
+-rw-rw-rw-   0        0        0     1919 2024-05-24 10:32:33.000000 flk-1.1.2/flk/variable.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:05:03.065271 flk-1.1.2/flk.egg-info/
+-rw-rw-rw-   0        0        0     4733 2024-05-28 17:05:02.000000 flk-1.1.2/flk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-05-28 17:05:02.000000 flk-1.1.2/flk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 17:05:02.000000 flk-1.1.2/flk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-28 17:05:02.000000 flk-1.1.2/flk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 17:05:03.069794 flk-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      576 2024-05-28 16:59:17.000000 flk-1.1.2/setup.py
```

### Comparing `flk-1.1.1/LICENSE` & `flk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flk-1.1.1/PKG-INFO` & `flk-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flk
-Version: 1.1.1
+Version: 1.1.2
 Summary: FLK - это библиотека для парсинга и работы с файлами в формате FL (File Language).
 Home-page: https://github.com/FlacSy/flk
 Author: FlacSy
 Author-email: flacsy.tw@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flk-1.1.1/README.md` & `flk-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flk-1.1.1/flk/__main__.py` & `flk-1.1.2/flk/__main__.py`

 * *Files identical despite different names*

### Comparing `flk-1.1.1/flk/parser.py` & `flk-1.1.2/flk/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         Параметры:
             value (str): Строка, представляющая словарь.
 
         Возврат:
             dict: Словарь спарсенных значений.
         """
         result = {}
-        # Удаление пробелов и переносов строк для упрощения парсинга
+        
         lines = re.sub(r'\s+', ' ', value.strip('{}')).split(',')
         for line in lines:
             line = line.strip()
             if line:
                 match = re.match(r'(\w+)\((\w+)\) *: *(\w+)\((\w+)\) *= *(.+)', line)
                 if match:
                     key, key_type, var_type, val_type, val = match.groups()
@@ -207,16 +207,16 @@
         for token in tokens:
             if token.startswith('$'):
                 result.append(str(self.parse_reference(token[1:])))
             elif token in self.constants:
                 result.append(str(self.constants[token]))
             else:
                 result.append(token)
-        # Используем eval для вычисления выражения и возвращаем результат
-        return eval(''.join(result))
+
+        return round(eval(''.join(result)), 5)
 
     def parse_line(self, line: str) -> None:
         line = line.split("//")[0].strip()
         if '{' in line:
             match = re.match(r'(\w+)\((\w+)\) = ({.*})', line, re.DOTALL)
             if match:
                 name, var_type, value = match.groups()
@@ -225,17 +225,17 @@
                 raise ValueError(f"Неправильный формат строки: {line}")
         else:
             match = re.match(r'(\w+)\((\w+)\) = (.+)', line)
             if match:
                 name, var_type, value = match.groups()
                 if name in self.data and self.data[name].get_type() != var_type:
                     raise TypeError(f"Переменная '{name}' уже определена с типом '{self.data[name].get_type()}'.")
-                if any(op in value for op in "+-*/%"):  # арифметическое выражение
+                if any(op in value for op in "+-*/%"):
                     parsed_value = self.evaluate_expression(value)
-                elif value.strip().startswith("$"):  # логическое выражение
+                elif value.strip().startswith("$"):
                     parsed_value = self.parse_logical_expression(value)
                 else:
                     parsed_value = self.parse_value(var_type, value.strip())
             else:
                 raise ValueError(f"Неправильный формат строки: {line}")
 
         if name in self.data:
```

### Comparing `flk-1.1.1/flk/variable.py` & `flk-1.1.2/flk/variable.py`

 * *Files identical despite different names*

### Comparing `flk-1.1.1/flk.egg-info/PKG-INFO` & `flk-1.1.2/flk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flk
-Version: 1.1.1
+Version: 1.1.2
 Summary: FLK - это библиотека для парсинга и работы с файлами в формате FL (File Language).
 Home-page: https://github.com/FlacSy/flk
 Author: FlacSy
 Author-email: flacsy.tw@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flk-1.1.1/setup.py` & `flk-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='flk',
-    version='1.1.1',
+    version='1.1.2',
     description='FLK - это библиотека для парсинга и работы с файлами в формате FL (File Language).',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     author='FlacSy',
     author_email='flacsy.tw@gmail.com',
     packages=find_packages(),
```

