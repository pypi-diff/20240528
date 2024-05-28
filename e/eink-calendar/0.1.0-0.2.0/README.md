# Comparing `tmp/eink_calendar-0.1.0.tar.gz` & `tmp/eink_calendar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eink_calendar-0.1.0.tar", max compression
+gzip compressed data, was "eink_calendar-0.2.0.tar", max compression
```

## Comparing `eink_calendar-0.1.0.tar` & `eink_calendar-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     5513 2023-11-24 16:03:02.608589 eink_calendar-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      150 2024-04-29 03:26:34.830139 eink_calendar-0.1.0/README.md
--rw-r--r--   0        0        0       66 2024-04-29 02:46:00.712186 eink_calendar-0.1.0/eink_calendar/__init__.py
--rw-r--r--   0        0        0     2853 2024-04-29 03:11:12.661989 eink_calendar-0.1.0/eink_calendar/__main__.py
--rw-r--r--   0        0        0      198 2024-04-29 02:52:44.826512 eink_calendar-0.1.0/eink_calendar/api/__init__.py
--rw-r--r--   0        0        0     2968 2024-04-29 03:22:10.987228 eink_calendar-0.1.0/eink_calendar/api/client.py
--rw-r--r--   0        0        0      957 2024-04-29 02:46:47.255992 eink_calendar-0.1.0/eink_calendar/api/event.py
--rw-r--r--   0        0        0     1439 2024-04-29 02:46:47.255992 eink_calendar-0.1.0/eink_calendar/api/event_stream.py
--rw-r--r--   0        0        0     1146 2024-04-29 02:46:47.255992 eink_calendar-0.1.0/eink_calendar/display.py
--rw-r--r--   0        0        0   212004 2023-11-24 16:03:02.612589 eink_calendar-0.1.0/eink_calendar/lora.ttf
--rw-r--r--   0        0        0      175 2024-04-29 02:46:47.255992 eink_calendar-0.1.0/eink_calendar/ui/__init__.py
--rw-r--r--   0        0        0     2454 2024-04-29 03:05:53.447289 eink_calendar-0.1.0/eink_calendar/ui/display.py
--rw-r--r--   0        0        0     1762 2024-04-29 03:11:37.233884 eink_calendar-0.1.0/eink_calendar/ui/event.py
--rw-r--r--   0        0        0     1030 2024-04-29 03:10:48.606088 eink_calendar-0.1.0/eink_calendar/ui/text.py
--rw-r--r--   0        0        0     1355 2024-04-29 03:10:48.586088 eink_calendar-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 eink_calendar-0.1.0/setup.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 eink_calendar-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5513 2023-11-24 16:03:02.608589 eink_calendar-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1193 2024-05-28 00:04:30.022934 eink_calendar-0.2.0/README.md
+-rw-r--r--   0        0        0       66 2024-04-29 02:46:00.712186 eink_calendar-0.2.0/eink_calendar/__init__.py
+-rw-r--r--   0        0        0     2398 2024-05-27 23:50:55.086114 eink_calendar-0.2.0/eink_calendar/__main__.py
+-rw-r--r--   0        0        0      198 2024-04-29 02:52:44.826512 eink_calendar-0.2.0/eink_calendar/api/__init__.py
+-rw-r--r--   0        0        0     2968 2024-05-28 00:04:30.002933 eink_calendar-0.2.0/eink_calendar/api/client.py
+-rw-r--r--   0        0        0      957 2024-04-29 02:46:47.255992 eink_calendar-0.2.0/eink_calendar/api/event.py
+-rw-r--r--   0        0        0     1439 2024-04-29 02:46:47.255992 eink_calendar-0.2.0/eink_calendar/api/event_stream.py
+-rw-r--r--   0        0        0     1169 2024-05-28 00:03:28.001350 eink_calendar-0.2.0/eink_calendar/display.py
+-rw-r--r--   0        0        0   212004 2023-11-24 16:03:02.612589 eink_calendar-0.2.0/eink_calendar/lora.ttf
+-rw-r--r--   0        0        0       77 2024-05-22 18:22:32.647084 eink_calendar-0.2.0/eink_calendar/ui/__init__.py
+-rw-r--r--   0        0        0     1585 2024-05-22 18:27:10.364189 eink_calendar-0.2.0/eink_calendar/ui/event.py
+-rw-r--r--   0        0        0      837 2024-05-22 18:26:45.330959 eink_calendar-0.2.0/eink_calendar/ui/text.py
+-rw-r--r--   0        0        0     1428 2024-05-28 00:05:05.815848 eink_calendar-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2247 1970-01-01 00:00:00.000000 eink_calendar-0.2.0/setup.py
+-rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 eink_calendar-0.2.0/PKG-INFO
```

### Comparing `eink_calendar-0.1.0/LICENSE.md` & `eink_calendar-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.1.0/eink_calendar/__main__.py` & `eink_calendar-0.2.0/eink_calendar/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import faulthandler
 import logging
 import signal
 from argparse import ArgumentParser
 from pathlib import Path
 from types import FrameType
 
-import sdl2
-from sdl2 import sdlttf
+from PIL import Image, ImageDraw, ImageFont
 
 from . import api, ui
 from .display import EInkDisplay, MockDisplay
 
 SCREEN_WIDTH = 600
 SCREEN_HEIGHT = 448
 
@@ -31,23 +30,17 @@
         help="Do not communicate with an eInk display",
     )
 
     args = parser.parse_args()
 
     api_client = api.Client()
 
-    try:
-        window, renderer = ui.init_display(SCREEN_WIDTH, SCREEN_HEIGHT)
-    except ui.SDLError as ex:
-        logging.error(f"{ex}")
-        return -1
-
     font_file = Path(__file__).parent / "lora.ttf"
-    day_font = sdlttf.TTF_OpenFont(str(font_file).encode(), 36)
-    times_font = sdlttf.TTF_OpenFont(str(font_file).encode(), 16)
+    day_font = ImageFont.truetype(str(font_file), 36)
+    times_font = ImageFont.truetype(str(font_file), 16)
 
     stop = False
 
     def on_sigint(_sig: int, _frame: FrameType | None) -> None:
         nonlocal stop
         stop = True
     signal.signal(signal.SIGINT, on_sigint)
@@ -55,54 +48,46 @@
     event_stream = api.EventStream(api_client)
 
     ui_events: list[ui.Event] = []
 
     display = MockDisplay() if args.no_display else EInkDisplay()
 
     while not stop:
-        input_event = sdl2.SDL_Event()
-        sdl2.SDL_PollEvent(input_event)
-        if input_event.type == sdl2.SDL_QUIT:
-            stop = True
-
-        sdl2.SDL_SetRenderDrawColor(renderer, 255, 255, 255, 255)
-        sdl2.SDL_RenderClear(renderer)
+        image = Image.new("RGB", (SCREEN_WIDTH, SCREEN_HEIGHT), (255, 255, 255))
+        draw = ImageDraw.Draw(image)
 
         today = datetime.date.today()
         day_text = ui.Text(
-            renderer=renderer,
+            draw=draw,
             font=day_font,
             text=today.strftime("%A, %B %d"),
-            color=sdl2.SDL_Color(0, 0, 0),
+            color=(0, 0, 0),
         )
-        day_text.set_position(int(SCREEN_WIDTH / 2 - day_text.rect.w / 2), 1)
-        day_text.draw(renderer)
+        day_text.set_position(int(SCREEN_WIDTH / 2 - day_text.width / 2), 1)
+        day_text.draw()
 
         for ui_event in ui_events:
-            ui_event.draw(renderer)
+            ui_event.draw()
 
         api_events = event_stream.get()
         if api_events is not None:
             ui_events = []
 
             for api_event in api_events:
                 ui_event = ui.Event(
-                    renderer,
+                    draw,
                     times_font,
                     api_event,
                     (ui.Event.HEIGHT + ui.Event.PADDING_BOTTOM) * len(ui_events)
                     + ui.Event.START_Y,
                 )
-                ui_event.draw(renderer)
+                ui_event.draw()
                 ui_events.append(ui_event)
 
-            image = ui.screenshot(window, renderer)
             display.set_image(image)
 
-        sdl2.SDL_RenderPresent(renderer)
-
     logging.info("Waiting for event stream to stop...")
     event_stream.close()
     logging.info("Waiting for display to finish up...")
     display.close()
 
     return 0
```

### Comparing `eink_calendar-0.1.0/eink_calendar/api/client.py` & `eink_calendar-0.2.0/eink_calendar/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         # Filter for today's events
         events = [e for e in events if e.start_time.date() == datetime.date.today()]
 
         return self._sort_events(events)
 
     def _get_credentials(self) -> Credentials:
         creds = None
-        data_path = Path(BaseDirectory.save_data_path("eink_calendar"))
+        data_path = Path(BaseDirectory.save_data_path("eink-calendar"))
 
         credentials_file = data_path / "credentials.json"
         if not credentials_file.is_file():
             logging.error(f"Missing credentials file at: {credentials_file}")
             sys.exit(1)
 
         token = data_path / "token.json"
```

### Comparing `eink_calendar-0.1.0/eink_calendar/api/event.py` & `eink_calendar-0.2.0/eink_calendar/api/event.py`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.1.0/eink_calendar/api/event_stream.py` & `eink_calendar-0.2.0/eink_calendar/api/event_stream.py`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.1.0/eink_calendar/display.py` & `eink_calendar-0.2.0/eink_calendar/display.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     @abstractmethod
     def close(self) -> None:
         pass
 
 
 class MockDisplay(Display):
     def set_image(self, image: Image.Image) -> None:
-        pass
+        image.show("eInk Calendar")
 
     def close(self) -> None:
         pass
 
 
 class EInkDisplay(Display):
     def __init__(self) -> None:
```

### Comparing `eink_calendar-0.1.0/eink_calendar/lora.ttf` & `eink_calendar-0.2.0/eink_calendar/lora.ttf`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.1.0/pyproject.toml` & `eink_calendar-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "eink-calendar"
-version = "0.1.0"
-description = ""
+version = "0.2.0"
+description = "Shows Google Calendar events on an Inky Impression display"
 authors = ["Tyler Compton <xaviosx@gmail.com>"]
 readme = "README.md"
 packages = [ { include = "eink_calendar" } ]
 
 [tool.poetry.scripts]
-eink_calendar = "eink_calendar.__main__:main"
+eink-calendar = "eink_calendar.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 inky = {extras = ["example-depends", "rpi"], version = "^1.5.0"}
 pillow = "^10.0.1"
-pysdl2 = "^0.9.16"
 google-api-python-client = "^2.100.0"
 google-auth-httplib2 = "^0.1.1"
 google-auth-oauthlib = "^1.1.0"
 pyxdg = "^0.28"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.7.1"
 ruff = "^0.4.2"
+types-pillow = "^10.2.0.20240520"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff.lint]
 # Rules documentation: https://docs.astral.sh/ruff/rules/#flake8-bandit-s
```

