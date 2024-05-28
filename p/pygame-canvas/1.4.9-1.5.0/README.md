# Comparing `tmp/pygame_canvas-1.4.9.tar.gz` & `tmp/pygame_canvas-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_canvas-1.4.9.tar", last modified: Wed May 22 13:12:06 2024, max compression
+gzip compressed data, was "pygame_canvas-1.5.0.tar", last modified: Tue May 28 17:29:19 2024, max compression
```

## Comparing `pygame_canvas-1.4.9.tar` & `pygame_canvas-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:12:06.150923 pygame_canvas-1.4.9/
--rw-rw-rw-   0        0        0     1797 2024-05-22 13:12:06.149317 pygame_canvas-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     1554 2024-05-21 15:04:12.000000 pygame_canvas-1.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 13:12:06.125229 pygame_canvas-1.4.9/pygame_canvas/
--rw-rw-rw-   0        0        0       28 2024-05-21 14:59:55.000000 pygame_canvas-1.4.9/pygame_canvas/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-22 13:11:12.000000 pygame_canvas-1.4.9/pygame_canvas/pygame_canvas.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:12:06.147665 pygame_canvas-1.4.9/pygame_canvas.egg-info/
--rw-rw-rw-   0        0        0     1797 2024-05-22 13:12:05.000000 pygame_canvas-1.4.9/pygame_canvas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-22 13:12:06.000000 pygame_canvas-1.4.9/pygame_canvas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:12:05.000000 pygame_canvas-1.4.9/pygame_canvas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-22 13:12:05.000000 pygame_canvas-1.4.9/pygame_canvas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-22 13:12:05.000000 pygame_canvas-1.4.9/pygame_canvas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 13:12:06.150923 pygame_canvas-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0      520 2024-05-22 13:11:58.000000 pygame_canvas-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:29:19.554602 pygame_canvas-1.5.0/
+-rw-rw-rw-   0        0        0     1797 2024-05-28 17:29:19.553601 pygame_canvas-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1554 2024-05-21 15:04:12.000000 pygame_canvas-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 17:29:19.542578 pygame_canvas-1.5.0/pygame_canvas/
+-rw-rw-rw-   0        0        0       28 2024-05-21 14:59:55.000000 pygame_canvas-1.5.0/pygame_canvas/__init__.py
+-rw-rw-rw-   0        0        0    19965 2024-05-28 17:21:45.000000 pygame_canvas-1.5.0/pygame_canvas/pygame_canvas.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:29:19.552601 pygame_canvas-1.5.0/pygame_canvas.egg-info/
+-rw-rw-rw-   0        0        0     1797 2024-05-28 17:29:19.000000 pygame_canvas-1.5.0/pygame_canvas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-28 17:29:19.000000 pygame_canvas-1.5.0/pygame_canvas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 17:29:19.000000 pygame_canvas-1.5.0/pygame_canvas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 17:29:19.000000 pygame_canvas-1.5.0/pygame_canvas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 17:29:19.000000 pygame_canvas-1.5.0/pygame_canvas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 17:29:19.554602 pygame_canvas-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-28 17:22:39.000000 pygame_canvas-1.5.0/setup.py
```

### Comparing `pygame_canvas-1.4.9/PKG-INFO` & `pygame_canvas-1.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: pygame_canvas
-Version: 1.4.9
-Summary: A library for canvas operations using pygame
-Home-page: https://x.com/gioseaxmc
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: pygame
-
 Canvas
 Canvas is a Python module built on top of Pygame, designed to simplify the creation of interactive applications and games. It provides a set of functions and classes for managing graphical elements, handling user input, and implementing game logic.
 
 Features
 Window Management: Create resizable windows with customizable properties such as title, size, and icon.
 Event Handling: Capture user input events like mouse clicks, keyboard presses, and window resizing.
 Sprite Management: Define and manipulate sprites with properties like position, scale, rotation, and collision detection.
@@ -30,8 +21,8 @@
 import pygame_canvas as c
 
 c.default_template(__file__)
 
 The code above will load a default template into the main python script OVERWRITING EVERYTHING ELSE
 
 Documentation
-For detailed documentation and usage examples, refer to the Canvas documentation at: https://docs.google.com/document/d/18SMSY5RbigaOX2WOaGQs0iEUvSFnpfpWjsBxBNwq0nA/edit?usp=sharing.
+For detailed documentation and usage examples, refer to the Canvas documentation at: https://docs.google.com/document/d/18SMSY5RbigaOX2WOaGQs0iEUvSFnpfpWjsBxBNwq0nA/edit?usp=sharing.
```

### Comparing `pygame_canvas-1.4.9/README.md` & `pygame_canvas-1.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: pygame_canvas
+Version: 1.5.0
+Summary: A library for canvas operations using pygame
+Home-page: https://x.com/gioseaxmc
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: pygame
+
 Canvas
 Canvas is a Python module built on top of Pygame, designed to simplify the creation of interactive applications and games. It provides a set of functions and classes for managing graphical elements, handling user input, and implementing game logic.
 
 Features
 Window Management: Create resizable windows with customizable properties such as title, size, and icon.
 Event Handling: Capture user input events like mouse clicks, keyboard presses, and window resizing.
 Sprite Management: Define and manipulate sprites with properties like position, scale, rotation, and collision detection.
@@ -21,8 +30,8 @@
 import pygame_canvas as c
 
 c.default_template(__file__)
 
 The code above will load a default template into the main python script OVERWRITING EVERYTHING ELSE
 
 Documentation
-For detailed documentation and usage examples, refer to the Canvas documentation at: https://docs.google.com/document/d/18SMSY5RbigaOX2WOaGQs0iEUvSFnpfpWjsBxBNwq0nA/edit?usp=sharing.
+For detailed documentation and usage examples, refer to the Canvas documentation at: https://docs.google.com/document/d/18SMSY5RbigaOX2WOaGQs0iEUvSFnpfpWjsBxBNwq0nA/edit?usp=sharing.
```

### Comparing `pygame_canvas-1.4.9/pygame_canvas/pygame_canvas.py` & `pygame_canvas-1.5.0/pygame_canvas/pygame_canvas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import os
 import pygame
 from math import *
 import copy
 
+pygame.joystick.init()
+
 flags = 0
 screen = 0
 frames = 0
 sprites = []
 left_clicked = 0
 right_clicked = 0
 left_released = 0
 right_released = 0
+button_press = 0
+button_up = 0
+axis = 0
 wheel_up = 0
 wheel_down = 0
 text_list = []
 key_pres = 0
 ascii = {chr(i): i for i in range(128)}
 clock = pygame.time.Clock()
 updating_sizes = 0
 minimum_sizes = (0,0)
 fullscreen = 0
+joypad = 0
+resizable = 0
 WIDTH = 0
 HEIGHT = 0
 FPS = 0
 
 def get_frames():
     return frames
 
@@ -61,15 +68,85 @@
 
 def rectangle(width, height, color):
     """color must be type _color (tuple of R,G,B)"""
     surface = pygame.Surface((width, height))
     surface.fill(color)
     return surface
 
-def window(width = 480,height = 360,title = "window", resizable=0, smallest_window_sizes = (0,0), icon = None, full_Screen = 0):
+if pygame.joystick.get_count() == 0:
+    print("No joystick detected.")
+else:
+    joypad = pygame.joystick.Joystick(0)
+    joypad.init()
+
+class joystick:
+    def button_clicked(button):
+        return button_press == button
+
+    def button_released(button):
+        return button_up == button
+    
+    def get_axis(multiplier = 1):
+        num_axes = joypad.get_numaxes()
+        axis_values = [round(joypad.get_axis(i), 2) * multiplier for i in range(num_axes)]
+        return axis_values
+    
+    def buttons_clicked(*buttons):
+        condition = 0
+        for button in buttons:
+            condition = condition or button_press == button
+        return condition
+    
+    def buttons_released(*buttons):
+        condition = 0
+        for button in buttons:
+            condition = condition or button_up == button
+        return condition
+    
+    def get_lever(lever):
+        num_axes = joypad.get_numaxes()
+        axis_values = [round(joypad.get_axis(i), 2) for i in range(num_axes)]
+        if "r" in lever.lower():
+            return axis_values[-1] > 0
+        elif "l" in lever.lower():
+            return axis_values[-2] > 0
+        
+    def button_down(button):
+        return joypad.get_button(button)
+
+    def buttons_down(*buttons):
+        condition = 0
+        for butt in buttons:
+            condition = condition or joypad.get_button(butt)
+        return condition
+
+    def get_sticks(side, direction):
+        if "l" in side.lower():
+            side = 0
+        elif "r" in side.lower():
+            side = 2
+        if "x" in direction.lower():
+            direction = 0
+        elif "y" in direction.lower():
+            direction = 1
+        num_axes = joypad.get_numaxes()
+        axis_values = [round(joypad.get_axis(i), 2) for i in range(num_axes)]
+        return axis_values[direction+side]
+    
+    def get_d_pad(direction):
+        conv = {"up" : 11,
+                "down" : 12,
+                "left" : 13,
+                "right" : 14}
+        return joypad.get_button(conv[direction])
+
+    
+
+def window(width = 480,height = 360,title = "window", can_resize=1, smallest_window_sizes = (480,360), icon = None, full_Screen = 0):
+    global resizable; resizable = can_resize
     global minimum_sizes; minimum_sizes = smallest_window_sizes
     global fullscreen; fullscreen = full_Screen
     global flags
     global updating_sizes; updating_sizes = 1
     pygame.init()
     global screen
     if resizable:
@@ -86,28 +163,31 @@
 def loop(fps_goal = None, background = (255,255,255)):
     global frames
     if frames > 1:
         pygame.display.flip()
     running = 1
     global FPS; FPS = int(clock.get_fps())
     frames += 1
+    global button_up; button_up = 0
+    global button_press; button_press = 0
+    global axis; axis = 0
     global screen; screen.fill(background)
     global left_clicked, right_clicked; left_clicked = 0 ; right_clicked = 0
     global right_released, left_released; right_released = 0; left_released = 0
     global wheel_up, wheel_down; wheel_down = 0; wheel_up = 0
     global text_list, key_pres; key_pres = 0
     global updating_sizes; updating_sizes = 0
     global minimum_sizes
     global flags
     global fullscreen
     global WIDTH; global HEIGHT
+    global resizable
 
     if frames > (1 << 16):
         frames = 0
-
     for sprite in sprites:
         sprite.draw()
     for text in text_list:
         screen.blit(text[0],text[1])
     text_list = []
     if fps_goal:
         clock.tick(fps_goal)
@@ -131,25 +211,32 @@
                 right_released = 1
         elif event.type == pygame.KEYDOWN:
             key_pres = event.key
         elif event.type == pygame.VIDEORESIZE:
             updating_sizes = 1
             screen = pygame.display.set_mode((max(event.w,minimum_sizes[0]),max(event.h,minimum_sizes[1])), flags)
             WIDTH,HEIGHT = screen_size()
+        elif event.type == pygame.JOYBUTTONDOWN:
+            button_press = event.button
+        elif event.type == pygame.JOYBUTTONUP:
+            button_up = event.button
+        elif event.type == pygame.JOYAXISMOTION:
+            axis = joypad.get_numaxes()
         if key_clicked(pygame.K_F11):
-            if fullscreen:
-                fullscreen = 0
-                flags &= ~pygame.FULLSCREEN
-                screen = pygame.display.set_mode(minimum_sizes, flags)
-            else:
-                fullscreen = 1
-                flags |= pygame.FULLSCREEN
-                screen = pygame.display.set_mode((0,0), flags)
-            WIDTH,HEIGHT = screen_size()
-            updating_sizes = 1    
+            if resizable:
+                if fullscreen:
+                    fullscreen = 0
+                    flags &= ~pygame.FULLSCREEN
+                    screen = pygame.display.set_mode(minimum_sizes, flags)
+                else:
+                    fullscreen = 1
+                    flags |= pygame.FULLSCREEN
+                    screen = pygame.display.set_mode((0,0), flags)
+                WIDTH,HEIGHT = screen_size()
+                updating_sizes = 1    
     return running
 
 def mouse_down(button = "left"):
     if button == "left" or button == 0:
         return pygame.mouse.get_pressed()[0]
     elif button == "right" or button == 1:
         return pygame.mouse.get_pressed()[2]
```

### Comparing `pygame_canvas-1.4.9/pygame_canvas.egg-info/PKG-INFO` & `pygame_canvas-1.5.0/pygame_canvas.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_canvas
-Version: 1.4.9
+Version: 1.5.0
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
```

### Comparing `pygame_canvas-1.4.9/setup.py` & `pygame_canvas-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_desc = fh.read()
 
 setup(
     name='pygame_canvas',
-    version='1.4.9',
+    version='1.5.0',
     packages=find_packages(),
     include_package_data=True,
     description='A library for canvas operations using pygame',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://x.com/gioseaxmc',
     install_requires=[
```

