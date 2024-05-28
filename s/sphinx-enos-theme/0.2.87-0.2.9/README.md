# Comparing `tmp/sphinx_enos_theme-0.2.87.tar.gz` & `tmp/sphinx_enos_theme-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_enos_theme-0.2.87.tar", last modified: Tue May 28 02:50:08 2024, max compression
+gzip compressed data, was "dist/sphinx_enos_theme-0.2.9.tar", last modified: Wed Nov 20 12:56:43 2019, max compression
```

## Comparing `sphinx_enos_theme-0.2.87.tar` & `sphinx_enos_theme-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 02:50:08.740436 sphinx_enos_theme-0.2.87/
--rw-rw-rw-   0        0        0      421 2023-08-10 16:44:40.000000 sphinx_enos_theme-0.2.87/MANIFEST.in
--rw-rw-rw-   0        0        0     3928 2024-05-28 02:50:08.740436 sphinx_enos_theme-0.2.87/PKG-INFO
--rw-rw-rw-   0        0        0     2917 2024-05-28 02:35:10.000000 sphinx_enos_theme-0.2.87/README.md
--rw-rw-rw-   0        0        0      118 2024-05-28 02:50:08.742435 sphinx_enos_theme-0.2.87/setup.cfg
--rw-rw-rw-   0        0        0     1878 2023-08-10 16:44:40.000000 sphinx_enos_theme-0.2.87/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 02:50:08.680434 sphinx_enos_theme-0.2.87/sphinx_enos_theme/
--rw-rw-rw-   0        0        0      523 2024-05-28 02:48:24.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/__init__.py
--rw-rw-rw-   0        0        0     5173 2024-05-28 02:48:14.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/breadcrumbs.html
--rw-rw-rw-   0        0        0      791 2024-05-28 02:48:14.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/footer.html
--rw-rw-rw-   0        0        0      391 2024-05-28 02:48:21.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/gfooter.html
--rw-rw-rw-   0        0        0     1337 2024-05-28 02:48:22.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/header.html
--rw-rw-rw-   0        0        0    15428 2024-05-28 02:48:49.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/layout.html
--rw-rw-rw-   0        0        0     1580 2024-05-28 02:48:22.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/search.html
--rw-rw-rw-   0        0        0      716 2024-05-28 02:48:24.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/searchbox.html
--rw-rw-rw-   0        0        0     1059 2024-05-28 02:48:24.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/side.html
-drwxrwxrwx   0        0        0        0 2024-05-28 02:50:08.654434 sphinx_enos_theme-0.2.87/sphinx_enos_theme/static/
-drwxrwxrwx   0        0        0        0 2024-05-28 02:50:08.731433 sphinx_enos_theme-0.2.87/sphinx_enos_theme/static/css/
--rw-rw-rw-   0        0        0   882434 2024-05-28 02:48:49.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/static/css/theme.css
-drwxrwxrwx   0        0        0        0 2024-05-28 02:50:08.735435 sphinx_enos_theme-0.2.87/sphinx_enos_theme/static/js/
--rw-rw-rw-   0        0        0  2013749 2024-05-28 02:48:49.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/static/js/theme.f512c65e8ee7466aa617.js
--rw-rw-rw-   0        0        0      659 2024-05-28 02:48:24.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/theme.conf
--rw-rw-rw-   0        0        0     1021 2024-05-28 02:48:24.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme/tools.html
-drwxrwxrwx   0        0        0        0 2024-05-28 02:50:08.730433 sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/
--rw-rw-rw-   0        0        0     3928 2024-05-28 02:50:08.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2024-05-28 02:50:08.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 02:50:08.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-28 02:50:08.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-10 16:44:40.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-05-28 02:50:08.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-28 02:50:08.000000 sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/top_level.txt
+drwxr-xr-x   0 wanfeng.tang   (501) staff       (20)        0 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)     3430 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/PKG-INFO
+drwxr-xr-x   0 wanfeng.tang   (501) staff       (20)        0 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)     3430 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/PKG-INFO
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)        1 2019-01-18 09:26:44.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/not-zip-safe
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      760 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)       60 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/entry_points.txt
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)        7 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/requires.txt
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)       18 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/top_level.txt
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)        1 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      411 2019-01-18 09:22:42.000000 sphinx_enos_theme-0.2.9/MANIFEST.in
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)     1485 2019-11-20 10:23:33.000000 sphinx_enos_theme-0.2.9/README.md
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)     1820 2019-08-06 13:01:37.000000 sphinx_enos_theme-0.2.9/setup.py
+drwxr-xr-x   0 wanfeng.tang   (501) staff       (20)        0 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/
+-rw-rw-rw-   0 wanfeng.tang   (501) staff       (20)     5751 2019-11-20 12:56:41.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/layout.html
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      618 2019-11-20 10:01:25.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/theme.conf
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)     3509 2019-10-29 05:22:04.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/breadcrumbs.html
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)     1034 2019-11-20 10:18:40.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/side.html
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      503 2019-11-20 12:56:03.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/__init__.py
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      375 2019-06-21 11:56:17.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/gfooter.html
+drwxr-xr-x   0 wanfeng.tang   (501) staff       (20)        0 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/static/
+drwxr-xr-x   0 wanfeng.tang   (501) staff       (20)        0 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/static/css/
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)   495116 2019-11-20 12:56:41.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/static/css/theme.css
+drwxr-xr-x   0 wanfeng.tang   (501) staff       (20)        0 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/static/js/
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)   767709 2019-11-20 12:56:41.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/static/js/theme.5655a83c85c857a363ad.js
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      852 2019-11-20 10:00:07.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/tools.html
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)     1530 2019-01-18 06:24:58.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/search.html
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      703 2019-03-25 06:17:08.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/footer.html
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      975 2019-11-20 09:28:49.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/header.html
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      700 2019-03-25 06:37:53.000000 sphinx_enos_theme-0.2.9/sphinx_enos_theme/searchbox.html
+-rw-r--r--   0 wanfeng.tang   (501) staff       (20)      108 2019-11-20 12:56:43.000000 sphinx_enos_theme-0.2.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sphinx_enos_theme-0.2.87/setup.py` & `sphinx_enos_theme-0.2.9/setup.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# -*- coding: utf-8 -*-
-"""`sphinx_enos_theme` lives on `Github`_.
-
-.. _github:  https://github.com/TRoam/sphinx_enos_theme.git
-
-"""
-from io import open
-from setuptools import setup
-from sphinx_enos_theme import __version__
-
-
-setup(
-    name='sphinx_enos_theme',
-    version=__version__,
-    url='https://github.com/TRoam/sphinx_enos_theme/',
-    license='MIT',
-    author='wanfeng tang',
-    author_email='roam.tang@gmail.com',
-    description='ENOS Docs theme for Sphinx',
-    long_description=open('README.md', encoding='utf-8').read(),
-    zip_safe=False,
-    packages=['sphinx_enos_theme'],
-    package_data={'sphinx_enos_theme': [
-        'theme.conf',
-        '*.html',
-        'static/css/*.css',
-        'static/js/*.js',
-        'static/assets/*.*'
-    ]},
-    include_package_data=True,
-    # See http://www.sphinx-doc.org/en/stable/theming.html#distribute-your-theme-as-a-python-package
-    entry_points = {
-        'sphinx.html_themes': [
-            'sphinx_enos_theme = sphinx_enos_theme',
-        ]
-    },
-    install_requires=[
-       'sphinx'
-    ],
-    classifiers=[
-        'Framework :: Sphinx',
-        'Framework :: Sphinx :: Theme',
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: MIT License',
-        'Environment :: Console',
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Operating System :: OS Independent',
-        'Topic :: Documentation',
-        'Topic :: Software Development :: Documentation',
-    ],
-)
+# -*- coding: utf-8 -*-
+"""`sphinx_enos_theme` lives on `Github`_.
+
+.. _github:  https://github.com/TRoam/sphinx_enos_theme.git
+
+"""
+from io import open
+from setuptools import setup
+from sphinx_enos_theme import __version__
+
+
+setup(
+    name='sphinx_enos_theme',
+    version=__version__,
+    url='https://github.com/TRoam/sphinx_enos_theme/',
+    license='MIT',
+    author='wanfeng tang',
+    author_email='roam.tang@gmail.com',
+    description='ENOS Docs theme for Sphinx',
+    long_description=open('README.md', encoding='utf-8').read(),
+    zip_safe=False,
+    packages=['sphinx_enos_theme'],
+    package_data={'sphinx_enos_theme': [
+        'theme.conf',
+        '*.html',
+        'static/css/*.css',
+        'static/js/*.js',
+        'static/assets/*.*'
+    ]},
+    include_package_data=True,
+    # See http://www.sphinx-doc.org/en/stable/theming.html#distribute-your-theme-as-a-python-package
+    entry_points = {
+        'sphinx.html_themes': [
+            'sphinx_enos_theme = sphinx_enos_theme',
+        ]
+    },
+    install_requires=[
+       'sphinx'
+    ],
+    classifiers=[
+        'Framework :: Sphinx',
+        'Framework :: Sphinx :: Theme',
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: MIT License',
+        'Environment :: Console',
+        'Environment :: Web Environment',
+        'Intended Audience :: Developers',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Operating System :: OS Independent',
+        'Topic :: Documentation',
+        'Topic :: Software Development :: Documentation',
+    ],
+)
```

### Comparing `sphinx_enos_theme-0.2.87/sphinx_enos_theme/searchbox.html` & `sphinx_enos_theme-0.2.9/sphinx_enos_theme/searchbox.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-{%- if (language == 'en') or (language == 'en_us') or (language == 'en_US') or (language == 'EN_US') %}
-{%- set search_placeholder = 'Search this document' %}
-{%- else %}
-{%- set search_placeholder = '搜索此文档' %}
-{%- endif%}
-{%- if builder != 'singlehtml' %}
-<div role="search">
-  <form id="rtd-search-form" class="wy-form" action="{{ pathto('search') }}" method="get">
-    <input class="search-input" type="text" name="q" placeholder="{{search_placeholder}}" />
-    <span class="dplicon_search"></span>
-    <span class="dplicon_wrong"></span>
-    <input type="hidden" name="check_keywords" value="yes" />
-    <input type="hidden" name="area" value="default" />
-  </form>
-</div>
-{%- endif %}
+{%- if (language == 'en') or (language == 'en_us') or (language == 'en_US') or (language == 'EN_US') %}
+{%- set search_placeholder = 'Search this document' %}
+{%- else %}
+{%- set search_placeholder = '搜索此文档' %}
+{%- endif%}
+{%- if builder != 'singlehtml' %}
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="{{ pathto('search') }}" method="get">
+    <input class="search-input" type="text" name="q" placeholder="{{search_placeholder}}" />
+    <span class="icon-search"></span>
+    <span class="icon-wrong_small"></span>
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+{%- endif %}
```

### Comparing `sphinx_enos_theme-0.2.87/sphinx_enos_theme/theme.conf` & `sphinx_enos_theme-0.2.9/sphinx_enos_theme/theme.conf`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-00000000: 5b74 6865 6d65 5d0d 0a69 6e68 6572 6974  [theme]..inherit
-00000010: 203d 2062 6173 6963 0d0a 7374 796c 6573   = basic..styles
-00000020: 6865 6574 203d 2063 7373 2f74 6865 6d65  heet = css/theme
-00000030: 2e63 7373 0d0a 7079 676d 656e 7473 5f73  .css..pygments_s
-00000040: 7479 6c65 203d 2064 6566 6175 6c74 0d0a  tyle = default..
-00000050: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 726f  ..[options]..pro
-00000060: 6475 6374 5f6e 616d 6520 3d0d 0a63 616e  duct_name =..can
-00000070: 6f6e 6963 616c 5f75 726c 203d 0d0a 616e  onical_url =..an
-00000080: 616c 7974 6963 735f 6964 203d 0d0a 636f  alytics_id =..co
-00000090: 6c6c 6170 7365 5f6e 6176 6967 6174 696f  llapse_navigatio
-000000a0: 6e20 3d20 5472 7565 0d0a 7374 6963 6b79  n = True..sticky
-000000b0: 5f6e 6176 6967 6174 696f 6e20 3d20 5472  _navigation = Tr
-000000c0: 7565 0d0a 6e61 7669 6761 7469 6f6e 5f64  ue..navigation_d
-000000d0: 6570 7468 203d 2038 0d0a 696e 636c 7564  epth = 8..includ
-000000e0: 6568 6964 6465 6e20 3d20 5472 7565 0d0a  ehidden = True..
-000000f0: 7469 746c 6573 5f6f 6e6c 7920 3d0d 0a6c  titles_only =..l
-00000100: 6f67 6f5f 6f6e 6c79 203d 0d0a 6469 7370  ogo_only =..disp
-00000110: 6c61 795f 7665 7273 696f 6e20 3d20 5472  lay_version = Tr
-00000120: 7565 0d0a 7072 6576 5f6e 6578 745f 6275  ue..prev_next_bu
-00000130: 7474 6f6e 735f 6c6f 6361 7469 6f6e 203d  ttons_location =
-00000140: 2062 6f74 746f 6d0d 0a73 7479 6c65 5f65   bottom..style_e
-00000150: 7874 6572 6e61 6c5f 6c69 6e6b 7320 3d20  xternal_links = 
-00000160: 4661 6c73 650d 0a64 6973 706c 6179 5f68  False..display_h
-00000170: 6561 6465 7220 3d20 5472 7565 0d0a 6469  eader = True..di
-00000180: 7370 6c61 795f 736f 7572 6365 203d 2054  splay_source = T
-00000190: 7275 650d 0a63 6f70 7972 6967 6874 5f65  rue..copyright_e
-000001a0: 6e20 3d20 436f 7079 7269 6768 74c2 a920  n = Copyright.. 
-000001b0: 3230 3132 2d32 3031 3920 456e 7669 7369  2012-2019 Envisi
-000001c0: 6f6e 2045 6e65 7267 7920 7c20 4163 7175  on Energy | Acqu
-000001d0: 6972 696e 6720 4a69 616e 6773 7520 4943  iring Jiangsu IC
-000001e0: 5020 4c69 6365 6e73 6520 3137 3035 3039  P License 170509
-000001f0: 3735 0d0a 636f 7079 7269 6768 745f 7a68  75..copyright_zh
-00000200: 203d 2043 6f70 7972 6967 6874 c2a9 2032   = Copyright.. 2
-00000210: 3031 322d 3230 3139 20e8 bf9c e699 afe6  012-2019 .......
-00000220: 99ba e883 bd20 7c20 4943 5020 e5a4 87e6  ..... | ICP ....
-00000230: a188 e58f b720 3137 3035 3039 3735 0d0a  ..... 17050975..
-00000240: 646f 6373 203d 2054 7275 650d 0a64 6f63  docs = True..doc
-00000250: 735f 7572 6c5f 656e 203d 202f 646f 6373  s_url_en = /docs
-00000260: 2f65 6e2f 0d0a 646f 6373 5f75 726c 5f7a  /en/..docs_url_z
-00000270: 6820 3d20 2f64 6f63 732f 7a68 5f43 4e2f  h = /docs/zh_CN/
-00000280: 0d0a 646f 6373 5f61 7574 6820 3d20 4661  ..docs_auth = Fa
-00000290: 6c73 65                                  lse
+00000000: 5b74 6865 6d65 5d0a 696e 6865 7269 7420  [theme].inherit 
+00000010: 3d20 6261 7369 630a 7374 796c 6573 6865  = basic.styleshe
+00000020: 6574 203d 2063 7373 2f74 6865 6d65 2e63  et = css/theme.c
+00000030: 7373 0a70 7967 6d65 6e74 735f 7374 796c  ss.pygments_styl
+00000040: 6520 3d20 6465 6661 756c 740a 0a5b 6f70  e = default..[op
+00000050: 7469 6f6e 735d 0a70 726f 6475 6374 5f6e  tions].product_n
+00000060: 616d 6520 3d0a 6361 6e6f 6e69 6361 6c5f  ame =.canonical_
+00000070: 7572 6c20 3d0a 616e 616c 7974 6963 735f  url =.analytics_
+00000080: 6964 203d 0a63 6f6c 6c61 7073 655f 6e61  id =.collapse_na
+00000090: 7669 6761 7469 6f6e 203d 2054 7275 650a  vigation = True.
+000000a0: 7374 6963 6b79 5f6e 6176 6967 6174 696f  sticky_navigatio
+000000b0: 6e20 3d20 5472 7565 0a6e 6176 6967 6174  n = True.navigat
+000000c0: 696f 6e5f 6465 7074 6820 3d20 380a 696e  ion_depth = 8.in
+000000d0: 636c 7564 6568 6964 6465 6e20 3d20 5472  cludehidden = Tr
+000000e0: 7565 0a74 6974 6c65 735f 6f6e 6c79 203d  ue.titles_only =
+000000f0: 0a6c 6f67 6f5f 6f6e 6c79 203d 0a64 6973  .logo_only =.dis
+00000100: 706c 6179 5f76 6572 7369 6f6e 203d 2054  play_version = T
+00000110: 7275 650a 7072 6576 5f6e 6578 745f 6275  rue.prev_next_bu
+00000120: 7474 6f6e 735f 6c6f 6361 7469 6f6e 203d  ttons_location =
+00000130: 2062 6f74 746f 6d0a 7374 796c 655f 6578   bottom.style_ex
+00000140: 7465 726e 616c 5f6c 696e 6b73 203d 2046  ternal_links = F
+00000150: 616c 7365 0a64 6973 706c 6179 5f68 6561  alse.display_hea
+00000160: 6465 7220 3d20 5472 7565 0a64 6973 706c  der = True.displ
+00000170: 6179 5f73 6f75 7263 6520 3d20 4661 6c73  ay_source = Fals
+00000180: 650a 636f 7079 7269 6768 745f 656e 203d  e.copyright_en =
+00000190: 2043 6f70 7972 6967 6874 c2a9 2032 3031   Copyright.. 201
+000001a0: 322d 3230 3139 2045 6e76 6973 696f 6e20  2-2019 Envision 
+000001b0: 456e 6572 6779 207c 2041 6371 7569 7269  Energy | Acquiri
+000001c0: 6e67 204a 6961 6e67 7375 2049 4350 204c  ng Jiangsu ICP L
+000001d0: 6963 656e 7365 2031 3730 3530 3937 350a  icense 17050975.
+000001e0: 636f 7079 7269 6768 745f 7a68 203d 2043  copyright_zh = C
+000001f0: 6f70 7972 6967 6874 c2a9 2032 3031 322d  opyright.. 2012-
+00000200: 3230 3139 20e8 bf9c e699 afe6 99ba e883  2019 ...........
+00000210: bd20 7c20 4943 5020 e5a4 87e6 a188 e58f  . | ICP ........
+00000220: b720 3137 3035 3039 3735 0a64 6f63 7320  . 17050975.docs 
+00000230: 3d20 5472 7565 0a64 6f63 735f 7572 6c5f  = True.docs_url_
+00000240: 656e 203d 202f 646f 6373 2f65 6e2f 0a64  en = /docs/en/.d
+00000250: 6f63 735f 7572 6c5f 7a68 203d 202f 646f  ocs_url_zh = /do
+00000260: 6373 2f7a 685f 434e 2f0a                 cs/zh_CN/.
```

### Comparing `sphinx_enos_theme-0.2.87/sphinx_enos_theme.egg-info/SOURCES.txt` & `sphinx_enos_theme-0.2.9/sphinx_enos_theme.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 sphinx_enos_theme.egg-info/SOURCES.txt
 sphinx_enos_theme.egg-info/dependency_links.txt
 sphinx_enos_theme.egg-info/entry_points.txt
 sphinx_enos_theme.egg-info/not-zip-safe
 sphinx_enos_theme.egg-info/requires.txt
 sphinx_enos_theme.egg-info/top_level.txt
 sphinx_enos_theme/static/css/theme.css
-sphinx_enos_theme/static/js/theme.f512c65e8ee7466aa617.js
+sphinx_enos_theme/static/js/theme.5655a83c85c857a363ad.js
```

