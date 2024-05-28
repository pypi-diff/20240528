# Comparing `tmp/macaw_auth-1.2.0.tar.gz` & `tmp/macaw_auth-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macaw_auth-1.2.0.tar", last modified: Fri Apr 26 22:14:12 2024, max compression
+gzip compressed data, was "macaw_auth-2.0.0.tar", last modified: Tue May 28 21:36:04 2024, max compression
```

## Comparing `macaw_auth-1.2.0.tar` & `macaw_auth-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/macaw_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 22:14:12.000000 macaw_auth-1.2.0/macaw_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.557889 macaw_auth-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/src/macaw_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/src/macaw_auth/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/idp_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/sts_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/classes/username_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/src/macaw_auth/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/src/macaw_auth/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:14:12.561889 macaw_auth-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-26 22:13:57.000000 macaw_auth-1.2.0/tests/test_usernames.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:36:04.590282 macaw_auth-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-28 21:36:04.590282 macaw_auth-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:36:04.590282 macaw_auth-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:36:04.586282 macaw_auth-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:36:04.586282 macaw_auth-2.0.0/src/macaw_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:36:04.586282 macaw_auth-2.0.0/src/macaw_auth/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/classes/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/classes/idp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/classes/sts_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/classes/user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/classes/username_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:36:04.590282 macaw_auth-2.0.0/src/macaw_auth/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/functions/assume_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/functions/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/functions/web_logon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/src/macaw_auth/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:36:04.590282 macaw_auth-2.0.0/src/macaw_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-28 21:36:04.000000 macaw_auth-2.0.0/src/macaw_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-28 21:36:04.000000 macaw_auth-2.0.0/src/macaw_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:36:04.000000 macaw_auth-2.0.0/src/macaw_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 21:36:04.000000 macaw_auth-2.0.0/src/macaw_auth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 21:36:04.000000 macaw_auth-2.0.0/src/macaw_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 21:36:04.000000 macaw_auth-2.0.0/src/macaw_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:36:04.590282 macaw_auth-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-28 21:35:47.000000 macaw_auth-2.0.0/tests/test_usernames.py
```

### Comparing `macaw_auth-1.2.0/LICENSE` & `macaw_auth-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macaw_auth-1.2.0/macaw_auth.egg-info/SOURCES.txt` & `macaw_auth-2.0.0/src/macaw_auth.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
-macaw_auth.egg-info/PKG-INFO
-macaw_auth.egg-info/SOURCES.txt
-macaw_auth.egg-info/dependency_links.txt
-macaw_auth.egg-info/entry_points.txt
-macaw_auth.egg-info/requires.txt
-macaw_auth.egg-info/top_level.txt
 src/macaw_auth/__init__.py
+src/macaw_auth/main.py
+src/macaw_auth.egg-info/PKG-INFO
+src/macaw_auth.egg-info/SOURCES.txt
+src/macaw_auth.egg-info/dependency_links.txt
+src/macaw_auth.egg-info/entry_points.txt
+src/macaw_auth.egg-info/requires.txt
+src/macaw_auth.egg-info/top_level.txt
 src/macaw_auth/classes/__init__.py
-src/macaw_auth/classes/aws_credentials.py
 src/macaw_auth/classes/configuration.py
-src/macaw_auth/classes/errors.py
 src/macaw_auth/classes/idp_connection.py
 src/macaw_auth/classes/sts_saml.py
 src/macaw_auth/classes/user_credentials.py
 src/macaw_auth/classes/username_validation.py
-src/macaw_auth/cli/__init__.py
-src/macaw_auth/cli/__main__.py
-src/macaw_auth/cli/cli.py
+src/macaw_auth/functions/__init__.py
+src/macaw_auth/functions/assume_role.py
+src/macaw_auth/functions/common.py
+src/macaw_auth/functions/login.py
+src/macaw_auth/functions/web_logon.py
 tests/test_usernames.py
```

### Comparing `macaw_auth-1.2.0/src/macaw_auth/classes/configuration.py` & `macaw_auth-2.0.0/src/macaw_auth/classes/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 import configparser
 from pathlib import Path
-from .errors import ConfigurationError
+
+class ConfigurationError(Exception):
+    """Raises an exception when required configuration items are
+    set incorrectly.
+
+    Attributes:
+        message -- message indicating the specifics of the error
+    """
+
+    def __init__(self,
+            message='Incorrect configuration. Check your configuration file'):
+        self.message = message
+        super().__init__(self.message)
 
 class Configuration:
     """
     A base class used to define various configurations used by the utility
-    including client config, role config, and user credentials
+    including role config and user credentials
 
     ...
 
     Attributes
     ----------
     # config_type : str
     #     username for validation
@@ -22,120 +34,115 @@
     # config_parameters :
     #     temp
     """
 
     default_configuration_file = Path.home() / ".aws" / "config"
     default_credentials_file = Path.home() / ".aws" / "credentials"
 
-    def __init__(
-            self, config_type, section_name, config_file=None,
-            **config_parameters : tuple):
-        self.config_type = config_type
+    def __init__(self, config_type, section_name, config_file=None, **config_parameters):
+        self.config_type = self.arg_to_string(config_type)
         self.config_path = self.select_config_file_path(
             config_type, config_file)
-        self.config_section = self.select_config_section(section_name)
+        self.config_section = self.select_config_section(self.arg_to_string(section_name))
         self.config = self.initialize_config()
-        self.config_parameters = config_parameters
-        self.parse_config_parameters()
+        if len(config_parameters) > 0:
+            self.parse_config_parameters(config_parameters)
 
     # Set the configuration/credential file to use
     def select_config_file_path(self, file_type, file_path):
         if file_path is not None:
             config_path = file_path
         else:
-            if file_type == 'client' or file_type == 'user':
+            if file_type == 'user':
                 config_path = self.default_configuration_file
             elif file_type == 'credential':
                 config_path = self.default_credentials_file
             else:
                 # The config type should be transparent to end users but add an
                 # error just in case
                 message = "Invalid config type passed: {}. ".format(file_type) + \
-                    "Valid config types are 'client', 'user, and 'credential'"
-                raise Configuration(message)
+                    "Valid config types are 'user' and 'credential'"
+                raise ConfigurationError(message)
         return config_path
 
     # Select which section of the configuration file will be used
     def select_config_section(self, section):
         if self.config_type == 'credential':
             if section is None:
                 config_section = 'default'
             else:
                 config_section = section
-        elif section is None:
-            config_section = 'macaw-auth'
-        elif self.config_type == 'client':
-            config_section = section
         elif self.config_type == 'user':
-            config_section = 'profile ' + section
+            if section is None:
+                config_section = 'macaw-auth'
+            else:
+                config_section = 'profile ' + section
         else:
             # The config type should be transparent to end users but add an
             # error just in case
             message = "Invalid config type passed: {}. ".format(self.config_type) + \
-                "Valid config types are 'client', 'user, and 'credential'"
-            raise Configuration(message)
+                "Valid config types are 'user, and 'credential'"
+            raise ConfigurationError(message)
         return config_section
 
     def initialize_config(self):
-
-        # if self.config_section is None:
-        #     config = configparser.ConfigParser()
-        # else:
-
-
         # Check if config file already exists
         file_exists = Path.is_file(self.config_path)
         #TODO - build logic to avoid erroring out if user passes everything via command line
         #TODO - create credentials file if it doesn't exist. May do the same for config but probably not
         if not file_exists:
             message = "Configuration file: {} does not exist. ".format(
                 self.config_path) + "Please create the file and set the " + \
                 "configuration options"
             raise ConfigurationError(message)
         config = configparser.ConfigParser()
         config.read(self.config_path)
         if self.config_section not in config.sections():
             config.add_section(self.config_section)
         return config
-    
+
+    @staticmethod
+    def arg_to_string(arg):
+        if arg is not None:
+            value = str(arg)
+        else:
+            value = arg
+        return value
+
     def get_config_setting(self, attribute):
-        # if self.config_section is None:
-        #     return None
-        # else:
         setting = self.config[self.config_section].get(attribute)
+        # If value isn't found in profile, check macaw-auth section
+        if setting is None and self.config_type == 'user' and self.config_section != 'macaw-auth':
+            setting = self.config['macaw-auth'].get(attribute)
         return setting
 
-    def set_optional_setting(self, setting, default):
-        # if self.config_section is None:
-        #     self.config.add_section('None')
-        #     self.config['None'][setting] = default
-        #     print(self.config['None'][setting])
-        # else:
-        value = self.get_config_setting(setting)
-        if value is None:
-            self.config[self.config_section][setting] = default
-
-    def get_required_setting(self, attribute):
-        # if self.config_section is None:
-        #     message = "Required configuration value: {} ".format(attribute) + \
-        #         "was not provided via command line and no profile was selected."
-        #     raise ConfigurationError(message)
-        # else:
-        value = self.get_config_setting(attribute)
-        if value is None:
-            message = "Required configuration value is missing: " + attribute
-            raise ConfigurationError(message)
-
     def set_config_value(self, attribute_name, value, required=False, default=''):
         if value is not None:
-            # if self.config_section is None:
-            #     self.config[attribute_name] = str(value)
-            # else:
             self.config[self.config_section][attribute_name] = str(value)
-        elif required:
-            self.get_required_setting(attribute_name)
         else:
-            self.set_optional_setting(attribute_name, default)
+            setting = self.get_config_setting(attribute_name)
+            if setting is None:
+                if required:
+                    message = "Required configuration value is missing: " + attribute_name
+                    raise ConfigurationError(message)
+                else:
+                    self.config[self.config_section][attribute_name] = default
+            else:
+                self.config[self.config_section][attribute_name] = setting
     
-    def parse_config_parameters(self):
-        for key, value in self.config_parameters.items():
-            self.set_config_value(key, value[0], value[1], value[2])
+    def parse_config_parameters(self, parameters : dict):
+        for key, value in parameters.items():
+            self.set_config_value(key, self.arg_to_string(value[0]), value[1], value[2])
+
+    def write_config(self):
+        # Write the updated config file
+        with open(self.config_path, 'w+') as configfile:
+            self.config.write(configfile)
+
+        # Give the user some basic info as to what has just happened
+        print('\n\n----------------------------------------------------------------')
+        print('Your new access key pair has been stored in the AWS configuration file {0} under the {1} profile.'.format(self.config_path, self.config_section))
+        print('Note that it will expire at {0}.'.format(self.config[self.config_section]['expiration']))
+        print('After this time, you may safely rerun this script to refresh your access key pair.')
+        if self.config_section != 'default':
+            print('To use this credential, call the AWS CLI with the --profile option (e.g. aws --profile {0} ec2 describe-instances).'.format(self.config_section))
+        print('----------------------------------------------------------------\n\n')
```

### Comparing `macaw_auth-1.2.0/src/macaw_auth/classes/idp_connection.py` & `macaw_auth-2.0.0/src/macaw_auth/classes/idp_connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 from bs4 import BeautifulSoup #pip install beautifulsoup4
 from getpass import getpass
 from urllib.parse import urlparse
 import re
 import sys
 import base64
 
+class AuthenticationError(Exception):
+    """Raises an exception when the user is unable to successfully
+    authenticate.
+
+    Attributes:
+        message -- message indicating the specifics of the error
+    """
+
+    def __init__(self,
+            message='Authentication response did not contain a valid SAML assertion'):
+        self.message = message
+        super().__init__(self.message)
+
 class SAMLAssertion:
 
     def __init__(self, username, password, identity_url, auth_type, ssl_verification=True):
         self.identity_url = identity_url
         self.ssl_verification = ssl_verification
         self.auth_type = auth_type
         self.__username = username
@@ -21,27 +34,18 @@
             self.create_web_form_payload()
             self.authenticate_to_web_form()
         self.get_saml_assertion()
 
     def make_saml_request(self):
         if self.auth_type == 'ntlm':
             self.session.auth = HttpNtlmAuth(self.__username, self.__password, self.session)
-            feature = "html.parser"
-        elif self.auth_type == 'web_form':
-            # feature = "lxml"
-            feature = "html.parser"
-        else:
-            message = "Incorrect authorization type provided. Valid types are 'ntlm' or 'web_form'"
-            ##RAISE ERROR - TODO
         self.response = self.session.get(self.identity_url, verify=self.ssl_verification)
-        self._redirect_url = self.response.url
-        self.__soup = BeautifulSoup(self.response.text, features=feature)
-
-        # formsoup = BeautifulSoup(response.text, features="lxml")
-        # payload = {}
+        if self.auth_type == 'web_form':
+            self._redirect_url = self.response.url
+        self.__soup = BeautifulSoup(self.response.text, features="html.parser")
 
     def create_web_form_payload(self):
         payload = {}
 
         for inputtag in self.__soup.find_all(re.compile('(INPUT|input)')):
             name = inputtag.get('name','')
             value = inputtag.get('value','')
@@ -75,57 +79,69 @@
         mfa_enabled = False
         assertion = ''
 
         # Look for the SAMLResponse attribute of the input tag (determined by
         # analyzing the debug print lines above)
         for inputtag in self.__soup.find_all('input'):
             if(inputtag.get('name') == 'SAMLResponse'):
-                #print(inputtag.get('value'))
                 assertion = inputtag.get('value')
                 break
             if('vip' in inputtag.get('name')):
                 mfa_enabled = True
 
         if (assertion == ''):
             invalid_assertion = True
             if mfa_enabled:
-                self.authenticate_with_mfa()
-                for inputtag in self.__soup.find_all('input'):
-                    if(inputtag.get('name') == 'SAMLResponse'):
-                        assertion = inputtag.get('value')
-                        invalid_assertion = False
-                        break
-            if invalid_assertion:
-                #TODO: Insert valid error checking/handling
-                print('Response did not contain a valid SAML assertion')
-                sys.exit(0)
+                assertion = self.authenticate_with_mfa()
+            else:
+                message = "Authentication attempt did not contain a valid SAML assertion. Please confirm credentials and network connectivity."
+                raise AuthenticationError(message)
         self.assertion = assertion
 
         # Debug only
         # print(base64.b64decode(assertion))
 
     def get_vip_code(self):
-        self.__vipcode = getpass(prompt='Enter your Symantec VIP security code: ')
+        vip_code = getpass(prompt='Enter your Symantec VIP security code: ')
         try:
-            int(self.__vipcode)
+            int(vip_code)
+            return vip_code
         except ValueError as err:
             print('ERROR: Code must be a number. Try again...')
             self.get_vip_code()
 
-    def authenticate_with_mfa(self):
-        self.get_vip_code()
-        payload = {}
+    def authenticate_with_mfa(self, attempt=0):
+        current_attempt = attempt + 1
+        # Attempt to authenticate with MFA up to 3 times
+        if current_attempt <= 3:
+            invalid_assertion = True
+            code = self.get_vip_code()
+            payload = {}
 
-        for inputtag in self.__soup.find_all('input'):
-            name = inputtag.get('name','')
-            value = inputtag.get('value','')
-            # Locate VIP code fields in web form by searching for "[security_]code"
-            if "code" in name.lower():
-                payload[name] = self.__vipcode
+            for inputtag in self.__soup.find_all('input'):
+                name = inputtag.get('name','')
+                value = inputtag.get('value','')
+                # Locate VIP code fields in web form by searching for "[security_]code"
+                if "code" in name.lower():
+                    payload[name] = code
+                else:
+                    # Keep existing value
+                    payload[name] = value
+
+            # Performs the submission of the Symantec VIP code
+            response = self.session.post(
+                self._redirect_url, data=payload, verify=self.ssl_verification)
+            self.__soup = BeautifulSoup(response.text, features="html.parser")
+            for inputtag in self.__soup.find_all('input'):
+                if(inputtag.get('name') == 'SAMLResponse'):
+                    assertion = inputtag.get('value')
+                    invalid_assertion = False
+                    break
+            if invalid_assertion:
+                print("Incorrect code. Try again... (Strike {}!)".format(str(current_attempt)))
+                self.authenticate_with_mfa(current_attempt)
             else:
-                # Keep existing value
-                payload[name] = value
-
-        # Performs the submission of the Symantec VIP code
-        response = self.session.post(
-            self._redirect_url, data=payload, verify=self.ssl_verification)
-        self.__soup = BeautifulSoup(response.text, features="html.parser")
+                return assertion
+        else:
+            # Error out if user enters MFA code incorrectly 3 times
+            message = "Sorry, you struck out. Aborting login...".format(str(attempt))
+            raise AuthenticationError(message)
```

### Comparing `macaw_auth-1.2.0/src/macaw_auth/classes/user_credentials.py` & `macaw_auth-2.0.0/src/macaw_auth/classes/user_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # from . import errors
 # Keyring may require importing dbus-python to work on Linux
 # dbus-python may not install properly via pip, so may need to disable keyring on linux
 import keyring
 from getpass import getpass
-from .idp_connection import SAMLAssertion
+from macaw_auth.classes.idp_connection import SAMLAssertion
 
 class UserCredentials:
     """
     A class to represent a user's credentials for authenticating to AWS
 
     ...
```

### Comparing `macaw_auth-1.2.0/src/macaw_auth/classes/username_validation.py` & `macaw_auth-2.0.0/src/macaw_auth/classes/username_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-from .errors import InvalidUsernameError
+class InvalidUsernameError(Exception):
+    """Raises an exception when an invalid username is entered
+
+    Attributes:
+        message -- message indicating the specifics of the error
+    """
+
+    def __init__(self, message='Invalid user name entered'):
+        self.message = message
+        super().__init__(self.message)
 
 class UsernameValidation:
     """
     A class to check the validity of a provided username
 
     ...
```

### Comparing `macaw_auth-1.2.0/tests/test_usernames.py` & `macaw_auth-2.0.0/tests/test_usernames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from src.macaw_auth.classes.username_validation import UsernameValidation
-from src.macaw_auth.classes.errors import InvalidUsernameError
+from src.macaw_auth.classes.username_validation import InvalidUsernameError
 import pytest
 
 class TestUsernameValidation:
 
     @staticmethod
     def validate_user(
             username : str,
```

