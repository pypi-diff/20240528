# Comparing `tmp/pyuptech-0.1.6.3.tar.gz` & `tmp/pyuptech-0.1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.6.3.tar", last modified: Sun May 26 11:39:02 2024, max compression
+gzip compressed data, was "pyuptech-0.1.6.4.tar", last modified: Tue May 28 02:24:01 2024, max compression
```

## Comparing `pyuptech-0.1.6.3.tar` & `pyuptech-0.1.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     8813 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/README.md
--rw-r--r--   0        0        0      547 2024-05-26 11:39:02.549803 pyuptech-0.1.6.3/pyproject.toml
--rw-r--r--   0        0        0     1182 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/__init__.py
--rw-r--r--   0        0        0   219512 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/lib/libuptech.so
--rw-r--r--   0        0        0      190 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1976 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/modules/emulation.py
--rw-r--r--   0        0        0     1007 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1761 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    14588 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0    13599 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     7316 2024-05-26 11:38:45.025703 pyuptech-0.1.6.3/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0      252 2024-05-26 11:38:45.029703 pyuptech-0.1.6.3/tests/__init__.py
--rw-r--r--   0        0        0     1189 2024-05-26 11:38:45.029703 pyuptech-0.1.6.3/tests/display_tests.py
--rw-r--r--   0        0        0     1036 2024-05-26 11:38:45.029703 pyuptech-0.1.6.3/tests/perf_tests.py
--rw-r--r--   0        0        0      208 2024-05-26 11:38:45.029703 pyuptech-0.1.6.3/tests/raw_test.py
--rw-r--r--   0        0        0     2480 2024-05-26 11:38:45.029703 pyuptech-0.1.6.3/tests/test_sensor.py
--rw-r--r--   0        0        0      424 2024-05-26 11:38:45.029703 pyuptech-0.1.6.3/tests/utils.py
--rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 pyuptech-0.1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     8813 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/README.md
+-rw-r--r--   0        0        0      547 2024-05-28 02:24:01.668554 pyuptech-0.1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1182 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      190 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     1976 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/modules/emulation.py
+-rw-r--r--   0        0        0     1007 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1761 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    17105 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0    13599 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     7316 2024-05-28 02:23:41.476265 pyuptech-0.1.6.4/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0      252 2024-05-28 02:23:41.480265 pyuptech-0.1.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     1189 2024-05-28 02:23:41.480265 pyuptech-0.1.6.4/tests/display_tests.py
+-rw-r--r--   0        0        0     1036 2024-05-28 02:23:41.480265 pyuptech-0.1.6.4/tests/perf_tests.py
+-rw-r--r--   0        0        0      208 2024-05-28 02:23:41.480265 pyuptech-0.1.6.4/tests/raw_test.py
+-rw-r--r--   0        0        0     2480 2024-05-28 02:23:41.480265 pyuptech-0.1.6.4/tests/test_sensor.py
+-rw-r--r--   0        0        0      424 2024-05-28 02:23:41.480265 pyuptech-0.1.6.4/tests/utils.py
+-rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 pyuptech-0.1.6.4/PKG-INFO
```

### Comparing `pyuptech-0.1.6.3/README.md` & `pyuptech-0.1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/pyproject.toml` & `pyuptech-0.1.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyuptech"
-version = "0.1.6.3"
+version = "0.1.6.4"
 description = "A Python wrapper for the uptech binary lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "terminaltables>=3.1.10",
```

### Comparing `pyuptech-0.1.6.3/src/pyuptech/__init__.py` & `pyuptech-0.1.6.4/src/pyuptech/__init__.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/src/pyuptech/lib/libuptech.so` & `pyuptech-0.1.6.4/src/pyuptech/lib/libuptech.so`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/src/pyuptech/modules/emulation.py` & `pyuptech-0.1.6.4/src/pyuptech/modules/emulation.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/src/pyuptech/modules/loader.py` & `pyuptech-0.1.6.4/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/src/pyuptech/modules/logger.py` & `pyuptech-0.1.6.4/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/src/pyuptech/modules/pins.py` & `pyuptech-0.1.6.4/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/src/pyuptech/modules/screen.py` & `pyuptech-0.1.6.4/src/pyuptech/modules/screen.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,33 @@
     """
 
     VERTICAL = 1
     HORIZONTAL = 2
 
     @property
     def width(self) -> int:
+        """
+        Returns the width of the screen based on the screen direction.
+
+        :return: An integer representing the width of the screen.
+        :rtype: int
+        """
         return {
             ScreenDirection.VERTICAL: 64,
             ScreenDirection.HORIZONTAL: 128,
         }[self]
+
     @property
     def height(self) -> int:
+        """
+        Returns the height of the screen based on the screen direction.
+
+        :return: An integer representing the height of the screen.
+        :rtype: int
+        """
         return {
             ScreenDirection.VERTICAL: 128,
             ScreenDirection.HORIZONTAL: 64,
         }[self]
 
 
 class FontSize(Enum):
@@ -46,15 +59,21 @@
     FONT_12X16 = 10
     FONT_12X20 = 11
     FONT_16X26 = 12
     FONT_22X36 = 13
     FONT_24X40 = 14
 
     @property
-    def row_height(self):
+    def row_height(self) -> int:
+        """
+        Returns the row height of the current font size.
+
+        :return: An integer representing the row height of the current font size.
+        :rtype: int
+        """
         return {
             FontSize.FONT_4X6: 6,
             FontSize.FONT_5X8: 8,
             FontSize.FONT_5X12: 12,
             FontSize.FONT_6X8: 8,
             FontSize.FONT_6X10: 10,
             FontSize.FONT_7X12: 12,
@@ -66,15 +85,21 @@
             FontSize.FONT_12X20: 20,
             FontSize.FONT_16X26: 26,
             FontSize.FONT_22X36: 36,
             FontSize.FONT_24X40: 40,
         }[self]
 
     @property
-    def column_width(self):
+    def column_width(self) -> int:
+        """
+        Returns the column width of the current font size.
+
+        :return: An integer representing the column width of the current font size.
+        :rtype: int
+        """
         return {
             FontSize.FONT_4X6: 4,
             FontSize.FONT_5X8: 5,
             FontSize.FONT_5X12: 5,
             FontSize.FONT_6X8: 6,
             FontSize.FONT_6X10: 6,
             FontSize.FONT_7X12: 7,
@@ -263,21 +288,81 @@
         Returns:
             Self: The instance of the class to allow for method chaining.
         """
         __lib__.adc_led_set(index, color)
         return self
 
     def set_led_0(self, color: Color | int) -> Self:
+        """
+        Set the color of LED 0.
+
+        Args:
+            color (Color | int): The color to set for LED 0.
+
+        Returns:
+            Self: The instance of the class to allow for method chaining.
+        """
         __lib__.adc_led_set(0, color)
         return self
 
     def set_led_1(self, color: Color | int) -> Self:
+        """
+        Set the color of LED 1.
+
+        Args:
+            color (Color | int): The color to set for LED 1.
+
+        Returns:
+            Self: The instance of the class to allow for method chaining.
+        """
+        __lib__.adc_led_set(1, color)
+        return self
+
+    def set_all_leds_same(self, color: Color | int) -> Self:
+        """
+        Sets the color of both LEDs to the same value.
+
+        Parameters:
+            color (Color | int): The color to set for both LEDs.
+
+        Returns:
+            Self: The instance of the class to allow for method chaining.
+        """
+        __lib__.adc_led_set(0, color)
         __lib__.adc_led_set(1, color)
         return self
 
+    def set_all_leds_single(self, first: Color | int, second: Color | int) -> Self:
+        """
+        Sets the color of both LEDs to different values.
+
+        Parameters:
+            first (Color | int): The color to set for the first LED.
+            second (Color | int): The color to set for the second LED.
+
+        Returns:
+            Self: The instance of the class to allow for method chaining.
+        """
+        __lib__.adc_led_set(0, first)
+        __lib__.adc_led_set(1, second)
+        return self
+
+    def set_all_leds_off(self) -> Self:
+        """
+        Set all LEDs to off state.
+
+        This function sets the color of both LEDs to 0, effectively turning them off.
+
+        Returns:
+            Self: The instance of the class to allow for method chaining.
+        """
+        __lib__.adc_led_set(0, 0)
+        __lib__.adc_led_set(1, 0)
+        return self
+
     def fill_screen(self, color: Color | int) -> Self:
         """
         Fill the entire screen with the specified color.
 
         Args:
           color (Color): The color to fill the screen with.
 
@@ -309,19 +394,20 @@
         Args:
           display_string (str): The string to display on the LCD.
 
         Returns:
           Self for chainable calls.
         """
 
-        __lib__.UG_PutString(0,0, display_string.encode())
+        __lib__.UG_PutString(0, 0, display_string.encode())
 
         return self
+
     def fill_frame(
-        self, x1: int, y1: int, x2: int, y2: int, color: Color | int
+            self, x1: int, y1: int, x2: int, y2: int, color: Color | int
     ) -> Self:
         """
         Fill a rectangular frame with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
@@ -332,15 +418,15 @@
         Returns:
           Self for chainable calls.
         """
         __lib__.UG_FillFrame(x1, y1, x2, y2, color)
         return self
 
     def fill_round_frame(
-        self, x1: int, y1: int, x2: int, y2: int, r: int, color: Color | int
+            self, x1: int, y1: int, x2: int, y2: int, r: int, color: Color | int
     ) -> Self:
         """
         Fill a rounded rectangular frame with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
@@ -385,15 +471,15 @@
         Returns:
           Self for chainable calls.
         """
         __lib__.UG_DrawMesh(x1, y1, x2, y2, color)
         return self
 
     def draw_frame(
-        self, x1: int, y1: int, x2: int, y2: int, color: Color | int
+            self, x1: int, y1: int, x2: int, y2: int, color: Color | int
     ) -> Self:
         """
         Draw an empty rectangular frame with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
@@ -404,15 +490,15 @@
         Returns:
           Self for chainable calls.
         """
         __lib__.UG_DrawFrame(x1, y1, x2, y2, color)
         return self
 
     def draw_round_frame(
-        self, x1: int, y1: int, x2: int, y2: int, r: int, color: Color | int
+            self, x1: int, y1: int, x2: int, y2: int, r: int, color: Color | int
     ) -> Self:
         """
         Draw an empty rounded rectangular frame with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
```

### Comparing `pyuptech-0.1.6.3/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.6.4/src/pyuptech/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/src/pyuptech/tools/display.py` & `pyuptech-0.1.6.4/src/pyuptech/tools/display.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/tests/display_tests.py` & `pyuptech-0.1.6.4/tests/display_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/tests/perf_tests.py` & `pyuptech-0.1.6.4/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/tests/test_sensor.py` & `pyuptech-0.1.6.4/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.3/PKG-INFO` & `pyuptech-0.1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.6.3
+Version: 0.1.6.4
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
```

