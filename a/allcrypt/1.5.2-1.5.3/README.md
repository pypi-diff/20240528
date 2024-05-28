# Comparing `tmp/allcrypt-1.5.2.tar.gz` & `tmp/allcrypt-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allcrypt-1.5.2.tar", last modified: Tue May 28 11:49:28 2024, max compression
+gzip compressed data, was "allcrypt-1.5.3.tar", last modified: Tue May 28 12:31:14 2024, max compression
```

## Comparing `allcrypt-1.5.2.tar` & `allcrypt-1.5.3.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 11:49:28.200968 allcrypt-1.5.2/
--rw-rw-rw-   0        0        0     2609 2024-05-28 11:49:28.198970 allcrypt-1.5.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-28 11:49:28.168697 allcrypt-1.5.2/allcrypt/
--rw-rw-rw-   0        0        0        0 2024-01-05 05:40:04.000000 allcrypt-1.5.2/allcrypt/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-06 12:24:33.000000 allcrypt-1.5.2/allcrypt/better.py
--rw-rw-rw-   0        0        0     4006 2024-03-10 23:00:38.000000 allcrypt-1.5.2/allcrypt/idk.py
--rw-rw-rw-   0        0        0    16113 2024-05-28 11:45:46.000000 allcrypt-1.5.2/allcrypt/main.py
--rw-rw-rw-   0        0        0       63 2024-04-08 06:10:20.000000 allcrypt-1.5.2/allcrypt/test.py
-drwxrwxrwx   0        0        0        0 2024-05-28 11:49:28.194035 allcrypt-1.5.2/allcrypt.egg-info/
--rw-rw-rw-   0        0        0     2609 2024-05-28 11:49:27.000000 allcrypt-1.5.2/allcrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-28 11:49:27.000000 allcrypt-1.5.2/allcrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 11:49:27.000000 allcrypt-1.5.2/allcrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-28 11:49:27.000000 allcrypt-1.5.2/allcrypt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2024-05-28 11:49:27.000000 allcrypt-1.5.2/allcrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 11:49:27.000000 allcrypt-1.5.2/allcrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 11:49:28.200968 allcrypt-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-05-28 11:48:56.000000 allcrypt-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:31:14.976838 allcrypt-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 12:31:02.000000 allcrypt-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-28 12:31:14.976838 allcrypt-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-28 12:31:02.000000 allcrypt-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:31:14.976838 allcrypt-1.5.3/allcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-28 12:31:14.000000 allcrypt-1.5.3/allcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 12:31:14.000000 allcrypt-1.5.3/allcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:31:14.000000 allcrypt-1.5.3/allcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 12:31:14.000000 allcrypt-1.5.3/allcrypt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 12:31:14.000000 allcrypt-1.5.3/allcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:31:14.000000 allcrypt-1.5.3/allcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:31:14.976838 allcrypt-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 12:31:02.000000 allcrypt-1.5.3/setup.py
```

### Comparing `allcrypt-1.5.2/PKG-INFO` & `allcrypt-1.5.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,32 @@
-Metadata-Version: 2.1
-Name: allcrypt
-Version: 1.5.2
-Summary: Allcrypt - file/message encryption/decryption GUI with hardware token (USB) support.
-Author: Pranav A.
-Author-email: prnv.school@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-
+[![allcrypt build](https://github.com/pranavnasrani/allcrypt/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pranavnasrani/allcrypt/actions/workflows/python-publish.yml)
 # Allcrypt Encryption/Decryption
 
-Allcrypt is a Python application for file and message encryption/decryption using Fernet symmetric key cryptography.
+Allcrypt is a Python application for file and message encryption/decryption using Fernet symmetric key cryptography for Windows and Linux users.
 
 ## Features
 
 - Encrypt and decrypt files securely
 - Encrypt and decrypt messages
 - Generate and manage encryption keys on a USB drive
 
 ## Installation
 
-1. Install the package using pip:
+1. Install the latest package using pip:
 
     ```bash
     pip install allcrypt
     ```
 
 2. Run the Allcrypt GUI:
 
     ```bash
     allcrypt
     ```
-
+3. You can also install from the installer in the releases. (recommended for inexperienced users or those without Python)
 ## Usage
 
 ### Encrypt a Message
 
 1. Launch the Allcrypt GUI.
 2. Enter the path to the USB drive in the provided field.
 3. Enter the message or encrypted bytes in the text box.
@@ -75,14 +67,14 @@
 2. Enter the path to the USB drive in the provided field.
 3. Click the "Generate New Key for this USB" button.
 4. Enter a password for key encryption when prompted.
 5. The new key will be generated and saved on the USB drive.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the GNU v3 License - see the [LICENSE](LICENSE) file for details.
 
 ## About Me:
 
 1. My name is Pranav
-2. Visit my [Github](https://github.com/pranavnasrani)
-3. To look at source code on github and raise issues: [Allcrypt Source code](https://github.com/pranavnasrani/allcrypt)
+2. Visit my [Github](github.com/pranavnasrani)
+3. To look at source code on github and raise issues: [Allcrypt Source code](github.com/pranavnasrani/allcrypt)
```

### Comparing `allcrypt-1.5.2/allcrypt.egg-info/PKG-INFO` & `allcrypt-1.5.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,94 @@
-Metadata-Version: 2.1
-Name: allcrypt
-Version: 1.5.2
-Summary: Allcrypt - file/message encryption/decryption GUI with hardware token (USB) support.
-Author: Pranav A.
-Author-email: prnv.school@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-
-# Allcrypt Encryption/Decryption
-
-Allcrypt is a Python application for file and message encryption/decryption using Fernet symmetric key cryptography.
-
-## Features
-
-- Encrypt and decrypt files securely
-- Encrypt and decrypt messages
-- Generate and manage encryption keys on a USB drive
-
-## Installation
-
-1. Install the package using pip:
-
-    ```bash
-    pip install allcrypt
-    ```
-
-2. Run the Allcrypt GUI:
-
-    ```bash
-    allcrypt
-    ```
-
-## Usage
-
-### Encrypt a Message
-
-1. Launch the Allcrypt GUI.
-2. Enter the path to the USB drive in the provided field.
-3. Enter the message or encrypted bytes in the text box.
-4. Click the "Encrypt Message" button.
-5. Follow any prompts to enter the password for key encryption.
-
-### Decrypt a Message
-
-1. Launch the Allcrypt GUI.
-2. Enter the path to the USB drive in the provided field.
-3. Enter the encrypted message in the text box.
-4. Click the "Decrypt Message" button.
-5. Follow any prompts to enter the password for key decryption.
-
-### Encrypt a File
-
-1. Launch the Allcrypt GUI.
-2. Enter the path to the USB drive in the provided field.
-3. Click the "Encrypt File" button.
-4. Choose the source file to encrypt.
-5. Choose the destination file for the encrypted output.
-6. Optionally, check the "Compress Files" and "Shred Original File" checkboxes.
-7. Click the "Encrypt File" button.
-
-### Decrypt a File
-
-1. Launch the Allcrypt GUI.
-2. Enter the path to the USB drive in the provided field.
-3. Click the "Decrypt File" button.
-4. Choose the source file to decrypt.
-5. Choose the destination file for the decrypted output.
-6. Optionally, check the "Shred Original File" checkbox.
-7. Click the "Decrypt File" button.
-
-### Generate a New Key
-
-1. Launch the Allcrypt GUI.
-2. Enter the path to the USB drive in the provided field.
-3. Click the "Generate New Key for this USB" button.
-4. Enter a password for key encryption when prompted.
-5. The new key will be generated and saved on the USB drive.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-## About Me:
-
-1. My name is Pranav
-2. Visit my [Github](https://github.com/pranavnasrani)
-3. To look at source code on github and raise issues: [Allcrypt Source code](https://github.com/pranavnasrani/allcrypt)
+Metadata-Version: 2.1
+Name: allcrypt
+Version: 1.5.3
+Summary: Allcrypt - file/message encryption/decryption GUI with hardware token (USB) support.
+Author: Pranav A.
+Author-email: prnv.school@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cryptography
+Requires-Dist: tqdm
+Requires-Dist: psutil
+Requires-Dist: tkinter
+
+[![allcrypt build](https://github.com/pranavnasrani/allcrypt/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pranavnasrani/allcrypt/actions/workflows/python-publish.yml)
+# Allcrypt Encryption/Decryption
+
+Allcrypt is a Python application for file and message encryption/decryption using Fernet symmetric key cryptography for Windows and Linux users.
+
+## Features
+
+- Encrypt and decrypt files securely
+- Encrypt and decrypt messages
+- Generate and manage encryption keys on a USB drive
+
+## Installation
+
+1. Install the latest package using pip:
+
+    ```bash
+    pip install allcrypt
+    ```
+
+2. Run the Allcrypt GUI:
+
+    ```bash
+    allcrypt
+    ```
+3. You can also install from the installer in the releases. (recommended for inexperienced users or those without Python)
+## Usage
+
+### Encrypt a Message
+
+1. Launch the Allcrypt GUI.
+2. Enter the path to the USB drive in the provided field.
+3. Enter the message or encrypted bytes in the text box.
+4. Click the "Encrypt Message" button.
+5. Follow any prompts to enter the password for key encryption.
+
+### Decrypt a Message
+
+1. Launch the Allcrypt GUI.
+2. Enter the path to the USB drive in the provided field.
+3. Enter the encrypted message in the text box.
+4. Click the "Decrypt Message" button.
+5. Follow any prompts to enter the password for key decryption.
+
+### Encrypt a File
+
+1. Launch the Allcrypt GUI.
+2. Enter the path to the USB drive in the provided field.
+3. Click the "Encrypt File" button.
+4. Choose the source file to encrypt.
+5. Choose the destination file for the encrypted output.
+6. Optionally, check the "Compress Files" and "Shred Original File" checkboxes.
+7. Click the "Encrypt File" button.
+
+### Decrypt a File
+
+1. Launch the Allcrypt GUI.
+2. Enter the path to the USB drive in the provided field.
+3. Click the "Decrypt File" button.
+4. Choose the source file to decrypt.
+5. Choose the destination file for the decrypted output.
+6. Optionally, check the "Shred Original File" checkbox.
+7. Click the "Decrypt File" button.
+
+### Generate a New Key
+
+1. Launch the Allcrypt GUI.
+2. Enter the path to the USB drive in the provided field.
+3. Click the "Generate New Key for this USB" button.
+4. Enter a password for key encryption when prompted.
+5. The new key will be generated and saved on the USB drive.
+
+## License
+
+This project is licensed under the GNU v3 License - see the [LICENSE](LICENSE) file for details.
+
+## About Me:
+
+1. My name is Pranav
+2. Visit my [Github](github.com/pranavnasrani)
+3. To look at source code on github and raise issues: [Allcrypt Source code](github.com/pranavnasrani/allcrypt)
```

### Comparing `allcrypt-1.5.2/setup.py` & `allcrypt-1.5.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='allcrypt',
-    version='1.5.2',  # Update with your version number
+    version='1.5.3',  # Update with your version number
     long_description_content_type="text/markdown",
     long_description=open("allcrypt/README.md").read(),
     packages=find_packages(),
     install_requires=[
         'cryptography',
         'tqdm',
-        'psutil'
+        'psutil',
+        'tkinter'
     ],
     entry_points={
         'console_scripts': [
             'allcrypt = allcrypt.main:main',
         ],
     },
     author='Pranav A.',
```

