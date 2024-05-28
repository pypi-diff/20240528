# Comparing `tmp/kebbie-0.2.0.tar.gz` & `tmp/kebbie-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kebbie-0.2.0.tar", last modified: Mon May 13 09:28:44 2024, max compression
+gzip compressed data, was "kebbie-0.3.0.tar", last modified: Tue May 28 09:58:28 2024, max compression
```

## Comparing `kebbie-0.2.0.tar` & `kebbie-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:28:44.934783 kebbie-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 09:28:42.000000 kebbie-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-13 09:28:44.934783 kebbie-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-13 09:28:42.000000 kebbie-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:28:44.930783 kebbie-0.2.0/kebbie/
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/correctors.py
--rw-r--r--   0 runner    (1001) docker     (127)    46981 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/gesture.py
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/noise_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:28:44.934783 kebbie-0.2.0/kebbie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-13 09:28:42.000000 kebbie-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:28:44.934783 kebbie-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-13 09:28:42.000000 kebbie-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:58:28.863760 kebbie-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 09:58:24.000000 kebbie-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-28 09:58:28.863760 kebbie-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-28 09:58:24.000000 kebbie-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:58:28.863760 kebbie-0.3.0/kebbie/
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51089 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/gesture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/noise_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:58:28.863760 kebbie-0.3.0/kebbie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-28 09:58:24.000000 kebbie-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:58:28.863760 kebbie-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 09:58:24.000000 kebbie-0.3.0/setup.py
```

### Comparing `kebbie-0.2.0/LICENSE` & `kebbie-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/PKG-INFO` & `kebbie-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebbie
-Version: 0.2.0
+Version: 0.3.0
 Summary: A small framework to test and compare mobile keyboards
 Home-page: https://github.com/FleksySDK/kebbie
 Author: Nicolas REMOND
 Author-email: nicolas.remond@thingthing.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -38,14 +38,17 @@
   <a href="#install">Install</a> •
   <a href="#usage">Usage</a> •
   <a href="#contribute">Contribute</a>
   <br>
   <a href="https://FleksySDK.github.io/kebbie/" target="_blank">Documentation</a>
 </p>
 
+<p align="center">
+    <img src="docs/assets/kebbie_logo.gif" alt="kebbie_logo" />
+</p>
 
 <h2 align="center">Description</h2>
 
 `kebbie` is a small framework for **testing and benchmarking mobile keyboards**.  
 The primary goal of this package is to establish a *cohesive* and *standardized* method for evaluating the various NLP capabilities of a mobile keyboard and comparing them to existing alternatives.
 
 `kebbie` achieves this through the following two features :
```

### Comparing `kebbie-0.2.0/README.md` & `kebbie-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,17 @@
   <a href="#install">Install</a> •
   <a href="#usage">Usage</a> •
   <a href="#contribute">Contribute</a>
   <br>
   <a href="https://FleksySDK.github.io/kebbie/" target="_blank">Documentation</a>
 </p>
 
+<p align="center">
+    <img src="docs/assets/kebbie_logo.gif" alt="kebbie_logo" />
+</p>
 
 <h2 align="center">Description</h2>
 
 `kebbie` is a small framework for **testing and benchmarking mobile keyboards**.  
 The primary goal of this package is to establish a *cohesive* and *standardized* method for evaluating the various NLP capabilities of a mobile keyboard and comparing them to existing alternatives.
 
 `kebbie` achieves this through the following two features :
```

### Comparing `kebbie-0.2.0/kebbie/__init__.py` & `kebbie-0.3.0/kebbie/__init__.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie/cmd.py` & `kebbie-0.3.0/kebbie/cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         instantiate_emulator (bool, optional): If `True`, the emulators are
             instantiated (which trigger the layout detection). If `False`, only
             the corrector is instantiated, not the emulator.
 
     Returns:
         The list of created Correctors.
     """
-    if keyboard in ["gboard", "tappa"]:
+    if keyboard in ["gboard", "tappa", "swiftkey", "yandex"]:
         # Android keyboards
         return [
             EmulatorCorrector(
                 device=d,
                 platform="android",
                 keyboard=keyboard,
                 fast_mode=fast_mode,
@@ -64,15 +64,15 @@
     """
     parser.add_argument(
         "--keyboard",
         "-K",
         dest="keyboard",
         type=str,
         required=True,
-        choices=["gboard", "ios", "kbkitpro", "kbkitoss", "tappa", "fleksy"],
+        choices=["gboard", "ios", "kbkitpro", "kbkitoss", "tappa", "fleksy", "swiftkey", "yandex"],
         help="Which keyboard, to be tested, is currently installed on the emulator.",
     )
 
 
 def cli():
     """Entry-point of the `kebbie` command line."""
     # create the top-level parser
```

### Comparing `kebbie-0.2.0/kebbie/correctors.py` & `kebbie-0.3.0/kebbie/correctors.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie/emulator.py` & `kebbie-0.3.0/kebbie/emulator.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,22 @@
 ANDROID = "android"
 IOS = "ios"
 GBOARD = "gboard"
 TAPPA = "tappa"
 FLEKSY = "fleksy"
 KBKITPRO = "kbkitpro"
 KBKITOSS = "kbkitoss"
+SWIFTKEY = "swiftkey"
+YANDEX = "yandex"
+KEYBOARD_PACKAGE = {
+    GBOARD: "com.google.android.inputmethod.latin",
+    SWIFTKEY: "com.touchtype.swiftkey",
+    YANDEX: "ru.yandex.androidkeyboard",
+    TAPPA: "com.tappa.keyboard",
+}
 ANDROID_CAPABILITIES = {
     "platformName": "android",
     "automationName": "UiAutomator2",
     "enableMultiWindows": True,
     "deviceName": "test",
     "newCommandTimeout": 3600,
 }
@@ -82,30 +90,38 @@
     "EmojiCategories/symbols",
     "EmojiCategories/flags",
     "Add",
     "And",
     "Are",
     "“A”",
     "🚀",
+    "Switch language.",
 ]
 CONTENT_TO_RENAME = {
     "Shift": "shift",
     "Delete": "backspace",
     "Backspace": "backspace",
     "Space": "spacebar",
     "space": "spacebar",
+    "Space.": "spacebar",
     "Emoji button": "smiley",
     "Emoji": "smiley",
     "Keyboard Type - emojis": "smiley",
     "Search": "enter",
     "return": "enter",
+    "Enter": "enter",
+    "Delete.": "backspace",
+    "To symbols.": "numbers",
+    "Return.": "enter",
     "Symbol keyboard": "numbers",
     "Symbols": "numbers",
+    "Symbols and numbers": "numbers",
     "Keyboard Type - numeric": "numbers",
     "Voice input": "mic",
+    ",, alternatives available, Voice typing, long press to activate": "mic",
     "Close features menu": "magic",
     "Open features menu": "magic",
     "underline": "_",
     "&amp;": "&",
     "ampersand": "&",
     "Dash": "-",
     "Plus": "+",
@@ -116,18 +132,49 @@
     "Colon": ":",
     "Semicolon": ";",
     "Exclamation": "!",
     "Question mark": "?",
     "Letter keyboard": "letters",
     "Letters": "letters",
     "Keyboard Type - auto": "letters",
+    "To letters.": "letters",
     "Digit keyboard": "numbers",
     "More symbols": "shift",
     "Keyboard Type - symbolic": "shift",
+    "Double tap for uppercase": "shift",
+    "Double tap for caps lock": "shift",
+    "Uppercase key.": "shift",
+    "Additional symbols.": "shift",
+    "capital Q": "Q",
+    "capital W": "W",
+    "capital E": "E",
+    "capital R": "R",
+    "capital T": "T",
+    "capital Y": "Y",
+    "capital U": "U",
+    "capital I": "I",
     "Capital I": "I",
+    "capital O": "O",
+    "capital P": "P",
+    "capital A": "A",
+    "capital S": "S",
+    "capital D": "D",
+    "capital F": "F",
+    "capital G": "G",
+    "capital H": "H",
+    "capital J": "J",
+    "capital K": "K",
+    "capital L": "L",
+    "capital Z": "Z",
+    "capital X": "X",
+    "capital C": "C",
+    "capital V": "V",
+    "capital B": "B",
+    "capital N": "N",
+    "capital M": "M",
 }
 FLEKSY_LAYOUT = {
     "keyboard_frame": [0, 517, 393, 266],  # Only the keyboard frame is defined as absolute position
     # The layout is then defined as relative position (to the keyboard frame)
     # so that if the device size change, we just have to adjust the keyboard
     # frame, and the rest should follow
     "lowercase": {
@@ -248,15 +295,15 @@
         host (str, optional): Appium server's address.
         port (str, optional): Appium server's port.
 
     Raises:
         ValueError: Error raised if the given platform doesn't exist.
     """
 
-    def __init__(
+    def __init__(  # noqa: C901
         self,
         platform: str,
         keyboard: str,
         device: str = None,
         host: str = "127.0.0.1",
         port: str = "4723",
         ios_name: str = None,
@@ -289,14 +336,18 @@
 
         # Keep track of the keyboard behavior
         # When the typing field is empty, the keyboard is uppercase by default
         self.kb_is_upper = True
         self.last_char_is_space = False
         self.last_char_is_eos = False
 
+        # Set the keyboard as default
+        if self.platform == ANDROID:
+            self.select_keyboard(keyboard)
+
         # Get the right layout
         if self.keyboard == GBOARD:
             self.detected = GboardLayoutDetector(self.driver, self._tap)
             self.layout = self.detected.layout
         elif self.keyboard == TAPPA:
             self.detected = TappaLayoutDetector(self.driver, self._tap)
             self.layout = self.detected.layout
@@ -308,18 +359,24 @@
             self.layout = self.detected.layout
         elif self.keyboard == KBKITPRO:
             self.detected = KbkitproLayoutDetector(self.driver, self._tap)
             self.layout = self.detected.layout
         elif self.keyboard == KBKITOSS:
             self.detected = KbkitossLayoutDetector(self.driver, self._tap)
             self.layout = self.detected.layout
+        elif self.keyboard == SWIFTKEY:
+            self.detected = SwiftkeyLayoutDetector(self.driver, self._tap)
+            self.layout = self.detected.layout
+        elif self.keyboard == YANDEX:
+            self.detected = YandexLayoutDetector(self.driver, self._tap)
+            self.layout = self.detected.layout
         else:
             raise ValueError(
-                f"Unknown keyboard : {self.keyboard}. Please specify `{GBOARD}`, `{TAPPA}`, `{FLEKSY}`, `{KBKITPRO}`, "
-                f"`{KBKITOSS}` or `{IOS}`."
+                f"Unknown keyboard : {self.keyboard}. Please specify `{GBOARD}`, `{TAPPA}`, `{FLEKSY}`, "
+                f"`{SWIFTKEY}`, `{YANDEX}`, `{KBKITPRO}`, `{KBKITOSS}` or `{IOS}`."
             )
 
         self.typing_field.clear()
 
     def _access_typing_field(self):
         """Start the right application and access the typing field where we
         will type our text.
@@ -348,14 +405,41 @@
             List of detected device UDID.
         """
         result = subprocess.run(["adb", "devices"], stdout=subprocess.PIPE)
         devices = result.stdout.decode().split("\n")
         devices = [d.split()[0] for d in devices if not (d.startswith("List of devices attached") or len(d) == 0)]
         return devices
 
+    def select_keyboard(self, keyboard):
+        """Searches the IME of the desired keyboard and selects it, only for Android.
+
+        Args:
+            keyboard (str): Keyboard to search.
+        """
+        if keyboard not in KEYBOARD_PACKAGE:
+            print(
+                f"Warning ! {keyboard}'s IME isn't provided (in `KEYBOARD_PACKAGE`), can't automatically select the "
+                "keyboard."
+            )
+            return
+
+        ime_list = subprocess.check_output(["adb", "shell", "ime", "list", "-s"], universal_newlines=True)
+        ime_name = None
+        for ime in ime_list.strip().split("\n"):
+            if KEYBOARD_PACKAGE[keyboard] in ime:
+                ime_name = ime
+                break
+        if ime_name:
+            subprocess.run(
+                ["adb", "shell", "settings", "put", "secure", "show_ime_with_hard_keyboard", "1"],
+                stdout=subprocess.PIPE,
+            )
+            subprocess.run(["adb", "shell", "ime", "enable", ime_name], stdout=subprocess.PIPE)
+            subprocess.run(["adb", "shell", "ime", "set", ime_name], stdout=subprocess.PIPE)
+
     def get_ios_devices() -> List[Tuple[str, str]]:
         """Static method that uses the `xcrun simctl` command to retrieve the
         list of booted devices.
 
         Returns:
             List of booted device platform and device name.
         """
@@ -449,14 +533,17 @@
                 if self.last_char_is_eos:
                     self.kb_is_upper = True
             elif c in self.layout["lowercase"]:
                 # The character is a lowercase character
                 if self.kb_is_upper:
                     # If the keyboard is in uppercase mode, change it to lowercase
                     self._tap(self.layout["uppercase"]["shift"])
+                    if self.keyboard == SWIFTKEY:
+                        # Swiftkey needs double tap, otherwise we are capslocking
+                        self._tap(self.layout["uppercase"]["shift"])
                 self._tap(self.layout["lowercase"][c])
             elif c in self.layout["uppercase"]:
                 # The character is an uppercase character
                 if not self.kb_is_upper:
                     # Change the keyboard to uppercase
                     self._tap(self.layout["lowercase"]["shift"])
                 self._tap(self.layout["uppercase"][c])
@@ -466,17 +553,17 @@
                 # Access the number keyboard properly
                 if self.kb_is_upper:
                     self._tap(self.layout["uppercase"]["numbers"])
                 else:
                     self._tap(self.layout["lowercase"]["numbers"])
                 self._tap(self.layout["numbers"][c])
 
-                if c != "'" or self.keyboard == GBOARD:
+                if c != "'" or self.keyboard in [GBOARD, SWIFTKEY]:
                     # For some reason, when `'` is typed, the keyboard automatically goes back
-                    # to lowercase, so no need to re-tap the button (unless the keyboard is GBoard).
+                    # to lowercase, so no need to re-tap the button (unless the keyboard is GBoard / Swiftkey).
                     # In all other cases, switch back to letters keyboard
                     self._tap(self.layout["numbers"]["letters"])
             else:
                 # Can't type this character, ignore it
                 continue
 
             # Behavior of the keyboard : if the previous character typed was an EOS marker
@@ -530,17 +617,15 @@
         """Take a screenshot of the full screen.
 
         Returns:
             The image of the screen.
         """
         screen_data = self.driver.get_screenshot_as_png()
         screen = np.asarray(Image.open(io.BytesIO(screen_data)))
-        return cv2.resize(
-            screen, (self.screen_size["width"], self.screen_size["height"]), interpolation=cv2.INTER_AREA
-        )
+        return screen.copy()
 
     def get_predictions(self, lang: str = "en") -> List[str]:
         """Retrieve the predictions displayed by the keyboard.
 
         Args:
             lang (str): Language to use for the OCR.
 
@@ -692,19 +777,15 @@
         self.tap(layout["lowercase"]["numbers"], layout["keyboard_frame"])
         _, screen_layout = self._detect_keys(root, keyboard_frame=layout["keyboard_frame"], current_layout="numbers")
         layout["numbers"] = screen_layout
 
         # Reset out keyboard to the original layer
         self.tap(layout["numbers"]["letters"], layout["keyboard_frame"])
 
-        # Fix the keys' offset compared to the keyboard frame
-        if self.android:
-            self.layout = self._apply_status_bar_offset(layout)
-        else:
-            self.layout = layout
+        self.layout = layout
 
     def get_suggestions(self) -> List[str]:
         """Method to retrieve the keyboard suggestions from the XML tree.
 
         Note that it's slower to access the XML through methods like
         `find_element()`, and it's faster to access the raw XML with
         `self.driver.page_source` and parse it as text directly.
@@ -807,70 +888,24 @@
             else:
                 return "letters"
         elif content in CONTENT_TO_RENAME:
             return CONTENT_TO_RENAME[content]
         else:
             return content
 
-    def _get_status_bar_bounds(self) -> List[int]:
-        """For layout detection, this method retrieve the bounds of the status
-        bar from the XML tree.
-
-        Returns:
-            Bounds of the status bar.
-        """
-        sb = self.driver.find_element(By.ID, "com.android.systemui:id/status_bar")
-        return self._get_frame(sb)
-
-    def _apply_status_bar_offset(self, layout: Dict) -> Dict:
-        """Method offsetting the given layout to match the screen.
-
-        On Android, somehow the detected positions for the keys aren't matching
-        what we see on screen. This is because of the status bar, which shift
-        everything. So, detect the status bar, and shift back the keys to the
-        right position.
-
-        Args:
-            layout (Dict): Layout to fix.
-
-        Returns:
-            Fixed layout.
-        """
-        sb_bounds = self._get_status_bar_bounds()
-        dy = sb_bounds[3]
-        screen_size = layout["keyboard_frame"][1] + layout["keyboard_frame"][3]
-
-        # First of all, offset the keyboard frame
-        frame_dy1 = int(dy * (layout["keyboard_frame"][1] / screen_size))
-        frame_dy2 = int(dy * ((layout["keyboard_frame"][1] + layout["keyboard_frame"][3]) / screen_size))
-        layout["keyboard_frame"][1] -= frame_dy1
-        layout["keyboard_frame"][3] -= frame_dy2 - frame_dy1
-
-        # Then do the same for each keys of each layouts
-        for layer in ["lowercase", "uppercase", "numbers"]:
-            for k in layout[layer]:
-                dy1 = int(dy * ((layout["keyboard_frame"][1] + layout[layer][k][1]) / screen_size))
-                dy2 = int(
-                    dy * ((layout["keyboard_frame"][1] + layout[layer][k][1] + layout[layer][k][3]) / screen_size)
-                )
-                layout[layer][k][1] -= dy1 - frame_dy1
-                layout[layer][k][3] -= dy2 - dy1
-
-        return layout
-
 
 class GboardLayoutDetector(LayoutDetector):
     """Layout detector for the Gboard keyboard. See `LayoutDetector` for more
     information.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(
             *args,
-            xpath_root="./*/*[@package='com.google.android.inputmethod.latin']",
+            xpath_root=f"./*/*[@package='{KEYBOARD_PACKAGE[GBOARD]}']",
             xpath_keys=".//*[@resource-id][@content-desc]",
             **kwargs,
         )
 
     def get_suggestions(self) -> List[str]:
         """Method to retrieve the keyboard suggestions from the XML tree.
 
@@ -1005,38 +1040,124 @@
                     if m:
                         name = m.group(1)
                         suggestions.append(name.replace("“", "").replace("”", ""))
 
         return suggestions
 
 
+class SwiftkeyLayoutDetector(LayoutDetector):
+    """Layout detector for the Swiftkey keyboard. See `LayoutDetector` for more
+    information.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(
+            *args,
+            xpath_root=f"./*/*[@package='{KEYBOARD_PACKAGE[SWIFTKEY]}']",
+            xpath_keys=".//*[@class='android.view.View'][@content-desc]",
+            **kwargs,
+        )
+
+    def get_suggestions(self) -> List[str]:
+        """Method to retrieve the keyboard suggestions from the XML tree.
+
+        Returns:
+            List of suggestions from the keyboard.
+        """
+        suggestions = []
+
+        # Get the raw content as text, weed out useless elements
+        for data in self.driver.page_source.split("<android.widget.FrameLayout"):
+            if "com.touchtype.swiftkey" in data and "<android.view.View " in data:
+                sections = data.split("<android.view.View ")
+                for section in sections[1:]:
+                    m = re.search(r"content-desc=\"([^\"]*)\"", section)
+                    if m:
+                        suggestions.append(html.unescape(m.group(1)))
+                break
+
+        return suggestions
+
+
+class YandexLayoutDetector(LayoutDetector):
+    """Layout detector for the Yandex keyboard. See `LayoutDetector` for more
+    information.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(
+            *args,
+            xpath_root=f"./*/*[@package='{KEYBOARD_PACKAGE[YANDEX]}']",
+            xpath_keys=".//*[@class='ya.d'][@content-desc]",
+            **kwargs,
+        )
+
+    def get_suggestions(self) -> List[str]:
+        """Method to retrieve the keyboard suggestions from the XML tree.
+
+        Returns:
+            List of suggestions from the keyboard.
+        """
+        suggestions = []
+
+        # Depending if we are on a real device or on emulator, the
+        # Yandex keyboard uses different XML tags...
+        if "<javaClass" in self.driver.page_source:  # Real device
+            section = self.driver.page_source.split(f"{KEYBOARD_PACKAGE[YANDEX]}:id/drawable_suggest_container")[
+                1
+            ].split("</android.view.View>")[0]
+
+            for line in section.split("\n"):
+                if "<javaClass" in line:
+                    m = re.search(r"content-desc=\"([^\"]*)\"", line)
+                    if m:
+                        suggestions.append(html.unescape(m.group(1)))
+        else:  # Emulator
+            for s in self.driver.page_source.split("android.widget.LinearLayout"):
+                if f"{KEYBOARD_PACKAGE[YANDEX]}:id/kb_suggest_suggestions_container" in s:
+                    suggestions_section = s
+                    break
+
+            for line in suggestions_section.split("\n"):
+                if (
+                    "kb_suggest_left_suggestion" in line
+                    or "kb_suggest_center_suggestion" in line
+                    or "kb_suggest_right_suggestion" in line
+                ):
+                    m = re.search(r"content-desc=\"([^\"]*)\"", line)
+                    if m:
+                        suggestions.append(html.unescape(m.group(1)))
+
+        return suggestions
+
+
 class TappaLayoutDetector(LayoutDetector):
     """Layout detector for the Tappa keyboard. See `LayoutDetector` for more
     information.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(
             *args,
-            xpath_root="./*/*[@package='com.tappa.keyboard']",
+            xpath_root=f"./*/*[@package='{KEYBOARD_PACKAGE[TAPPA]}']",
             xpath_keys=".//com.mocha.keyboard.inputmethod.keyboard.Key",
             **kwargs,
         )
 
     def get_suggestions(self) -> List[str]:
         """Method to retrieve the keyboard suggestions from the XML tree.
 
         Returns:
             List of suggestions from the keyboard.
         """
         suggestions = []
 
         # Get the raw content as text, weed out useless elements
-        section = self.driver.page_source.split("com.tappa.keyboard:id/toolbar")[1].split(
-            "</android.widget.FrameLayout>"
+        section = self.driver.page_source.split(f"{KEYBOARD_PACKAGE[TAPPA]}:id/suggestions_strip")[1].split(
+            "</android.widget.LinearLayout>"
         )[0]
 
         for line in section.split("\n"):
             if "<android.widget.TextView" in line:
                 m = re.search(r"text=\"([^\"]*)\"", line)
                 if m:
                     suggestions.append(html.unescape(m.group(1)))
```

### Comparing `kebbie-0.2.0/kebbie/gesture.py` & `kebbie-0.3.0/kebbie/gesture.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie/layout.py` & `kebbie-0.3.0/kebbie/layout.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie/noise_model.py` & `kebbie-0.3.0/kebbie/noise_model.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie/oracle.py` & `kebbie-0.3.0/kebbie/oracle.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie/scorer.py` & `kebbie-0.3.0/kebbie/scorer.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie/tokenizer.py` & `kebbie-0.3.0/kebbie/tokenizer.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie/utils.py` & `kebbie-0.3.0/kebbie/utils.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/kebbie.egg-info/PKG-INFO` & `kebbie-0.3.0/kebbie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebbie
-Version: 0.2.0
+Version: 0.3.0
 Summary: A small framework to test and compare mobile keyboards
 Home-page: https://github.com/FleksySDK/kebbie
 Author: Nicolas REMOND
 Author-email: nicolas.remond@thingthing.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -38,14 +38,17 @@
   <a href="#install">Install</a> •
   <a href="#usage">Usage</a> •
   <a href="#contribute">Contribute</a>
   <br>
   <a href="https://FleksySDK.github.io/kebbie/" target="_blank">Documentation</a>
 </p>
 
+<p align="center">
+    <img src="docs/assets/kebbie_logo.gif" alt="kebbie_logo" />
+</p>
 
 <h2 align="center">Description</h2>
 
 `kebbie` is a small framework for **testing and benchmarking mobile keyboards**.  
 The primary goal of this package is to establish a *cohesive* and *standardized* method for evaluating the various NLP capabilities of a mobile keyboard and comparing them to existing alternatives.
 
 `kebbie` achieves this through the following two features :
```

### Comparing `kebbie-0.2.0/kebbie.egg-info/requires.txt` & `kebbie-0.3.0/kebbie.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/pyproject.toml` & `kebbie-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kebbie-0.2.0/setup.py` & `kebbie-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 extras_require["all"] = sum(extras_require.values(), [])
 extras_require["dev"] = (
     extras_require["test"] + extras_require["hook"] + extras_require["lint"] + extras_require["docs"]
 )
 
 setuptools.setup(
     name="kebbie",
-    version="0.2.0",
+    version="0.3.0",
     author="Nicolas REMOND",
     author_email="nicolas.remond@thingthing.co",
     description="A small framework to test and compare mobile keyboards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FleksySDK/kebbie",
     packages=setuptools.find_packages(),
```

