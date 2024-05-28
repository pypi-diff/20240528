# Comparing `tmp/pymongocrypt-1.8.0.tar.gz` & `tmp/pymongocrypt-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongocrypt-1.8.0.tar", last modified: Tue Jan  9 11:32:54 2024, max compression
+gzip compressed data, was "pymongocrypt-1.9.1.tar", last modified: Wed Feb 28 20:52:05 2024, max compression
```

## Comparing `pymongocrypt-1.8.0.tar` & `pymongocrypt-1.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-09 11:32:54.463497 pymongocrypt-1.8.0/
--rw-r--r--   0 runner     (501) staff       (20)    11357 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    21736 2024-01-09 11:32:54.462756 pymongocrypt-1.8.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     7362 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-09 11:32:54.455935 pymongocrypt-1.8.0/pymongocrypt/
--rw-r--r--   0 runner     (501) staff       (20)      687 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2053 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/auto_encrypter.py
--rw-r--r--   0 runner     (501) staff       (20)     3031 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/binary.py
--rw-r--r--   0 runner     (501) staff       (20)    55376 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/binding.py
--rw-r--r--   0 runner     (501) staff       (20)     1027 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/compat.py
--rw-r--r--   0 runner     (501) staff       (20)     5147 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/credentials.py
--rw-r--r--   0 runner     (501) staff       (20)     6157 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/crypto.py
--rw-r--r--   0 runner     (501) staff       (20)     1393 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/errors.py
--rw-r--r--   0 runner     (501) staff       (20)    11125 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/explicit_encrypter.py
--rw-r--r--   0 runner     (501) staff       (20)    32003 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/mongocrypt.py
--rw-r--r--   0 runner     (501) staff       (20)     4850 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/state_machine.py
--rw-r--r--   0 runner     (501) staff       (20)      642 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pymongocrypt/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-09 11:32:54.462069 pymongocrypt-1.8.0/pymongocrypt.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    21736 2024-01-09 11:32:54.000000 pymongocrypt-1.8.0/pymongocrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      602 2024-01-09 11:32:54.000000 pymongocrypt-1.8.0/pymongocrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-09 11:32:54.000000 pymongocrypt-1.8.0/pymongocrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       64 2024-01-09 11:32:54.000000 pymongocrypt-1.8.0/pymongocrypt.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2024-01-09 11:32:54.000000 pymongocrypt-1.8.0/pymongocrypt.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1708 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-01-09 11:32:54.463591 pymongocrypt-1.8.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1193 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-09 11:32:54.461406 pymongocrypt-1.8.0/test/
--rw-r--r--   0 runner     (501) staff       (20)     2398 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/test/test_binding.py
--rw-r--r--   0 runner     (501) staff       (20)     3479 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/test/test_crypto.py
--rw-r--r--   0 runner     (501) staff       (20)    35736 2024-01-09 11:31:46.000000 pymongocrypt-1.8.0/test/test_mongocrypt.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 20:52:05.267986 pymongocrypt-1.9.1/
+-rw-r--r--   0 runner     (501) staff       (20)    11357 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    22966 2024-02-28 20:52:05.266810 pymongocrypt-1.9.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     8592 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 20:52:05.257990 pymongocrypt-1.9.1/pymongocrypt/
+-rw-r--r--   0 runner     (501) staff       (20)      687 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2053 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/auto_encrypter.py
+-rw-r--r--   0 runner     (501) staff       (20)     3031 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/binary.py
+-rw-r--r--   0 runner     (501) staff       (20)    55676 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/binding.py
+-rw-r--r--   0 runner     (501) staff       (20)     1027 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/compat.py
+-rw-r--r--   0 runner     (501) staff       (20)     5147 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/credentials.py
+-rw-r--r--   0 runner     (501) staff       (20)     6157 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/crypto.py
+-rw-r--r--   0 runner     (501) staff       (20)     1393 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/errors.py
+-rw-r--r--   0 runner     (501) staff       (20)    11171 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/explicit_encrypter.py
+-rw-r--r--   0 runner     (501) staff       (20)    32663 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/mongocrypt.py
+-rw-r--r--   0 runner     (501) staff       (20)     4850 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/state_machine.py
+-rw-r--r--   0 runner     (501) staff       (20)      642 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pymongocrypt/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 20:52:05.264974 pymongocrypt-1.9.1/pymongocrypt.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    22966 2024-02-28 20:52:05.000000 pymongocrypt-1.9.1/pymongocrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      602 2024-02-28 20:52:05.000000 pymongocrypt-1.9.1/pymongocrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-02-28 20:52:05.000000 pymongocrypt-1.9.1/pymongocrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       64 2024-02-28 20:52:05.000000 pymongocrypt-1.9.1/pymongocrypt.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2024-02-28 20:52:05.000000 pymongocrypt-1.9.1/pymongocrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1708 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-02-28 20:52:05.268119 pymongocrypt-1.9.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1193 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 20:52:05.264325 pymongocrypt-1.9.1/test/
+-rw-r--r--   0 runner     (501) staff       (20)     2398 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/test/test_binding.py
+-rw-r--r--   0 runner     (501) staff       (20)     3479 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/test/test_crypto.py
+-rw-r--r--   0 runner     (501) staff       (20)    36894 2024-02-28 20:51:22.000000 pymongocrypt-1.9.1/test/test_mongocrypt.py
```

### Comparing `pymongocrypt-1.8.0/LICENSE` & `pymongocrypt-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/PKG-INFO` & `pymongocrypt-1.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongocrypt
-Version: 1.8.0
+Version: 1.9.1
 Summary: Python bindings for libmongocrypt
 Author-email: Shane Harvey <mongodb-user@googlegroups.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -307,15 +307,15 @@
 Installation
 ============
 
 PyMongoCrypt can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
   $ python -m pip install pymongocrypt
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 
 PyMongoCrypt ships wheels for macOS, Windows, and manylinux2010 that include
 an embedded libmongocrypt build.
 
 Installing from wheels on Linux requires pip 19 or later because it adds
 `support for manylinux2010 wheels <https://pip.pypa.io/en/stable/news/#id108>`_.
@@ -332,53 +332,74 @@
 Installing from source (or the pymongocrypt-X.Y.tar.gz source distribution,
 or pip < 19 on Linux) requires an extra step of installing libmongocrypt.
 First, install PyMongoCrypt from source::
 
   $ git clone git@github.com:mongodb/libmongocrypt.git
   $ python -m pip install ./libmongocrypt/bindings/python
 
-Next, install libmongocrypt.
+Next, install libmongocrypt:
+
+Installing libmongocrypt
+^^^^^^^^^^^^^^^^^^^^^^^^
 
 libmongocrypt is continuously built and published on evergreen.
 The latest tarball containing libmongocrypt built on all supported variants is
 `published here <https://s3.amazonaws.com/mciuploads/libmongocrypt/all/master/latest/libmongocrypt-all.tar.gz>`_.
 Download and extract ``libmongocrypt-all.tar.gz`` and set
 ``PYMONGOCRYPT_LIB`` to the path to your operating system's libmongocrypt.so file.
 For example::
 
   $ curl -O https://s3.amazonaws.com/mciuploads/libmongocrypt/all/master/latest/libmongocrypt-all.tar.gz
   $ mkdir libmongocrypt-all && tar xzf libmongocrypt-all.tar.gz -C libmongocrypt-all
   $ ls libmongocrypt-all
-  amazon2             rhel-62-64-bit      rhel72-zseries-test ubuntu1604-arm64
-  debian10            rhel-67-s390x       suse12-64           ubuntu1804-64
-  debian92            rhel-70-64-bit      suse12-s390x        ubuntu1804-arm64
-  linux-64-amazon-ami rhel-71-ppc64el     suse15-64           windows-test
-  macos               rhel-80-64-bit      ubuntu1604
+  amazon2             debian92            rhel-80-64-bit      rhel72-zseries-test ubuntu1804-arm64
+  amazon2-arm64       linux-64-amazon-ami rhel-81-ppc64el     suse12-64           ubuntu2004-64
+  amazon2023          macos               rhel-82-arm64       suse15-64           ubuntu2004-arm64
+  amazon2023-arm64    rhel-62-64-bit      rhel-83-zseries     ubuntu1604          ubuntu2204-64
+  debian10            rhel-70-64-bit      rhel-91-64-bit      ubuntu1604-arm64    ubuntu2204-arm64
+  debian11            rhel-71-ppc64el     rhel-91-arm64       ubuntu1804-64       windows-test
 
 macOS::
 
   $ # Set PYMONGOCRYPT_LIB for macOS:
-  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/macos/nocrypto/lib/libmongocrypt.dylib
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/macos/lib/libmongocrypt.dylib
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 Windows::
 
   $ # Set PYMONGOCRYPT_LIB for Windows:
-  $ chmod +x $(pwd)/libmongocrypt-all/windows-test/nocrypto/bin/mongocrypt.dll
-  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/windows-test/nocrypto/bin/mongocrypt.dll
+  $ chmod +x $(pwd)/libmongocrypt-all/windows-test/bin/mongocrypt.dll
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/windows-test/bin/mongocrypt.dll
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
+
+Linux: set the libmongocrypt build for your platform, for example for Ubuntu 22.04 x86_64::
 
-Linux::
+  $ # Set PYMONGOCRYPT_LIB for Ubuntu 22.04 x86_64:
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/ubuntu2204-64/lib/libmongocrypt.so
+  $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
+  1.9.0
+  $ # Check that native crypto is enabled for better performance:
+  $ python -c 'from pymongocrypt.binding import lib;print(lib.mongocrypt_is_crypto_available())'
+  True
+
+Note if your Linux platform is not available, the generic RHEL 6.2 x86_64 "nocrypto" build
+should still be compatible however the "nocrypto" build will result in lower performance
+for encryption and decryption::
 
   $ # Set PYMONGOCRYPT_LIB for RHEL 6.2 x86_64:
   $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/rhel-62-64-bit/nocrypto/lib64/libmongocrypt.so
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
+  $ python -c 'from pymongocrypt.binding import lib;print(lib.mongocrypt_is_crypto_available())'
+  False
+
+Other methods of installation (brew, rpm, yum, apt-get, deb, etc...) are documented here:
+https://www.mongodb.com/docs/manual/core/csfle/reference/libmongocrypt/#linux-installation
 
 Dependencies
 ============
 
 PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 PyMongoCrypt requires `cffi <https://pypi.org/project/cffi/>`_ and
@@ -408,14 +429,14 @@
 
 Use the ``PYMONGOCRYPT_LIB`` environment variable to load a locally installed
 libmongocrypt build without relying on platform specific library path environment
 variables, like ``LD_LIBRARY_PATH``. For example::
 
   $ export PYMONGOCRYPT_LIB='/path/to/libmongocrypt.so'
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 Testing
 =======
 
 The easiest way to run the tests is to run **python setup.py test** in
 the root of the distribution.
```

### Comparing `pymongocrypt-1.8.0/README.rst` & `pymongocrypt-1.9.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 Installation
 ============
 
 PyMongoCrypt can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
   $ python -m pip install pymongocrypt
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 
 PyMongoCrypt ships wheels for macOS, Windows, and manylinux2010 that include
 an embedded libmongocrypt build.
 
 Installing from wheels on Linux requires pip 19 or later because it adds
 `support for manylinux2010 wheels <https://pip.pypa.io/en/stable/news/#id108>`_.
@@ -98,53 +98,74 @@
 Installing from source (or the pymongocrypt-X.Y.tar.gz source distribution,
 or pip < 19 on Linux) requires an extra step of installing libmongocrypt.
 First, install PyMongoCrypt from source::
 
   $ git clone git@github.com:mongodb/libmongocrypt.git
   $ python -m pip install ./libmongocrypt/bindings/python
 
-Next, install libmongocrypt.
+Next, install libmongocrypt:
+
+Installing libmongocrypt
+^^^^^^^^^^^^^^^^^^^^^^^^
 
 libmongocrypt is continuously built and published on evergreen.
 The latest tarball containing libmongocrypt built on all supported variants is
 `published here <https://s3.amazonaws.com/mciuploads/libmongocrypt/all/master/latest/libmongocrypt-all.tar.gz>`_.
 Download and extract ``libmongocrypt-all.tar.gz`` and set
 ``PYMONGOCRYPT_LIB`` to the path to your operating system's libmongocrypt.so file.
 For example::
 
   $ curl -O https://s3.amazonaws.com/mciuploads/libmongocrypt/all/master/latest/libmongocrypt-all.tar.gz
   $ mkdir libmongocrypt-all && tar xzf libmongocrypt-all.tar.gz -C libmongocrypt-all
   $ ls libmongocrypt-all
-  amazon2             rhel-62-64-bit      rhel72-zseries-test ubuntu1604-arm64
-  debian10            rhel-67-s390x       suse12-64           ubuntu1804-64
-  debian92            rhel-70-64-bit      suse12-s390x        ubuntu1804-arm64
-  linux-64-amazon-ami rhel-71-ppc64el     suse15-64           windows-test
-  macos               rhel-80-64-bit      ubuntu1604
+  amazon2             debian92            rhel-80-64-bit      rhel72-zseries-test ubuntu1804-arm64
+  amazon2-arm64       linux-64-amazon-ami rhel-81-ppc64el     suse12-64           ubuntu2004-64
+  amazon2023          macos               rhel-82-arm64       suse15-64           ubuntu2004-arm64
+  amazon2023-arm64    rhel-62-64-bit      rhel-83-zseries     ubuntu1604          ubuntu2204-64
+  debian10            rhel-70-64-bit      rhel-91-64-bit      ubuntu1604-arm64    ubuntu2204-arm64
+  debian11            rhel-71-ppc64el     rhel-91-arm64       ubuntu1804-64       windows-test
 
 macOS::
 
   $ # Set PYMONGOCRYPT_LIB for macOS:
-  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/macos/nocrypto/lib/libmongocrypt.dylib
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/macos/lib/libmongocrypt.dylib
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 Windows::
 
   $ # Set PYMONGOCRYPT_LIB for Windows:
-  $ chmod +x $(pwd)/libmongocrypt-all/windows-test/nocrypto/bin/mongocrypt.dll
-  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/windows-test/nocrypto/bin/mongocrypt.dll
+  $ chmod +x $(pwd)/libmongocrypt-all/windows-test/bin/mongocrypt.dll
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/windows-test/bin/mongocrypt.dll
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
+
+Linux: set the libmongocrypt build for your platform, for example for Ubuntu 22.04 x86_64::
 
-Linux::
+  $ # Set PYMONGOCRYPT_LIB for Ubuntu 22.04 x86_64:
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/ubuntu2204-64/lib/libmongocrypt.so
+  $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
+  1.9.0
+  $ # Check that native crypto is enabled for better performance:
+  $ python -c 'from pymongocrypt.binding import lib;print(lib.mongocrypt_is_crypto_available())'
+  True
+
+Note if your Linux platform is not available, the generic RHEL 6.2 x86_64 "nocrypto" build
+should still be compatible however the "nocrypto" build will result in lower performance
+for encryption and decryption::
 
   $ # Set PYMONGOCRYPT_LIB for RHEL 6.2 x86_64:
   $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/rhel-62-64-bit/nocrypto/lib64/libmongocrypt.so
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
+  $ python -c 'from pymongocrypt.binding import lib;print(lib.mongocrypt_is_crypto_available())'
+  False
+
+Other methods of installation (brew, rpm, yum, apt-get, deb, etc...) are documented here:
+https://www.mongodb.com/docs/manual/core/csfle/reference/libmongocrypt/#linux-installation
 
 Dependencies
 ============
 
 PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 PyMongoCrypt requires `cffi <https://pypi.org/project/cffi/>`_ and
@@ -174,14 +195,14 @@
 
 Use the ``PYMONGOCRYPT_LIB`` environment variable to load a locally installed
 libmongocrypt build without relying on platform specific library path environment
 variables, like ``LD_LIBRARY_PATH``. For example::
 
   $ export PYMONGOCRYPT_LIB='/path/to/libmongocrypt.so'
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 Testing
 =======
 
 The easiest way to run the tests is to run **python setup.py test** in
 the root of the distribution.
```

### Comparing `pymongocrypt-1.8.0/pymongocrypt/__init__.py` & `pymongocrypt-1.9.1/pymongocrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pymongocrypt/auto_encrypter.py` & `pymongocrypt-1.9.1/pymongocrypt/auto_encrypter.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pymongocrypt/binary.py` & `pymongocrypt-1.9.1/pymongocrypt/binary.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pymongocrypt/binding.py` & `pymongocrypt-1.9.1/pymongocrypt/binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,24 @@
  *
  * @param[out] len  An optional length of the returned string. May be NULL.
  * @returns a NULL terminated version string for libmongocrypt.
  */
 const char *mongocrypt_version(uint32_t *len);
 
 /**
+ * Returns true if libmongocrypt was built with native crypto support.
+ *
+ * If libmongocrypt was not built with native crypto support, setting crypto
+ * hooks is required.
+ *
+ * @returns True if libmongocrypt was built with native crypto support.
+ */
+bool mongocrypt_is_crypto_available(void);
+
+/**
  * A non-owning view of a byte buffer.
  *
  * When constructing a mongocrypt_binary_t it is the responsibility of the
  * caller to maintain the lifetime of the viewed data. However, all public
  * functions that take a mongocrypt_binary_t as an argument will make a copy of
  * the viewed data. For example, the following is valid:
  *
```

### Comparing `pymongocrypt-1.8.0/pymongocrypt/compat.py` & `pymongocrypt-1.9.1/pymongocrypt/compat.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pymongocrypt/credentials.py` & `pymongocrypt-1.9.1/pymongocrypt/credentials.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pymongocrypt/crypto.py` & `pymongocrypt-1.9.1/pymongocrypt/crypto.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pymongocrypt/errors.py` & `pymongocrypt-1.9.1/pymongocrypt/errors.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pymongocrypt/explicit_encrypter.py` & `pymongocrypt-1.9.1/pymongocrypt/explicit_encrypter.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,16 @@
 
     def create_data_key(self, kms_provider, master_key=None,
                         key_alt_names=None, key_material=None):
         """Creates a data key used for explicit encryption.
 
         :Parameters:
           - `kms_provider`: The KMS provider to use. Supported values are
-            "aws", "azure", "gcp", "kmip", and "local".
+            "aws", "azure", "gcp", "kmip", "local", or a named provider like
+            "kmip:name".
           - `master_key`: See class:`DataKeyOpts`.
           - `key_alt_names` (optional): An optional list of string alternate
             names used to reference a key. If a key is created with alternate
             names, then encryption may refer to the key by the unique
             alternate name instead of by ``_id``.
           - `key_material`: (optional) See class:`DataKeyOpts`.
```

### Comparing `pymongocrypt-1.8.0/pymongocrypt/mongocrypt.py` & `pymongocrypt-1.9.1/pymongocrypt/mongocrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
+import sys
+import platform
 
+from packaging.version import Version
 
 from pymongocrypt.binary import (MongoCryptBinaryIn,
                                  MongoCryptBinaryOut)
 from pymongocrypt.binding import ffi, lib, _to_string
 from pymongocrypt.compat import str_to_bytes, unicode_type
 from pymongocrypt.credentials import _ask_for_kms_credentials
 from pymongocrypt.errors import MongoCryptError
@@ -47,14 +49,18 @@
                  and optionally a "sessionToken" for temporary credentials.
               - `azure`: Map with "clientId" and "clientSecret" as strings.
               - `gcp`: Map with "email" as a string and "privateKey" as
                 a byte array or a base64-encoded string.
               - `kmip`: Map with "endpoint" as a string.
               - `local`: Map with "key" as a 96-byte array or the equivalent
                 base64-encoded string.
+
+            KMS providers may be specified with an optional name suffix
+            separated by a colon, for example "kmip:name". Named KMS providers
+            do not support automatic credential lookup.
           - `schema_map`: Optional map of collection namespace ("db.coll") to
             JSON Schema.  By default, a collection's JSONSchema is periodically
             polled with the listCollections command. But a JSONSchema may be
             specified locally with the schemaMap option.
 
             Supplying a `schema_map` provides more security than relying on
             JSON Schemas obtained from the server. It protects against a
@@ -89,67 +95,50 @@
            as either a 96-byte array or the equivalent base64-encoded string.
         """
         if not isinstance(kms_providers, dict):
             raise ValueError('kms_providers must be a dict')
         if not kms_providers:
             raise ValueError('at least one KMS provider must be configured')
 
-        if 'aws' in kms_providers:
-            aws = kms_providers["aws"]
-            if not isinstance(aws, dict):
-                raise ValueError("kms_providers['aws'] must be a dict")
-            if len(aws):
-                if "accessKeyId" not in aws or "secretAccessKey" not in aws:
-                    raise ValueError("kms_providers['aws'] must contain "
-                                     "'accessKeyId' and 'secretAccessKey'")
-
-        if 'azure' in kms_providers:
-            azure = kms_providers["azure"]
-            if not isinstance(azure, dict):
-                raise ValueError("kms_providers['azure'] must be a dict")
-            if len(azure):
-                if 'clientId' not in azure or 'clientSecret' not in azure:
-                    raise ValueError("kms_providers['azure'] must contain "
-                                     "'clientId' and 'clientSecret'")
-
-        if 'gcp' in kms_providers:
-            gcp = kms_providers['gcp']
-            if not isinstance(gcp, dict):
-                raise ValueError("kms_providers['gcp'] must be a dict")
-            if len(gcp):
-                if 'email' not in gcp or 'privateKey' not in gcp:
-                    raise ValueError("kms_providers['gcp'] must contain "
-                                     "'email' and 'privateKey'")
-                if not isinstance(kms_providers['gcp']['privateKey'],
-                                  (bytes, unicode_type)):
-                    raise TypeError("kms_providers['gcp']['privateKey'] must "
-                                    "be an instance of bytes or str")
-
-        if 'kmip' in kms_providers:
-            kmip = kms_providers['kmip']
-            if not isinstance(kmip, dict):
-                raise ValueError("kms_providers['kmip'] must be a dict")
-            if 'endpoint' not in kmip:
-                raise ValueError("kms_providers['kmip'] must contain "
-                                 "'endpoint'")
-            if not isinstance(kms_providers['kmip']['endpoint'],
-                              (str, unicode_type)):
-                raise TypeError("kms_providers['kmip']['endpoint'] must "
-                                "be an instance of str")
-
-        if 'local' in kms_providers:
-            local = kms_providers['local']
-            if not isinstance(local, dict):
-                raise ValueError("kms_providers['local'] must be a dict")
-            if 'key' not in local:
-                raise ValueError("kms_providers['local'] must contain 'key'")
-            if not isinstance(kms_providers['local']['key'],
-                              (bytes, unicode_type)):
-                raise TypeError("kms_providers['local']['key'] must be an "
-                                "instance of bytes or str")
+        for name, provider in kms_providers.items():
+            # Account for provider names like "local:myname".
+            provider_type = name.split(":")[0]
+            if provider_type in ('aws', 'gcp', 'azure', 'kmip', 'local'):
+                if not isinstance(provider, dict):
+                    raise ValueError(f"kms_providers[{name!r}] must be a dict")
+            if provider_type == 'aws':
+                if len(provider):
+                    if "accessKeyId" not in provider or "secretAccessKey" not in provider:
+                        raise ValueError(f"kms_providers[{name!r}] must contain "
+                                         "'accessKeyId' and 'secretAccessKey'")
+            elif provider_type == 'azure':
+                if len(provider):
+                    if 'clientId' not in provider or 'clientSecret' not in provider:
+                        raise ValueError(f"kms_providers[{name!r}] must contain "
+                                         "'clientId' and 'clientSecret'")
+            elif provider_type == 'gcp':
+                if len(provider):
+                    if 'email' not in provider or 'privateKey' not in provider:
+                        raise ValueError(f"kms_providers[{name!r}] must contain "
+                                         "'email' and 'privateKey'")
+                    if not isinstance(provider['privateKey'], (bytes, unicode_type)):
+                        raise TypeError(f"kms_providers[{name!r}]['privateKey'] must "
+                                        "be an instance of bytes or str")
+            elif provider_type == 'kmip':
+                if 'endpoint' not in provider:
+                    raise ValueError(f"kms_providers[{name!r}] must contain 'endpoint'")
+                if not isinstance(provider['endpoint'], (str, unicode_type)):
+                    raise TypeError(f"kms_providers[{name!r}]['endpoint'] must "
+                                    "be an instance of str")
+            elif provider_type == 'local':
+                if 'key' not in provider:
+                    raise ValueError(f"kms_providers[{name!r}] must contain 'key'")
+                if not isinstance(provider['key'], (bytes, unicode_type)):
+                    raise TypeError(f"kms_providers[{name!r}]['key'] must be an "
+                                    "instance of bytes or str")
 
         if schema_map is not None and not isinstance(schema_map, bytes):
             raise TypeError("schema_map must be bytes or None")
 
         if encrypted_fields_map is not None and not isinstance(encrypted_fields_map, bytes):
             raise TypeError("encrypted_fields_map must be bytes or None")
 
@@ -214,26 +203,39 @@
                 if not lib.mongocrypt_setopt_encrypted_field_config_map(
                         self.__crypt, binary_encrypted_fields_map.bin):
                     self.__raise_from_status()
 
         if self.__opts.bypass_query_analysis:
             lib.mongocrypt_setopt_bypass_query_analysis(self.__crypt)
 
-        if not lib.mongocrypt_setopt_crypto_hooks(
-                self.__crypt, aes_256_cbc_encrypt, aes_256_cbc_decrypt,
-                secure_random, hmac_sha_512, hmac_sha_256, sha_256, ffi.NULL):
-            self.__raise_from_status()
+        # Prefer using the native crypto binding when we know it's available.
+        try:
+            crypto_available = lib.mongocrypt_is_crypto_available()
+        except AttributeError:
+            # libmongocrypt < 1.9
+            crypto_available = False
+
+        if not crypto_available:
+            if not lib.mongocrypt_setopt_crypto_hooks(
+                    self.__crypt, aes_256_cbc_encrypt, aes_256_cbc_decrypt,
+                    secure_random, hmac_sha_512, hmac_sha_256, sha_256, ffi.NULL):
+                self.__raise_from_status()
 
-        if not lib.mongocrypt_setopt_crypto_hook_sign_rsaes_pkcs1_v1_5(
-                self.__crypt, sign_rsaes_pkcs1_v1_5, ffi.NULL):
-            self.__raise_from_status()
+            if not lib.mongocrypt_setopt_crypto_hook_sign_rsaes_pkcs1_v1_5(
+                    self.__crypt, sign_rsaes_pkcs1_v1_5, ffi.NULL):
+                self.__raise_from_status()
 
-        if not lib.mongocrypt_setopt_aes_256_ctr(
-                self.__crypt, aes_256_ctr_encrypt, aes_256_ctr_decrypt, ffi.NULL):
-            self.__raise_from_status()
+            if not lib.mongocrypt_setopt_aes_256_ctr(
+                    self.__crypt, aes_256_ctr_encrypt, aes_256_ctr_decrypt, ffi.NULL):
+                self.__raise_from_status()
+        elif sys.platform == 'darwin' and Version(platform.mac_ver()[0]) < Version("10.15"):
+            # MONGOCRYPT-440 libmongocrypt does not support AES-CTR on macOS < 10.15.
+            if not lib.mongocrypt_setopt_aes_256_ctr(
+                    self.__crypt, aes_256_ctr_encrypt, aes_256_ctr_decrypt, ffi.NULL):
+                self.__raise_from_status()
 
         if self.__opts.crypt_shared_lib_path is not None:
             lib.mongocrypt_setopt_set_crypt_shared_lib_path_override(
                 self.__crypt, self.__opts.crypt_shared_lib_path.encode("utf-8"))
 
         if not self.__opts.bypass_encryption:
             lib.mongocrypt_setopt_append_crypt_shared_lib_search_path(self.__crypt, b"$SYSTEM")
@@ -607,47 +609,48 @@
           - `kms_providers`: The KMS provider map.
           - `kms_provider`: The KMS provider.
           - `opts`: An optional class:`DataKeyOpts`.
           - `callback`: A :class:`MongoCryptCallback`.
         """
         super(DataKeyContext, self).__init__(ctx, kms_providers)
         try:
-            if kms_provider not in ['aws', 'gcp', 'azure', 'kmip', 'local']:
+            if kms_provider not in kms_providers:
                 raise ValueError('unknown kms_provider: %s' % (kms_provider,))
 
+            # Account for provider names like "local:myname".
+            provider_type = kms_provider.split(":")[0]
             if opts is None or opts.master_key is None:
-                if kms_provider in ['kmip', 'local']:
+                if provider_type in ['kmip', 'local']:
                     master_key = {}
                 else:
                     raise ValueError(
-                        'master_key is required for kms_provider: "%s"' % (
-                            kms_provider,))
+                        f'master_key is required for kms_provider: {kms_provider!r}')
             else:
                 master_key = opts.master_key.copy()
 
-            if kms_provider == 'aws':
+            if provider_type == 'aws':
                 if ('region' not in master_key or
                         'key' not in master_key):
                     raise ValueError(
                         'master_key must include "region" and "key" for '
-                        'kms_provider: "aws"')
-            elif kms_provider == 'azure':
+                        f'kms_provider: {kms_provider!r}')
+            elif provider_type == 'azure':
                 if ('keyName' not in master_key or
                         'keyVaultEndpoint' not in master_key):
                     raise ValueError(
                         'master key must include "keyName" and '
-                        '"keyVaultEndpoint" for kms_provider: "azure"')
-            elif kms_provider == 'gcp':
+                        f'"keyVaultEndpoint" for kms_provider: {kms_provider!r}')
+            elif provider_type == 'gcp':
                 if ('projectId' not in master_key or
                         'location' not in master_key or
                         'keyRing' not in master_key or
                         'keyName' not in master_key):
                     raise ValueError(
                         'master key must include "projectId", "location",'
-                        '"keyRing", and "keyName" for kms_provider: "gcp"')
+                        f'"keyRing", and "keyName" for kms_provider: {kms_provider!r}')
 
             master_key['provider'] = kms_provider
             with MongoCryptBinaryIn(
                     callback.bson_encode(master_key)) as mkey:
                 if not lib.mongocrypt_ctx_setopt_key_encryption_key(
                         ctx, mkey.bin):
                     self._raise_from_status()
```

### Comparing `pymongocrypt-1.8.0/pymongocrypt/state_machine.py` & `pymongocrypt-1.9.1/pymongocrypt/state_machine.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pymongocrypt/version.py` & `pymongocrypt-1.9.1/pymongocrypt/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.8.0'
+__version__ = '1.9.1'
 
 _MIN_LIBMONGOCRYPT_VERSION = '1.8.0'
```

### Comparing `pymongocrypt-1.8.0/pymongocrypt.egg-info/PKG-INFO` & `pymongocrypt-1.9.1/pymongocrypt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongocrypt
-Version: 1.8.0
+Version: 1.9.1
 Summary: Python bindings for libmongocrypt
 Author-email: Shane Harvey <mongodb-user@googlegroups.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -307,15 +307,15 @@
 Installation
 ============
 
 PyMongoCrypt can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
   $ python -m pip install pymongocrypt
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 
 PyMongoCrypt ships wheels for macOS, Windows, and manylinux2010 that include
 an embedded libmongocrypt build.
 
 Installing from wheels on Linux requires pip 19 or later because it adds
 `support for manylinux2010 wheels <https://pip.pypa.io/en/stable/news/#id108>`_.
@@ -332,53 +332,74 @@
 Installing from source (or the pymongocrypt-X.Y.tar.gz source distribution,
 or pip < 19 on Linux) requires an extra step of installing libmongocrypt.
 First, install PyMongoCrypt from source::
 
   $ git clone git@github.com:mongodb/libmongocrypt.git
   $ python -m pip install ./libmongocrypt/bindings/python
 
-Next, install libmongocrypt.
+Next, install libmongocrypt:
+
+Installing libmongocrypt
+^^^^^^^^^^^^^^^^^^^^^^^^
 
 libmongocrypt is continuously built and published on evergreen.
 The latest tarball containing libmongocrypt built on all supported variants is
 `published here <https://s3.amazonaws.com/mciuploads/libmongocrypt/all/master/latest/libmongocrypt-all.tar.gz>`_.
 Download and extract ``libmongocrypt-all.tar.gz`` and set
 ``PYMONGOCRYPT_LIB`` to the path to your operating system's libmongocrypt.so file.
 For example::
 
   $ curl -O https://s3.amazonaws.com/mciuploads/libmongocrypt/all/master/latest/libmongocrypt-all.tar.gz
   $ mkdir libmongocrypt-all && tar xzf libmongocrypt-all.tar.gz -C libmongocrypt-all
   $ ls libmongocrypt-all
-  amazon2             rhel-62-64-bit      rhel72-zseries-test ubuntu1604-arm64
-  debian10            rhel-67-s390x       suse12-64           ubuntu1804-64
-  debian92            rhel-70-64-bit      suse12-s390x        ubuntu1804-arm64
-  linux-64-amazon-ami rhel-71-ppc64el     suse15-64           windows-test
-  macos               rhel-80-64-bit      ubuntu1604
+  amazon2             debian92            rhel-80-64-bit      rhel72-zseries-test ubuntu1804-arm64
+  amazon2-arm64       linux-64-amazon-ami rhel-81-ppc64el     suse12-64           ubuntu2004-64
+  amazon2023          macos               rhel-82-arm64       suse15-64           ubuntu2004-arm64
+  amazon2023-arm64    rhel-62-64-bit      rhel-83-zseries     ubuntu1604          ubuntu2204-64
+  debian10            rhel-70-64-bit      rhel-91-64-bit      ubuntu1604-arm64    ubuntu2204-arm64
+  debian11            rhel-71-ppc64el     rhel-91-arm64       ubuntu1804-64       windows-test
 
 macOS::
 
   $ # Set PYMONGOCRYPT_LIB for macOS:
-  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/macos/nocrypto/lib/libmongocrypt.dylib
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/macos/lib/libmongocrypt.dylib
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 Windows::
 
   $ # Set PYMONGOCRYPT_LIB for Windows:
-  $ chmod +x $(pwd)/libmongocrypt-all/windows-test/nocrypto/bin/mongocrypt.dll
-  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/windows-test/nocrypto/bin/mongocrypt.dll
+  $ chmod +x $(pwd)/libmongocrypt-all/windows-test/bin/mongocrypt.dll
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/windows-test/bin/mongocrypt.dll
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
+
+Linux: set the libmongocrypt build for your platform, for example for Ubuntu 22.04 x86_64::
 
-Linux::
+  $ # Set PYMONGOCRYPT_LIB for Ubuntu 22.04 x86_64:
+  $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/ubuntu2204-64/lib/libmongocrypt.so
+  $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
+  1.9.0
+  $ # Check that native crypto is enabled for better performance:
+  $ python -c 'from pymongocrypt.binding import lib;print(lib.mongocrypt_is_crypto_available())'
+  True
+
+Note if your Linux platform is not available, the generic RHEL 6.2 x86_64 "nocrypto" build
+should still be compatible however the "nocrypto" build will result in lower performance
+for encryption and decryption::
 
   $ # Set PYMONGOCRYPT_LIB for RHEL 6.2 x86_64:
   $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/rhel-62-64-bit/nocrypto/lib64/libmongocrypt.so
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
+  $ python -c 'from pymongocrypt.binding import lib;print(lib.mongocrypt_is_crypto_available())'
+  False
+
+Other methods of installation (brew, rpm, yum, apt-get, deb, etc...) are documented here:
+https://www.mongodb.com/docs/manual/core/csfle/reference/libmongocrypt/#linux-installation
 
 Dependencies
 ============
 
 PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 PyMongoCrypt requires `cffi <https://pypi.org/project/cffi/>`_ and
@@ -408,14 +429,14 @@
 
 Use the ``PYMONGOCRYPT_LIB`` environment variable to load a locally installed
 libmongocrypt build without relying on platform specific library path environment
 variables, like ``LD_LIBRARY_PATH``. For example::
 
   $ export PYMONGOCRYPT_LIB='/path/to/libmongocrypt.so'
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
-  1.2.1
+  1.9.0
 
 Testing
 =======
 
 The easiest way to run the tests is to run **python setup.py test** in
 the root of the distribution.
```

### Comparing `pymongocrypt-1.8.0/pymongocrypt.egg-info/SOURCES.txt` & `pymongocrypt-1.9.1/pymongocrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/pyproject.toml` & `pymongocrypt-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/setup.py` & `pymongocrypt-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/test/test_binding.py` & `pymongocrypt-1.9.1/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/test/test_crypto.py` & `pymongocrypt-1.9.1/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.8.0/test/test_mongocrypt.py` & `pymongocrypt-1.9.1/test/test_mongocrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 class TestMongoCryptOptions(unittest.TestCase):
 
     def test_mongocrypt_options(self):
         schema_map = bson_data('schema-map.json')
         valid = [
             ({'local': {'key': b'1' * 96}}, None),
-            ({ 'aws' : {} }, schema_map),
+            ({'aws': {}}, schema_map),
             ({'aws': {'accessKeyId': '', 'secretAccessKey': ''}}, schema_map),
             ({'aws': {'accessKeyId': 'foo', 'secretAccessKey': 'foo'}}, None),
             ({'aws': {'accessKeyId': 'foo', 'secretAccessKey': 'foo',
                       'sessionToken': 'token'}}, None),
             ({'aws': {'accessKeyId': 'foo', 'secretAccessKey': 'foo'},
               'local': {'key': b'1' * 96}}, None),
             ({'local': {'key': to_base64(b'1' * 96)}}, None),
@@ -105,16 +105,22 @@
             ({'azure': {'clientId': 'foo', 'clientSecret': 'bar'}}, None),
             ({'gcp': {}}, None),
             ({'gcp': {'email': 'foo@bar.baz',
                       'privateKey': b'1'}}, None),
             ({'gcp': {'email': 'foo@bar.baz',
                       'privateKey': to_base64(b'1')}}, None),
             ({'gcp': {'email': 'foo@bar.baz',
-                      'privateKey': Binary(b'1')}}, None)
+                      'privateKey': Binary(b'1')}}, None),
+            ({'kmip': {'endpoint': 'localhost'}}, None),
         ]
+        # Add tests for named KMS providers.
+        for kms_providers, schema_map in valid:
+            for name, val in list(kms_providers.items()):
+                kms_providers[f'{name}:named'] = val
+
         for kms_providers, schema_map in valid:
             opts = MongoCryptOptions(kms_providers, schema_map)
             self.assertEqual(opts.kms_providers, kms_providers, msg=kms_providers)
             self.assertEqual(opts.schema_map, schema_map)
             self.assertIsNone(opts.encrypted_fields_map)
             self.assertFalse(opts.bypass_query_analysis)
 
@@ -126,28 +132,38 @@
 
     def test_mongocrypt_options_validation(self):
         with self.assertRaisesRegex(
                 ValueError, 'at least one KMS provider must be configured'):
             MongoCryptOptions({})
         for invalid_kms_providers in [
                 {'aws': {'accessKeyId': 'foo'}},
-                {'aws': {'secretAccessKey': 'foo'}}]:
+                {'aws': {'secretAccessKey': 'foo'}},
+                {'aws:foo': {'accessKeyId': 'foo'}},
+                {'aws:foo': {'secretAccessKey': 'foo'}},
+        ]:
+            name = next(iter(invalid_kms_providers))
             with self.assertRaisesRegex(
-                    ValueError, r"kms_providers\['aws'\] must contain "
+                    ValueError, rf"kms_providers\[{name!r}\] must contain "
                                 "'accessKeyId' and 'secretAccessKey'"):
                 MongoCryptOptions(invalid_kms_providers)
         with self.assertRaisesRegex(
                 TypeError, r"kms_providers\['local'\]\['key'\] must be an "
                            r"instance of bytes or str"):
             MongoCryptOptions({'local': {'key': None}})
         with self.assertRaisesRegex(
                 TypeError, r"kms_providers\['gcp'\]\['privateKey'\] must be an "
                            r"instance of bytes or str"):
             MongoCryptOptions({'gcp': {'email': "foo@bar.baz",
                                        "privateKey": None}})
+        with self.assertRaisesRegex(
+                ValueError, r"kms_providers\['kmip'\] must contain 'endpoint'"):
+            MongoCryptOptions({'kmip': {}})
+        with self.assertRaisesRegex(
+                TypeError, r"kms_providers\['kmip'\]\['endpoint'\] must be an instance of str"):
+            MongoCryptOptions({'kmip': {'endpoint': None}})
 
         valid_kms = {'aws': {'accessKeyId': '', 'secretAccessKey': ''}}
         with self.assertRaisesRegex(
                 TypeError, "schema_map must be bytes or None"):
             MongoCryptOptions(valid_kms, schema_map={})
 
         with self.assertRaisesRegex(
@@ -220,16 +236,15 @@
             mc.close()
 
             # Case 3: pass key as unicode string containing bytes (invalid)
             kms_dict[f1][f2] = unicode_type(b'\x00' * 96)
             options = MongoCryptOptions(kms_dict)
             with self.assertRaisesRegex(
                     MongoCryptError,
-                    "unable to parse base64 from UTF-8 field %s.%s" % (
-                            f1, f2)):
+                    "unable to parse base64 from UTF-8 field"):
                 MongoCrypt(options, callback)
 
         # Case 4: pass key as base64-encoded string (invalid)
         # Only applicable to "local" as key length is not validated for gcp.
         kms_dict = copy.deepcopy(base_kms_dict)
         kms_dict['local']['key'] = base64.b64encode(b'\x00' * 96)
         options = MongoCryptOptions(kms_dict)
@@ -714,20 +729,28 @@
                 decrypted = encrypter.decrypt(encrypted)
                 self.assertEqual(bson.decode(decrypted, OPTS), val)
                 self.assertEqual(encoded_val, decrypted)
 
     def test_data_key_creation(self):
         mock_key_vault = KeyVaultCallback(
             kms_reply=http_data('kms-encrypt-reply.txt'))
-        encrypter = ExplicitEncrypter(mock_key_vault, self.mongo_crypt_opts())
+        opts = MongoCryptOptions({
+            'aws': {'accessKeyId': 'example', 'secretAccessKey': 'example'},
+            'aws:named': {'accessKeyId': 'example', 'secretAccessKey': 'example'},
+            'local': {'key': b'\x00' * 96},
+            'local:named': {'key': b'\x01' * 96},
+        })
+        encrypter = ExplicitEncrypter(mock_key_vault, opts)
         self.addCleanup(encrypter.close)
 
         valid_args = [
             ('local', None, ['first', 'second']),
+            ('local:named', None, ['local:named']),
             ('aws', {'region': 'region', 'key': 'cmk'}, ['third', 'forth']),
+            ('aws:named', {'region': 'region', 'key': 'cmk'}, ['aws:named']),
             # Unicode region and key
             ('aws', {'region': u'region-unicode', 'key': u'cmk-unicode'}, []),
             # Endpoint
             ('aws', {'region': 'region', 'key': 'cmk',
                      'endpoint': 'kms.us-east-1.amazonaws.com:443'}, []),
         ]
         for kms_provider, master_key, key_alt_names in valid_args:
```

