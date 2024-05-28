# Comparing `tmp/gspread_models-1.0.6.tar.gz` & `tmp/gspread_models-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread_models-1.0.6.tar", last modified: Thu May 23 03:00:29 2024, max compression
+gzip compressed data, was "gspread_models-1.0.7.tar", last modified: Tue May 28 21:37:57 2024, max compression
```

## Comparing `gspread_models-1.0.6.tar` & `gspread_models-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:00:29.100620 gspread_models-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 03:00:24.000000 gspread_models-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-23 03:00:29.100620 gspread_models-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-23 03:00:24.000000 gspread_models-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:00:29.096620 gspread_models-1.0.6/gspread_models/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 03:00:24.000000 gspread_models-1.0.6/gspread_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-23 03:00:24.000000 gspread_models-1.0.6/gspread_models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-23 03:00:24.000000 gspread_models-1.0.6/gspread_models/date_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-23 03:00:24.000000 gspread_models-1.0.6/gspread_models/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:00:29.100620 gspread_models-1.0.6/gspread_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:00:29.100620 gspread_models-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 03:00:24.000000 gspread_models-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:37:57.349258 gspread_models-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 21:37:48.000000 gspread_models-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-28 21:37:57.349258 gspread_models-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-28 21:37:48.000000 gspread_models-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:37:57.349258 gspread_models-1.0.7/gspread_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-28 21:37:48.000000 gspread_models-1.0.7/gspread_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-28 21:37:48.000000 gspread_models-1.0.7/gspread_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-28 21:37:48.000000 gspread_models-1.0.7/gspread_models/date_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-28 21:37:48.000000 gspread_models-1.0.7/gspread_models/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:37:57.349258 gspread_models-1.0.7/gspread_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-28 21:37:57.000000 gspread_models-1.0.7/gspread_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 21:37:57.000000 gspread_models-1.0.7/gspread_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:37:57.000000 gspread_models-1.0.7/gspread_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 21:37:57.000000 gspread_models-1.0.7/gspread_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 21:37:57.000000 gspread_models-1.0.7/gspread_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:37:57.349258 gspread_models-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 21:37:48.000000 gspread_models-1.0.7/setup.py
```

### Comparing `gspread_models-1.0.6/LICENSE` & `gspread_models-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.6/PKG-INFO` & `gspread_models-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread_models
-Version: 1.0.6
+Version: 1.0.7
 Summary: An Object Relational Mapper (ORM) for the Google Sheets API. Provides a straightforward and intuitive model-based query interface, making it easy to interact with Google Sheets as if it were more like a database. Offers a fast and flexible way to get up and running with a Google Sheets database, for rapid prototyping and development in Python.
 Home-page: https://github.com/s2t2/gspread-models-py
 Author: Michael Rossetti
 Author-email: datacreativellc@gmail.com
 License: MIT
 Keywords: google sheets gspread models orm spreadsheet google-sheets google-sheets-api gspread-models gspread_models
 Description-Content-Type: text/markdown
@@ -124,15 +124,15 @@
   + [Project File Organization](./docs/organization.md)
   + [Pandas Support](./docs/pandas_support.md)
 
 ## Examples
 
 Here are some examples that demonstrate the usage of `gspread-models` within a variety of contexts:
 
-  + [Demo Notebook](./docs/notebooks/demo_v1_0_6.ipynb)
+  + [Demo Notebook](./docs/notebooks/demo_v1_0_7.ipynb)
   + [Flask Sheets Web Application Template](https://github.com/prof-rossetti/flask-sheets-template-2024)
 
 If you use the `gspread-models` package, you are encouraged to add your project to this list, by submitting a pull request or opening an issue.
 
 ## Contributing
 
 Contributions welcome! Here are some reference guides to help you get started as a contributor or maintainer of this package:
```

### Comparing `gspread_models-1.0.6/README.md` & `gspread_models-1.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
   + [Project File Organization](./docs/organization.md)
   + [Pandas Support](./docs/pandas_support.md)
 
 ## Examples
 
 Here are some examples that demonstrate the usage of `gspread-models` within a variety of contexts:
 
-  + [Demo Notebook](./docs/notebooks/demo_v1_0_6.ipynb)
+  + [Demo Notebook](./docs/notebooks/demo_v1_0_7.ipynb)
   + [Flask Sheets Web Application Template](https://github.com/prof-rossetti/flask-sheets-template-2024)
 
 If you use the `gspread-models` package, you are encouraged to add your project to this list, by submitting a pull request or opening an issue.
 
 ## Contributing
 
 Contributions welcome! Here are some reference guides to help you get started as a contributor or maintainer of this package:
```

### Comparing `gspread_models-1.0.6/gspread_models/base.py` & `gspread_models-1.0.7/gspread_models/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,81 @@
 
-#from abc import abstractmethod
+from abc import ABC #abstractmethod
 from typing import List, Dict
 from functools import lru_cache #,cached_property
 from datetime import datetime
 
 from gspread import Worksheet #, Spreadsheet
 from gspread_models.service import SpreadsheetService
 #from pandas import DataFrame
 
 
-class BaseModel:
+class BaseModel(ABC):
+    """
+    The Base Model provides an intuitive query interface to any models inheriting from it.
+
+    Before reading and writing data to the sheet, you must first bind the base model
+    to a specified google sheet document, using your authorized credentials.
+
+    Then each child model which inherits from the base model will be configured to use
+    a specified sheet in that document.
+
+    Parameters
+    ----------
+    attrs : dict
+        A dictionary of attribute parameters that have been fetched from the sheet.
+
+        All values should be serializable, for example using datetime strings
+        instead of datetime objects.
+
+    See Also
+    --------
+    BaseModel.bind : Bind base model to a given spreadsheet document.
+
+    Notes
+    -----
+    Please reference the :ref:`API Index <api_index>` for more information.
+
+    Examples
+    --------
+    Defining a child model class that inherits from the base model:
+
+    >>> class Book(BaseModel):
+    ...     SHEET_NAME = "books"
+    ...
+    ...     COLUMNS = ["title", "author", "year"]
+
+    Constructing an object from a dictionary of values like those fetched from the sheet.
+
+    >>> book = Book({
+    ...     "id": 1,
+    ...     "title":"Book 1",
+    ...     "author": "Me",
+    ...     "created_at": ""
+    ... })
+    Book
+    >>> print(book.id)
+    1
+    >>> print(book.title)
+    Book 1
+    >>> print(book.author)
+    Me
+    >>> print(book.created_at)
+    datetime object
+    """
 
     SHEET_NAME = None # abstract constant (str) to be set in child class
 
     COLUMNS = [] # abstract constant to be set in child class
 
     SEEDS = [] # abstract constant to be set in child class
 
     service = None # SpreadsheetService()
 
     def __init__(self, attrs:Dict):
-        """
-        Need to set service afterwards to bind the base model (and models which inherit from it) to a given sheet.
-
-            service = SpreadsheetService() # opportunity to pass custom credentials and designate the sheet
-            BaseModel.service = service
-        """
         self.attrs = attrs
 
         # attributes common to all child models
         self.id = attrs.get("id")
 
         for col in self.COLUMNS:
             #setattr(self, col, self.attrs.get(col))
@@ -42,33 +88,39 @@
 
     #
     # INSTANCE METHODS
     #
 
     @property
     def created_at(self):
-        """Wraps timestamp string from the sheet in a native datetime object."""
+        """
+        Wraps timestamp string from the sheet in a native datetime object.
+        """
         return self.service.parse_timestamp(self.attrs.get("created_at"))
 
     #@property
     #def updated_at(self):
     #    """Wraps timestamp string from the sheet in a native datetime object."""
     #    return self.service.parse_timestamp(self.attrs.get("updated_at"))
 
     def __iter__(self):
-        """Enables dictionary conversion by passing an object instance into the dict() function."""
+        """
+        Enables dictionary conversion by passing an object instance into the dict() function.
+        """
         yield 'id', self.id
         for col in self.COLUMNS:
             yield col, getattr(self, col)
         yield 'created_at', self.created_at
         #yield 'updated_at', self.updated_at
 
     @property
     def row(self) -> List:
-        """Returns an ordered list of JSON serializable values, for writing to the sheet."""
+        """
+        Returns an ordered list of JSON serializable values, for writing to the sheet.
+        """
         values = []
         values.append(self.id)
         for col in self.COLUMNS:
             val = getattr(self, col)
             if isinstance(val, datetime):
                 val = str(val)
             values.append(val)
@@ -79,62 +131,101 @@
     #def save(self):
     #    print("SAVING RECORD TO SHEET:")
     #    print(dict(self))
     #    #if self.id:
     #    #    self.attrs["updated_at"] = self.service.generate_timestamp()
     #    #    self.update(dict(self))
     #    #return self.create(dict(self))
-        return self.create_all([dict(self)])
+    #    return self.create_all([dict(self)])
 
     #
     # CLASS METHODS
     #
 
     @classmethod
     def bind(cls, document_id, credentials_filepath=None, credentials=None, creds=None):
+        """
+        Bind the base model with a given document and set of credentials to access that document.
+
+        Parameters
+        --------------
+        credentials_filepath : (str)
+            path to local service account JSON file
+        document_id : (str)
+            google sheets document identifier (obtained from the URL)
+        creds or credentials : (google.auth.compute_engine.credentials.Credentials)
+            optionally pass credentials object instead of filepath
+
+        See Also
+        --------
+        SpreadsheetService : Uses similar credentials parameters
+
+        Examples
+        ----------
+        >>> from gspread_models.base import BaseModel
+        >>> BaseModel.service
+        None
+        >>> BaseModel.bind(
+        ...     credentials_filepath="google-credentials.json"
+        ...     document_id="your-document-id"
+        ... )
+        >>> BaseModel.service
+        SpreadsheetService object
+        """
         cls.service = SpreadsheetService(
             document_id=document_id,
             credentials_filepath=credentials_filepath,
             credentials=credentials,
             creds=creds
         )
 
     #@classmethod
     #def set_document_id(cls, document_id):
     #    cls.service.document_id = document_id
 
     @classmethod
     def get_sheet(cls) -> Worksheet:
-       print(f"GET SHEET ('{cls.SHEET_NAME}')...")
-       return cls.service.get_sheet(sheet_name=cls.SHEET_NAME)
+        """
+        Fetch the model-specific sheet, once it has been configured in the child class.
+
+        See Also
+        --------
+        BaseModel.SHEET_NAME
+        """
+        print(f"GET SHEET ('{cls.SHEET_NAME}')...")
+        return cls.service.get_sheet(sheet_name=cls.SHEET_NAME)
 
     # using @property + @lru_cache because @cached_property throws:
     # ... TypeError: Cannot use cached_property instance without calling __set_name__ on it.
     @classmethod
     @property
     @lru_cache(maxsize=None)
     def sheet(cls) -> Worksheet:
-        """Caches the sheet to avoid unnecessary API requests."""
+        """
+        Caches the sheet to avoid unnecessary API requests.
+        """
         return cls.get_sheet()
 
     # ... QUERY INTERFACE (API)
 
     @classmethod
     def find(cls, by_id):
-        """Fetches a record by its unique identifier.
+        """
+        Fetches a record by its unique identifier.
         """
         records = cls.sheet.get_all_records()
         for record in records:
             if record.get("id") == by_id:
                 return cls(record)
         return None
 
     @classmethod
     def all(cls): # as_df=False
-        """Fetches all records from a given sheet.
+        """
+        Fetches all records from a given sheet.
         """
         records = cls.sheet.get_all_records()
         # we can consider passing the data back in dataframe format:
         # see: https://github.com/s2t2/gspread-models-py/issues/12
         #if as_df:
         #    #df = DataFrame(records)
         #    # use model conversion to take advantage of datetime-conversion, etc:
@@ -148,38 +239,43 @@
     #@classmethod
     #def find_all(cls):
     #    """alias method"""
     #    return cls.all()
 
     @classmethod
     def destroy_all(cls):
-        """Removes all records from a given sheet, except the header row."""
+        """
+        Removes all records from a given sheet, except the header row.
+        """
         records = cls.sheet.get_all_records()
         # start on the second row, and delete one more than the number of records (to account for header row)
         return cls.sheet.delete_rows(start_index=2, end_index=len(records)+1)
 
     @classmethod
     def where(cls, **kwargs):
-        """Filter records which match all provided values."""
+        """
+        Filter records which match all provided values.
+        """
         records = cls.sheet.get_all_records()
         objs = []
         for attrs in records:
             obj = cls(attrs)
 
             match_all = all(getattr(obj, k) == v for k, v in kwargs.items())
 
             if match_all:
                 objs.append(obj)
 
         return objs
 
     @classmethod
     def create_all(cls, new_records:List[Dict], records=[]):
-        """Appends new records (list of dictionaries) to the sheet.
-            Adds auto-incrementing unique identifiers, and timestamp columns.
+        """
+        Appends new records (list of dictionaries) to the sheet.
+        Adds auto-incrementing unique identifiers, and timestamp columns.
         """
         records = records or cls.all()
 
         # auto-increment integer identifier:
         if any(records):
             existing_ids = [r.id for r in records]
             next_id = max(existing_ids) + 1
@@ -196,16 +292,19 @@
             rows.append(inst.row)
             next_id += 1
 
         return cls.sheet.append_rows(rows)
 
     @classmethod
     def create(cls, new_record:dict):
-        """Appends new records (list of dictionaries) to the sheet.
-            Adds auto-incrementing unique identifiers, and timestamp columns.
+        """
+        Appends new records (list of dictionaries) to the sheet.
+        Adds auto-incrementing unique identifiers, and timestamp columns.
         """
         return cls.create_all([new_record])
 
     @classmethod
     def seed(cls):
-        """Convenience method, if you would like to set SEEDS."""
+        """
+        Convenience method, if you would like to set SEEDS.
+        """
         return cls.create_all(new_records=cls.SEEDS)
```

### Comparing `gspread_models-1.0.6/gspread_models/date_parser.py` & `gspread_models-1.0.7/gspread_models/date_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,80 @@
 
 from datetime import datetime, timezone
 
 
 # see: https://docs.python.org/3/library/datetime.html#strftime-strptime-behavior
+# todo: allow configuration by moving into the class, and making the staticmethods classmethods
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S.%f%z" # consider allowing customization
 
 
 class DateParser:
-    """Mixin for date parsing / interfacing with google sheets date formatting."""
+    """
+    Mixin for date parsing / interfacing with google sheets date formatting.
+    """
 
     @staticmethod
     def generate_timestamp():
-        """Generates a new timestamp of the current time in UTC timezone.
-            Returns a datetime object.
+        """
+        Generates a new timestamp of the current time in UTC timezone.
+        Returns a datetime object.
+
+        Examples
+        ---------
+        >>> DateParser.generate_timestamp()
+        datetime(2023, 3, 8, 19, 59, 16, tzinfo=utc)
+
+        Returns
+        --------
+        datetime
         """
         return datetime.now(tz=timezone.utc)
 
     @staticmethod
     def parse_timestamp(ts:str) -> datetime:
-        """Converts a timestamp string to a datetime object as necessary.
-            Ensures you are working with a datetime object.
-
-            Params:
-                ts (str) : a timestamp string in format provided by google sheets
-
-            Example: DateParser.parse_timestamp('2023-03-08 19:59:16.471152+00:00')
-
-            Returns a datetime object.
+        """
+        Converts a timestamp string to a datetime object as necessary.
+        Ensures you are working with a datetime object.
+        Returns a datetime object.
+
+        Parameters
+        --------
+        ts : str
+            A timestamp string in format provided by google sheets
+
+        Examples
+        ---------
+        DateParser.parse_timestamp('2023-03-08 19:59:16.471152+00:00')
+        datetime(2023, 3, 8, 19, 59, 16, tzinfo=utc)
         """
         if isinstance(ts, datetime):
             return ts
         elif isinstance(ts, str):
             return datetime.strptime(ts, DATE_FORMAT)
         #else:
         #    # something went wrong! use original value. consider raising error
         #    return ts
 
     @staticmethod
-    def validate_timestamp(ts:str):
+    def validate_timestamp(ts:str) -> bool:
+        """
+        Determines whether or not a timestamp formatted string is properly formatted,
+        specifically using to the following format: '%Y-%m-%d %H:%M:%S.%f%z'.
+
+        See: https://docs.python.org/3/library/datetime.html#strftime-strptime-behavior
+
+        Examples
+        --------
+        >>> DateParser.validate_timestamp('2023-03-08 19:59:16.471152+00:00')
+        True
+
+        >>> DateParser.validate_timestamp('2023-03-08 19:59:16')
+        True
+
+        >>> DateParser.validate_timestamp('OOPS')
+        False
+        """
         try:
             datetime.strptime(ts, DATE_FORMAT)
             return True
         except:
             return False
```

### Comparing `gspread_models-1.0.6/gspread_models/service.py` & `gspread_models-1.0.7/gspread_models/service.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,63 +13,83 @@
 load_dotenv()
 
 DEFAULT_FILEPATH = os.path.join(os.path.dirname(__file__), "..", "google-credentials.json")
 GOOGLE_CREDENTIALS_FILEPATH = os.getenv("GOOGLE_CREDENTIALS_FILEPATH", default=DEFAULT_FILEPATH)
 GOOGLE_SHEETS_DOCUMENT_ID = os.getenv("GOOGLE_SHEETS_DOCUMENT_ID", default="OOPS, Please get the spreadsheet identifier from its URL, and set the 'GOOGLE_SHEETS_DOCUMENT_ID' environment variable accordingly...")
 
 class SpreadsheetService(DateParser):
+    """
+    The Spreadsheet Service provides a connection to a specified Google Sheets document.
 
-    def __init__(self, credentials_filepath=GOOGLE_CREDENTIALS_FILEPATH, document_id=GOOGLE_SHEETS_DOCUMENT_ID, creds=None, credentials=None):
-        """The Spreadsheet Service provides a connection to a specified Google Sheets document.
+    Parameters
+    --------------
 
-            Params:
+    credentials_filepath : str
+        path to local service account JSON file
 
-                credentials_filepath : path to local service account JSON file
+    document_id : str
+        google sheets document identifier (obtained from the URL)
 
-                document_id : google sheets document identifier (obtained from the URL)
+    credentials : google.auth.compute_engine.credentials.Credentials
+        optionally pass credentials object instead of filepath
+        alternatively use creds parameter as an alias
 
-                creds or credentials : optionally pass credentials (google.auth.compute_engine.credentials.Credentials)
+    Examples
+    -----------------------------
 
-                for example for use in colab notebook:
+    Example usage within a colab notebook:
 
-                        from google.colab import auth
-                        from google.auth import default
+    >>> from google.colab import auth
+    >>> from google.auth import default
+    >>> from gspread_models import SpreadsheetService
 
-                        auth.authenticate_user()
-                        creds, _ = default()
+    >>> auth.authenticate_user()
+    >>> creds, _ = default()
+    >>> service = SpreadsheetService(creds=creds, document_id="my-document-id")
+    >>> print(service.doc)
+    'doc-id'
+    """
 
-                        service = SpreadsheetService(creds=creds)
-        """
+    def __init__(self, document_id, credentials_filepath=None, creds=None, credentials=None):
         creds = creds or credentials
         if creds:
             self.client = authorize(creds)
         else:
+            credentials_filepath = credentials_filepath or GOOGLE_CREDENTIALS_FILEPATH
             self.client = service_account(filename=credentials_filepath)
 
-        self.document_id = document_id
+        self.document_id = document_id or GOOGLE_SHEETS_DOCUMENT_ID
 
         print("SPREADSHEET SERVICE...")
         print("DOCUMENT ID:", self.document_id)
 
     @cached_property
     def doc(self) -> Spreadsheet:
-        """Get the given document."""
+        """
+        Get the given document.
+        """
         return self.client.open_by_key(self.document_id)
 
     @property
     def sheets(self) -> List[Worksheet]:
-        """List all sheets in the given document."""
+        """
+        List all sheets in the given document.
+        """
         return self.doc.worksheets()
 
     def get_sheet(self, sheet_name) -> Worksheet:
-        """Get a specific sheet in the document."""
+        """
+        Get a specific sheet in the document.
+        """
         return self.doc.worksheet(sheet_name)
 
     def find_or_create_sheet(self, sheet_name) -> Worksheet:
-        """access a sheet within the document, or create if not exists"""
+        """
+        Access a sheet within the document, or create if not exists.
+        """
         try:
             sheet = self.doc.worksheet(sheet_name)
             print(f"FOUND SHEET: '{sheet_name}'")
         except WorksheetNotFound:
             print(f"CREATING NEW SHEET ('{sheet_name}')...")
             sheet = self.doc.add_worksheet(title=sheet_name, rows="3", cols="3") # rows and cols are required. can be overwritten later?
             # consider adding columns based on self.COLUMNS
@@ -78,15 +98,14 @@
 
 
 
 if __name__ == "__main__":
 
     from pprint import pprint
 
-
     ss = SpreadsheetService()
 
     print("SHEETS:")
     sheets = ss.sheets
     for sheet in sheets:
         #print(type(sheet)) #> <class 'gspread.worksheet.Worksheet'>
         print("...", sheet)
```

### Comparing `gspread_models-1.0.6/gspread_models.egg-info/PKG-INFO` & `gspread_models-1.0.7/gspread_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread_models
-Version: 1.0.6
+Version: 1.0.7
 Summary: An Object Relational Mapper (ORM) for the Google Sheets API. Provides a straightforward and intuitive model-based query interface, making it easy to interact with Google Sheets as if it were more like a database. Offers a fast and flexible way to get up and running with a Google Sheets database, for rapid prototyping and development in Python.
 Home-page: https://github.com/s2t2/gspread-models-py
 Author: Michael Rossetti
 Author-email: datacreativellc@gmail.com
 License: MIT
 Keywords: google sheets gspread models orm spreadsheet google-sheets google-sheets-api gspread-models gspread_models
 Description-Content-Type: text/markdown
@@ -124,15 +124,15 @@
   + [Project File Organization](./docs/organization.md)
   + [Pandas Support](./docs/pandas_support.md)
 
 ## Examples
 
 Here are some examples that demonstrate the usage of `gspread-models` within a variety of contexts:
 
-  + [Demo Notebook](./docs/notebooks/demo_v1_0_6.ipynb)
+  + [Demo Notebook](./docs/notebooks/demo_v1_0_7.ipynb)
   + [Flask Sheets Web Application Template](https://github.com/prof-rossetti/flask-sheets-template-2024)
 
 If you use the `gspread-models` package, you are encouraged to add your project to this list, by submitting a pull request or opening an issue.
 
 ## Contributing
 
 Contributions welcome! Here are some reference guides to help you get started as a contributor or maintainer of this package:
```

### Comparing `gspread_models-1.0.6/setup.py` & `gspread_models-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # setup.py
 
 from setuptools import setup
 
-from gspread_models import VERSION
+#from gspread_models import VERSION
+VERSION = "1.0.7"
 
 # FYI: PyPI doesn't display the links in this markdown
 # https://stackoverflow.com/a/26737672/670433
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
```

