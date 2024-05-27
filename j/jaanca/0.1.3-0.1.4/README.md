# Comparing `tmp/jaanca-0.1.3.tar.gz` & `tmp/jaanca-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca-0.1.3.tar", last modified: Fri May 24 20:14:06 2024, max compression
+gzip compressed data, was "jaanca-0.1.4.tar", last modified: Mon May 27 23:02:20 2024, max compression
```

## Comparing `jaanca-0.1.3.tar` & `jaanca-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.996433 jaanca-0.1.3/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4013 2024-05-24 20:14:05.996433 jaanca-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2828 2024-05-24 20:13:55.000000 jaanca-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.978433 jaanca-0.1.3/jaanca/
--rw-rw-rw-   0        0        0       70 2024-05-24 15:55:34.000000 jaanca-0.1.3/jaanca/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.988431 jaanca-0.1.3/jaanca/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca-0.1.3/jaanca/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.991431 jaanca-0.1.3/jaanca/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca-0.1.3/jaanca/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-24 15:55:34.000000 jaanca-0.1.3/jaanca/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.994433 jaanca-0.1.3/jaanca.egg-info/
--rw-rw-rw-   0        0        0     4013 2024-05-24 20:14:05.000000 jaanca-0.1.3/jaanca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-24 20:14:05.000000 jaanca-0.1.3/jaanca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 20:14:05.000000 jaanca-0.1.3/jaanca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-24 20:14:05.000000 jaanca-0.1.3/jaanca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 20:14:05.997430 jaanca-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1520 2024-05-24 20:12:43.000000 jaanca-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:02:20.278691 jaanca-0.1.4/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4296 2024-05-27 23:02:20.278691 jaanca-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2024-05-27 23:01:55.000000 jaanca-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 23:02:20.262690 jaanca-0.1.4/jaanca/
+-rw-rw-rw-   0        0        0       70 2024-05-24 15:55:34.000000 jaanca-0.1.4/jaanca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:02:20.271696 jaanca-0.1.4/jaanca/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca-0.1.4/jaanca/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:02:20.274690 jaanca-0.1.4/jaanca/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca-0.1.4/jaanca/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-27 13:33:48.000000 jaanca-0.1.4/jaanca/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:02:20.276690 jaanca-0.1.4/jaanca.egg-info/
+-rw-rw-rw-   0        0        0     4296 2024-05-27 23:02:20.000000 jaanca-0.1.4/jaanca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-27 23:02:20.000000 jaanca-0.1.4/jaanca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 23:02:20.000000 jaanca-0.1.4/jaanca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 23:02:20.000000 jaanca-0.1.4/jaanca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 23:02:20.279692 jaanca-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1520 2024-05-27 23:01:15.000000 jaanca-0.1.4/setup.py
```

### Comparing `jaanca-0.1.3/LICENSE.txt` & `jaanca-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca-0.1.3/PKG-INFO` & `jaanca-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool library created by jaanca.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta
@@ -48,16 +48,17 @@
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca)
 | [Package (PyPI)](https://pypi.org/project/jaanca/)
 
 ---
 
 # Here is a non-exhaustive list of related packages:
 
-- [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
-- [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) : jaanca's helper for date and time management and moving dates between time days by UTC
+- [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer.
+- [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) : jaanca's helper for date and time management and moving dates between time days by UTC.
+- [jaanca-datetime](https://pypi.org/project/jaanca-utils-os/) : jaanca's helper for operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 
 ---
 
 # Semantic Versioning
 
 jaanca < MAJOR >.< MINOR >.< PATCH >
 
@@ -103,7 +104,11 @@
 ## [0.1.2] - 2024-05-23
 ### Added
 - Documentation improvements.
 
 ## [0.1.3] - 2024-05-24
 ### Added
 - New feature jaanca-datetime.
+
+## [0.1.4] - 2024-05-27
+### Added
+- New feature jaanca-utils-os.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca Version: 0.1.3 Summary: A tool library
+Metadata-Version: 2.1 Name: jaanca Version: 0.1.4 Summary: A tool library
 created by jaanca. Home-page: https://github.com/jaanca/python-libraries/tree/
 main/jaanca Author: Jaime Andres Cardona Carrillo Author-email:
 jacardona@outlook.com License: MIT License Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
@@ -16,33 +16,37 @@
 File: LICENSE.txt
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca [Source code](https://github.com/jaanca/
 python-libraries/tree/main/jaanca) | [Package (PyPI)](https://pypi.org/project/
 jaanca/) --- # Here is a non-exhaustive list of related packages: - [jaanca-
 chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper
-chronometer - [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) :
+chronometer. - [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) :
 jaanca's helper for date and time management and moving dates between time days
-by UTC --- # Semantic Versioning jaanca < MAJOR >.< MINOR >.< PATCH > *
-**MAJOR**: version when you make incompatible API changes * **MINOR**: version
-when you add functionality in a backwards compatible manner * **PATCH**:
-version when you make backwards compatible bug fixes ## Definitions for
-releasing versions * https://peps.python.org/pep-0440/ - X.YaN (Alpha release):
-Identify and fix early-stage bugs. Not suitable for production use. - X.YbN
-(Beta release): Stabilize and refine features. Address reported bugs. Prepare
-for official release. - X.YrcN (Release candidate): Final version before
-official release. Assumes all major features are complete and stable.
-Recommended for testing in non-critical environments. - X.Y (Final release/
-Stable/Production): Completed, stable version ready for use in production. Full
-release for public use. --- # Changelog All notable changes to this project
-will be documented in this file. The format is based on [Keep a Changelog]
-(https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
-Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
-for new features. - Changed for changes in existing functionality. - Deprecated
-for soon-to-be removed features. - Removed for now removed features. - Fixed
-for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
-05-21 ### Added - First tests using pypi.org in develop environment. - Examples
-of use are added to the documentation of the functions in docstring - In the
-samples folder of this library, there are complete working examples of using
-the code. ## [0.1.X] - 2024-05-21 ### Added - Completion of testing and launch
-into production. ## [0.1.2] - 2024-05-23 ### Added - Documentation
-improvements. ## [0.1.3] - 2024-05-24 ### Added - New feature jaanca-datetime.
+by UTC. - [jaanca-datetime](https://pypi.org/project/jaanca-utils-os/) :
+jaanca's helper for operating system help functions such as reading environment
+variables, reading/writing files, file properties, among others. --- # Semantic
+Versioning jaanca < MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version when you
+make incompatible API changes * **MINOR**: version when you add functionality
+in a backwards compatible manner * **PATCH**: version when you make backwards
+compatible bug fixes ## Definitions for releasing versions * https://
+peps.python.org/pep-0440/ - X.YaN (Alpha release): Identify and fix early-stage
+bugs. Not suitable for production use. - X.YbN (Beta release): Stabilize and
+refine features. Address reported bugs. Prepare for official release. - X.YrcN
+(Release candidate): Final version before official release. Assumes all major
+features are complete and stable. Recommended for testing in non-critical
+environments. - X.Y (Final release/Stable/Production): Completed, stable
+version ready for use in production. Full release for public use. --- #
+Changelog All notable changes to this project will be documented in this file.
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/
+), and this project adheres to [Semantic Versioning](https://semver.org/spec/
+v2.0.0.html). ## Types of changes - Added for new features. - Changed for
+changes in existing functionality. - Deprecated for soon-to-be removed
+features. - Removed for now removed features. - Fixed for any bug fixes. -
+Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-05-21 ### Added -
+First tests using pypi.org in develop environment. - Examples of use are added
+to the documentation of the functions in docstring - In the samples folder of
+this library, there are complete working examples of using the code. ## [0.1.X]
+- 2024-05-21 ### Added - Completion of testing and launch into production. ##
+[0.1.2] - 2024-05-23 ### Added - Documentation improvements. ## [0.1.3] - 2024-
+05-24 ### Added - New feature jaanca-datetime. ## [0.1.4] - 2024-05-27 ###
+Added - New feature jaanca-utils-os.
```

### Comparing `jaanca-0.1.3/README.md` & `jaanca-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca)
 | [Package (PyPI)](https://pypi.org/project/jaanca/)
 
 ---
 
 # Here is a non-exhaustive list of related packages:
 
-- [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
-- [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) : jaanca's helper for date and time management and moving dates between time days by UTC
+- [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer.
+- [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) : jaanca's helper for date and time management and moving dates between time days by UTC.
+- [jaanca-datetime](https://pypi.org/project/jaanca-utils-os/) : jaanca's helper for operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 
 ---
 
 # Semantic Versioning
 
 jaanca < MAJOR >.< MINOR >.< PATCH >
 
@@ -74,7 +75,11 @@
 ## [0.1.2] - 2024-05-23
 ### Added
 - Documentation improvements.
 
 ## [0.1.3] - 2024-05-24
 ### Added
 - New feature jaanca-datetime.
+
+## [0.1.4] - 2024-05-27
+### Added
+- New feature jaanca-utils-os.
```

#### html2text {}

```diff
@@ -1,32 +1,36 @@
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca [Source code](https://github.com/jaanca/
 python-libraries/tree/main/jaanca) | [Package (PyPI)](https://pypi.org/project/
 jaanca/) --- # Here is a non-exhaustive list of related packages: - [jaanca-
 chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper
-chronometer - [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) :
+chronometer. - [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) :
 jaanca's helper for date and time management and moving dates between time days
-by UTC --- # Semantic Versioning jaanca < MAJOR >.< MINOR >.< PATCH > *
-**MAJOR**: version when you make incompatible API changes * **MINOR**: version
-when you add functionality in a backwards compatible manner * **PATCH**:
-version when you make backwards compatible bug fixes ## Definitions for
-releasing versions * https://peps.python.org/pep-0440/ - X.YaN (Alpha release):
-Identify and fix early-stage bugs. Not suitable for production use. - X.YbN
-(Beta release): Stabilize and refine features. Address reported bugs. Prepare
-for official release. - X.YrcN (Release candidate): Final version before
-official release. Assumes all major features are complete and stable.
-Recommended for testing in non-critical environments. - X.Y (Final release/
-Stable/Production): Completed, stable version ready for use in production. Full
-release for public use. --- # Changelog All notable changes to this project
-will be documented in this file. The format is based on [Keep a Changelog]
-(https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
-Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
-for new features. - Changed for changes in existing functionality. - Deprecated
-for soon-to-be removed features. - Removed for now removed features. - Fixed
-for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
-05-21 ### Added - First tests using pypi.org in develop environment. - Examples
-of use are added to the documentation of the functions in docstring - In the
-samples folder of this library, there are complete working examples of using
-the code. ## [0.1.X] - 2024-05-21 ### Added - Completion of testing and launch
-into production. ## [0.1.2] - 2024-05-23 ### Added - Documentation
-improvements. ## [0.1.3] - 2024-05-24 ### Added - New feature jaanca-datetime.
+by UTC. - [jaanca-datetime](https://pypi.org/project/jaanca-utils-os/) :
+jaanca's helper for operating system help functions such as reading environment
+variables, reading/writing files, file properties, among others. --- # Semantic
+Versioning jaanca < MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version when you
+make incompatible API changes * **MINOR**: version when you add functionality
+in a backwards compatible manner * **PATCH**: version when you make backwards
+compatible bug fixes ## Definitions for releasing versions * https://
+peps.python.org/pep-0440/ - X.YaN (Alpha release): Identify and fix early-stage
+bugs. Not suitable for production use. - X.YbN (Beta release): Stabilize and
+refine features. Address reported bugs. Prepare for official release. - X.YrcN
+(Release candidate): Final version before official release. Assumes all major
+features are complete and stable. Recommended for testing in non-critical
+environments. - X.Y (Final release/Stable/Production): Completed, stable
+version ready for use in production. Full release for public use. --- #
+Changelog All notable changes to this project will be documented in this file.
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/
+), and this project adheres to [Semantic Versioning](https://semver.org/spec/
+v2.0.0.html). ## Types of changes - Added for new features. - Changed for
+changes in existing functionality. - Deprecated for soon-to-be removed
+features. - Removed for now removed features. - Fixed for any bug fixes. -
+Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-05-21 ### Added -
+First tests using pypi.org in develop environment. - Examples of use are added
+to the documentation of the functions in docstring - In the samples folder of
+this library, there are complete working examples of using the code. ## [0.1.X]
+- 2024-05-21 ### Added - Completion of testing and launch into production. ##
+[0.1.2] - 2024-05-23 ### Added - Documentation improvements. ## [0.1.3] - 2024-
+05-24 ### Added - New feature jaanca-datetime. ## [0.1.4] - 2024-05-27 ###
+Added - New feature jaanca-utils-os.
```

### Comparing `jaanca-0.1.3/jaanca/utils/helpers/chronometer.py` & `jaanca-0.1.4/jaanca/utils/helpers/chronometer.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.__end_time = time.time()
     def reset(self)->None:
         '''Set the stopwatch to zero
         '''
         self.__start_time=0
         self.__end_time=0
     def get_elapsed_time(self)->Interval:
-        '''Descripcion
+        '''Description
         :return Interval(str): HH:mm:ss format supported for inserting records into databases and adding elapsed times
 
         ## Example
         ```Python
         import time
 
         chronometer=Chronometer()
```

### Comparing `jaanca-0.1.3/jaanca.egg-info/PKG-INFO` & `jaanca-0.1.4/jaanca.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool library created by jaanca.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta
@@ -48,16 +48,17 @@
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca)
 | [Package (PyPI)](https://pypi.org/project/jaanca/)
 
 ---
 
 # Here is a non-exhaustive list of related packages:
 
-- [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
-- [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) : jaanca's helper for date and time management and moving dates between time days by UTC
+- [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer.
+- [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) : jaanca's helper for date and time management and moving dates between time days by UTC.
+- [jaanca-datetime](https://pypi.org/project/jaanca-utils-os/) : jaanca's helper for operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 
 ---
 
 # Semantic Versioning
 
 jaanca < MAJOR >.< MINOR >.< PATCH >
 
@@ -103,7 +104,11 @@
 ## [0.1.2] - 2024-05-23
 ### Added
 - Documentation improvements.
 
 ## [0.1.3] - 2024-05-24
 ### Added
 - New feature jaanca-datetime.
+
+## [0.1.4] - 2024-05-27
+### Added
+- New feature jaanca-utils-os.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca Version: 0.1.3 Summary: A tool library
+Metadata-Version: 2.1 Name: jaanca Version: 0.1.4 Summary: A tool library
 created by jaanca. Home-page: https://github.com/jaanca/python-libraries/tree/
 main/jaanca Author: Jaime Andres Cardona Carrillo Author-email:
 jacardona@outlook.com License: MIT License Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
@@ -16,33 +16,37 @@
 File: LICENSE.txt
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca [Source code](https://github.com/jaanca/
 python-libraries/tree/main/jaanca) | [Package (PyPI)](https://pypi.org/project/
 jaanca/) --- # Here is a non-exhaustive list of related packages: - [jaanca-
 chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper
-chronometer - [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) :
+chronometer. - [jaanca-datetime](https://pypi.org/project/jaanca-datetime/) :
 jaanca's helper for date and time management and moving dates between time days
-by UTC --- # Semantic Versioning jaanca < MAJOR >.< MINOR >.< PATCH > *
-**MAJOR**: version when you make incompatible API changes * **MINOR**: version
-when you add functionality in a backwards compatible manner * **PATCH**:
-version when you make backwards compatible bug fixes ## Definitions for
-releasing versions * https://peps.python.org/pep-0440/ - X.YaN (Alpha release):
-Identify and fix early-stage bugs. Not suitable for production use. - X.YbN
-(Beta release): Stabilize and refine features. Address reported bugs. Prepare
-for official release. - X.YrcN (Release candidate): Final version before
-official release. Assumes all major features are complete and stable.
-Recommended for testing in non-critical environments. - X.Y (Final release/
-Stable/Production): Completed, stable version ready for use in production. Full
-release for public use. --- # Changelog All notable changes to this project
-will be documented in this file. The format is based on [Keep a Changelog]
-(https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
-Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
-for new features. - Changed for changes in existing functionality. - Deprecated
-for soon-to-be removed features. - Removed for now removed features. - Fixed
-for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
-05-21 ### Added - First tests using pypi.org in develop environment. - Examples
-of use are added to the documentation of the functions in docstring - In the
-samples folder of this library, there are complete working examples of using
-the code. ## [0.1.X] - 2024-05-21 ### Added - Completion of testing and launch
-into production. ## [0.1.2] - 2024-05-23 ### Added - Documentation
-improvements. ## [0.1.3] - 2024-05-24 ### Added - New feature jaanca-datetime.
+by UTC. - [jaanca-datetime](https://pypi.org/project/jaanca-utils-os/) :
+jaanca's helper for operating system help functions such as reading environment
+variables, reading/writing files, file properties, among others. --- # Semantic
+Versioning jaanca < MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version when you
+make incompatible API changes * **MINOR**: version when you add functionality
+in a backwards compatible manner * **PATCH**: version when you make backwards
+compatible bug fixes ## Definitions for releasing versions * https://
+peps.python.org/pep-0440/ - X.YaN (Alpha release): Identify and fix early-stage
+bugs. Not suitable for production use. - X.YbN (Beta release): Stabilize and
+refine features. Address reported bugs. Prepare for official release. - X.YrcN
+(Release candidate): Final version before official release. Assumes all major
+features are complete and stable. Recommended for testing in non-critical
+environments. - X.Y (Final release/Stable/Production): Completed, stable
+version ready for use in production. Full release for public use. --- #
+Changelog All notable changes to this project will be documented in this file.
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/
+), and this project adheres to [Semantic Versioning](https://semver.org/spec/
+v2.0.0.html). ## Types of changes - Added for new features. - Changed for
+changes in existing functionality. - Deprecated for soon-to-be removed
+features. - Removed for now removed features. - Fixed for any bug fixes. -
+Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-05-21 ### Added -
+First tests using pypi.org in develop environment. - Examples of use are added
+to the documentation of the functions in docstring - In the samples folder of
+this library, there are complete working examples of using the code. ## [0.1.X]
+- 2024-05-21 ### Added - Completion of testing and launch into production. ##
+[0.1.2] - 2024-05-23 ### Added - Documentation improvements. ## [0.1.3] - 2024-
+05-24 ### Added - New feature jaanca-datetime. ## [0.1.4] - 2024-05-27 ###
+Added - New feature jaanca-utils-os.
```

### Comparing `jaanca-0.1.3/setup.py` & `jaanca-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca"
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME}.',
```

