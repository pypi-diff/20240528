# Comparing `tmp/display_colors-0.4.1.tar.gz` & `tmp/display_colors-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "display_colors-0.4.1.tar", max compression
+gzip compressed data, was "display_colors-1.0.3.tar", max compression
```

## Comparing `display_colors-0.4.1.tar` & `display_colors-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0    11356 2024-04-05 11:48:59.515054 display_colors-0.4.1/LICENSE
--rw-r--r--   0        0        0     5743 2024-04-04 11:17:34.146042 display_colors-0.4.1/README.md
--rw-r--r--   0        0        0     1053 2024-04-21 20:39:42.046790 display_colors-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 01:43:36.634637 display_colors-0.4.1/src/display_colors/__init__.py
--rw-r--r--   0        0        0    10758 2024-04-04 22:34:28.218668 display_colors-0.4.1/src/display_colors/__main__.py
--rw-r--r--   0        0        0     6754 1970-01-01 00:00:00.000000 display_colors-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-04-05 11:48:59.515054 display_colors-1.0.3/LICENSE
+-rw-r--r--   0        0        0     8784 2024-05-28 21:37:05.940378 display_colors-1.0.3/README.md
+-rw-r--r--   0        0        0     1052 2024-05-28 21:37:05.941680 display_colors-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 01:43:36.634637 display_colors-1.0.3/src/display_colors/__init__.py
+-rw-r--r--   0        0        0    17745 2024-05-28 21:37:05.943169 display_colors-1.0.3/src/display_colors/__main__.py
+-rw-r--r--   0        0        0     1014 2024-05-28 21:37:05.946111 display_colors-1.0.3/src/display_colors/cell.py
+-rw-r--r--   0        0        0     1695 2024-05-28 21:37:05.949952 display_colors-1.0.3/src/display_colors/cmd/effects.py
+-rw-r--r--   0        0        0     9431 2024-05-28 21:37:05.952168 display_colors-1.0.3/src/display_colors/cmd/eight_bit.py
+-rw-r--r--   0        0        0     6171 2024-05-28 21:37:05.953274 display_colors-1.0.3/src/display_colors/cmd/four_bit.py
+-rw-r--r--   0        0        0     1546 2024-05-28 21:37:05.953935 display_colors-1.0.3/src/display_colors/const.py
+-rw-r--r--   0        0        0      389 2024-05-28 21:37:05.954644 display_colors-1.0.3/src/display_colors/gen.py
+-rw-r--r--   0        0        0     3607 2024-05-28 21:37:05.955802 display_colors-1.0.3/src/display_colors/init.py
+-rw-r--r--   0        0        0      221 2024-05-28 21:37:05.957990 display_colors-1.0.3/src/display_colors/math.py
+-rw-r--r--   0        0        0     9795 1970-01-01 00:00:00.000000 display_colors-1.0.3/PKG-INFO
```

### Comparing `display_colors-0.4.1/LICENSE` & `display_colors-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `display_colors-0.4.1/pyproject.toml` & `display_colors-1.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "display-colors"
-version = "0.4.1"
+version = "1.0.3"
 description = "Shows the 4-bit color and display effect capabilities of a terminal emulator"
 authors     = ["Joe Rodrigue <joe.rodrigue@gmail.com>"]
 maintainers = ["Joe Rodrigue <joe.rodrigue@gmail.com>"]
 repository  = "https://github.com/JoeRodrigue/display-colors"
 readme      = "README.md"
 classifiers = [
 	"License :: OSI Approved :: Apache Software License",
@@ -20,12 +20,12 @@
 packages = [{include = "display_colors", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^8.1.7"
 
 [tool.poetry.scripts]
-	display-colors = 'display_colors.__main__:main'
+	display-colors = 'display_colors.__main__:cli'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `display_colors-0.4.1/PKG-INFO` & `display_colors-1.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: display-colors
-Version: 0.4.1
+Version: 1.0.3
 Summary: Shows the 4-bit color and display effect capabilities of a terminal emulator
 Home-page: https://github.com/JoeRodrigue/display-colors
 Keywords: color,terminal,emulator,SGR,ECMA-48
 Author: Joe Rodrigue
 Author-email: joe.rodrigue@gmail.com
 Maintainer: Joe Rodrigue
 Maintainer-email: joe.rodrigue@gmail.com
@@ -24,15 +24,15 @@
 
 # display-colors
 
 `display-colors` is a program to explore the color and display effect capabilities of a terminal emulator
 
 ## Compatibility
 
-At present `display-colors` only runs on macOS.
+`display-colors` runs on macOS and Linux.
 It requires Python 3.
 
 ## Installation and Use
 
 `display-colors` should be installed in a virtual environment.
 
 ### How to Create, Use and Destroy a Virtual Environment
@@ -51,59 +51,88 @@
 (.venv) python -m pip   install display-colors  // Install
 (.venv) python -m pip uninstall display-colors  // Uninstall
 ```
 
 ### Use
 
 ```
-(.venv) display-colors [OPTIONS]
+(.venv) display-colors [--help|--version] COMMAND [OPTIONS]
 ```
 
+COMMAND: 4-bit | 8-bit | effects
+
+OPTIONS vary depending on the command; do `display-colors COMMAND --help` to list them
+
 ## Features
 
-`display-colors` produces test patterns that show the capabilities of your terminal emulator.  They include each combination of foreground and background four-bit colors, which can vary depending on the theme (some themes barely support the bright variants of the eight basic colors, which are not included in the original ECMA-48 standard).  The program also demonstrates each Select Graphic Rendition (SGR) code controlling effects like underline and blink.  Support for these among emulators is spotty.
+Modern terminal emulators support color but the results vary across emulators, let alone across platforms.  Three sets of colors are available: 4 bit, 8 bit and 24 bit.  They may not be completely supported.
+
+`display-colors` produces test patterns that include all of the 4- and 8-bit colors: all foreground-background combinations of 4-bit colors, which can vary depending on the theme, and swatches of all 8-bit colors.  It also demonstrates each Select Graphic Rendition (SGR) code controlling effects like underline and blink.  Support for these among emulators is spotty.
 
-It has three modes:
+The SGR codes also specify four font weights: default, dim, medium and bold.  Implementation of these varies.  The `--weight` option in 4-bit mode lets you specify what weights you would like to see (8-bit mode text uses the default weight).
 
- - Standard -- A color palette in the traditional format (*qv* [iTerm2 Color Schemes](https://iterm2colorschemes.com/))
- - Transpose -- A palette with one foreground color per column
- - Test -- A test pattern of terminal effects
+One of the widely-supported effects is reverse video.  This is not always implemented by swapping foreground and background colors.  The `--reverse-video` option displays each line twice, the second with foreground and background colors swapped *and* reverse video turned on.  If reverse video is implemented simply by swapping the two lines will appear identical; if not, they won't.
 
-### Standard mode (default)
+The program has four modes:
+
+ - 4-bit -- A color palette in the traditional format, one background color per column (*qv* [iTerm2 Color Schemes](https://iterm2colorschemes.com/))
+ - 4-bit transpose -- A palette with one foreground color per column
+ - 8-bit -- A palette of background colors, including the standard 16 and grayscale (*qv* [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code#8-bit))
+ - effects -- A test pattern of terminal effects
+
+### 4-bit mode (`display-colors 4-bit`)
 
 Options:
 
  - `--col-width` *`n`* -- Width of the columns in the body of the output table (default: 7)
  - `--gutter` *`string`* -- Delimiter between output columns (default: empty string)
- - `--reverse-video` -- Repeats each row using BG-color on FG-color in reverse video.  Some terminal emulators don't implement reverse video as BG-color on FG-color.  If yours does, this transformation is a no-op and this row should appear identical to the row above it
- - `--stanzas` -- Group output rows by color (default: off)
- - `--text` *`string`* -- Specifies the sample text to be displayed in each cell (default: `gYw`)
+ - `--reverse-video` -- Displays each row twice, the second time with BG-color on FG-color in reverse video.  If your terminal emulator implements reverse video by swapping background and foreground, the two lines will appear identical
+  - `--stanzas` -- Group output rows by color (default: off)
+ - `--text` *`string`* -- Specifies the sample text to be displayed in each cell (default: 'gYw')
  - `-w` *`string`*, `--weight` *`string`* -- Specifies which weight font to display and in what order (use multiple times).  Supported weights are `dim`, `default`, `medium`, `bold` and `all` (default: `default`, `bold`)
 
 This format lists background colors one per column with their SGR codes at top and left.  The default background color is the leftmost column and the topmost rows show the default foreground color.
 
 Each row is labeled on the left with its weight.  If the row is reverse video, the weight label will appear in reverse video.
 
-### Transpose mode (`--transpose`)
+### 4-bit transpose mode (`display-colors 4-bit --transpose`)
 
 Options:
 
- - `--col-width` *`n`* -- (see 'Standard mode' above)
- - `--gutter` *`string`* -- (see 'Standard mode' above)
- - `--reverse-video` -- (see 'Standard mode' above)
- - `-w` *`string`*, `--weight` *`string`* -- (see 'Standard mode' above)
+ - `--col-width` *`n`* -- (see '4-bit mode' above)
+ - `--gutter` *`string`* -- (see '4-bit mode' above)
+ - `--reverse-video` -- (see '4-bit mode' above)
+ - `-w` *`string`*, `--weight` *`string`* -- (see '4-bit mode' above)
+
+This format lists foreground colors one per column, with the default foreground color in the leftmost column and the default background color in the topmost rows.  The SGR codes are not shown and the sample text is of the form FG/BG.
+
+### 8-bit mode (`display-colors 8-bit`)
+
+This has three parts:
+
+ - 16 standard and bright colors
+ - The palette of 216 RGB colors
+ - 24 grayscale colors
+
+These are displayed as background colors.  The text in each cell is the hexadecimal value of the color code; for example, the background color of cell D8 in the test pattern is given by the ANSI escape code `\033[48;5;216m`.  The foreground colors in the test pattern are (standard) white for the darker cells and black for the lighter ones.  Some terminal emulators modify this in an attempt to improve the contrast.
+
+The text in the cells is in hexadecimal by default because it is more readable and to save space.
 
-This format lists foreground colors one per column, with the default foreground color in the leftmost column and the default background color in the topmost rows.  The SGR codes are not shown and the sample text is of the form fg/bg.
+The sixteen standard colors are presented just above their 4-bit equivalents (sometimes these are different).
 
-### Test mode (`--test`)
+The 216 RGB colors are arranged in a 6x6 cube, displayed in 6 slices with the origin at the back upper left corner.  We assign codes to them in xyz order, with the x coordinate varying first.  The x coordinate moves left to right, the y coordinate top to bottom and the z coordinate back to front.  The display shows three views of the cube, one per row: head-on sliced back to front, from above sliced top to bottom and from the left sliced left to right.  (The view in the [ANSI escape code illustration](https://en.wikipedia.org/wiki/ANSI_escape_code#8-bit) is the second of these views).
+
+From these slices you can see that the darker cells occupy the top half of the cube, the greens the back lower left corner, the reds the front upper left corner and the blues the back upper right corner.
+
+### Effects mode (`display-colors effects`)
 
 Options:
 
  - `--pattern` *`string`* -- Specify a string to use as a sample text pattern (default: '|').  Most screens will not be wide enough to accomodate a test pattern string of more than one character.  (If the pattern string contains a character that has a special meaning to the shell, like '|', it must be escaped (preceded) by a backslash: `--pattern \|`).
- - `--gutter` *`string`* -- (see 'Standard mode' above)
+ - `--gutter` *`string`* -- (see '4-bit mode' above)
 
 Displays a sample of the effect of each SGR code in all 4-bit foreground and background colors (see [Wikipedia](https://en.wikipedia.org/wiki/ANSI_escape_code#SGR_(Select_Graphic_Rendition)_parameters) for the list of SGR codes).  Some effects may be more visible in certain colors than in others.  The text samples are displayed in groups of three:
 
  1.  Without applying the effect
  2.  After turning the effect on
  3.  After turning the effect off again
 
@@ -131,27 +160,35 @@
  | GR | Bright green |
  | YE | Bright yellow |
  | BL | Bright blue |
  | MA | Bright magenta |
  | CY | Bright cyan |
  | WH | Bright white |
 
-## Examples
+## Problems
 
-Traditional palette, including all font weights, with reverse-video rows, divided into stanzas by color:
+If the terminal somehow gets into a confused state, it will not display colors correctly.  If the output of `display-colors` looks incorrect, try one of the following to reset the terminal:
 
 ```bash
-display-colors --weight all --reverse-video --stanzas
+reset
+tput reset
 ```
 
-Palette with one column per foreground color, rows ordered 'dim, medium, bold, medium' and spaces between the columns:
+## Examples
 
+Traditional 4-bit palette, including all font weights, with reverse-video rows, divided into stanzas by color:
 ```bash
-display-colors --transpose -w dim -w medium -w bold -w medium --gutter ' '
+display-colors 4-bit --weight all --reverse-video --stanzas
+```
+4-bit palette with one column per foreground color, rows ordered 'dim, medium, bold, medium' and spaces between the columns:
+```bash
+display-colors 4-bit --transpose -w dim -w medium -w bold -w medium --gutter ' '
+```
+8-bit display including standard and bright colors, 216-color RGB palette and grayscale background colors:
+```bash
+display-colors 8-bit
 ```
-
 Terminal effect test pattern with spaces between the columns:
-
 ```bash
-display-colors --test --gutter ' '
+display-colors effects --gutter ' '
 ```
```

