# Comparing `tmp/pelican_pdf-1.0.3.tar.gz` & `tmp/pelican_pdf-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_pdf-1.0.3.tar", max compression
+gzip compressed data, was "pelican_pdf-1.0.4.tar", last modified: Tue May 28 13:19:09 2024, max compression
```

## Comparing `pelican_pdf-1.0.3.tar` & `pelican_pdf-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    34674 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/LICENSE
--rw-r--r--   0        0        0     1835 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/README.md
--rw-r--r--   0        0        0       27 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/__init__.py
--rw-r--r--   0        0        0     4803 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/pdf.py
--rw-r--r--   0        0        0      431 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_data/testfile.md
--rw-r--r--   0        0        0      468 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_data/testfile.rst
--rw-r--r--   0        0        0      294 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_data/testfile_link.md
--rw-r--r--   0        0        0      329 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_data/testfile_link.rst
--rw-r--r--   0        0        0     1158 2023-07-03 09:12:50.777331 pelican_pdf-1.0.3/pelican/plugins/pdf/test_pdf.py
--rw-r--r--   0        0        0     2010 2023-07-03 09:13:09.761512 pelican_pdf-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 pelican_pdf-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1219 2024-05-28 13:06:15.265957 pelican_pdf-1.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      556 2021-03-03 06:26:33.000000 pelican_pdf-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34674 2021-03-03 06:26:33.000000 pelican_pdf-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2311 2024-05-27 15:03:49.498642 pelican_pdf-1.0.4/README.md
+-rw-r--r--   0        0        0       27 2021-03-03 06:26:33.000000 pelican_pdf-1.0.4/pelican/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0     4747 2024-05-27 15:11:35.457778 pelican_pdf-1.0.4/pelican/plugins/pdf/pdf.py
+-rw-r--r--   0        0        0      431 2021-06-29 06:29:53.000000 pelican_pdf-1.0.4/pelican/plugins/pdf/test_data/testfile.md
+-rw-r--r--   0        0        0      468 2021-06-29 06:29:53.000000 pelican_pdf-1.0.4/pelican/plugins/pdf/test_data/testfile.rst
+-rw-r--r--   0        0        0      294 2021-06-29 06:29:53.000000 pelican_pdf-1.0.4/pelican/plugins/pdf/test_data/testfile_link.md
+-rw-r--r--   0        0        0      329 2021-06-29 06:29:53.000000 pelican_pdf-1.0.4/pelican/plugins/pdf/test_data/testfile_link.rst
+-rw-r--r--   0        0        0     1199 2024-05-27 15:11:35.458414 pelican_pdf-1.0.4/pelican/plugins/pdf/test_pdf.py
+-rw-r--r--   0        0        0     2575 2024-05-28 13:19:09.779690 pelican_pdf-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 pelican_pdf-1.0.4/PKG-INFO
```

### Comparing `pelican_pdf-1.0.3/LICENSE` & `pelican_pdf-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_pdf-1.0.3/README.md` & `pelican_pdf-1.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 PDF Generator: A Plugin for Pelican
 ===================================
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/pdf/main.yml?branch=main)](https://github.com/pelican-plugins/pdf/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-pdf)](https://pypi.org/project/pelican-pdf/)
+[![Downloads](https://img.shields.io/pypi/dm/pelican-pdf)](https://pypi.org/project/pelican-pdf/)
 ![License](https://img.shields.io/pypi/l/pelican-pdf?color=blue)
 
 The PDF Generator plugin automatically exports articles and pages as PDF files as part of the site generation process.
 PDFs are saved to: `output/pdf/`
 
 Installation
 ------------
 
 This plugin can be installed via:
 
     python -m pip install pelican-pdf
 
+As long as you have not explicitly added a `PLUGINS` setting to your Pelican settings file, then the newly-installed plugin should be automatically detected and enabled. Otherwise, you must add `pdf` to your existing `PLUGINS` list. For more information, please see the [How to Use Plugins](https://docs.getpelican.com/en/latest/plugins.html#how-to-use-plugins) documentation.
+
 Usage
 -----
 
 To customize the PDF output, you can use the following settings in your Pelican configuration file:
 
 	PDF_STYLE = ""
 	PDF_STYLE_PATH = ""
```

### Comparing `pelican_pdf-1.0.3/pelican/plugins/pdf/pdf.py` & `pelican_pdf-1.0.4/pelican/plugins/pdf/pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-"""
-PDF Generator
--------
+"""PDF Generator plugin for Pelican.
 
-The pdf plugin generates PDF files from reStructuredText and Markdown sources.
+This plugin generates PDF files from reStructuredText and Markdown source files.
 """
 
 from itertools import chain
 import logging
 import os
 import re
 import time
@@ -17,30 +15,27 @@
 from pelican.generators import Generator
 from pelican.readers import MarkdownReader
 
 logger = logging.getLogger(__name__)
 
 
 class PdfGenerator(Generator):
-    "Generate PDFs on the output dir, for all articles and pages"
+    """Generate PDFs on the output dir, for all articles and pages."""
 
     supported_md_fields = ["date"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if "PDF_STYLE_PATH" in self.settings:
             pdf_style_path = [self.settings["PDF_STYLE_PATH"]]
         else:
             pdf_style_path = []
 
-        if "PDF_STYLE" in self.settings:
-            pdf_style = [self.settings["PDF_STYLE"]]
-        else:
-            pdf_style = []
+        pdf_style = [self.settings["PDF_STYLE"]] if "PDF_STYLE" in self.settings else []
 
         self.pdfcreator = RstToPdf(
             breakside=0, stylesheets=pdf_style, style_path=pdf_style_path, raw_html=True
         )
 
     def _create_pdf(self, obj, output_path):
         filename = obj.slug + ".pdf"
@@ -91,28 +86,26 @@
             logger.warn("Ignoring unsupported file " + obj.source_path)
             return
 
         # Find intra-site links and replace placeholder with actual path / url
         hrefs = self._get_intrasite_link_regex()
         text = hrefs.sub(lambda m: obj._link_replacer(obj.get_siteurl(), m), text)
 
-        logger.info(" [ok] writing %s" % output_pdf)
+        logger.info(f" [ok] writing {output_pdf}")
 
         self.pdfcreator.createPdf(text=(header + text), output=output_pdf)
 
         if obj.date is not None:
             self._set_file_utime(output_pdf, obj.date)
 
     def _get_intrasite_link_regex(self):
         intrasite_link_regex = self.settings["INTRASITE_LINK_REGEX"]
-        regex = r"""
-                (?P<markup>)(?P<quote>)(?P<path>(\:?){}(?P<value>.*?)(?=[>\n]))
-                """.format(
-            intrasite_link_regex
-        )
+        regex = rf"""
+                (?P<markup>)(?P<quote>)(?P<path>(\:?){intrasite_link_regex}(?P<value>.*?)(?=[>\n]))
+                """
         return re.compile(regex, re.X)
 
     def _set_file_utime(self, path, datetime):
         """Set modified time (mtime) of specified file."""
         mtime = time.mktime(datetime.timetuple())
         os.utime(path, (mtime, mtime))
 
@@ -124,15 +117,15 @@
         # since we write our own files
         logger.info(" Generating PDF files...")
         pdf_path = os.path.join(self.output_path, "pdf")
         if not os.path.exists(pdf_path):
             try:
                 os.mkdir(pdf_path)
             except OSError:
-                logger.error("Couldn't create the pdf output folder in " + pdf_path)
+                logger.exception("Couldn't create the pdf output folder in " + pdf_path)
 
         for obj in chain(self.context["articles"], self.context["pages"]):
             self._create_pdf(obj, pdf_path)
             for obj_trans in obj.translations:
                 self._create_pdf(obj_trans, pdf_path)
```

### Comparing `pelican_pdf-1.0.3/pelican/plugins/pdf/test_pdf.py` & `pelican_pdf-1.0.4/pelican/plugins/pdf/test_pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import locale
 import os
 from shutil import rmtree
 from tempfile import mkdtemp
 import unittest
 
+import pdf
 from pelican import Pelican
 from pelican.readers import MarkdownReader
 from pelican.settings import read_settings
 
-import pdf
-
 CUR_DIR = os.path.dirname(__file__)
 
 
 class TestPdfGeneration(unittest.TestCase):
+    """Test class for PDF generation."""
+
     def setUp(self, override=None):
         self.temp_path = mkdtemp(prefix="pelicantests.")
         settings = {
             "PATH": os.path.join(CUR_DIR, "test_data"),
             "OUTPUT_PATH": self.temp_path,
             "PLUGINS": [pdf],
             "LOCALE": locale.normalize("en_US"),
```

### Comparing `pelican_pdf-1.0.3/PKG-INFO` & `pelican_pdf-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: pelican-pdf
-Version: 1.0.3
+Version: 1.0.4
 Summary: PDF Generator is a Pelican plugin that exports articles and pages as PDF files during site generation
-Home-page: https://github.com/pelican-plugins/pdf
-License: AGPL-3.0
 Keywords: pelican,plugin,pdf,generator
-Author: Pelican Dev Team
-Author-email: authors@getpelican.com
-Requires-Python: >=3.8.1,<4.0
+Author-Email: Justin Mayer <entroP@gmail.com>, Dominik Wombacher <dominik@wombacher.cc>
+License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: markdown
-Requires-Dist: markdown (>=3.2.2) ; extra == "markdown"
-Requires-Dist: pelican (>=4.5)
-Requires-Dist: rst2pdf (>=0.99)
-Requires-Dist: xhtml2pdf (>=0.2.5)
-Project-URL: Documentation, https://docs.getpelican.com
+Project-URL: Homepage, https://github.com/pelican-plugins/pdf
+Project-URL: Issue tracker, https://github.com/pelican-plugins/pdf/issues
 Project-URL: Funding, https://donate.getpelican.com/
-Project-URL: Issue Tracker, https://github.com/pelican-plugins/pdf/issues
-Project-URL: Repository, https://github.com/pelican-plugins/pdf
+Requires-Python: <4.0,>=3.8.1
+Requires-Dist: pelican>=4.5
+Requires-Dist: rst2pdf>=0.99
+Requires-Dist: xhtml2pdf<0.2.12,>=0.2.5
 Description-Content-Type: text/markdown
 
 PDF Generator: A Plugin for Pelican
 ===================================
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/pdf/main.yml?branch=main)](https://github.com/pelican-plugins/pdf/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-pdf)](https://pypi.org/project/pelican-pdf/)
+[![Downloads](https://img.shields.io/pypi/dm/pelican-pdf)](https://pypi.org/project/pelican-pdf/)
 ![License](https://img.shields.io/pypi/l/pelican-pdf?color=blue)
 
 The PDF Generator plugin automatically exports articles and pages as PDF files as part of the site generation process.
 PDFs are saved to: `output/pdf/`
 
 Installation
 ------------
 
 This plugin can be installed via:
 
     python -m pip install pelican-pdf
 
+As long as you have not explicitly added a `PLUGINS` setting to your Pelican settings file, then the newly-installed plugin should be automatically detected and enabled. Otherwise, you must add `pdf` to your existing `PLUGINS` list. For more information, please see the [How to Use Plugins](https://docs.getpelican.com/en/latest/plugins.html#how-to-use-plugins) documentation.
+
 Usage
 -----
 
 To customize the PDF output, you can use the following settings in your Pelican configuration file:
 
 	PDF_STYLE = ""
 	PDF_STYLE_PATH = ""
@@ -75,8 +75,7 @@
 [existing issues]: https://github.com/pelican-plugins/pdf/issues
 [Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
 
 License
 -------
 
 This project is licensed under the AGPL 3.0 license.
-
```

