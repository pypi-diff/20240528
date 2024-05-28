# Comparing `tmp/prettypretty-0.2.0.tar.gz` & `tmp/prettypretty-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettypretty-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "prettypretty-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `prettypretty-0.2.0.tar` & `prettypretty-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,67 @@
--rw-r--r--   0        0        0     1891 2024-05-16 19:41:31.436717 prettypretty-0.2.0/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0     2793 2024-05-02 16:16:46.878000 prettypretty-0.2.0/.gitignore
--rw-r--r--   0        0        0      351 2024-05-08 11:44:14.092903 prettypretty-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0    11358 2024-05-10 23:06:53.590972 prettypretty-0.2.0/LICENSE
--rw-r--r--   0        0        0     2644 2024-05-17 00:06:53.091896 prettypretty-0.2.0/README.md
--rw-r--r--   0        0        0      634 2024-05-06 06:14:58.399937 prettypretty-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     1459 2024-05-16 22:39:39.714324 prettypretty-0.2.0/docs/apidocs/color.rst
--rw-r--r--   0        0        0      299 2024-05-16 19:27:36.542585 prettypretty-0.2.0/docs/apidocs/prettypretty.rst
--rw-r--r--   0        0        0     1837 2024-05-16 12:45:08.223904 prettypretty-0.2.0/docs/conf.py
--rw-r--r--   0        0        0     5390 2024-05-15 17:10:11.260351 prettypretty-0.2.0/docs/conversions.rst
--rw-r--r--   0        0        0   205416 2024-05-16 23:49:30.072296 prettypretty-0.2.0/docs/figures/rgb6-ansi-iterm2.png
--rw-r--r--   0        0        0   402258 2024-05-16 23:49:17.744169 prettypretty-0.2.0/docs/figures/rgb6-ansi-macos.png
--rw-r--r--   0        0        0   459630 2024-05-16 23:49:27.026617 prettypretty-0.2.0/docs/figures/rgb6-background.png
--rw-r--r--   0        0        0   451366 2024-05-16 23:49:25.445383 prettypretty-0.2.0/docs/figures/rgb6-text.png
--rw-r--r--   0        0        0     4210 2024-05-13 23:07:43.595548 prettypretty-0.2.0/docs/formats-and-spaces.rst
--rw-r--r--   0        0        0     3500 2024-05-17 00:07:11.716839 prettypretty-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      800 2024-05-06 06:14:58.400754 prettypretty-0.2.0/docs/make.bat
--rw-r--r--   0        0        0      319 2024-05-16 22:40:04.066388 prettypretty-0.2.0/docs/tools.rst
--rw-r--r--   0        0        0     1091 2024-05-02 16:16:18.007588 prettypretty-0.2.0/package-lock.json
--rw-r--r--   0        0        0       54 2024-05-02 16:16:09.342077 prettypretty-0.2.0/package.json
--rw-r--r--   0        0        0       22 2024-05-17 00:10:25.518484 prettypretty-0.2.0/prettypretty/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 20:14:19.249777 prettypretty-0.2.0/prettypretty/color/__init__.py
--rw-r--r--   0        0        0     3643 2024-05-15 04:46:14.229875 prettypretty-0.2.0/prettypretty/color/apca.py
--rw-r--r--   0        0        0    12096 2024-05-16 22:58:18.351293 prettypretty-0.2.0/prettypretty/color/conversion.py
--rw-r--r--   0        0        0     1865 2024-05-15 03:43:07.902917 prettypretty-0.2.0/prettypretty/color/difference.py
--rw-r--r--   0        0        0     8633 2024-05-16 22:58:25.188032 prettypretty-0.2.0/prettypretty/color/lores.py
--rw-r--r--   0        0        0     6109 2024-05-15 23:55:49.255258 prettypretty-0.2.0/prettypretty/color/serde.py
--rw-r--r--   0        0        0     7174 2024-05-15 03:48:44.497474 prettypretty-0.2.0/prettypretty/color/space.py
--rw-r--r--   0        0        0     2773 2024-05-16 04:27:39.507626 prettypretty-0.2.0/prettypretty/color/spec.py
--rw-r--r--   0        0        0      634 2024-05-05 17:58:20.659244 prettypretty-0.2.0/prettypretty/color/style.py
--rw-r--r--   0        0        0     4631 2024-05-16 04:45:02.880375 prettypretty-0.2.0/prettypretty/color/theme.py
--rw-r--r--   0        0        0     7453 2024-05-16 19:25:15.223741 prettypretty-0.2.0/prettypretty/color_object.py
--rw-r--r--   0        0        0     7796 2024-05-16 23:06:50.625401 prettypretty-0.2.0/prettypretty/grid.py
--rw-r--r--   0        0        0    15321 2024-05-16 19:34:53.347084 prettypretty-0.2.0/prettypretty/termio.py
--rw-r--r--   0        0        0      856 2024-05-16 19:44:38.278771 prettypretty-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1507 2024-05-10 00:55:29.680752 prettypretty-0.2.0/runtest.py
--rw-r--r--   0        0        0       49 2024-05-10 01:03:55.934703 prettypretty-0.2.0/test/__init__.py
--rw-r--r--   0        0        0     9112 2024-05-02 16:13:52.778390 prettypretty-0.2.0/test/runtime.py
--rw-r--r--   0        0        0    10115 2024-05-16 19:30:16.747923 prettypretty-0.2.0/test/test_color.py
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 prettypretty-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      620 2024-05-25 10:22:25.520563 prettypretty-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1942 2024-05-27 04:44:51.795424 prettypretty-0.8.0/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0     2793 2024-05-02 16:16:46.878000 prettypretty-0.8.0/.gitignore
+-rw-r--r--   0        0        0      351 2024-05-08 11:44:14.092903 prettypretty-0.8.0/.vscode/settings.json
+-rw-r--r--   0        0        0    11358 2024-05-10 23:06:53.590972 prettypretty-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3725 2024-05-28 00:03:54.966717 prettypretty-0.8.0/README.md
+-rw-r--r--   0        0        0      634 2024-05-06 06:14:58.399937 prettypretty-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0     2306 2024-05-23 06:12:03.706335 prettypretty-0.8.0/docs/apidocs/color.rst
+-rw-r--r--   0        0        0      767 2024-05-26 05:00:12.087062 prettypretty-0.8.0/docs/apidocs/prettypretty.rst
+-rw-r--r--   0        0        0      314 2024-05-26 05:00:49.208948 prettypretty-0.8.0/docs/apidocs/tools.rst
+-rw-r--r--   0        0        0     1901 2024-05-27 03:20:00.407669 prettypretty-0.8.0/docs/conf.py
+-rw-r--r--   0        0        0     7944 2024-05-20 04:38:13.061007 prettypretty-0.8.0/docs/conversions.rst
+-rw-r--r--   0        0        0    18285 2024-05-26 04:30:28.459202 prettypretty-0.8.0/docs/figures/progress-bar-dark.png
+-rw-r--r--   0        0        0    18260 2024-05-26 04:30:28.551592 prettypretty-0.8.0/docs/figures/progress-bar-light.png
+-rw-r--r--   0        0        0   205416 2024-05-16 23:49:30.072296 prettypretty-0.8.0/docs/figures/rgb6-ansi-iterm2.png
+-rw-r--r--   0        0        0   402258 2024-05-16 23:49:17.744169 prettypretty-0.8.0/docs/figures/rgb6-ansi-macos.png
+-rw-r--r--   0        0        0   478158 2024-05-19 12:36:09.853510 prettypretty-0.8.0/docs/figures/rgb6-ansi-ubuntu.png
+-rw-r--r--   0        0        0   459630 2024-05-16 23:49:27.026617 prettypretty-0.8.0/docs/figures/rgb6-background.png
+-rw-r--r--   0        0        0   451366 2024-05-16 23:49:25.445383 prettypretty-0.8.0/docs/figures/rgb6-text.png
+-rw-r--r--   0        0        0    69476 2024-05-18 16:43:08.695397 prettypretty-0.8.0/docs/figures/slice-b00-reduced.png
+-rw-r--r--   0        0        0    78615 2024-05-18 16:43:08.797879 prettypretty-0.8.0/docs/figures/slice-b00.png
+-rw-r--r--   0        0        0    66834 2024-05-18 16:43:08.882545 prettypretty-0.8.0/docs/figures/slice-bff-reduced.png
+-rw-r--r--   0        0        0    78888 2024-05-18 16:43:08.977646 prettypretty-0.8.0/docs/figures/slice-bff.png
+-rw-r--r--   0        0        0    64380 2024-05-18 16:43:09.080046 prettypretty-0.8.0/docs/figures/slice-g00-reduced.png
+-rw-r--r--   0        0        0    80965 2024-05-18 16:43:09.176459 prettypretty-0.8.0/docs/figures/slice-g00.png
+-rw-r--r--   0        0        0    67376 2024-05-18 16:43:09.281319 prettypretty-0.8.0/docs/figures/slice-gff-reduced.png
+-rw-r--r--   0        0        0    75597 2024-05-18 16:43:09.442358 prettypretty-0.8.0/docs/figures/slice-gff.png
+-rw-r--r--   0        0        0    64235 2024-05-18 16:43:09.544805 prettypretty-0.8.0/docs/figures/slice-r00-reduced.png
+-rw-r--r--   0        0        0    77821 2024-05-18 16:43:09.639053 prettypretty-0.8.0/docs/figures/slice-r00.png
+-rw-r--r--   0        0        0    65937 2024-05-18 16:43:09.735657 prettypretty-0.8.0/docs/figures/slice-rff-reduced.png
+-rw-r--r--   0        0        0    84569 2024-05-18 16:43:09.838889 prettypretty-0.8.0/docs/figures/slice-rff.png
+-rw-r--r--   0        0        0     1450 2024-05-17 03:31:16.000000 prettypretty-0.8.0/docs/figures/social.png
+-rw-r--r--   0        0        0     5529 2024-05-26 09:44:58.023713 prettypretty-0.8.0/docs/formats-and-spaces.rst
+-rw-r--r--   0        0        0     2062 2024-05-23 11:18:32.984627 prettypretty-0.8.0/docs/hires-slices.rst
+-rw-r--r--   0        0        0    14706 2024-05-27 15:38:33.666475 prettypretty-0.8.0/docs/howto-color.rst
+-rw-r--r--   0        0        0     8294 2024-05-27 15:32:43.865199 prettypretty-0.8.0/docs/howto-style.rst
+-rw-r--r--   0        0        0     5189 2024-05-28 00:01:23.869575 prettypretty-0.8.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-06 06:14:58.400754 prettypretty-0.8.0/docs/make.bat
+-rw-r--r--   0        0        0     1091 2024-05-02 16:16:18.007588 prettypretty-0.8.0/package-lock.json
+-rw-r--r--   0        0        0       99 2024-05-25 09:25:41.296822 prettypretty-0.8.0/package.json
+-rw-r--r--   0        0        0       22 2024-05-27 23:50:47.749838 prettypretty-0.8.0/prettypretty/__init__.py
+-rw-r--r--   0        0        0     6120 2024-05-24 17:57:35.468842 prettypretty-0.8.0/prettypretty/ansi.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:14:19.249777 prettypretty-0.8.0/prettypretty/color/__init__.py
+-rw-r--r--   0        0        0     3643 2024-05-15 04:46:14.229875 prettypretty-0.8.0/prettypretty/color/apca.py
+-rw-r--r--   0        0        0    12080 2024-05-25 03:24:12.056694 prettypretty-0.8.0/prettypretty/color/conversion.py
+-rw-r--r--   0        0        0     1865 2024-05-18 06:41:01.091536 prettypretty-0.8.0/prettypretty/color/difference.py
+-rw-r--r--   0        0        0     3693 2024-05-23 07:35:50.287446 prettypretty-0.8.0/prettypretty/color/equality.py
+-rw-r--r--   0        0        0     3658 2024-05-23 00:45:28.162403 prettypretty-0.8.0/prettypretty/color/gamut.py
+-rw-r--r--   0        0        0    10279 2024-05-25 03:23:45.019835 prettypretty-0.8.0/prettypretty/color/lores.py
+-rw-r--r--   0        0        0     9952 2024-05-23 04:34:48.169172 prettypretty-0.8.0/prettypretty/color/object.py
+-rw-r--r--   0        0        0     6806 2024-05-23 04:46:08.092965 prettypretty-0.8.0/prettypretty/color/serde.py
+-rw-r--r--   0        0        0    10807 2024-05-24 15:36:40.921925 prettypretty-0.8.0/prettypretty/color/space.py
+-rw-r--r--   0        0        0     4429 2024-05-26 20:41:40.797123 prettypretty-0.8.0/prettypretty/color/spec.py
+-rw-r--r--   0        0        0     5977 2024-05-26 04:07:36.104292 prettypretty-0.8.0/prettypretty/color/theme.py
+-rw-r--r--   0        0        0     4113 2024-05-27 15:59:36.123814 prettypretty-0.8.0/prettypretty/darkmode.py
+-rw-r--r--   0        0        0     9956 2024-05-27 07:26:36.986605 prettypretty-0.8.0/prettypretty/fidelity.py
+-rw-r--r--   0        0        0     9829 2024-05-27 23:50:03.558368 prettypretty-0.8.0/prettypretty/grid.py
+-rw-r--r--   0        0        0     2770 2024-05-27 14:53:45.400891 prettypretty-0.8.0/prettypretty/progress.py
+-rw-r--r--   0        0        0        0 2024-05-20 19:14:47.717105 prettypretty-0.8.0/prettypretty/py.typed
+-rw-r--r--   0        0        0    18950 2024-05-27 14:41:01.300755 prettypretty-0.8.0/prettypretty/style.py
+-rw-r--r--   0        0        0    40222 2024-05-27 23:54:48.841066 prettypretty-0.8.0/prettypretty/terminal.py
+-rw-r--r--   0        0        0      881 2024-05-27 04:45:59.226719 prettypretty-0.8.0/pyproject.toml
+-rwxr-xr-x   0        0        0     2599 2024-05-25 10:37:17.733888 prettypretty-0.8.0/runtest.py
+-rw-r--r--   0        0        0       49 2024-05-10 01:03:55.934703 prettypretty-0.8.0/test/__init__.py
+-rw-r--r--   0        0        0     9613 2024-05-25 09:22:31.550743 prettypretty-0.8.0/test/runtime.py
+-rw-r--r--   0        0        0    13464 2024-05-25 00:38:12.416240 prettypretty-0.8.0/test/test_color.py
+-rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 prettypretty-0.8.0/PKG-INFO
```

### Comparing `prettypretty-0.2.0/.github/workflows/gh-pages.yml` & `prettypretty-0.8.0/.github/workflows/gh-pages.yml`

 * *Files 7% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 
     - name: Set up Python 3.12
       uses: actions/setup-python@v5
       with:
         python-version: "3.12"
         cache: "pip"
 
-    - name: Install Sphinx & Autoprogram, Design, RTD Theme
+    - name: Install Sphinx & Autoprogram, Copy Button, Design, RTD Theme
       run: |
         python -m pip install --upgrade pip
-        pip install sphinx sphinxcontrib-autoprogram sphinx_design sphinx-rtd-theme
+        pip install sphinx sphinxcontrib-autoprogram
+        pip install sphinx-copybutton sphinx_design sphinx-rtd-theme
 
     - name: Set up Pages
       id: pages
       uses: actions/configure-pages@v5
 
     - name: Build documentation
       run: |
```

### Comparing `prettypretty-0.2.0/.gitignore` & `prettypretty-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/LICENSE` & `prettypretty-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/README.md` & `prettypretty-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Prettypretty
 
-Prettypretty is a Python package for building awesome terminal user interfaces.
+[![Run Tests](https://github.com/apparebit/prettypretty/actions/workflows/ci.yml/badge.svg)](https://github.com/apparebit/prettypretty/actions/workflows/ci.yml)
+[![Publish to GitHub Pages](https://github.com/apparebit/prettypretty/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/apparebit/prettypretty/actions/workflows/gh-pages.yml)
 
+Prettypretty helps build awesome terminal user interfaces in Python. Notably, it
+incorporates a powerful and general color library. The resulting, near seemless
+integration of 1970s archaic but beloved ANSI escape codes for terminal styling
+with 2020s color science, notably via the [Oklab perceptual color
+space](https://bottosson.github.io/posts/oklab/), is unique to prettypretty and
+enables your application to easily adapt its visual styles to a user's current
+color theme, dark or light mode, and color preferences. So, what are you waiting
+for? Switch to prettypretty for all your terminal styling needs. Prettypretty is
+awesome!
+
+\[ [Repository](https://github.com/apparebit/prettypretty)
+| [Package](https://pypi.org/project/prettypretty/)
+| [Documentation](https://apparebit.github.io/prettypretty/)
+\]
 
 ## Prettypretty Illustrated
 
 The first screenshot illustrates prettypretty's support for maximizing text
 contrast by comparing against backgrounds in all 216 colors from the 6x6x6 RGB
 cube of 8-bit terminal colors.
```

### Comparing `prettypretty-0.2.0/docs/Makefile` & `prettypretty-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/docs/conf.py` & `prettypretty-0.8.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 sys.path.insert(0, os.path.abspath('..'))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'prettypretty'
-copyright = '© 2024 Robert Grimm'
+copyright = '2024 Robert Grimm'
 author = 'Robert Grimm'
 
 # Source order is nicer than alphabetizing fields and methods.
 autodoc_member_order = 'bysource'
 
 # Known types are linked, so the fully qualified name adds mostly noise.
 python_use_unqualified_type_names = True
@@ -32,21 +32,23 @@
 extensions = [
     "sphinx.ext.napoleon",
     "sphinx.ext.autodoc",
     #"sphinx.ext.intersphinx",
     #"sphinx.ext.extlinks",
     "sphinx.ext.viewcode",
     "sphinxcontrib.autoprogram",
+    "sphinx_copybutton",
     "sphinx_design",
     "sphinx_rtd_theme",
 ]
 
 napoleon_include_init_with_doc = True
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+copybutton_exclude = '.linenos, .gp, .go'
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 #html_theme = "sphinxawesome"
 html_static_path = ['_static']
 html_theme = 'sphinx_rtd_theme'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prettypretty-0.2.0/docs/conversions.rst` & `prettypretty-0.8.0/docs/conversions.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Color Conversions
 =================
 
+.. warning::
+
+   Converting colors between color spaces is not guaranteed to result in colors
+   that are within the target color space's gamut. For example, ``p3(0, 1, 0)``
+   (to use prettypretty's function syntax for colors) is well outside of sRGB's
+   gamut. Like Color.js, prettypretty does *not* automatically clip or gamut-map
+   colors and instead preserves their out-of-gamut coordinates. Hence a primary
+   green in P3 converts to ``srgb(-0.5116, 1.0183, -0.31067)``, with G slightly
+   out of gamut and R and B very much out of gamut.
+
+   In other words, if you need in-gamut colors, you *must* explicitly clip or
+   gamut-map colors.
+
+
 For starters, we consider only color formats and spaces that are *not*
 terminal-specific.
 
 With exception of the XYZ color space, all other color formats and spaces have a
 *base* color space, which may be XYZ. Taking together, they form a tree with XYZ
 as root. For every such color format or space, prettypretty also includes
 handwritten functions that convert from and to the base color space. For
@@ -65,30 +79,61 @@
 ``ansi``, ``eight_bit``, and ``rgb6``, is the same as for the other color
 formats and spaces: For each terminal-specific color format, we write a pair of
 functions that convert to and from higher-resolution color. By putting those
 functions first and/or last in the sequence of conversions and otherwise routing
 as described above, we can convert between all color formats and spaces,
 terminal-specific formats included.
 
-In practice, however, there are a few complications:
+In practice, however, there are several complications:
 
- 1. The extended ANSI colors have no widely accepted mapping to high-resolution
-    colors and usually are configured through themes. Hence prettypretty also
-    supports color themes. The colors of VGA text mode provide the default.
- 2. With theme support in place, converting low-resolution colors to
-    higher-resolution RGB256 is straightforward. In particular, xterm's formulae
-    for converting the 6x6x6 RGB cube and 24-step gray gradient embedded in
-    8-bit color are widely used.
- 3. However, there are no good formulae for converting RGB256 back to
-    low-resolution. To yield good results, prettypretty performs the
-    downconversion in Oklab, finding the closest color amongst the 16 extended
-    ANSI colors when converting to ANSI, the 240 RGB6 and gray gradient colors
-    when converting to 8-bit, and the 216 RGB6 colors when converting to RGB6.
-    The conversion to 8-bit colors ignores the 16 ANSI colors because they stick
-    out when converting gradients of color.
- 4. While not excessively large, the look-up tables for downconversion are
-    created only on demand and thereafter cached.
- 5. Similarly, the modules for low-resolution color conversions and color themes
-    aren't particularly large. Still, the module implementing generic
-    conversions only loads the module implementing low-resolution color
-    operations when strictly needed. That nicely avoids an error due to circular
-    module dependencies as well.
+ 1. The 16 extended ANSI colors have no widely accepted mapping to
+    high-resolution colors and usually are configured through themes. Colors are
+    usually specified in ``#<hexdigits>`` notation, i.e., RGB256.
+ 2. Xterm's formulae for converting the 6x6x6 RGB cube and 24-step gray gradient
+    *to* RGB256 are widely accepted. But there are no established techniques for
+    converting back.
+ 3. Prettypretty's color themes are a form of state duplication, with all
+    attendant problems. Notably, if a manually configured theme does not match
+    the terminal's current theme, the results of color manipulation may just
+    look awful.
+ 4. ANSI escape sequences support querying the terminal for currently configured
+    colors. But the results are in xterm's ``rgb:`` notation with *four*
+    hexadecimal digits per coordinate, which is well beyond RGB256's resolution.
+
+Prettypretty indeed addresses the fundamental conversion challenge for the 16
+extended ANSI colors by supporting color themes, with each color having an
+arbitrary color format or space. Since manual color theme configuration is
+problematic, it also supports dynamically querying terminals for configured
+colors and preserves the resolution of the responses as sRGB colors.
+
+To convert low-resolution to high-resolution colors, prettypretty currently
+targets sRGB as the "base" color space for all low-resolution colors. For the
+6x6x6 RGB cube and 24-step gray gradient, it simply uses the established
+formulae to convert to RGB256 and then performs the trivial conversion to sRGB.
+For the 16 extended ANSI colors, it looks up the target color in the current
+color theme and, if it is not RGB256 or sRGB, does a high-resolution conversion
+to sRGB. Since high-resolution conversion does not clip or gamut-map colors,
+this conversion does preserve the represented color. The result should probably
+be cached, but it currently is not.
+
+For converting high-resolution to low-resolution colors, there is not
+established algorithm. Since the low-resolution colors, by definition, do not
+comprise that many colors, exhaustive search becomes a realistic possibility and
+is just the technique used by prettypretty. In particular, prettypretty compares
+the high-resolution source color with high-resolution versions of all
+low-resolution colors (thus assuming that the conversion from low-resolution to
+high-resolution is functional) and returns the color with the smallest distance.
+All comparisons are performed in Oklab, which is perceptually uniform.
+
+To speed up conversion to low-resolution color, prettypretty uses look-up tables
+for the Oklab-equivalent colors. Those tables are initialized lazily, on demand.
+When targeting 8-bit color, prettypretty does not include the 16 extended ANSI
+colors as candidates because experiments with color gradients resulted in
+low-resolution gradients disrupted by one of those 16 colors, which just
+happened to be closer.
+
+The exhaustive search for closest matching low-resolution color may still
+produce suboptimal results because it optimizes for Euclidian distance in Oklab.
+In other words, it treats a difference in lightness just as it treats the same
+difference in one of the two color axes. That may indeed be the right approach
+for small color differences but it's not clear that is the right approach at the
+granularity of 8-bit colors.
```

### Comparing `prettypretty-0.2.0/docs/figures/rgb6-ansi-iterm2.png` & `prettypretty-0.8.0/docs/figures/rgb6-ansi-iterm2.png`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/docs/figures/rgb6-ansi-macos.png` & `prettypretty-0.8.0/docs/figures/rgb6-ansi-macos.png`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/docs/figures/rgb6-background.png` & `prettypretty-0.8.0/docs/figures/rgb6-background.png`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/docs/figures/rgb6-text.png` & `prettypretty-0.8.0/docs/figures/rgb6-text.png`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/docs/formats-and-spaces.rst` & `prettypretty-0.8.0/docs/formats-and-spaces.rst`

 * *Files 19% similar despite different names*

```diff
@@ -12,29 +12,40 @@
 RGB color spaces are based on an additive color model, with the overall color
 being the sum of the colors of the component lights. Every RGB color space has
 three coordinates ``r``, ``g``, and ``b``, which range from 0 to 1, inclusive,
 for in-gamut colors. The supported RGB color spaces are:
 
   * **srgb** is the default, gamma-corrected color space of the web, sRGB
   * **linear_srgb** is the linear version of sRGB, without gamma correction
-  * **p3** is the larger P3 color space, with gamma correction
+  * **p3** is the larger Display P3 color space, with gamma correction
   * **linear_p3** is the linear version of P3, without gammar correction
 
-sRGB and P3 use the same gamma correction, hence :func:`.p3_to_linear_p3` is
-just an alias to :func:`.srgb_to_linear_srgb` and :func:`.linear_p3_to_p3` is
-just an alias to :func:`.linear_srgb_to_srgb`.
+sRGB and Display P3 use the same gamma correction, hence
+:func:`.p3_to_linear_p3` is just an alias to :func:`.srgb_to_linear_srgb` and
+:func:`.linear_p3_to_p3` is just an alias to :func:`.linear_srgb_to_srgb`. Alas,
+even though the numeric transformations are the same, the coordinate spaces are
+*not*. Identical coordinates in sRGB and Display P3 usually are different
+colors, though black (at 0, 0, 0) and white (at 1, 1, 1) have the same
+coordinates in both color spaces.
 
-Prettypretty supports the following non-RGB color spaces:
+Prettypretty also supports the following non-RGB color spaces:
 
   * **xyz** is the XYZ color space with the D65 standard illuminant
   * **oklab** is a perceptually uniform color space, with ``L`` standing for
     lightness and ``a``/``b`` serving as orthogonal color axes
   * **oklch** is a cylindrical version of Oklab, with ``L`` standing for
     lightness, ``C`` for chroma, and ``h`` for hue.
 
+sRGB, Display P3, Oklab, and Oklch share the same white point, D65, and hence
+are defined relative to the D65 version of the XYZ color space and not the
+original D50 version of XYZ. For now, there is no reason to support chromatic
+adaptation between illuminants. However, since Lab and Lch use D50 as white
+point, adding support for these two color spaces would entail also adding
+support for chromatic adaptation.
+
 In Oklab, the difference ΔE between two colors is just the Euclidian distance.
 Though Oklab's designer, Björn Ottosson, has suggested that a more accurate ΔE
 should scale Δa and Δb by a constant factor of around 2.1 before squaring.
 Prettypretty implements both versions, like Color.js using a factor of 2 for
 version 2 for now.
 
 
@@ -48,16 +59,16 @@
     coordinate being an integer between 0 and 255, inclusive
 
 There is one terminal-specific RGB format:
 
   * **rgb6** is an RGB color, with each coordinate being an integer between
     0 and 5, inclusive
 
-Finally, there are two more terminal-specific color formats with a single
-integer coordinate:
+There also are two more terminal-specific color formats with a single integer
+coordinate:
 
   * **ansi** is an integer between 0 and 15, inclusive, denoting one of the
     sixteen extended ANSI colors
   * **eight_bit** is an integer between 0 and 255, inclusive, denoting one
     of the 8-bit colors:
 
       * 0–15 are the sixteen extended ANSI colors
@@ -69,30 +80,44 @@
 standardized names but not color values. Furthermore, almost all terminals have
 robust support for customizing just those colors through themes. Consequently,
 any conversion from and to ANSI colors must take the color theme into account,
 too. Prettypretty does just that, even supporting arbitrary color spaces for
 theme colors.
 
 
+A Total Lack of Color
+---------------------
+
+At first, terminals were monochrome with a 1-bit color depth. In fact, even
+though DEC's VT100 popularized ANSI escape codes, none of the models in that
+line supported colors. It was all light text against a dark background. To
+account for such a total lack of color, prettypretty defines one more "color
+space":
+
+  * **nocolor** technically corresponds to 1-bit monochrome displays, though
+    it primarily serves as an abstract label indicating a lack of color.
+
+
 Color Serde
 -----------
 
-Prettypretty supports two formats for both serialization to and deserialization
-from strings:
+Prettypretty supports three formats for both serialization to and
+deserialization from strings:
 
+  * **f** for function uses the color's format or space tag as function name and
+    the comma-separated coordinates as arguments: e.g., ``rgb256(128, 64, 0)``.
   * **h** for hexadecimal is the hash-prefixed color format familiar from the
-    web
+    web: e.g., ``#804000``.
   * **x** for X Windows or xterm uses the `rgb:` and `rgbi:` prefixes followed
     by three slash-separated coordinates in hexadecimal for `rgb:` and floating
-    point for `rgbi:`
+    point for `rgbi:`, e.g., ``rgb:80/40/00`` or ``rgbi:0.5/0.25/0``
 
-For serialization to strings, prettypretty supports two additional formats:
+For serialization to strings, prettypretty supports one additional format:
 
-  * **f** for function uses one of the above format or color space tags as
-    function name and the comma-separated coordinates as arguments
   * **s** for CSS uses ``color()``, ``oklab()``, ``oklch()``, or ``rgb()``
     notation with space-separated coordinates
 
-The four letters serve as format identifiers for colors in Python's f-strings.
-However, only RGB256 colors can be serialized in h-format or the ``rgb:``
-prefixed x-format; only sRGB colors can be serialized in the ``rgb:`` prefixed
-x-format; and the s-format cannot serialize ``linear_p3`` colors.
+The boldfaced letters serve as format identifiers for `color objects <.Color>`
+in Python's f-strings. However, only RGB256 colors can be serialized in h-format
+or the ``rgb:`` prefixed x-format; only sRGB colors can be serialized in the
+``rgb:`` prefixed x-format; and the c-format cannot serialize ``linear_p3``
+colors.
```

### Comparing `prettypretty-0.2.0/docs/make.bat` & `prettypretty-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/package-lock.json` & `prettypretty-0.8.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/prettypretty/color/apca.py` & `prettypretty-0.8.0/prettypretty/color/apca.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/prettypretty/color/conversion.py` & `prettypretty-0.8.0/prettypretty/color/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     """
     Instantiate a closure that applies the given conversions. Doing so in a
     dedicated top-level function keeps the closure environment minimal.
     """
     def converter(*coordinates: float) -> CoordinateSpec:
         value = cast(CoordinateSpec, coordinates)
         for fn in conversions:
-            value = fn(*value)  # type: ignore
+            value = fn(*value)
         return value
     return cast(ConverterSpec, converter)
 
 
 _LORES_FORMAT = {'ansi', 'eight_bit', 'rgb6'}
 
 _converter_cache: dict[str, dict[str, ConverterSpec]] = {}
```

### Comparing `prettypretty-0.2.0/prettypretty/color/difference.py` & `prettypretty-0.8.0/prettypretty/color/difference.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.2.0/prettypretty/color/lores.py` & `prettypretty-0.8.0/prettypretty/color/lores.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         theme. After all, the current theme determines the RGB256 values for all
         extended ANSI colors.
     """
     assert 0 <= color <= 15
     c = current_theme().ansi(color)
 
     assert c.tag == 'rgb256'
-    return c.coordinates  # type: ignore
+    return cast(tuple[int, int, int], c.coordinates)
 
 
 def _eight_bit_gray_to_rgb256(color: int) -> tuple[int, int, int]:
     """Convert the given 8-bit gray to RGB256 format."""
     assert 232 <= color <= 255
     c = 10 * (color - 232) + 8
     return c, c, c
@@ -154,37 +154,42 @@
 
 def rgb6_to_srgb(r: int, g: int, b: int) -> tuple[float, float, float]:
     """Convert the given color in RGB6 format to sRGB format."""
     assert 0 <= r <= 5 and 0 <= g <= 5 and 0 <= b <= 5
     return _rgb256_to_srgb(*rgb6_to_rgb256(r, g, b))
 
 
+def _eight_bit_gray_to_srgb(color: int) -> tuple[float, float, float]:
+    """Convert the given 8-bit gray to sRGB."""
+    return _rgb256_to_srgb(*_eight_bit_gray_to_rgb256(color))
+
+
 def eight_bit_to_srgb(color: int) -> tuple[float, float, float]:
     """
     Convert the given 8-bit terminal color to sRGB.
 
     .. warning::
         The result of this function may depend on the current color theme.
         It provides RGB256 color values for 8-bit colors 0–15, i.e., the
         extended ANSI colors.
     """
     if 0 <= color <= 15:
         return ansi_to_srgb(color)
     if 16 <= color <= 231:
         return _rgb256_to_srgb(*rgb6_to_rgb256(*eight_bit_to_rgb6(color)))
     if 232 <= color <= 255:
-        return _rgb256_to_srgb(*_eight_bit_gray_to_rgb256(color))
+        return _eight_bit_gray_to_srgb(color)
 
     raise ValueError(f'{color} is not a valid 8-bit terminal color')
 
 
 # --------------------------------------------------------------------------------------
 
 
-_RGB256_TO_OKLAB = Callable[[int, int, int], tuple[float, float, float]]
+_RGB256_TO_OKLAB = Callable[[float, float, float], tuple[float, float, float]]
 
 class _LUT:
 
     def __init__(self) -> None:
         self._ansi: dict[Theme, CoordinateVectorSpec] = {}
         self._rgb: None | CoordinateVectorSpec = None
         self._gray: None | CoordinateVectorSpec = None
@@ -199,33 +204,33 @@
 
     @property
     def ansi(self) -> CoordinateVectorSpec:
         theme = current_theme()
         if theme not in self._ansi:
             self._ansi[theme] = tuple(
                 (self.convert if c.tag == 'srgb' else get_converter(c.tag, 'oklab'))
-                (*c.coordinates)  # type: ignore
+                (*c.coordinates)
                 for n, c in theme.colors() if n not in ('text', 'background')
             )
         return self._ansi[theme]
 
     @property
     def rgb(self) -> CoordinateVectorSpec:
         if self._rgb is None:
             self._rgb = tuple(
-                self.convert(*rgb6_to_rgb256(r, g, b))
+                self.convert(*rgb6_to_srgb(r, g, b))
                 for r in range(6) for g in range(6) for b in range(6)
             )
         return self._rgb
 
     @property
     def gray(self) -> CoordinateVectorSpec:
         if self._gray is None:
             self._gray = tuple(
-                self.convert(*_eight_bit_gray_to_rgb256(c))
+                self.convert(*_eight_bit_gray_to_srgb(c))
                 for c in range(232, 256)
             )
         return self._gray
 
 _look_up_table = _LUT()
 
 
@@ -253,7 +258,47 @@
 
     .. warning::
         The result of this function critically depends on the current color
         theme. It provides an implicit input in addition to the arguments.
     """
     index, _ = closest_oklab((L, a, b), _look_up_table.ansi)
     return index,
+
+
+# --------------------------------------------------------------------------------------
+
+
+def naive_eight_bit_to_ansi(color: int) -> tuple[int]:
+    """
+    Perform the naive RGB component conversion from 8-bit to ANSI colors.
+
+    This function maps 6x6x6 RGB colors and the 24-step gray gradient to the 16
+    extended ANSI colors:
+
+     1. It converts the input color to a 3-bit RGB color.
+     2. If the sum of the components exceeds some threshold, it makes the 3-bit
+        color a bright color.
+
+    Alas, if the sum of the components uses the 3-bit RGB color, possible
+    thresholds 0—3 simply are too coarse. Instead the implementation uses
+    performs downsampling in floating point and retains the resulting normal
+    values for summation during the second step. A threshold of 1.8 has been
+    experimentally validated as reasonable.
+
+    Arguably, this isn't the naive conversion any more. For example, the chalk
+    library implements an `even more naive version
+    <https://github.com/chalk/chalk/blob/main/source/vendor/ansi-styles/index.js>`_.
+    """
+    if 0 <= color <= 15:
+        return color,
+
+    if 16 <= color <= 231:
+        r, g, b = tuple(c / 5 for c in eight_bit_to_rgb6(color))
+    elif 232 <= color <= 255:
+        r = g = b = (color - 232) / 23
+    else:
+        raise ValueError(f'{color} is not a valid 8-bit terminal color')
+
+    color = 4 * round(b) + 2 * round(g) + round(r)
+    if r + g + b >= 1.8:
+        color += 8
+    return color,
```

### Comparing `prettypretty-0.2.0/prettypretty/grid.py` & `prettypretty-0.8.0/prettypretty/grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """
 A script to visualize 8-bit terminal colors as well as prettypretty's support
 for down-sampling colors and maximizing contrast.
 """
 import argparse
 import os
+from typing import Literal
 
+from .ansi import Layer
 from .color.conversion import get_converter
 from .color.apca import use_black_text, use_black_background
 from .color.lores import (
     rgb6_to_eight_bit,
     rgb6_to_srgb,
     eight_bit_to_srgb,
     oklab_to_ansi,
     oklab_to_eight_bit,
+    naive_eight_bit_to_ansi,
 )
-from .color.theme import MACOS_TERMINAL, VGA, XTERM, current_theme
-from .color.style import eight_bit_to_sgr_params, Layer, sgr
-from .termio import TermIO
+from .color.theme import MACOS_TERMINAL, VGA, XTERM, builtin_theme_name, current_theme
+from .terminal import Terminal
 
 
 class FramedBoxes:
     """
-    Boxes in a frame.
+    Emit boxes in a frame.
 
-    This class helps with incrementally formatting a grid of boxes with a
+    This class helps with incrementally emitting a grid of boxes with a
     surrounding frame (or border). Each box has the same width and a height of
     one line. Boxes are formatted left-to-right.
     """
-    width: int
-    box_count: int
-    box_width: int
-    fragments: list[str]
-
-    def __init__(self, width: int, box_count: int = 1, min_width: int = 5) -> None:
+    def __init__(self, term: Terminal, box_count: int = 1, min_width: int = 5) -> None:
+        self._term = term
         self._box_count = box_count
-        self._box_width = (width - 2) // box_count
+        self._box_width = (term.width - 2) // box_count
         if self._box_width < min_width:
-            raise ValueError(f'unable to fit {box_count} boxes into {width} columns')
+            raise ValueError(
+                f'unable to fit {box_count} boxes into {term.width} columns'
+            )
         self._width = self._box_count * self._box_width + 2
-        self._fragments: list[str] = []
+        self._indent = (term.width - self.outer_width) // 2
         self._line_content_width = 0
 
     @property
     def outer_width(self) -> int:
         """The total width of the frame."""
         return self._width
 
@@ -57,159 +57,187 @@
         """Format the top of the frame."""
         title = f' {t} ' if (t := title.strip()) != '' else t
         filling = self.outer_width - 4 - len(title)
         if filling < 0:
             raise ValueError(f'"{title}" is too long for {self.outer_width}-wide frame')
         if title:
             title = f'\x1b[1m{title}\x1b[m'
-        self._fragments.append(f'┏━{title}{"━" * filling}━┓\n')
+        self._term.writeln(f'{" " * self._indent}┏━{title}{"━" * filling}━┓')
 
     def left(self) -> None:
         """Start formatting a line of content."""
-        self._fragments.append('┃')
         if self._line_content_width != 0:
             raise ValueError('Line started before line ended')
+        self._term.write(f'{" " * self._indent}┃')
 
     def box(
         self,
         text: str,
         foreground: tuple[int] | tuple[int, int, int],
         background: tuple[int] | tuple[int, int, int]
     ) -> None:
         """Format one box of the content."""
         box = text.center(self._box_width)
         if len(box) != self._box_width:
             raise ValueError(f'"{text}" does not fit into {self._box_width}-wide box')
 
-        if len(background) == 1:
-            bg_params = eight_bit_to_sgr_params(*background, Layer.BACKGROUND)
-        else:
-            bg_params = 48, 2, *background
-
-        if len(foreground) == 1:
-            fg_params = eight_bit_to_sgr_params(*foreground, Layer.TEXT)
-        else:
-            fg_params = 38, 2, *foreground
-
-        self._fragments.append(f'{sgr(*bg_params, *fg_params)}{box}\x1b[m')
+        self._term.fg(*foreground).bg(*background).write(box)
         self._line_content_width += self._box_width
 
     def right(self) -> None:
         """Complete formatting a line of content."""
+        self._term.reset_style()
+        self._term.writeln('┃')
+
         if self._line_content_width != self.inner_width:
             raise ValueError(
                 f'content spans {self._line_content_width}, '
                 f'not {self.inner_width} columns'
             )
 
-        self._fragments.append('┃\n')
         self._line_content_width = 0
 
     def bottom(self) -> None:
         """Format the bottom of the frame."""
-        self._fragments.append(f'┗{"━" * self.inner_width}┛')
+        self._term.writeln(f'{" " * self._indent}┗{"━" * self.inner_width}┛')
 
-    def __str__(self) -> str:
-        return ''.join(self._fragments)
 
-
-def format_color_cube(
-    width: int,
+def write_color_cube(
+    term: Terminal,
     *,
     layer: Layer = Layer.BACKGROUND,
-    ansi_only: bool = False,
-) -> str:
+    strategy: Literal['8bit', 'pretty', 'naive'] = '8bit',
+    label: bool = True,
+) -> None:
     """
     Format a framed grid with 216 cells, where each cell displays a distinct
     color from the 6x6x6 cube of 8-bit terminal colors.
 
     Args:
-        width: is the number of columns available to the framed grid
+        term: is the terminal for write the framed grid to
         layer: determines whether to color text or background, with background
             the default
-        ansi_only: determines whether to down-sample the 8-bit color to an
-            extended ANSI color
-
-    Returns:
-        The fully formated and framed grid
+        strategy: determines whether to display the original 8-bit colors, to
+            downsample using prettypretty, or to use the naive RGB conversion
+        label: determines whether boxes are labelled with their color
+            components
     """
-    frame = FramedBoxes(width, 6)
+    frame = FramedBoxes(term, 6)
+
+    prefix = (
+        'Original ' if strategy == '8bit'
+        else 'Pretty Compression of ' if strategy == 'pretty'
+        else 'Naive Compression of '
+    )
+
     frame.top(
         layer.name.capitalize()
         + ': '
-        + ('Downsampled ' if ansi_only else '')
+        + prefix
         + '6•6•6 RGB Cube'
     )
 
     srgb_to_oklab = get_converter('srgb', 'oklab')
 
     for r in range(6):
         for b in range(6):
             frame.left()
 
             for g in range(6):
                 srgb = rgb6_to_srgb(r, g, b)
 
-                if ansi_only:
+                if strategy == '8bit':
+                    eight_bit = rgb6_to_eight_bit(r, g, b)
+                elif strategy == 'pretty':
                     eight_bit = oklab_to_ansi(*srgb_to_oklab(*srgb))
                     srgb = eight_bit_to_srgb(*eight_bit)
+                elif strategy == 'naive':
+                    eight_bit = naive_eight_bit_to_ansi(*rgb6_to_eight_bit(r, g, b))
+                    srgb = eight_bit_to_srgb(*eight_bit)
                 else:
-                    eight_bit = rgb6_to_eight_bit(r, g, b)
+                    raise ValueError(f'invalid strategy "{strategy}"')
 
                 # Pick black or white for other color based on contrast
                 if layer is Layer.BACKGROUND:
                     foreground = (232 if use_black_text(*srgb) else 255),
                     background = eight_bit
                 else:
                     foreground = eight_bit
                     background = (232 if use_black_background(*srgb) else 255),
 
-                frame.box(f'{r}•{g}•{b}', foreground, background)
+                frame.box(f'{r}•{g}•{b}' if label else ' ', foreground, background)
 
             frame.right()
 
     frame.bottom()
-    return str(frame)
+    term.writeln()
 
 
-def format_hires_slice(
-    width: int,
+def write_hires_slice(
+    term: Terminal,
     *,
+    hold: Literal['r', 'g', 'b'] = 'g',
+    level: int = 0,
     eight_bit_only: bool = False,
-) -> str:
-    frame = FramedBoxes(width, 32, min_width=1)
+) -> None:
+    frame = FramedBoxes(term, 32, min_width=1)
+    label = '/'.join(
+        f'{l.upper()}={level}' if l == hold else l.upper() for l in ('r', 'g', 'b')
+    )
     frame.top(
-        'High-Resolution Color Slice'
+        ('Downsampled ' if eight_bit_only else '')
+        + 'Hi-Res Color Slice for '
+        + label
     )
 
-    rgb256_to_oklab = get_converter('rgb256', 'oklab')
+    rgb256_to_oklab = None
+    if eight_bit_only:
+        rgb256_to_oklab = get_converter('rgb256', 'oklab')
+
+    def emit_box(r: int, g: int, b: int) -> None:
+        color = r, g, b
+        if eight_bit_only:
+            assert rgb256_to_oklab is not None
+            color = oklab_to_eight_bit(*rgb256_to_oklab(*color))
+        frame.box(' ', (0,), color)
 
-    for r in range(0, 256, 8):
+    for x in range(0, 256, 8):
         frame.left()
-        g = 0
+        for y in range(0, 256, 8):
+            if hold == 'r':
+                r = level
+                g = x
+                b = y
+            elif hold == 'g':
+                r = x
+                g = level
+                b = y
+            elif hold == 'b':
+                r = x
+                g = y
+                b = level
+            else:
+                raise AssertionError(f'invalid hold "{hold}"')
 
-        for b in range(0, 256, 8):
-            color = r, g, b
-            if eight_bit_only:
-                color = oklab_to_eight_bit(*rgb256_to_oklab(*color))
-            frame.box(' ', (0,), color)
+            emit_box(r, g, b)
 
         frame.right()
 
     frame.bottom()
-    return str(frame)
+    term.writeln()
 
 
 def create_parser() -> argparse.ArgumentParser:
     """Create a command line argument parser."""
     parser = argparse.ArgumentParser(
         description="""
             Display color grids that visualize the range of terminal colors,
             while also exercising prettypretty's support for maximizing
-            contrast and down-sampling colors.
+            contrast and down-sampling colors. If not color theme is requested
+            with a command line argument, try to use terminal's current theme.
         """,
     )
 
     group = parser.add_mutually_exclusive_group()
     group.add_argument(
         '--macos-terminal',
         action='store_const',
@@ -228,30 +256,53 @@
         '--vga',
         action='store_const',
         const=VGA,
         dest='theme',
         help='use the same colors as VGA in text mode'
     )
 
+    parser.add_argument(
+        '--truecolor',
+        action=argparse.BooleanOptionalAction,
+        default=None,
+        help='ignore advertised capabilities and force/suppress 24-bit color slices',
+    )
+
+    parser.add_argument(
+        '--no-label',
+        action='store_const',
+        const=False,
+        default=True,
+        dest='label',
+        help='do not display color labels',
+    )
+
     return parser
 
 
 if __name__ == '__main__':
     options = create_parser().parse_args()
-    width, _ = os.get_terminal_size()
 
-    theme = options.theme
-    if theme is None:
-        termio = TermIO()
-        with termio.cbread_mode():
-            theme = TermIO().extract_theme()
-    if theme is None:
-        theme = VGA
-
-    with current_theme(theme):
-        print(f'\n{format_color_cube(width)}')
-        print(f'\n{format_color_cube(width, ansi_only=True)}')
-        print(f'\n{format_color_cube(width, layer=Layer.TEXT)}')
-
-        if os.getenv('COLORTERM') == 'truecolor':
-            print(f'\n{format_hires_slice(width)}')
-            print(f'\n{format_hires_slice(width, eight_bit_only=True)}')
+    with Terminal().terminal_theme(options.theme).scoped_style() as term:
+        term.writeln()
+
+        write_color_cube(term, label=options.label)
+        write_color_cube(term, strategy='pretty', label=options.label)
+        write_color_cube(term, strategy='naive', label=options.label)
+        write_color_cube(term, layer=Layer.TEXT)
+
+        # First clause tests for absence of --truecolor/--no-truecolor or --truecolor
+        if options.truecolor in (None, True) and os.getenv('COLORTERM') == 'truecolor':
+            for hold in ('r', 'g', 'b'):
+                for level in (0, 128, 255):
+                    for downsample in (False, True):
+                        write_hires_slice(
+                            term,
+                            hold=hold,
+                            level=level,
+                            eight_bit_only=downsample,
+                        )
+
+        theme_name = builtin_theme_name(current_theme())
+        term.writeln(
+            f'Prettypretty used ', theme_name or 'current terminal theme', '!\n'
+        ).flush()
```

### Comparing `prettypretty-0.2.0/pyproject.toml` & `prettypretty-0.8.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["pyright", "flit"]
 doc = [
     "sphinx",
     "sphinxcontrib-autoprogram",
+    "sphinx-copybutton",
     "sphinx_design",
     "sphinx-rtd-theme",
 ]
 
 [project.urls]
 repository = "https://github.com/apparebit/prettypretty"
 package = "https://pypi.org/project/prettypretty/"
```

### Comparing `prettypretty-0.2.0/test/runtime.py` & `prettypretty-0.8.0/test/runtime.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,32 @@
 import json
 import os
 from types import TracebackType
 from typing import Any, Callable, TextIO, TypeAlias, TYPE_CHECKING
 import unittest
 
 
+# --------------------------------------------------------------------------------------
+
+@dataclasses.dataclass(frozen=True, slots=True)
+class Symbols:
+    h0: str
+    h1: str
+    h2: str
+    dot0: str
+    dot1: str
+
+
+UNICODE_SYMBOLS = Symbols('═', '━', '─', '•', '⋅')
+ASCII_SYMBOLS = Symbols('=', '=', '-', '.', '.')
+SYMBOLS = ASCII_SYMBOLS if os.name == 'nt' else UNICODE_SYMBOLS
+
+# --------------------------------------------------------------------------------------
+
+
 ExcInfo: TypeAlias = tuple[type[BaseException], BaseException, TracebackType]
 OptExcInfo: TypeAlias = ExcInfo | tuple[None, None, None]
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class testunit:
     """Adapter for making instances of `unittest.TestCase` usable."""
@@ -108,21 +126,21 @@
         return min(self.width, TIGHT_WIDTH)
 
     def _hn(self, dash: str, length: int, text: str) -> str:
         length = self.tight_width - 4 - length - 1
         return f"\n{dash * 3} {text} {dash * length}"
 
     def h0(self, text: str) -> str:
-        return self._hn("═", len(text), self.strong(text))
+        return self._hn(SYMBOLS.h0, len(text), self.strong(text))
 
     def h1(self, text: str) -> str:
-        return self._hn("━", len(text), self.strong(text))
+        return self._hn(SYMBOLS.h1, len(text), self.strong(text))
 
     def h2(self, text: str) -> str:
-        return self._hn("─", len(text), self.italic(text))
+        return self._hn(SYMBOLS.h2, len(text), text)
 
     def sgr(self, ps: str, text: str) -> str:
         return f"\x1b[{ps}m{text}\x1b[0m" if self.isatty else text
 
     def pad(self, text: str) -> str:
         return text.ljust(self.tight_width) if self.isatty else text
 
@@ -156,15 +174,15 @@
 def track_progress(stream: TextIO) -> ProgressTracker:
     columns = 0
 
     def track_progress(test: testunit, err: None | OptExcInfo) -> None:
         nonlocal columns
 
         if test.is_success(err):
-            stream.write("⋅" if test.is_subtest else "•")
+            stream.write(SYMBOLS.dot1 if test.is_subtest else SYMBOLS.dot0)
         elif test.is_failure(err):
             stream.write("f" if test.is_subtest else "F")
         else:
             stream.write("e" if test.is_subtest else "E")
 
         columns += 1
         if columns >= TIGHT_WIDTH:
```

### Comparing `prettypretty-0.2.0/test/test_color.py` & `prettypretty-0.8.0/test/test_color.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,24 +15,22 @@
     linear_p3_to_xyz,
     linear_p3_to_p3,
     p3_to_linear_p3,
     xyz_to_oklab,
     oklab_to_xyz,
     oklab_to_oklch,
     oklch_to_oklab,
+    get_converter,
 )
-
-from prettypretty.color.serde import (
-    parse_hex,
-    parse_x_rgb,
-    parse_x_rgbi,
-)
-
+from prettypretty.color.equality import normalize, PRECISION
+from prettypretty.color.gamut import map_into_gamut
+from prettypretty.color.object import Color
+from prettypretty.color.serde import parse_hex, parse_x_rgb, parse_x_rgbi
+from prettypretty.color.spec import ColorSpec
 from prettypretty.color.theme import VGA
-from prettypretty.color_object import Color
 
 
 @dataclass(frozen=True)
 class ColorValues:
     spec: str
     parsed: tuple[int, int, int]
     srgb: tuple[float, float, float]
@@ -42,15 +40,15 @@
     xyz: tuple[float, float, float]
     oklab: tuple[float, float, float]
     oklch: tuple[float, float, float]
     ansi: tuple[int]
     black_text: bool
     black_background: bool
     closest_index: int
-    x: str
+    xterm: str
     css: str
 
 
 class TestColor(unittest.TestCase):
 
     BLACK = ColorValues(
         spec = '#000',
@@ -62,15 +60,15 @@
         xyz = (0.0, 0.0, 0.0),
         oklab = (0.0, 0.0, 0.0),
         oklch = (0.0, 0.0, math.nan),
         ansi = (0,),
         black_text = False,
         black_background = False,
         closest_index = 0,
-        x = 'rgb:00/00/00',
+        xterm = 'rgb:00/00/00',
         css = 'rgb(0 0 0)',
     )
 
     YELLOW = ColorValues(
         spec = '#ffca00',
         parsed = (255, 202, 0),
         srgb = (1.0, 0.792156862745098, 0.0),
@@ -80,15 +78,15 @@
         xyz = (0.6235868473237722, 0.635031101987136, 0.08972950140152941),
         oklab = (0.8613332073307732, 0.0017175723640959761, 0.1760013937170005),
         oklch = (0.8613332073307732, 0.17600977428868128, 89.440876452466),
         ansi = (11,),
         black_text = True,
         black_background = True,
         closest_index = 1,
-        x = 'rgb:ff/ca/00',
+        xterm = 'rgb:ff/ca/00',
         css = 'rgb(255 202 0)',
     )
 
     BLUE = ColorValues(
         spec = '#3178ea',
         parsed = (49, 120, 234),
         srgb = (0.19215686274509805, 0.47058823529411764, 0.9176470588235294),
@@ -98,15 +96,15 @@
         xyz = (0.22832473003420622, 0.20025321836938537, 0.80506528557483),
         oklab = (0.5909012953108558, -0.03348086515869708, -0.1836287492414714),
         oklch = (0.5909012953108558, 0.18665606306724153, 259.66681920272583),
         ansi = (12,),
         black_text = False,
         black_background = False,
         closest_index = 2,
-        x = 'rgb:31/78/ea',
+        xterm = 'rgb:31/78/ea',
         css = 'rgb(49 120 234)',
     )
 
     WHITE = ColorValues(
         spec = '#fff',
         parsed = (255, 255, 255),
         srgb = (1.0, 1.0, 1.0),
@@ -116,93 +114,128 @@
         xyz = (0.9504559270516717, 1.0, 1.0890577507598784),
         oklab = (1.0000000000000002, -4.996003610813204e-16, 1.734723475976807e-17),
         oklch = (1.0000000000000002, 4.999014376318559e-16, math.nan),
         ansi = (15,),
         black_text = True,
         black_background = True,
         closest_index = 3,
-        x = 'rgb:ff/ff/ff',
+        xterm = 'rgb:ff/ff/ff',
         css = 'rgb(255 255 255)',
     )
 
-
-    def assertCloseEnough(
+    def assertSameCoordinates(
         self,
-        color1: tuple[float, float, float],
-        color2: tuple[float, float, float],
-        places: int = 14,
+        coordinates1: tuple[float, float, float],
+        coordinates2: tuple[float, float, float],
+        *,
+        angular_index: int = -1,
     ) -> None:
-        for c1, c2 in zip(color1, color2):
-            self.assertAlmostEqual(c1, c2, places=places)
+        # A double cannot encode more than 17 decimal digits...
+        s1 = ', '.join(f'{c:.17f}' for c in coordinates1)
+        s2 = ', '.join(f'{c:.17f}' for c in coordinates2)
+
+        # Show coordinates above each other to help compare close values
+        msg = (
+            f'coordinates differ within {PRECISION} '
+            f'digits:\n    {s1}\n    {s2}'
+        )
+
+        n1 = normalize(coordinates1, angular_index=angular_index)
+        n2 = normalize(coordinates2, angular_index=angular_index)
+        self.assertTrue(n1 == n2, msg)
+
+    def test_same_coordinates(self) -> None:
+        # One less than the precision is rounded up or down, with 0.5
+        # represented by a floating point number slightly smaller and hence
+        # still rounding down.
+        f00 = 0.0
+        f01 = float(f'1e-{PRECISION + 1}')
+        f02 = float(f'2e-{PRECISION + 1}')
+        f05 = float(f'5e-{PRECISION + 1}')
+        f07 = float(f'7e-{PRECISION + 1}')
+        f08 = float(f'8e-{PRECISION + 1}')
+        f09 = float(f'9e-{PRECISION + 1}')
+        f10 = float(f'1e-{PRECISION}')
+        f20 = float(f'2e-{PRECISION}')
+
+        self.assertSameCoordinates(
+            (f01, f02, f05),
+            (f00, f00, f00),
+        )
+
+        self.assertSameCoordinates(
+            (f07, f08, f09),
+            (f10, f10, f10),
+        )
+
+        with self.assertRaises(AssertionError):
+            self.assertSameCoordinates(
+                (f10, f10, f10),
+                (f20, f20, f20),
+            )
 
 
     def test_conversions(self) -> None:
         for color_name in ('BLACK', 'YELLOW', 'BLUE', 'WHITE'):
             values = getattr(self, color_name)
             spec = values.spec
 
             color_name = color_name.lower()
             with self.subTest('hex-string to RGB256', color=color_name):
                 _, rgb256 = parse_hex(spec)
                 self.assertTupleEqual(rgb256, values.parsed)
 
             with self.subTest('RGB256 to sRGB', color=color_name):
                 srgb = rgb256_to_srgb(*rgb256)
-                self.assertTupleEqual(srgb, values.srgb)
+                self.assertSameCoordinates(srgb, values.srgb)
 
             with self.subTest('sRGB back to RGB256', color=color_name):
                 self.assertTupleEqual(srgb_to_rgb256(*srgb), rgb256)
 
             with self.subTest('sRGB to linear sRGB', color=color_name):
                 linear_srgb = srgb_to_linear_srgb(*srgb)
-                self.assertTupleEqual(linear_srgb, values.linear_srgb)
+                self.assertSameCoordinates(linear_srgb, values.linear_srgb)
 
             with self.subTest('linear sRGB back to sRGB', color=color_name):
-                self.assertCloseEnough(linear_srgb_to_srgb(*linear_srgb), srgb)
+                self.assertSameCoordinates(linear_srgb_to_srgb(*linear_srgb), srgb)
 
             with self.subTest('linear sRGB to XYZ', color=color_name):
                 xyz = linear_srgb_to_xyz(*linear_srgb)
-                self.assertTupleEqual(xyz, values.xyz)
+                self.assertSameCoordinates(xyz, values.xyz)
 
             with self.subTest('XYZ back to linear sRGB', color=color_name):
-                self.assertCloseEnough(xyz_to_linear_srgb(*xyz), linear_srgb)
+                self.assertSameCoordinates(xyz_to_linear_srgb(*xyz), linear_srgb)
 
             with self.subTest('XYZ to linear P3', color=color_name):
                 linear_p3 = xyz_to_linear_p3(*xyz)
-                self.assertTupleEqual(linear_p3, values.linear_p3)
+                self.assertSameCoordinates(linear_p3, values.linear_p3)
 
             with self.subTest('linear P3 back to XYZ', color=color_name):
-                self.assertCloseEnough(linear_p3_to_xyz(*linear_p3), xyz)
+                self.assertSameCoordinates(linear_p3_to_xyz(*linear_p3), xyz)
 
             with self.subTest('linear P3 to P3', color=color_name):
                 p3 = linear_p3_to_p3(*linear_p3)
-                self.assertTupleEqual(p3, values.p3)
+                self.assertSameCoordinates(p3, values.p3)
 
             with self.subTest('P3 back to linear P3', color=color_name):
-                self.assertCloseEnough(p3_to_linear_p3(*p3), linear_p3)
+                self.assertSameCoordinates(p3_to_linear_p3(*p3), linear_p3)
 
-            with self.subTest('XYZ to OkLab', color=color_name):
+            with self.subTest('XYZ to Oklab', color=color_name):
                 oklab = xyz_to_oklab(*xyz)
-                self.assertTupleEqual(oklab, values.oklab)
+                self.assertSameCoordinates(oklab, values.oklab)
 
-            with self.subTest('OkLab back to XYZ', color=color_name):
-                self.assertCloseEnough(oklab_to_xyz(*oklab), xyz)
+            with self.subTest('Oklab back to XYZ', color=color_name):
+                self.assertSameCoordinates(oklab_to_xyz(*oklab), xyz)
 
-            with self.subTest('OkLab to OkLCh', color=color_name):
+            with self.subTest('Oklab to Oklch', color=color_name):
                 oklch = oklab_to_oklch(*oklab)
-                expected = values.oklch
-                self.assertEqual(oklch[0], expected[0])
-                self.assertEqual(oklch[1], expected[1])
-                self.assertTrue(
-                    (math.isnan(oklch[2]) and math.isnan(expected[2]))
-                    or oklch[2] == expected[2]
-                )
+                self.assertSameCoordinates(oklch, values.oklch, angular_index=2)
 
-            with self.subTest('OkLCh to OkLab', color=color_name):
-                self.assertCloseEnough(oklch_to_oklab(*oklch), oklab)
+            with self.subTest('Oklch back to Oklab', color=color_name):
+                self.assertSameCoordinates(oklch_to_oklab(*oklch), oklab)
 
 
     def test_lores(self) -> None:
         self.assertFalse('prettypretty.color.lores' in sys.modules)
         cache = sys.modules['prettypretty.color.conversion']._converter_cache
         self.assertEqual(len(cache['ansi']), 0)
 
@@ -213,41 +246,75 @@
             with self.subTest('lores conversion', color=color_name):
                 color = Color(values.spec)
                 self.assertEqual(color.tag, 'rgb256')
                 self.assertTupleEqual(color.coordinates, values.parsed)
 
                 ansi = color.to('ansi')
                 self.assertEqual(ansi.tag, 'ansi')
-                self.assertEqual(ansi.coordinates, values.ansi)
+                self.assertTupleEqual(ansi.coordinates, values.ansi)
 
                 rgb256 = ansi.to('rgb256')
                 self.assertTupleEqual(
                     rgb256.coordinates,
                     VGA.ansi(cast(int, ansi.coordinates[0])).coordinates
                 )
 
         self.assertTrue('prettypretty.color.lores' in sys.modules)
         self.assertEqual(len(cache['ansi']), 3)
 
 
+    def test_gamut_mapping(self) -> None:
+        # A very green green
+        p3 = 0, 1, 0
+        srgb = get_converter('p3', 'srgb')(*p3)
+        self.assertSameCoordinates(
+            srgb, (-0.5116049825853448, 1.0182656579378029, -0.3106746212905826)
+        )
+
+        srgb_mapped = map_into_gamut('srgb', srgb)
+        self.assertSameCoordinates(
+            srgb_mapped, (0, 0.9857637107710327, 0.15974244397343721)
+        )
+
+        # A strong yellow
+        p3 = 1, 1, 0
+        linear_srgb = get_converter('p3', 'linear_srgb')(*p3)
+        self.assertSameCoordinates(
+            linear_srgb, (1, 1.0000000000000002, -0.09827360014096621)
+        )
+
+        linear_srgb_mapped = map_into_gamut('linear_srgb', linear_srgb)
+        self.assertSameCoordinates(
+            linear_srgb_mapped, (0.9914525477996113, 0.9977581974546286, 0)
+        )
+
+
     def test_color_object(self) -> None:
         for color_name in ('BLACK', 'YELLOW', 'BLUE', 'WHITE'):
             values = getattr(self, color_name)
             spec = values.spec
 
             color_name = color_name.lower()
             with self.subTest('parse color', color=color_name):
                 color = Color(spec)
                 self.assertEqual(color.tag, 'rgb256')
-                self.assertEqual(color.coordinates, values.parsed)
+                self.assertTupleEqual(color.coordinates, values.parsed)
+                self.assertEqual(color, color)
+                self.assertEqual(color, ColorSpec('rgb256', values.parsed))
 
             with self.subTest('convert to OkLab', color=color_name):
                 oklab = color.to('oklab')
                 self.assertEqual(oklab.tag, 'oklab')
-                self.assertEqual(oklab.coordinates, values.oklab)
+                self.assertSameCoordinates(
+                    cast(tuple[float, float, float], oklab.coordinates),
+                    values.oklab
+                )
+                self.assertEqual(oklab, oklab)
+                self.assertNotEqual(oklab, color)
+                self.assertEqual(oklab, ColorSpec('oklab', values.oklab))
 
             with self.subTest('check distance', color=color_name):
                 self.assertEqual(
                     oklab.closest([
                         Color('#444'),
                         Color('#bb0'),
                         Color('#00b'),
@@ -257,21 +324,37 @@
                 )
 
             with self.subTest('check contrast', color=color_name):
                 self.assertEqual(oklab.use_black_text(), values.black_text)
                 self.assertEqual(oklab.use_black_background(), values.black_background)
 
             with self.subTest('check string', color=color_name):
-                self.assertEqual(f'{color:x}', values.x)
-                self.assertEqual(f'{color:s}', values.css)
+                self.assertEqual(f'{color:x}', values.xterm)
+                self.assertEqual(f'{color:c}', values.css)
 
 
     def test_x_parse_color(self) -> None:
         for text, expected in {
             'rgb:0/8/80': (0, 0x88, 0x80),
             'rgb:800/8000/0': (0.5, 0.5, 0.0),
             'rgbi:0/0.5/1': (0.0, 0.5, 1.0),
             'rgbi:1e0/1e-1/1e-2': (1.0, 0.1, 0.01),
         }.items():
             fn = parse_x_rgb if text.startswith('rgb:') else parse_x_rgbi
             _, actual = fn(text)
             self.assertEqual(actual, expected)
+
+
+    def test_parameters(self) -> None:
+        from prettypretty.style import Style
+
+        for style, expected_params, inverse_params in (
+            (Style.fg(-1), (39,), ()),
+            (Style.fg(1), (31,), (39,)),
+            (Style.bg(9), (101,), (49,)),
+            (Style.bg(240), (48, 5, 240), (49,)),
+            (Style.fg(ColorSpec('eight_bit', (12,))), (38, 5, 12), (39,)),
+        ):
+            actual_params = style.sgr_parameters()
+            self.assertSequenceEqual(actual_params, expected_params)
+            actual_inverse = (~style).sgr_parameters()
+            self.assertSequenceEqual(actual_inverse, inverse_params)
```

### Comparing `prettypretty-0.2.0/PKG-INFO` & `prettypretty-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 Metadata-Version: 2.1
 Name: prettypretty
-Version: 0.2.0
+Version: 0.8.0
 Summary: Library support for awesome command line interfaces
 Keywords: awesome terminals
 Author-email: Robert Grimm <rgrimm@alum.mit.edu>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pyright ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinxcontrib-autoprogram ; extra == "doc"
+Requires-Dist: sphinx-copybutton ; extra == "doc"
 Requires-Dist: sphinx_design ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme ; extra == "doc"
 Project-URL: documentation, https://apparebit.github.io/prettypretty/
 Project-URL: package, https://pypi.org/project/prettypretty/
 Project-URL: repository, https://github.com/apparebit/prettypretty
 Provides-Extra: dev
 Provides-Extra: doc
 
 # Prettypretty
 
-Prettypretty is a Python package for building awesome terminal user interfaces.
+[![Run Tests](https://github.com/apparebit/prettypretty/actions/workflows/ci.yml/badge.svg)](https://github.com/apparebit/prettypretty/actions/workflows/ci.yml)
+[![Publish to GitHub Pages](https://github.com/apparebit/prettypretty/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/apparebit/prettypretty/actions/workflows/gh-pages.yml)
 
+Prettypretty helps build awesome terminal user interfaces in Python. Notably, it
+incorporates a powerful and general color library. The resulting, near seemless
+integration of 1970s archaic but beloved ANSI escape codes for terminal styling
+with 2020s color science, notably via the [Oklab perceptual color
+space](https://bottosson.github.io/posts/oklab/), is unique to prettypretty and
+enables your application to easily adapt its visual styles to a user's current
+color theme, dark or light mode, and color preferences. So, what are you waiting
+for? Switch to prettypretty for all your terminal styling needs. Prettypretty is
+awesome!
+
+\[ [Repository](https://github.com/apparebit/prettypretty)
+| [Package](https://pypi.org/project/prettypretty/)
+| [Documentation](https://apparebit.github.io/prettypretty/)
+\]
 
 ## Prettypretty Illustrated
 
 The first screenshot illustrates prettypretty's support for maximizing text
 contrast by comparing against backgrounds in all 216 colors from the 6x6x6 RGB
 cube of 8-bit terminal colors.
```

