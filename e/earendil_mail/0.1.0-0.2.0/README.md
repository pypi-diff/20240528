# Comparing `tmp/earendil_mail-0.1.0.tar.gz` & `tmp/earendil_mail-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earendil_mail-0.1.0.tar", max compression
+gzip compressed data, was "earendil_mail-0.2.0.tar", max compression
```

## Comparing `earendil_mail-0.1.0.tar` & `earendil_mail-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      192 2021-12-27 03:27:33.865902 earendil_mail-0.1.0/earendil/__init__.py
--rw-r--r--   0        0        0      655 2021-12-27 03:27:33.830995 earendil_mail-0.1.0/earendil/base_email.py
--rw-r--r--   0        0        0     1642 2021-12-27 03:27:33.838974 earendil_mail-0.1.0/earendil/mailer.py
--rw-r--r--   0        0        0     1262 2021-12-27 03:27:33.850942 earendil_mail-0.1.0/earendil/markdown_email.py
--rw-r--r--   0        0        0     1557 2021-12-27 04:26:12.702299 earendil_mail-0.1.0/earendil/plaintext_renderer.py
--rw-r--r--   0        0        0      856 2021-12-27 01:43:23.159213 earendil_mail-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2669 2021-12-27 00:46:54.943119 earendil_mail-0.1.0/README.md
--rw-r--r--   0        0        0     3357 2021-12-27 04:53:39.983217 earendil_mail-0.1.0/setup.py
--rw-r--r--   0        0        0     3419 2021-12-27 04:53:39.983217 earendil_mail-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      192 2024-05-15 05:37:33.473404 earendil_mail-0.2.0/earendil/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-15 05:58:28.487440 earendil_mail-0.2.0/earendil/base_email.py
+-rw-r--r--   0        0        0     1994 2024-05-15 06:09:06.909378 earendil_mail-0.2.0/earendil/mailer.py
+-rw-r--r--   0        0        0     1789 2024-05-15 06:00:46.826730 earendil_mail-0.2.0/earendil/markdown_email.py
+-rw-r--r--   0        0        0     1607 2024-05-15 05:54:36.393183 earendil_mail-0.2.0/earendil/plaintext_renderer.py
+-rw-r--r--   0        0        0      893 2024-05-28 00:06:35.648467 earendil_mail-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2768 2024-05-15 06:03:18.666962 earendil_mail-0.2.0/README.md
+-rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 earendil_mail-0.2.0/PKG-INFO
```

### Comparing `earendil_mail-0.1.0/earendil/mailer.py` & `earendil_mail-0.2.0/earendil/mailer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,40 +2,60 @@
 
 from pathlib import Path
 from smtplib import SMTP
 
 from earendil.markdown_email import MarkdownEmail
 
 
-def send_markdown_email(server: SMTP, sender: str, recipient: str, subject: str, body: str):
+def send_markdown_email(
+    server: SMTP,
+    sender: str,
+    to: str | list[str],
+    subject: str,
+    body: str,
+    cc: str | list[str] | None = None,
+    bcc: str | list[str] | None = None,
+):
     """Sends a Markdown-formatted email message with the given parameters.
 
     Before calling, server must be ready for a send_message method invocation.
 
     Args:
         server: The SMTP server to send the email on.
         sender: The email address of the message's author.
-        recipient: The intended recipient of the email.
+        to: The intended recipient of the email.
         subject: The subject header of the email.
         body: The body of the email, written in Markdown.
+        cc: Address(es) to CC.
+        bcc: Address(es) to BCC.
     """
     email = MarkdownEmail(sender, subject, body)
-    message = email.get_message(recipient)
+    message = email.get_message(to, cc, bcc)
 
     server.send_message(message)
 
 
-def send_markdown_email_from_file(server: SMTP, sender: str, recipient: str, subject: str, file_name: Path):
+def send_markdown_email_from_file(
+    server: SMTP,
+    sender: str,
+    to: str | list[str],
+    subject: str,
+    file_name: Path,
+    cc: str | list[str] | None = None,
+    bcc: str | list[str] | None = None,
+):
     """Sends a Markdown-formatted email message loaded from a file with the given parameters.
 
     Before calling, server must be ready for a send_message method invocation.
 
     Args:
         server: The SMTP server to send the email on.
         sender: The email address of the message's author.
-        recipient: The intended recipient of the email.
+        to: The intended recipient of the email.
         subject: The subject header of the email.
         file_name: The path to the file containing the message to send.
+        cc: Address(es) to CC.
+        bcc: Address(es) to BCC.
     """
     with file_name.open() as file:
         body = file.read()
-    send_markdown_email(server, sender, recipient, subject, body)
+    send_markdown_email(server, sender, to, subject, body, cc, bcc)
```

### Comparing `earendil_mail-0.1.0/earendil/markdown_email.py` & `earendil_mail-0.2.0/earendil/markdown_email.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,17 +25,33 @@
 
         self.markdown_body = body
         self.plain_text = render_plain(body)
         self.plain_mime = MIMEText(self.plain_text, "plain")
         self.html_text = render_html(body)
         self.html_mime = MIMEText(self.html_text, "html")
 
-    def get_message(self, recipient: str) -> MIMEMultipart:
+    def get_message(
+        self,
+        to: str | list[str],
+        cc: str | list[str] | None = None,
+        bcc: str | list[str] | None = None,
+    ) -> MIMEMultipart:
+        cc = [] if cc is None else cc
+        bcc = [] if bcc is None else bcc
+
         mime = MIMEMultipart("alternative")
         mime["From"] = self.sender
-        mime["To"] = recipient
+        mime["To"] = self.normalize_recipients(to)
+        mime["Cc"] = self.normalize_recipients(cc)
+        mime["Bcc"] = self.normalize_recipients(bcc)
         mime["Subject"] = self.subject
 
         mime.attach(self.plain_mime)
         mime.attach(self.html_mime)
 
         return mime
+
+    @staticmethod
+    def normalize_recipients(recipients: str | list[str]) -> str:
+        if isinstance(recipients, str):
+            return recipients
+        return ", ".join(recipients)
```

### Comparing `earendil_mail-0.1.0/earendil/plaintext_renderer.py` & `earendil_mail-0.2.0/earendil/plaintext_renderer.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         line = line[heading_count:]
         line = line.strip()
 
     # Remove unescaped asterisks used for emphasis.
     line = re.sub(__unescaped_emphasis, lambda match: match.group(0)[:-1], line)
 
     # Convert hyperlinks into URLs in parentheses.
-    line = re.sub(__hyperlink, lambda match: f"{match.group(1)} ({match.group(2)})", line)
+    line = re.sub(
+        __hyperlink, lambda match: f"{match.group(1)} ({match.group(2)})", line
+    )
 
     return line
 
 
 def markdown_to_plaintext(text: str) -> str:
     """Converts the given Markdown string to plaintext.
 
@@ -38,14 +40,18 @@
 
     Returns:
         Plaintext version of text, with extra formatting stripped out.
     """
     lines = text.split("\n")
 
     # Remove consecutive lines of whitespace.
-    trimmed_lines = [line for i, line in enumerate(lines) if i == 0 or line != lines[i - 1] or line != ""]
+    trimmed_lines = [
+        line
+        for i, line in enumerate(lines)
+        if i == 0 or line != lines[i - 1] or line != ""
+    ]
 
     new_lines = []
     for line in trimmed_lines:
         new_lines.append(__convert_markdown_line(line))
 
     return "\n".join(new_lines)
```

### Comparing `earendil_mail-0.1.0/pyproject.toml` & `earendil_mail-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "earendil_mail"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Markdown-based HTML email API."
 authors = ["Alex Steele <45648397+ADSteele916@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ADSteele916/earendil"
 repository = "https://github.com/ADSteele916/earendil"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "earendil" },
 ]
 
+[tool.poetry.urls]
+"Issue Tracker" = "https://github.com/ADSteele916/earendil/issues"
+
 [tool.poetry.dependencies]
-python = "^3.6.2"
-Markdown = "^3.3.6"
+python = "^3.10"
+Markdown = "^3.6"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-pytest-mock = "^3.6.1"
-pylint = "^2.12.2"
-yapf = "^0.32.0"
-isort = "^5.10.1"
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.0"
+pytest-mock = "^3.14.0"
+ruff = "^0.4.4"
+black = "^24.4.2"
+isort = "^5.13.2"
 
-[tool.poetry.urls]
-"Issue Tracker" = "https://github.com/ADSteele916/earendil/issues"
+[tool.isort]
+profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `earendil_mail-0.1.0/README.md` & `earendil_mail-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Eärendil
 
+> Eärendil was a mariner\
+> that tarried in Arvernien;\
+> he built a boat of timber felled\
+> in Nimbrethil to journey in;
+
 Eärendil is a Markdown-based HTML email API written in Python. It allows users to draft an email message in Markdown 
 and send it as a rich email viewable as both HTML and plaintext.
 
 My primary motivation for creating this library was the lack of good options for sending rich emails with an alternative
 plaintext message for recipients who may be using a dated email service. I think that providing a faithful 
 alternative message is important, and that simply using the Markdown used to generate the HTML message as the 
 alternative is insufficient. Markdown, while fairly human-readable compared to most markup languages, still contains 
@@ -14,15 +19,14 @@
 
 * Renders Common Markdown messages into HTML.
 * Renders a subset of Markdown into plaintext.
 * Sends Markdown emails from either strings or files.
 
 ### Planned Features
 
-* Bulk mailing functionality.
 * Support for rendering a greater subset of Markdown as plaintext.
 * Support for attachments.
 
 ## Usage
 
 To send Markdown-formatted emails using Eärendil, use either the `send_markdown_email`or `send_markdown_email_from_file`
 functions. Here is an example that uses each:
```

### Comparing `earendil_mail-0.1.0/setup.py` & `earendil_mail-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,99 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: earendil_mail
+Version: 0.2.0
+Summary: A Markdown-based HTML email API.
+Home-page: https://github.com/ADSteele916/earendil
+Author: Alex Steele
+Author-email: 45648397+ADSteele916@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Markdown (>=3.6,<4.0)
+Project-URL: Issue Tracker, https://github.com/ADSteele916/earendil/issues
+Project-URL: Repository, https://github.com/ADSteele916/earendil
+Description-Content-Type: text/markdown
+
+# Eärendil
+
+> Eärendil was a mariner\
+> that tarried in Arvernien;\
+> he built a boat of timber felled\
+> in Nimbrethil to journey in;
+
+Eärendil is a Markdown-based HTML email API written in Python. It allows users to draft an email message in Markdown 
+and send it as a rich email viewable as both HTML and plaintext.
+
+My primary motivation for creating this library was the lack of good options for sending rich emails with an alternative
+plaintext message for recipients who may be using a dated email service. I think that providing a faithful 
+alternative message is important, and that simply using the Markdown used to generate the HTML message as the 
+alternative is insufficient. Markdown, while fairly human-readable compared to most markup languages, still contains 
+redundant or unhelpful syntax that is better expressed differently in plaintext. For example, escape characters 
+should be removed, as should heading and emphasis symbols.
+
+## Features
+
+* Renders Common Markdown messages into HTML.
+* Renders a subset of Markdown into plaintext.
+* Sends Markdown emails from either strings or files.
+
+### Planned Features
+
+* Support for rendering a greater subset of Markdown as plaintext.
+* Support for attachments.
+
+## Usage
+
+To send Markdown-formatted emails using Eärendil, use either the `send_markdown_email`or `send_markdown_email_from_file`
+functions. Here is an example that uses each:
+
+```python
+from pathlib import Path
+from smtplib import SMTP
+
+from earendil import send_markdown_email, send_markdown_email_from_file
+
+sender_email = "sender@gmail.com"
+password = "password"
+recipient = "receiver@example.com"
+
+subject = "Example Subject"
+message_path = Path("/path/to/markdown.md")
+with message_path.open("r") as file:
+    message = file.read()
+
+with SMTP("smtp.gmail.com", 587) as server:
+    server.starttls()
+    server.login(sender_email, password)
+    # Here, you can either use:
+    send_markdown_email(server, sender_email, recipient, subject, message)
+    # or, alternatively:
+    send_markdown_email_from_file(server, sender_email, recipient, subject, message_path)
+```
+
+## Installation
+
+### Requirements
+
+Eärendil can run on any version of Python since `3.6.2` (inclusive). It also depends on the `markdown` library.
+
+### From PyPI
+
+The easiest way to install Eärendil is to simply run the command `pip3 install earendil-mail`.
+
+### From Source
+
+Alternatively, Eärendil can be installed from source by cloning this repository. To do so, run the following commands:
+```commandline
+git clone https://github.com/ADSteele916/earendil
+cd earendil
+pip3 install .
+```
 
-packages = \
-['earendil']
+## Uninstallation
 
-package_data = \
-{'': ['*']}
+To uninstall, simply run the command `pip3 uninstall earendil-mail`
 
-install_requires = \
-['Markdown>=3.3.6,<4.0.0']
-
-setup_kwargs = {
-    'name': 'earendil-mail',
-    'version': '0.1.0',
-    'description': 'A Markdown-based HTML email API.',
-    'long_description': '# Eärendil\n\nEärendil is a Markdown-based HTML email API written in Python. It allows users to draft an email message in Markdown \nand send it as a rich email viewable as both HTML and plaintext.\n\nMy primary motivation for creating this library was the lack of good options for sending rich emails with an alternative\nplaintext message for recipients who may be using a dated email service. I think that providing a faithful \nalternative message is important, and that simply using the Markdown used to generate the HTML message as the \nalternative is insufficient. Markdown, while fairly human-readable compared to most markup languages, still contains \nredundant or unhelpful syntax that is better expressed differently in plaintext. For example, escape characters \nshould be removed, as should heading and emphasis symbols.\n\n## Features\n\n* Renders Common Markdown messages into HTML.\n* Renders a subset of Markdown into plaintext.\n* Sends Markdown emails from either strings or files.\n\n### Planned Features\n\n* Bulk mailing functionality.\n* Support for rendering a greater subset of Markdown as plaintext.\n* Support for attachments.\n\n## Usage\n\nTo send Markdown-formatted emails using Eärendil, use either the `send_markdown_email`or `send_markdown_email_from_file`\nfunctions. Here is an example that uses each:\n\n```python\nfrom pathlib import Path\nfrom smtplib import SMTP\n\nfrom earendil import send_markdown_email, send_markdown_email_from_file\n\nsender_email = "sender@gmail.com"\npassword = "password"\nrecipient = "receiver@example.com"\n\nsubject = "Example Subject"\nmessage_path = Path("/path/to/markdown.md")\nwith message_path.open("r") as file:\n    message = file.read()\n\nwith SMTP("smtp.gmail.com", 587) as server:\n    server.starttls()\n    server.login(sender_email, password)\n    # Here, you can either use:\n    send_markdown_email(server, sender_email, recipient, subject, message)\n    # or, alternatively:\n    send_markdown_email_from_file(server, sender_email, recipient, subject, message_path)\n```\n\n## Installation\n\n### Requirements\n\nEärendil can run on any version of Python since `3.6.2` (inclusive). It also depends on the `markdown` library.\n\n### From PyPI\n\nThe easiest way to install Eärendil is to simply run the command `pip3 install earendil-mail`.\n\n### From Source\n\nAlternatively, Eärendil can be installed from source by cloning this repository. To do so, run the following commands:\n```commandline\ngit clone https://github.com/ADSteele916/earendil\ncd earendil\npip3 install .\n```\n\n## Uninstallation\n\nTo uninstall, simply run the command `pip3 uninstall earendil-mail`\n',
-    'author': 'Alex Steele',
-    'author_email': '45648397+ADSteele916@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ADSteele916/earendil',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

